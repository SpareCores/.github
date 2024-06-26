<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/SpareCores/.github/assets/495736/2b906091-cc0b-4e05-9dbc-114e5fb1852b">
  <source media="(prefers-color-scheme: light)" srcset="https://github.com/SpareCores/.github/assets/495736/bba4ff17-0f39-413c-bbcd-3b37f65a52aa">
  <img alt="Spare Cores logo" src="https://github.com/SpareCores/.github/assets/495736/bba4ff17-0f39-413c-bbcd-3b37f65a52aa">
</picture>

# `$ cat /etc/motd`

> Harnessing the compute resources of the cloud to optimize efficiency and costs of batch and service tasks.

# `$ whatis sc`

Spare Cores, a Python-based open-source ecosystem, provides a comprehensive and standardized inventory, along with performance evaluations of available compute resources across public cloud and server providers.

# `$ apropos sc`

Spare Cores is an ecosystem, including Python packages, SDKs in other programming languages, CLI tools, public APIs, and web applications, providing:

- A standardized server type listing of several cloud and other server providers. It includes data on compute/memory/storage/graphical processing units etc, along with benchmark scenarios and related performance/cores/cost metrics.
- An easy-to-search web application to compare listings, along with detailed product pages for each server type, including historical on-demand and spot prices, and lists of similar machines.
- HTTP API and SDKs to search programmatically.
- A generalized launcher CLI tool to start any instance type at the supported vendors.
- Coming soon: SaaS for seamlessly launching batch jobs and services on any supported instance type at the Spare Cores cloud environment without any vendor engagement.

# `$ man sc.EXAMPLES`

Using Spare Cores to find the optimal instance type among many supported vendors might be useful for the below use-cases (among many other):

- Batch jobs, for example, in Data Science or ETL, often have unusual compute requirements that may not be a good fit for Kubernetes. While binpacking potentially works great for microservices, batch jobs have varying memory and compute needs, as well as long run times. This makes them a better fit to run on dedicated (spot) instances.
- Digital artists rendering videos using GPUs.
- One-off scripts requiring a lot of memory (e.g. ad-hoc analysis you cannot run on your laptop).
- Classic CI/CD tasks, like compiling and testing software, are also common use-cases. This includes scenarios such as utilizing expensive GitHub Action runners on private repositories.
- Training ML/AI models.

# `$ poetry search sc-`

Spare Cores is still in the early development phase, initiated in Q3 of 2023 and gaining momentum in 2024, particularly due to the support from NGI Search funding. Below, you can find the status and brief descriptions of all the existing and planned components:

