# $ cat /etc/motd

> Harnessing the compute resources of the cloud to optimize efficiency and costs of batch and service tasks.

# $ whatis sc

Spare Cores, a Python-based open-source ecosystem, provides a comprehensive and standardized inventory, along with performance evaluations of available compute resources across public cloud and server providers.

# $ apropos sc

Spare Cores is an ecosystem, including Python packages, SDKs in other programming languages, CLI tools, public APIs, and web applications providing:

- A standardized server type listing of several cloud and other server providers, including data on compute/memory/storage/graphical processing units etc, along with benchmark scenarios and related cores/performance/cost metrics.
- An easy-to-search web application to compare listings, along with detailed product pages for each server type, including historical on-demand and spot prices, and list of similar machines.
- HTTP API and SDKs to search programatically.
- Standardized launcher CLI tool to start any instance type at the supported vendors.
- Coming soon! SaaS to seamlessly launch batch jobs and services on any supported instance type at the Spare Cores cloud environment without any vendor engagement.

# $ man sc.EXAMPLES

Using Spare Cores to find the optimal instance type among many supported vendors might be useful e.g. for the below use-cases:

- Batch (e.g. Data Science or ETL) jobs with unusual compute requirements, which are not a good fit for Kubernetes. While binpacking potentially works great for microservices, batch jobs have varying memory and compute needs and long run times, which makes them a better fit to run on dedicated (spot) instances.
- Digital artists rendering videos using GPUs.
- One-off scripts requiring a lot of memory (e.g. ad-hoc analysis you cannot run on your laptop).
- Classic CI/CD tasks (compiling and testing software), such as your expensive GitHub Action runners on private repos.
- Training ML/AI models.

