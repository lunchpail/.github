We present Lunchpail, a tool that compiles a batch job specification into a shrinkwrapped platform binary. Application owners and platform engineers compile a binary, and users or automation run that binary to launch a job. With use cases from ML and Electronic Design Automation, we demonstrate how Lunchpail binaries facilitate a tight inner loop for collaborative development of Kubernetes batch jobs.

A Lunchpail binary encapsulates preflight configuration (e.g. secrets), launching a job, observing it, scaling it, running tasks across multiple clusters, and load balancing as the workers and workload ebbs and flows. The compiled executable relies only on built-in Kubernetes capabilities.

Using Lunchpail, team members collaborate by incrementally contributing to what it takes to run jobs well. This is done by capturing their knowledge (e.g. source code, configuration values) along with a lightweight and portable runtime, and encoding these into the binary itself — like Go, for jobs.

Lunchpail repository can be found at https://github.com/IBM/lunchpail, with some initial examples here: https://github.com/IBM/lunchpail-openroad-max-utilization, https://github.com/IBM/lunchpail-demo.