| Component | Status | Repository | Description |
| --------- | ------ | ---------- | ----------- |
| SC Crawler | <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/Status-Alpha-blue"><source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/Status-Alpha-blue"><img alt="Project Status: Alpha" src="https://img.shields.io/badge/Status-Alpha-blue"></picture> | [![PyPI: SC Data](https://img.shields.io/pypi/v/sparecores-crawler?logo=python&logoColor=ffdd54&label=&labelColor=gray&color=blue)](https://pypi.org/project/sparecores-crawler/) [![](https://img.shields.io/badge/-sc--crawler-blue?logo=github&labelColor=gray)](https://github.com/SpareCores/sc-crawler) [![](https://img.shields.io/badge/-docs-lightblue?logo=materialformkdocs&labelColor=gray&logoColor=white)](https://sparecores.github.io/sc-crawler/) | Inventory cloud resources into a SQlite database.|
| SC Data | <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/Status-Alpha-blue"><source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/Status-Alpha-blue"><img alt="Project Status: Alpha" src="https://img.shields.io/badge/Status-Alpha-blue"></picture> | [![PyPI: SC Data](https://img.shields.io/pypi/v/sparecores-data?logo=python&logoColor=ffdd54&label=&labelColor=gray&color=blue)](https://pypi.org/project/sparecores-data/) [![](https://img.shields.io/badge/-sc--data-blue?logo=github&labelColor=gray)](https://github.com/SpareCores/sc-data) | Wrapper around data collected using the Crawler.|
| SC Keeper | <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/Status-Pre--alpha-lightblue"><source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/Status-Pre--alpha-lightblue"><img alt="Project Status: Pre Alpha" src="https://img.shields.io/badge/Status-Pre--alpha-lightblue"></picture> | [![](https://img.shields.io/badge/pip-sc--keeper-lightblue?logo=python)](https://github.com/SpareCores/sc-keeper)  | API to search the database.|
| SC Scanner | <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/Status-Pre--alpha-lightblue"><source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/Status-Pre--alpha-lightblue"><img alt="Project Status: Pre Alpha" src="https://img.shields.io/badge/Status-Pre--alpha-lightblue"></picture> | | Programming language SDKs to use the API for searching.|
| SC Runner | <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/Status-Planning-lightgrey"><source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/Status-Planning-lightgrey"><img alt="Project Status: Planning" src="https://img.shields.io/badge/Status-Planning-lightgrey"></picture> |   | Launching actual cloud instances.|

# `$ licensecheck`

[!["MPL 2.0 License](https://img.shields.io/github/license/sparecores/sc-crawler?label=software&color=blue)](https://www.mozilla.org/en-US/MPL/2.0/) [!["CC-BY-SA 4.0 License](https://img.shields.io/github/license/sparecores/sc-data?label=data&color=blue)](https://creativecommons.org/licenses/by-sa/4.0/)

# `$ git shortlog -s -n`

- Attila Nagy ([@bra-fsn](https://www.github.com/bra-fsn)): Infrastructure and Python veteran.
- Balazs Hodobay ([@palabola](https://www.github.com/palabola)): Guardian of the front-end and Node.js tools.
- Gergely Daroczi ([@daroczig](https://www.github.com/daroczig)): Hack of all trades, master of `NaN`.

[![NGI Search Open Call 3 beneficiary](https://img.shields.io/badge/NGI%20Search-Open%20Call%20%233-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4NCjwhLS0gR2VuZXJhdG9yOiBBZG9iZSBJbGx1c3RyYXRvciAyMi4xLjAsIFNWRyBFeHBvcnQgUGx1Zy1JbiAuIFNWRyBWZXJzaW9uOiA2LjAwIEJ1aWxkIDApICAtLT4NCjxzdmcgdmVyc2lvbj0iMS4xIiBpZD0iTGF5ZXJfMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeD0iMHB4IiB5PSIwcHgiDQoJIHdpZHRoPSIxODBweCIgaGVpZ2h0PSIxODBweCIgdmlld0JveD0iMCAwIDE4MCAxODAiIHN0eWxlPSJlbmFibGUtYmFja2dyb3VuZDpuZXcgMCAwIDE4MCAxODA7IiB4bWw6c3BhY2U9InByZXNlcnZlIj4NCjxzdHlsZSB0eXBlPSJ0ZXh0L2NzcyI+DQoJLnN0MHtjbGlwLXBhdGg6dXJsKCNTVkdJRF8yXyk7fQ0KCS5zdDF7Y2xpcC1wYXRoOnVybCgjU1ZHSURfNF8pO2ZpbGw6dXJsKCNTVkdJRF81Xyk7fQ0KCS5zdDJ7ZmlsbDp1cmwoI1NWR0lEXzZfKTt9DQoJLnN0M3tmaWxsOiNGRkZGRkY7fQ0KPC9zdHlsZT4NCjxnPg0KCTxnPg0KCQk8ZGVmcz4NCgkJCTxwYXRoIGlkPSJTVkdJRF8xXyIgZD0iTTkwLDVDNDMuMiw1LDUsNDMuMiw1LDkwdjBjMCw0Ni43LDM4LjIsODUsODUsODVoMGM0Ni43LDAsODUtMzguMiw4NS04NXYwQzE3NSw0My4yLDEzNi44LDUsOTAsNUw5MCw1eiINCgkJCQkvPg0KCQk8L2RlZnM+DQoJCTxjbGlwUGF0aCBpZD0iU1ZHSURfMl8iPg0KCQkJPHVzZSB4bGluazpocmVmPSIjU1ZHSURfMV8iICBzdHlsZT0ib3ZlcmZsb3c6dmlzaWJsZTsiLz4NCgkJPC9jbGlwUGF0aD4NCgkJPGcgY2xhc3M9InN0MCI+DQoJCQk8Zz4NCgkJCQk8ZGVmcz4NCgkJCQkJPHJlY3QgaWQ9IlNWR0lEXzNfIiB3aWR0aD0iMTgwIiBoZWlnaHQ9IjE4MCIvPg0KCQkJCTwvZGVmcz4NCgkJCQk8Y2xpcFBhdGggaWQ9IlNWR0lEXzRfIj4NCgkJCQkJPHVzZSB4bGluazpocmVmPSIjU1ZHSURfM18iICBzdHlsZT0ib3ZlcmZsb3c6dmlzaWJsZTsiLz4NCgkJCQk8L2NsaXBQYXRoPg0KCQkJCQ0KCQkJCQk8bGluZWFyR3JhZGllbnQgaWQ9IlNWR0lEXzVfIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgeDE9Ii0zMjQuNTY0MyIgeTE9IjIxMi4yNTg1IiB4Mj0iLTMyMy4zOTAzIiB5Mj0iMjEyLjI1ODUiIGdyYWRpZW50VHJhbnNmb3JtPSJtYXRyaXgoLTE1NS40ODE5IDE1MS4wOTY2IC0xNTEuMDk2NiAtMTU1LjQ4MTkgLTE4MjExLjA1ODYgODIwNDQuMjI2NikiPg0KCQkJCQk8c3RvcCAgb2Zmc2V0PSIwIiBzdHlsZT0ic3RvcC1jb2xvcjojRTUzNTAwIi8+DQoJCQkJCTxzdG9wICBvZmZzZXQ9IjEiIHN0eWxlPSJzdG9wLWNvbG9yOiM1MDAwMkQiLz4NCgkJCQk8L2xpbmVhckdyYWRpZW50Pg0KCQkJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMjcwLDkyLjYgODcuNCwyNzAgLTkwLDg3LjQgOTIuNiwtOTAgCQkJCSIvPg0KCQkJPC9nPg0KCQk8L2c+DQoJCTxnIGNsYXNzPSJzdDAiPg0KCQkJDQoJCQkJPGxpbmVhckdyYWRpZW50IGlkPSJTVkdJRF82XyIgZ3JhZGllbnRVbml0cz0idXNlclNwYWNlT25Vc2UiIHgxPSItMzM3Ljg2MDYiIHkxPSIxOTguNzY1NSIgeDI9Ii0zMzguMzY1MiIgeTI9IjE5OC43NzI3IiBncmFkaWVudFRyYW5zZm9ybT0ibWF0cml4KC0xMjEuNzc5NCAxMTguMzQ0NiAtMTE4LjM0NDYgLTEyMS43Nzk0IC0xNzU2MS45Mzc1IDY0MzA5LjgxMjUpIj4NCgkJCQk8c3RvcCAgb2Zmc2V0PSIwIiBzdHlsZT0ic3RvcC1jb2xvcjojNTAwMDJEIi8+DQoJCQkJPHN0b3AgIG9mZnNldD0iMSIgc3R5bGU9InN0b3AtY29sb3I6I0U1MzUwMCIvPg0KCQkJPC9saW5lYXJHcmFkaWVudD4NCgkJCTxwYXRoIGNsYXNzPSJzdDIiIGQ9Ik0xMDUuNiw4OC4yVjYzLjhjMC00LjMsMy41LTcuOCw3LjgtNy44aDBjNC4zLDAsNy44LDMuNSw3LjgsNy44djUyLjRjMCw0LjMtMy41LDcuOC03LjgsNy44aC0xLjUNCgkJCQljLTIuMywwLTQuNS0xLTYtMi44TDgwLjEsODkuN2MtMS45LTIuMy01LjctMS01LjcsMnYyNC41YzAsNC4zLTMuNSw3LjgtNy44LDcuOHMtNy44LTMuNS03LjgtNy44VjYzLjhjMC00LjMsMy41LTcuOCw3LjgtNy44DQoJCQkJaDEuNmMyLjMsMCw0LjUsMSw2LDIuOGwyNS43LDMxLjRDMTAxLjgsOTIuNiwxMDUuNiw5MS4zLDEwNS42LDg4LjJ6Ii8+DQoJCQk8cGF0aCBjbGFzcz0ic3QzIiBkPSJNNjguMiw1NmgtMS42Yy00LjMsMC03LjgsMy41LTcuOCw3Ljh2NTIuNGMwLDQuMywzLjUsNy44LDcuOCw3LjhzNy44LTMuNSw3LjgtNy44VjkxLjdjMC0zLDMuOC00LjQsNS43LTINCgkJCQlsMjUuOCwzMS41YzEuNSwxLjgsMy43LDIuOCw2LDIuOGgxLjVjNC4zLDAsNy44LTMuNSw3LjgtNy44VjYzLjhjMC00LjMtMy41LTcuOC03LjgtNy44aDBjLTQuMywwLTcuOCwzLjUtNy44LDcuOHYyNC41DQoJCQkJYzAsMy0zLjgsNC40LTUuNywyTDc0LjIsNTguOUM3Mi43LDU3LjEsNzAuNSw1Niw2OC4yLDU2eiIvPg0KCQk8L2c+DQoJPC9nPg0KPC9nPg0KPC9zdmc+DQo=)](https://www.ngisearch.eu/view/Events/OC3Searchers)

> Funded by the European Union. Views and opinions expressed are however those of the author(s) only and do not necessarily reflect those of the European Union or European Commission. Neither the European Union nor the granting authority can be held responsible for them. Funded within the framework of the NGI Search project under grant agreement No 101069364.
