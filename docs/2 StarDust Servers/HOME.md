# 2 StarDust Servers

![diagram](https://www.plantuml.com/plantuml/svg/0/RLBBRjim4BmRy3ziVQa395BJ5YYIKrwkKy2fYpf6q9Em9cc9A4KAvDAEKFJVkvJYn7MY4pNSdTsPuKKWz1HhCnoyqrQOA1LKH4quptEFswpKLCLL3CeBPqbPoeIhSvHUezsOsCJy-lF93uEMbdUpt22fG0mLrroDsYgVDHtvS32x_3LVtXSFt-vlYzbaElb-CpvA-A8DfEfYyaZZq21fDCNMUIEFORJe_-SBU4Z8YA5BQ9GFEgHLO8ija8D0pYieiLOI2KT7Rt7ki_KyGQ31bL4x5kT5nSjxbW1e9LGkK4VAsZSyyu2tCTYkSSLKhBxzYgl4kaYR141Z8DqhV-8LUw8t2hHTEr_psTcEQa_wbOjMec_7AGiP0nNzo8uG_GqZxmFyPyRlRY7uCnm0VyzcZwFLr1PfQ-DABPXXcP0f0xC4FFMETXVmySFfMVOb-xG-JLYgWtuuSEOo-S9vDv4zwUixFNpHqISTVvEGdygy7dsOvkHHL6XB1IabsFB3IlrljhwOErNqP6NVbf89YaZRCi3QkxhtCh4y9_tQnblECkoclTGTB3ZVUm7Q0WhXl4Gh5DlGZxbGLdRF-Hy0)

**Level 2: Container diagram**

Once you understand how your system fits in to the overall IT environment, a really useful next step is to zoom-in to the system boundary with a Container diagram. A "container" is something like a server-side web application, single-page application, desktop application, mobile app, database schema, file system, etc. Essentially, a container is a separately runnable/deployable unit (e.g. a separate process space) that executes code or stores data.

The Container diagram shows the high-level shape of the software architecture and how responsibilities are distributed across it. It also shows the major technology choices and how the containers communicate with one another. It's a simple, high-level technology focussed diagram that is useful for software developers and support/operations staff alike.

**Scope**: A single software system.

**Primary elements**: Containers within the software system in scope.
Supporting elements: People and software systems directly connected to the containers.

**Intended audience**: Technical people inside and outside of the software development team; including software architects, developers and operations/support staff.

**Notes**: This diagram says nothing about deployment scenarios, clustering, replication, failover, etc.