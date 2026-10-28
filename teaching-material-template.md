# Teaching Material Template

A reusable framework for generating instructor-facing class material for any course. It was extracted from the finished Kubernetes Class 1 material and is built on the research below.

## How to use it

1. Fill in the **Intake** (section 1) for the class you are preparing.
2. Paste the **Generation Prompt** (section 9) together with your source material (a chapter, a table of contents, your own notes).
3. Review the result against the **Quality Checklist** (section 8), teach it, then bring the retrieval results back for revision.

---

## 1. Intake

Provide these before generation. Anything left blank, the generator assumes and states.

| Item | What to provide |
|---|---|
| Course and topic | e.g. "Spring Boot: dependency injection" |
| Source material | The chapter, table of contents or notes the class is based on |
| Audience | Who they are and **what they already know** (this sets the depth of every definition) |
| Environment | Operating systems, tools and installs students will have |
| Class goals | What students should be able to **do** by the end, in plain words |
| Scope | Must-cover topics; topics to leave for later classes |
| Readers | Instructor only, or students too (decides whether answers appear in the file) |
| Labs | Hands-on work, demos or case exercises, if any |

---

## 2. House Rules

These apply to every segment.

- State each idea directly, as a plain definition followed by a concrete example.
- Define every term at its first use, before it appears anywhere else in the file.
- Explain every command, symbol or notation the first time it appears, part by part.
- Show the exact expected output for every command or demo.
- Present each idea as a titled segment with one specific topic.
- Put the question to ask beside the segment title, not as scripted dialogue.
- Leave out timings, history and tangents that serve no learning goal.
- Keep the instructor view and the student view in one file; the student sheet is its own section with no answers.
- Write in plain prose. Keep lists and tables for content that is naturally a list or a comparison.

---

## 3. Sequencing Rules

Order the segments so each one rests only on what students already have.

1. **Prerequisite concepts first.** If the topic depends on a base concept (for Kubernetes, containers), teach that concept fully before the topic.
2. **Define the topic and its category.** What it is, and what kind of thing it is.
3. **The problem it solves.** Each problem with how it was handled before the topic existed, and how it is handled now, together.
4. **The core idea.** The single idea the rest of the class rests on.
5. **Core vocabulary.** The few objects students will name constantly.
6. **Tools and setup**, with attached notes per tool and per operating system.
7. **Hands-on work**, ahead of the internal theory.
8. **Internal structure or architecture**, after students have seen the thing work, so each part attaches to something observed.
9. **Recap**, including the before/now pairs again.
10. **Retrieval** at the end.
11. **Student sheet.**

For a conceptual course with no tools, replace steps 6 and 7 with worked cases the students solve.

---

## 4. Document Skeleton

```markdown
# [Course]: [Class Title]

Source: [chapter or material]. Audience: [who, and prior knowledge]. [Environment notes.]

Where a segment title is followed by *Pose as a question*, put that question to the class before explaining the idea beneath it.

## Learning Goals
By the end of this class, students can:
1. [observable verb] ...
(4 to 6 goals; each must be checkable in the retrieval section)

## Session Plan
| # | Segment |
(one row per segment, in teaching order)

## 1. [Prerequisite concept]
## 2. [The topic: what it is]
## 3. [The problems it solves: before and now]
## 4. [The core idea]
## 5. [Core vocabulary]
## 6. [Tools and setup, with attached notes]
## 7. [Lab or case 1: setup checkpoints]
## 8. [Lab or case 2: first real task, predict-run-explain]
## 9. [Internal structure]
## 10. Recap
## 11. Retrieval: Did They Get It?
## 12. Student Sheet
## Instructor Notes
```

---

## 5. Segment Pattern

Every concept segment follows the same shape.

```markdown
## N. [Specific title]

### N.1 [Sub-topic]

*Pose as a question:* [question that makes students recall, predict or explain]

[Terms defined first, if any.]

[The idea stated directly: definition, then a concrete example.]

[Demo or example with exact expected output, if the idea can be shown.]

### N.x Check

*Pose as a question:* [question that tests whether the idea landed]
```

Question types to rotate through:

- **Activate:** what do they already know or have experienced?
- **Predict:** what will happen before it is shown?
- **Explain:** say it in your own words.
- **Compare:** how do two similar things differ?
- **Transfer:** apply it to a case they haven't seen.

Every segment opens or closes with at least one question, and every new segment includes one question that recalls an earlier segment.

---

## 6. Lab and Demo Pattern

