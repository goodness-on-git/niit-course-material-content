## Table of Contents

* **Horizontal pod autoscaling** — 370
  * **Using the horizontal pod autoscaler** — 371
* **Cluster autoscaling** — 373
* **Vertical pod autoscaling** — 374
* **Provisioning resources with Kubernetes** — 376
  * **What resources should you provision?** — 376
  * **Defining container limits** — 377
  * **Specifying resource quotas** — 379
  * **Manual provisioning** — 380
  * **Utilizing autoscaling** — 380
  * **Rolling your own automated provisioning** — 380
* **Getting performance right** — 381
  * **Performance and user experience** — 382
  * **Performance and high availability** — 382
  * **Performance and cost** — 382
  * **Performance and security** — 383
* **Logging** — 383
  * **What should you log?** — 384
  * **Logging versus error reporting** — 384
  * **The quest for the perfect Go logging interface** — 384
  * **Logging with Go-kit** — 385
    * **Setting up a logger with Go-kit** — 385
    * **Using a logging middleware** — 387
  * **Centralized logging with Kubernetes** — 390
* **Collecting metrics on Kubernetes** — 391
  * **Introducing the Kubernetes metrics API** — 391
  * **Understanding the Kubernetes metrics server** — 392
  * **Using Prometheus** — 394
    * **Deploying Prometheus into the cluster** — 394
    * **Recording custom metrics from Delinkcious** — 399
* **Alerting** — 403
  * **Embracing component failure** — 403
  * **Grudgingly accepting system failure** — 404
  * **Taking human factors into account** — 404
    * **Warnings versus alerts** — 404
    * **Considering severity levels** — 405
    * **Determining alert channels** — 405
    * **Fine-tuning noisy alerts** — 405
  * **Utilizing the Prometheus alert manager** — 406
    * **Configuring alerts in Prometheus** — 407
* **Distributed tracing** — 407
  * **Installing Jaeger** — 408
  * **Integrating tracing into your services** — 410
* **Summary** — 412
* **Further reading** — 412

***

**Chapter 13: Service Mesh - Working with Istio** — 413
* **Technical requirements** — 413
  * **The code** — 415
* **What is a service mesh?** — 415
  * **Comparing monoliths to microservices** — 415
  * **Using a shared library to manage the cross-cutting concerns of microservices** — 416
  * **Using a service mesh to manage the cross-cutting concerns of microservices** — 417
  * **Understanding the relationship between Kubernetes and a service mesh** — 418
* **What does Istio bring to the table?** — 419
  * **Getting to know the Istio architecture** — 419
    * **Envoy** — 420
    * **Pilot** — 421
    * **Mixer** — 421
    * **Citadel** — 422
    * **Galley** — 422
  * **Managing traffic with Istio** — 422
    * **Routing requests** — 423
    * **Load balancing** — 423
    * **Handling failures** — 424
    * **Injecting faults for testing** — 426
    * **Doing canary deployments** — 426
  * **Securing your cluster with Istio** — 427
    * **Understanding Istio identity** — 428
    * **Authenticating users with Istio** — 428
    * **Authorizing requests with Istio** — 429
  * **Enforcing policies with Istio** — 432
  * **Collecting metrics with Istio** — 432
  * **When should you avoid Istio?** — 434
* **Delinkcious on Istio** — 435
  * **Removing mutual authentication between services** — 435
  * **Utilizing better canary deployments** — 438
  * **Automatic logging and error reporting** — 439
  * **Accommodating NATS** — 441
  * **Examining the Istio footprint** — 442
* **Alternatives to Istio** — 444
  * **Linkerd 2.0** — 445
  * **Envoy** — 445
  * **HashiCorp Consul** — 445
  * **AWS App Mesh** — 446
  * **Others** — 446
  * **The no mesh option** — 446
* **Summary** — 446
* **Further reading** — 447

***

**Chapter 14: The Future of Microservices and Kubernetes** — 449
* **The future of microservices** — 450
  * **Microservices versus serverless functions** — 450
  * **Microservices, containers, and orchestration** — 451
  * **gRPC and gRPC-Web** — 451
  * **GraphQL** — 452
  * **HTTP/3 is coming** — 452
* **The future of Kubernetes** — 453
  * **Kubernetes extensibility** — 454
    * **Abstracting the container runtime** — 454
    * **Abstracting networking** — 455
    * **Abstracting storage** — 455
    * **The cloud provider interface** — 456
  * **Service mesh integration** — 457
  * **Serverless computing on Kubernetes** — 458
  * **Kubernetes and VMs** — 459
    * **gVisor** — 460
    * **Firecracker** — 460
    * **Kata containers** — 460
  * **Cluster autoscaling** — 461
  * **Using operators** — 461
  * **Federation** — 463
* **Summary** — 464
* **Further reading** — 465

***

**Other Books You May Enjoy** — 467

**Index** — 471