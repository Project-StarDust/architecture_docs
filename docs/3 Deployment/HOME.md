# 3 Deployment

![diagram](https://www.plantuml.com/plantuml/svg/0/ZLHHRzem47v7od-uPGy3QOLrcpHjJqMKqKcqHQC8xIaoZY5M7JkoBq0szR_lx925CLejBudjk-_k--vphXmoYsMkeiuhgRagKm4POk6-30QMxVeRYLcvAfsmt6WK6llSv0EMMidqLfL5EHXzl9Wffd5nEnqeXi8XRINNeb2codr24T2ZpdJuutxna2o_FTmaq_5aV7VTxVdzUULGvCbuZrrNC9HC9JjZLVeMudczlf_3qk_4j3M4GbWddUy5Tgm2DE3GM04RbekK8Ojxvp2FqMeSnvbYAoKQ56DvHjrRuW1Cfv0PXm6Ko6-fvWbkeLYrPYk28lhLLxRog7FVYGEc5FXpOI-i857aLe3KQsDp-ZOwG4MTLgFapgIYwvldj1AMa2QZMLo_eDsFUx-Y3j1pcdeat2ErUYhTOsZ_aEkV4GsJIIrijzGIgwIcI6aBlvmGwQdPI7x8ZPi3UF_kydF_K__3-Z8qHt5Gfm9P9FKgaZsAaXIiumDxEb0UpRFsnP-YpjCv_Zxr8AUmRrm35ShVIZAWCsk4fTIfsH75OL7Gy7B6YQEnC9Mwt3yha9zZqx5Fb3nCuYopbuJYIX9capKAgnTK2aOQlVP7CsksacuNtICjk2yE9KhbutsGgpJFhD7oPsWCTdJne7NiYNJVXMgD_U_mRyYwmMH7SUtnwIqRxtd6z4R0DHaj57usjJNzH23Kamh-h3a8HAat3jRMv0t6txhzV-rwOcr1RqZz9oBgN0cTqf_bDm00)

**Deployment diagram**

A deployment diagram allows you to illustrate how containers in the static model are mapped to infrastructure. This deployment diagram is based upon a UML deployment diagram, although simplified slightly to show the mapping between containers and deployment nodes. A deployment node is something like physical infrastructure (e.g. a physical server or device), virtualised infrastructure (e.g. IaaS, PaaS, a virtual machine), containerised infrastructure (e.g. a Docker container), an execution environment (e.g. a database server, Java EE web/application server, Microsoft IIS), etc. Deployment nodes can be nested.

**Scope**: A single software system.

**Primary elements**: Deployment nodes and containers within the software system in scope.

**Intended audience**: Technical people inside and outside of the software development team; including software architects, developers and operations/support staff.