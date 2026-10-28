# Table of Contents

* **Preface** .................... 1
* **Chapter 1: Retrospective On Software Quality And Java Testing** (Page 7)
    * Software quality .................... 8
    * Quality engineering .................... 8
    * Requirements and specification .................... 9
    * Quality Assurance .................... 10
    * ISO/IEC-25000 .................... 10
    * Verification and Validation .................... 12
    * Software defects .................... 14
    * Static analysis .................... 15
    * Software testing .................... 17
    * Testing levels .................... 18
    * Unit testing .................... 20
    * Integration testing .................... 21
    * System testing .................... 22
    * Testing methods .................... 22
    * Black-box testing .................... 22
    * White-box testing .................... 23
    * Non-functional testing .................... 24
    * Testing types .................... 25
    * Other testing approaches .................... 26
    * Testing frameworks for the JVM .................... 27
    * JUnit 3 .................... 28
    * Standard tests in JUnit 3 .................... 28
    * Test execution in JUnit 3 .................... 30
    * JUnit 4 .................... 33
    * Standard tests in JUnit 4 .................... 34
    * Test execution in JUnit 4 .................... 37
    * Advanced features of JUnit 4 .................... 40
    * JUnit ecosystem .................... 41
    * Summary .................... 43
* **Chapter 2: What's New In JUnit 5** (Page 45)
    * Road to JUnit 5 .................... 46
    * JUnit 5 motivation .................... 46
    * Modularity .................... 48
    * JUnit 4 runners .................... 48
    * JUnit 4 rules .................... 50
    * JUnit 5 inception .................... 50
    * JUnit 5 community .................... 52
    * JUnit 5 architecture .................... 55
    * Test Engine SPI .................... 58
    * Test Launcher API .................... 60
    * Running tests in JUnit 5 .................... 61
    * Jupiter tests with Maven .................... 61
    * Jupiter tests with Gradle .................... 64
    * Legacy tests with Maven .................... 65
    * Legacy tests with Gradle .................... 67
    * The ConsoleLauncher .................... 69
    * Jupiter tests in JUnit 4 .................... 70
    * IntelliJ .................... 73
    * Eclipse .................... 74
    * The extension model of JUnit 5 .................... 75
    * Test lifecycle .................... 77
    * Conditional extension points .................... 80
    * Dependency injection .................... 81
    * Third-party extensions .................... 83
    * Summary .................... 83
* **Chapter 3: JUnit 5 Standard Tests** (Page 85)
    * Test lifecycle .................... 86
    * Test instance lifecycle .................... 86
    * Skipping tests .................... 90
    * Display names .................... 91
    * Assertions .................... 93
    * Jupiter assertions .................... 95
    * Group of assertions .................... 96
    * Asserting exceptions .................... 99
    * Asserting timeouts .................... 100
    * Third-party assertion libraries .................... 101
    * Tagging and filtering tests .................... 105
    * Filtering tests with Maven .................... 107
    * Maven regular support .................... 108
    * Filtering tests with Gradle .................... 111
    * Meta-annotations .................... 111
    * Conditional test execution .................... 113
    * Assumptions .................... 118
    * Nested tests .................... 122
    * Repeated tests .................... 124
    * Migration from JUnit 4 to JUnit 5 .................... 129
    * Rule support in Jupiter .................... 131
    * Summary .................... 132
* **Chapter 4: Simplifying Testing With Advanced JUnit Features** (Page 137)
    * Dependency injection .................... 139
    * TestInfoParameterResolver .................... 140
    * RepetitionInfoParameterResolver .................... 140
    * TestReporterParameterResolver .................... 143
    * Dynamic tests .................... 144
    * Test interfaces .................... 145
    * Test templates .................... 152
    * Parameterized tests .................... 155
    * @ValueSource .................... 157
    * @EnumSource .................... 159
    * @MethodSource .................... 161
    * @CsvSource and @CsvFileSource .................... 165
    * @ArgumentsSource .................... 171
    * Argument conversion .................... 174
    * Implicit conversion .................... 178
    * Explicit conversion .................... 178
    * Custom names .................... 181
    * Java 9 .................... 183
    * JUnit 5 and Java 9 compatibility .................... 184
    * Beyond JUnit 5.0 .................... 186
    * Summary .................... 186
* **Chapter 5: Integration Of JUnit 5 With External Frameworks** (Page 187)
    * Mockito .................... 189
    * Mockito in a nutshell .................... 190
    * JUnit 5 extension for Mockito .................... 190
    * Spring .................... 191
    * Spring in a nutshell .................... 197
    * Spring modules .................... 214
    * Introduction to Spring Test .................... 214
    * Testing Spring Boot applications .................... 220
    * JUnit 5 extension for Spring .................... 221
    * Selenium .................... 223
    * Selenium in a nutshell .................... 225
    * JUnit 5 extension for Selenium .................... 238
    * Cucumber .................... 238
    * Cucumber in a nutshell .................... 242
    * JUnit 5 extension for Cucumber .................... 247
    * Docker .................... 247
    * Docker in a nutshell .................... 248
    * JUnit 5 extension for Docker .................... 253
    * Android .................... 253
    * Android in a nutshell .................... 254
    * Gradle plugin for JUnit 5 in Android projects .................... 257
    * REST .................... 258
    * REST in a nutshell .................... 261
    * Using REST test libraries with Jupiter .................... 264
    * Summary .................... 264
* **Chapter 6: From Requirements To Test Cases** (Page 267)
    * The importance of requirements .................... 276
    * Test planning .................... 277
    * Test design .................... 278
    * Equivalence partitioning .................... 282
    * Boundary analysis .................... 283
    * Test coverage .................... 285
    * Software testing principles .................... 286
    * The psychology of testing .................... 286
    * Test anti-patterns .................... 288
    * Code smells .................... 289
    * Summary .................... 290
* **Chapter 7: Testing Management** (Page 291)
    * Software development processes .................... 292
    * Continuous Integration .................... 293
    * Jenkins .................... 294
    * Travis CI .................... 296
    * Test reporting .................... 299
    * Maven Surefire Report .................... 301
    * Allure .................... 303
    * Defect-tracking systems .................... 305
    * Static analysis .................... 306
    * Putting all pieces together .................... 309
    * Features and requirements .................... 310
    * Design .................... 313
    * Tests .................... 313