Each step follows predict, run, explain.

1. A titled step with *Pose as a question:* asking for a prediction.
2. The command or action, with its parts explained the first time.
3. The exact expected output.
4. One or two sentences on what the output means and which concept it demonstrates.
5. A link back to the problem or idea that the step proves.

Setup labs are written as numbered **checkpoints**: each has an action, the expected result, and a troubleshooting row for the likely failures. Setup notes cover each operating system students use, and a **typical failures** line per tool.

---

## 7. Retrieval and Student Sheet

### Retrieval section (end of class, closed notes)

1. **Question table**, one row per question:

   | # | Question | Goal | A strong answer includes | If wrong, they probably... |
   |---|---|---|---|---|

   Cover every learning goal at least once, and include at least one question on each before/now problem pair.

2. **Transfer scenario:** a case the students have not seen, answered in their own words.
3. **Reading the results:** 4 to 5 rules that map patterns of wrong answers to what to reteach.
4. **Exit ticket:** one thing that makes sense, one thing still confusing, one short explanation of the central idea.
5. **Next-class use:** the two most common problems become the opening questions of the next class.

### Student sheet (contains no answers)

- Key terms
- Setup checkpoints with tick boxes
- Prediction log table for the lab
- A blank diagram to label from memory
- Command or formula cheat sheet
- Homework: re-do the lab from memory, a written recall within 24 hours, one explanation question

### Instructor notes

- Extra questions for a quiet room
- A short before-class preparation list (run the lab yourself, pre-download anything slow, prepare the likeliest setup fix)

---

## 8. Quality Checklist

Before using the material, confirm:

- [ ] Every learning goal is observable and has a matching retrieval question
- [ ] No term is used before it is defined
- [ ] Every command, flag or symbol is explained the first time it appears
- [ ] Every demo and command has its exact expected output
- [ ] Each problem is paired with how it was handled before and how it is handled now
- [ ] The core idea is stated plainly in one sentence, and restated in the recap
- [ ] Hands-on work comes before internal theory
- [ ] Every segment has a title, a pose-as-question note and a check
- [ ] Setup notes cover every operating system students use
- [ ] Setup commands were checked against the current official documentation
- [ ] The retrieval table says what each wrong answer reveals
- [ ] The student sheet has no answers in it
- [ ] There are no timings, no analogies, and no tangents unrelated to a goal

---

## 9. Generation Prompt

Paste this, fill the brackets, and attach your source material.

```text
Generate instructor-facing class material as one .md file, following my Teaching Material Template.

Course and topic: [ ]
Source material: [attached or pasted]
Audience and what they already know: [ ]
Environment (OS, tools): [ ]
Class goals (what students can do by the end): [ ]
Must cover: [ ]
Leave for later classes: [ ]
Readers: [instructor only / instructor and students]
Labs or demos: [ ]

Requirements:
- Use the skeleton, segment pattern, lab pattern and retrieval pattern from the template.
- Follow the sequencing rules: prerequisite concept first, then the topic, then the problems with before and now together, then the core idea, vocabulary, tools and setup, hands-on work, internal structure, recap, retrieval, student sheet.
- State ideas directly with definitions and concrete examples. Define every term before first use and explain every command part by part.
- Put the question to ask beside each segment title as "Pose as a question".
- Include exact expected output for every command or demo.
- Verify install and setup commands against current official documentation, and flag anything unverified.
- Leave out timings.
- Before finishing, check the result against the Quality Checklist.
- If anything in the intake is missing and changes the structure, ask me before generating.
```

---

## 10. Research Basis

| Template element | Principle behind it |
|---|---|
| Observable learning goals, each tied to a retrieval question | Backward design and constructive alignment |
| Prerequisite concept first; terms defined before use | Reducing extraneous cognitive load; building on prior knowledge |
| Questions placed before the idea; predict-run-explain | Retrieval practice; prediction before reveal |
| Question that recalls an earlier segment in each new segment | Spaced and interleaved retrieval within the session |
| Concrete demo with expected output before theory | Worked examples and modelling before independent practice |
| Hands-on work before internal structure | Learners attach abstractions to something they have observed |
| Problem, before, now | Motivation through a real task (Merrill's task-centred principle) |
| End-of-class retrieval with diagnostic table | Checking understanding; feedback that tells the instructor what to reteach |
| Homework recalling the class within 24 hours | Distributed practice |
| Student sheet with prediction log | Active engagement and self-explanation |
