
# DevConf.us

This year, I had the pleasure of attending **DevConf US**, a free conference organized by **Red Hat**.
The conference took place at Boston University.
You can find the full list of talks [here](https://youtube.com/playlist?list=PLU1vS0speL2a-MgC0CmlLi8-cC1VwRjvB&si=ssMpy7slQghp7LYK)

Here are my takeaways from the conference.

## Keynotes

### [Fireside chat with Kelsey Hightwower and Sally Ann O'Malley](https://www.youtube.com/live/dWCxGZix75s)

_Quote:_
  **You put someone in a position to success and they just might** ( Kelsey Hightower)

#### Takeaways

- There are many paths to success, and every individual is unique, learning in their own way. 
- You are unique. To stand out from the crowd, focus on discovering your personality instead of merely mimicking others.
- Being yourself comes with the challenge of risking that others might not accept you, but it allows you to attract people who genuinely appreciate your true self.
- Being **patient** and **paying attention** are crucial.
- Taking risks and making mistakes are integral parts of the often long journey to success.

The first day of the conference began with a Fireside Chat featuring Sally Ann O'Malley and the legend himself, Kelsey Hightower. 
Kelsey is a minimalist, self-taught engineer, and a retired Google Distinguished Engineer.

Kelsey shared a [fun and creative description](https://www.youtube.com/live/dWCxGZix75s?si=CHhiqHi7xaO5uUYe&t=242) 
of the essence of open source, illustrated with a real-life experience involving tailoring.

Kelsey emphasized the importance of seeing beyond the hype of AI, reminding us that it is still just a type of software. 
Understanding the basics and subtleties of AI can help debunk the hype and enable better usage of it.

Kelsey advised not to focus solely on the final achievements of successful engineers. The path to success is often a long journey, and everyone starts from a different point. 
Making mistakes is part of the process. He emphasized the importance of building on past knowledge and adapting it to new technologies. 
Kelsey also encouraged taking risks and not letting other people's fears, stemming from their own failures or limitations, hold you back.

Finally, Kelsey reminded us that [documentation](https://www.youtube.com/live/dWCxGZix75s?si=zzOdAz2kseUi1d2f&t=1513) is an essential part of the engineering process.


### [Keynote: Operation and AI with Jen Krieger](https://www.youtube.com/watch?v=MZrfs9Rswew)

_Quote:_
**Become a system thinker in everything you do; and be kind** (Jen Krieger)

#### Takeaways
- **Change lead time** plays a critical role in how organizations perform and adapt to business challenges.
- Similar to previous waves of automation, AI will impact the IT profession by rendering some jobs obsolete while creating and transforming others.
- Some technology professions cannot fully automate their tasks, sometimes leading to bottlenecks in automated environments. 
  AI tools can help address these bottlenecks by automating specific tasks.
- To avoid frustration, collaboration and transparency between business and engineering are essential.
- Humans remain at the core of an enterprise's success.

The second day began with a keynote by [Jen Krieger](https://x.com/mrry550?lang=en). 
Jen Krieger is a tech enthusiast with 25 years of experience in the open-source software space and is currently the VP of Engineering Operations at GitHub.

Jen spoke about AI and its impact on how we work. AI has existed for some time, but recent advancements have brought its usage to a broader audience.
Jen highlights the fact that we have a conflicted relationship with **change**. We need to remain open to evaluating the new tools introduced by the 
current AI movement and embrace them to improve our productivity when they prove useful. Technology can be both a benefit to our personal lives and 
a potential threat to our jobs. The current AI trend is similar to past groundbreaking technologies. We need to be mindful of the **social changes** 
brought about by technology and adopt a **systems thinking** approach to its implementation.

Some technology professions cannot fully automate their tasks. For instance, **product management** tools have not evolved as quickly as development tools. 
This can create bottlenecks in delivering enterprise software, potentially leading to unsatisfied customers and lost revenue.
AI tools can assist **product managers** by analyzing large datasets, automating workflows, and enhancing decision-making capabilities.

Jen highlights the importance of engineering and business teams collaborating to understand each other's processes and agreeing on shared workflows to streamline software delivery.
Some companies have achieved a change lead time of less than one day. High-performing teams are often the result of investments in development processes. 
Agile practices, DevOps transformations, and Cloud-Native development are a few examples of processes that help streamline the software development lifecycle.

Finally Jen emphasizes that companies need to empower teams and invest in upskilling. 


## Talks

### [Building a Better Software Supply Chain](https://youtu.be/Ye6nyDcXE_8)

#### Takeaways: 
- **Never** commit your AWS Admin Key or Any Access Key to your git repository.
- **Automation** of cluster operations is valuable, even if it takes more time initially. 
  It is essential to implement automation and documentation for predictable and reproducible cluster creation.
- Backups are easy, but recovery can be challenging. It is crucial to perform practical scenarios to ensure that the backup/recovery process works as intended.
- SRE and platform engineering efforts can be more complex than anticipated. 
  Live clusters may require 24/7 infrastructure support, monitoring, and observability. Training SREs and platform engineers on the product can take several months.
- Penetration testing can help identify obvious vulnerabilities before going live.
- Onboarding teams to new technology takes time. Providing good documentation and code examples can significantly improve the onboarding process.

This talk show the security risk that can happen during the process of delivery a solution to client.

The talk tells the story of the building of [Konflux](https://konflux-ci.dev/) by Red Hat. Konflux help developer builds a secure software supply chain process. It is a spin off of a Entreprise solution devolped at Red Hat.

Ann Marie Fred talk about the challenges encouters during the devolpment of Konflux Enterprise version. 

### [Zero-instrumentation observability based on eBPF](https://youtu.be/xDrygKuR1ZM)

#### Takeaways
- There are four observability signals: logs, metrics, traces, and profiling.
- Each observability signal contributes to a different aspect of the observability system, and they complement one another.
- Instrumentation can be either static or dynamic and may vary in scope depending on the system.
- eBPF can be used to achieve observability without modifying a program's codebase.

Peter Zaitsev presents the use of various observability signals, including logs, metrics, traces, and profiling. 
He explains the purpose of each signal and how they contribute to system observability.

[eBPF](https://ebpf.io/) allow to get visibility into many Linux kernels events. 
The talk explains how [eBPF](https://ebpf.io/) programs can be used to have observability without modifying a program's codebase. 

[Caroot](https://github.com/coroot/coroot) is a open source tool that can help add observability to a program.

### [ORAS: Powering the next generation of Cloud Native](https://youtu.be/RfMbKGWPwBw)

#### Takeaways
- OCI artifacts are an emerging standard for storing various types of artifacts for container workloads.
- OCI artifacts can benefit from the same processes and software lifecycle as OCI images.

Andrew Block presents the container runtime specification and explains the different components of a container image.

An OCI image consists of an image manifest, an optional image index, a set of filesystem layers, and a configuration. A container is a running instance of this image. Deep down, containers are files and processes.

The OCI image manifest defines the media type for the image and its layers.

OCI supports storing arbitrary content types called **artifacts**, enabling the storage and serving of content types other than container images.

OCI Artifacts can store:
- Software Bill Of Materials (SBOM)
- Signatures
- Software packages (.jar,rpm)
- AI/ML models

The benefict of OCI Artifacts :
- Standardized format and packaging: Various types of content can be stored in a standardized manner, and software lifecycle best practices applied to OCI images can also be used.
- Centralized management: OCI artifacts can be managed in the same container registries as OCI images.
- Reuse of existing tools: The same container management tools used for images can be reused.
- Evolving existing practices: OCI artifacts allow for extending the types of content that can be managed using existing best practices.

[ORAS](https://github.com/oras-project/oras) is a CNCF project that provides tooling to manage OCI artifacts. It uses a similar API to Docker for managing OCI artifacts.
The demo shows how Helm packages can be managed using OCI artifacts with ORAS.

### [Auto-Instrumenting Go Libraries for Tracing with eBPF and OpenTelemetry](https://youtu.be/GvcwiiCkMtE?si=ec_bx6Hf7YQEbCpF)

#### Takeaways
- [Open telemetry](https://opentelemetry.io/) combined with eBPF enables code auto-instrumentation and helps mitigate the risk of vendor lock-in.
- Using eBPF may introduce security concerns and performance trade-offs, which should be carefully analyzed based on the specific use case.

Open Telemetry defines [semantic conventions](https://opentelemetry.io/docs/concepts/semantic-conventions/) to help establish a **common naming scheme** 
that can be standardized across codebases, libraries, and platforms. This ensures data can be universally interpreted.

The pre-provided APIs for OpenTelemetry/eBPF instrumentation enable auto-instrumentation in Go code with minimal changes to the codebase.

It is important to note that using eBPF can raise security concerns and lead to performance trade-offs. 
For example, eBPF may require privileged access, which is often not permitted in production environments.

Additionally, log and metric signals are not yet fully supported in the available OpenTelemetry libraries.

### [Observability and instrumentation via OpenTelemetry](https://youtu.be/YVKU-MAEPY4)

#### Takeaways
- Manual and automatic instrumentation can be combined for optimal results.

This talk presents the basics of OpenTelemetry for observability and instrumentation.

Karl Johan Grahn demonstrates various instrumentation scenarios, 
comparing the behavior of no instrumentation, manual instrumentation, automatic instrumentation, 
and a combination of manual and automatic instrumentation.

The demo materials are available  [github](https://github.com/karl-johan-grahn/opentelemetry_demo).