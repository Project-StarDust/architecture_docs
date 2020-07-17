# Project StarDust Architecture Docs

* [Overview](#Overview)
  * [1 StarDust Client](#1-StarDust-Client)
    * [1 UnityClient Worker](#1-UnityClient-Worker)
  * [2 StarDust Servers](#2-StarDust-Servers)
    * [1 UnityGameLogic Worker](#1-UnityGameLogic-Worker)
  * [3 Deployment](#3-Deployment)

---

## Overview

![diagram](https://www.plantuml.com/plantuml/svg/0/dLHDRzim3BqNw7_GSig0Dhdij5E3D6i7f4kmj2jsCXY9iJN8aY7H-UYl7sKbTkRaj5CO-l4zae_sGo3mL9VczkQJjjBK2aL1L8Mlux67tIZNLDJhEg2NpX9Q6abNZa5v3NPhwgeUJx_SBmrOUdkPZmqG1k9KDeteFOsgXlhsPZxvlNXxpTw_lpvdyzdJxCVZy7FCBz47PuULWGFwEp5ODi60euc8gi9jnDAxFoX9hBZLnphGdTXnLm8I0AHqjQK1qwqEWR0Snf4Kup9fD7VCNATACMqoaJv5aK89SeAdir63mxwSO9KjjtbD8JqwLrWTmJ6NmZEDige9HGub2kDoBJlARBQdOQY0D9XivxnHaI3zNwp4UyoahLHCgKEqGkpW47a3EPzO5H1SvpndIpn1We6rmHEByx9WypnRAC0gKJYU9f9UZD_mHiSsi3vQzWtMpSInao30694SlVV8Dw6tABJTE5zox6n3TJGULAbjx2V-fiPABDV9U2fGADoYSLM5PPoO4Cf1SpW_qRHNSsbux2bqm0j0VzEplIp0vYp76spEAnPVBUq6dxE5jWNtuAVB-0-bKscdz8HqN6WgY_u49D8s3sBZtTbEMhylR_IP7GsjMelhDRWukmCUBxvUNe6Lo4VIoHnzwnV_qg46ep_m9FClZX4lO27lF-ucdLWmXuzqWQLJUdDe1uqr3sXLyqNv2m00)

**Level 1: System Context diagram**

A System Context diagram is a good starting point for diagramming and documenting a software system, allowing you to step back and see the big picture. Draw a diagram showing your system as a box in the centre, surrounded by its users and the other systems that it interacts with.

Detail isn't important here as this is your zoomed out view showing a big picture of the system landscape. The focus should be on people (actors, roles, personas, etc) and software systems rather than technologies, protocols and other low-level details. It's the sort of diagram that you could show to non-technical people.

**Scope**: A single software system.

**Primary elements**: The software system in scope.
Supporting elements: People (e.g. users, actors, roles, or personas) and software systems (external dependencies) that are directly connected to the software system in scope. Typically these other software systems sit outside the scope or boundary of your own software system, and you don’t have responsibility or ownership of them.

**Intended audience**: Everybody, both technical and non-technical people, inside and outside of the software development team.

## 1 StarDust Client

`\1 StarDust Client`

[Overview](#Project-StarDust-Architecture-Docs)

![diagram](https://www.plantuml.com/plantuml/svg/0/PP9FJ-Cm4CNlbVeTPdCA4YJBBXA24spf_f4AL8GAxIcQEcxhNSUEx34bMkrtPnn3Ao0dUpJp_7jlSk497OLMZqUVb14wD18sH9q_Bqk7ssAjQ1EMmKidh25fg12sBR5n2isZ3bqe9oT7Sus65jUpKYD9Jrog9zoDoaXNT8FuU3Ix_7sxkAyVVjt_h6VJ7zERg_mWrkVIUMloJcCltI5ay-6GyUaIuhjWLp1tzeyK11N3NWLFXx1bBi3KW4BOO2XZkQht9Djw-aIvxv0KwdfhdMvOhKhtsmeUOYKzqF7ZoaTViCKUo88dwoIiiPKD4hxJZ90hNBvGViTbLAdYX0VK6fA98oSv2FKeGPcLTIsVhV7Pu7OdzusH6tHz7XVGiATQQCKSWs1o2PEXaXt0l_48-Dk5cWUZgDzFBE8rTKTtVrD-GnM-V3u-AqwBhwlZMBj6Wsi9QH9ufuPpZNWfqNr8Q9hNBctNIaJy_yd1dTIxTNsaZycyc8sDRqdVBsNw93Pe62Y6FI34oOzp--1d36DsdHVIDCF_zGm0)

**Level 2: Container diagram**

Once you understand how your system fits in to the overall IT environment, a really useful next step is to zoom-in to the system boundary with a Container diagram. A "container" is something like a server-side web application, single-page application, desktop application, mobile app, database schema, file system, etc. Essentially, a container is a separately runnable/deployable unit (e.g. a separate process space) that executes code or stores data.

The Container diagram shows the high-level shape of the software architecture and how responsibilities are distributed across it. It also shows the major technology choices and how the containers communicate with one another. It's a simple, high-level technology focussed diagram that is useful for software developers and support/operations staff alike.

**Scope**: A single software system.

**Primary elements**: Containers within the software system in scope.
Supporting elements: People and software systems directly connected to the containers.

**Intended audience**: Technical people inside and outside of the software development team; including software architects, developers and operations/support staff.

**Notes**: This diagram says nothing about deployment scenarios, clustering, replication, failover, etc.

## 1 UnityClient Worker

`\1 StarDust Client\1 UnityClient Worker`

[Overview](#Project-StarDust-Architecture-Docs)

![diagram](https://www.plantuml.com/plantuml/svg/0/TPB1Rjim38Rl0V8Ed7T9WBM-xDHJCpVh2gJjq2GeTZ8Ocqs5of8XKVNSOky-KR6xR4Dz4Ydo_pzIFlUCZaEZfvCFobGwr0IFpAq_otE7tUbUyMFO1K-kieR9y6bbcnnhfz0ywz26lFXyybsZuUtrAjV8v3ccoi8shJLItoRnwMIr-76xtPJtLvjlvMfvkRovcCqbl-uzKrCkV_BCjyWATTbPf-jFaAqFyUqQxYMJnTG2Md9UUK613djW2vwj8zXZGpKoPlE_D5kD_GFkOckaxB_YJbJMqk41jGQv9tVYABAhPm9b7gnhujaQdoN08WwEof0hlzXWQdJzB1Z5VLbf5IcYt5R28aL2-aGkcyFhT0BnUrl4xE1KLewI-a143eeX8sJ5npIbVuBXSYoNGPFFPPnpPVUgWcwmUiT8nw8Z5-aviaZXQDB5LuR5IuXh7BUKHXVTEzB_e__xKWACezhISEGSkOxw1w8_JtA047Uf_YMMvsJgzCVy1W00)

**Level 3: Component diagram**

Next you can zoom in and decompose each container further to identify the major structural building blocks and their interactions.

The Component diagram shows how a container is made up of a number of "components", what each of those components are, their responsibilities and the technology/implementation details.

**Scope**: A single container.

**Primary elements**: Components within the container in scope.
Supporting elements: Containers (within the software system in scope) plus people and software systems directly connected to the components.

**Intended audience**: Software architects and developers.


## 2 StarDust Servers

`\2 StarDust Servers`

[Overview](#Project-StarDust-Architecture-Docs)

![diagram](https://www.plantuml.com/plantuml/svg/0/RLBBRjim4BmRy3ziVQa395BJ5YYIKrwkKy2fYpf6q9Em9cc9A4KAvDAEKFJVkvJYn7MY4pNSdTsPuKKWz1HhCnoyqrQOA1LKH4quptEFswpKLCLL3CeBPqbPoeIhSvHUezsOsCJy-lF93uEMbdUpt22fG0mLrroDsYgVDHtvS32x_3LVtXSFt-vlYzbaElb-CpvA-A8DfEfYyaZZq21fDCNMUIEFORJe_-SBU4Z8YA5BQ9GFEgHLO8ija8D0pYieiLOI2KT7Rt7ki_KyGQ31bL4x5kT5nSjxbW1e9LGkK4VAsZSyyu2tCTYkSSLKhBxzYgl4kaYR141Z8DqhV-8LUw8t2hHTEr_psTcEQa_wbOjMec_7AGiP0nNzo8uG_GqZxmFyPyRlRY7uCnm0VyzcZwFLr1PfQ-DABPXXcP0f0xC4FFMETXVmySFfMVOb-xG-JLYgWtuuSEOo-S9vDv4zwUixFNpHqISTVvEGdygy7dsOvkHHL6XB1IabsFB3IlrljhwOErNqP6NVbf89YaZRCi3QkxhtCh4y9_tQnblECkoclTGTB3ZVUm7Q0WhXl4Gh5DlGZxbGLdRF-Hy0)

**Level 2: Container diagram**

Once you understand how your system fits in to the overall IT environment, a really useful next step is to zoom-in to the system boundary with a Container diagram. A "container" is something like a server-side web application, single-page application, desktop application, mobile app, database schema, file system, etc. Essentially, a container is a separately runnable/deployable unit (e.g. a separate process space) that executes code or stores data.

The Container diagram shows the high-level shape of the software architecture and how responsibilities are distributed across it. It also shows the major technology choices and how the containers communicate with one another. It's a simple, high-level technology focussed diagram that is useful for software developers and support/operations staff alike.

**Scope**: A single software system.

**Primary elements**: Containers within the software system in scope.
Supporting elements: People and software systems directly connected to the containers.

**Intended audience**: Technical people inside and outside of the software development team; including software architects, developers and operations/support staff.

**Notes**: This diagram says nothing about deployment scenarios, clustering, replication, failover, etc.

## 1 UnityGameLogic Worker

`\2 StarDust Servers\1 UnityGameLogic Worker`

[Overview](#Project-StarDust-Architecture-Docs)

![diagram](https://www.plantuml.com/plantuml/svg/0/TLF1ZjCm4BrNwZyCvT9AxER2YTEMKBP8XIAwrOfJD7NSniAnmzXk2OX_PoPDI-akYHGbp-FttZnFxa94Ygcsmy4BuvHDfOOgnYQyoJB2m-tEn2fjKj2al8lQnLlbwmnBCkZsDZKfor_VVBReulhZ8hCOTOWC5Rcl6--alkd8XuF5zEjo_L0yVdYO5ulP_UpJk_54y5KRegwBsOyu3Wr6WxOuUBBbAnYjZj_B5JmACc9e2escO89OWGEs43s4w4d33cjTOiJHv3dEIxOZJr1eSMFrYSMJgjWySGk0heJAXzYHSkzxrhpYRIosMzmm5NVVliUDiAx4IG2q5cHTqmrfpiJiDHYtzLJpktSTbTmvHuh6QIhU-kHAf7QSd8bj8RBMxunYphKWzmmi190alcaQJU3NS01ydOCU7nKBHRfJwPrfWhn7n67-KfvpRf0xlre7qjyJHm1RyZLqkharNT2zw7yanUg5dXYz49kcM76nKP9iNtBWiOBfpqH7HEBhCX7wBze-xULwD3hFPpgXZ-t9tmL1x-plOJrZHhRz5d7PTnwNfmSnvu6Gsd_AhdqjBwR8E42bF9NebEOHEntxdNPbzrFy0G00)

**Level 3: Component diagram**

Next you can zoom in and decompose each container further to identify the major structural building blocks and their interactions.

The Component diagram shows how a container is made up of a number of "components", what each of those components are, their responsibilities and the technology/implementation details.

**Scope**: A single container.

**Primary elements**: Components within the container in scope.
Supporting elements: Containers (within the software system in scope) plus people and software systems directly connected to the components.

**Intended audience**: Software architects and developers.


## 3 Deployment

`\3 Deployment`

[Overview](#Project-StarDust-Architecture-Docs)

![diagram](https://www.plantuml.com/plantuml/svg/0/ZLHHRzem47v7od-uPGy3QOLrcpHjJqMKqKcqHQC8xIaoZY5M7JkoBq0szR_lx925CLejBudjk-_k--vphXmoYsMkeiuhgRagKm4POk6-30QMxVeRYLcvAfsmt6WK6llSv0EMMidqLfL5EHXzl9Wffd5nEnqeXi8XRINNeb2codr24T2ZpdJuutxna2o_FTmaq_5aV7VTxVdzUULGvCbuZrrNC9HC9JjZLVeMudczlf_3qk_4j3M4GbWddUy5Tgm2DE3GM04RbekK8Ojxvp2FqMeSnvbYAoKQ56DvHjrRuW1Cfv0PXm6Ko6-fvWbkeLYrPYk28lhLLxRog7FVYGEc5FXpOI-i857aLe3KQsDp-ZOwG4MTLgFapgIYwvldj1AMa2QZMLo_eDsFUx-Y3j1pcdeat2ErUYhTOsZ_aEkV4GsJIIrijzGIgwIcI6aBlvmGwQdPI7x8ZPi3UF_kydF_K__3-Z8qHt5Gfm9P9FKgaZsAaXIiumDxEb0UpRFsnP-YpjCv_Zxr8AUmRrm35ShVIZAWCsk4fTIfsH75OL7Gy7B6YQEnC9Mwt3yha9zZqx5Fb3nCuYopbuJYIX9capKAgnTK2aOQlVP7CsksacuNtICjk2yE9KhbutsGgpJFhD7oPsWCTdJne7NiYNJVXMgD_U_mRyYwmMH7SUtnwIqRxtd6z4R0DHaj57usjJNzH23Kamh-h3a8HAat3jRMv0t6txhzV-rwOcr1RqZz9oBgN0cTqf_bDm00)

**Deployment diagram**

A deployment diagram allows you to illustrate how containers in the static model are mapped to infrastructure. This deployment diagram is based upon a UML deployment diagram, although simplified slightly to show the mapping between containers and deployment nodes. A deployment node is something like physical infrastructure (e.g. a physical server or device), virtualised infrastructure (e.g. IaaS, PaaS, a virtual machine), containerised infrastructure (e.g. a Docker container), an execution environment (e.g. a database server, Java EE web/application server, Microsoft IIS), etc. Deployment nodes can be nested.

**Scope**: A single software system.

**Primary elements**: Deployment nodes and containers within the software system in scope.

**Intended audience**: Technical people inside and outside of the software development team; including software architects, developers and operations/support staff.