# 1 StarDust Client

![diagram](https://www.plantuml.com/plantuml/svg/0/PP9FJ-Cm4CNlbVeTPdCA4YJBBXA24spf_f4AL8GAxIcQEcxhNSUEx34bMkrtPnn3Ao0dUpJp_7jlSk497OLMZqUVb14wD18sH9q_Bqk7ssAjQ1EMmKidh25fg12sBR5n2isZ3bqe9oT7Sus65jUpKYD9Jrog9zoDoaXNT8FuU3Ix_7sxkAyVVjt_h6VJ7zERg_mWrkVIUMloJcCltI5ay-6GyUaIuhjWLp1tzeyK11N3NWLFXx1bBi3KW4BOO2XZkQht9Djw-aIvxv0KwdfhdMvOhKhtsmeUOYKzqF7ZoaTViCKUo88dwoIiiPKD4hxJZ90hNBvGViTbLAdYX0VK6fA98oSv2FKeGPcLTIsVhV7Pu7OdzusH6tHz7XVGiATQQCKSWs1o2PEXaXt0l_48-Dk5cWUZgDzFBE8rTKTtVrD-GnM-V3u-AqwBhwlZMBj6Wsi9QH9ufuPpZNWfqNr8Q9hNBctNIaJy_yd1dTIxTNsaZycyc8sDRqdVBsNw93Pe62Y6FI34oOzp--1d36DsdHVIDCF_zGm0)

**Level 2: Container diagram**

Once you understand how your system fits in to the overall IT environment, a really useful next step is to zoom-in to the system boundary with a Container diagram. A "container" is something like a server-side web application, single-page application, desktop application, mobile app, database schema, file system, etc. Essentially, a container is a separately runnable/deployable unit (e.g. a separate process space) that executes code or stores data.

The Container diagram shows the high-level shape of the software architecture and how responsibilities are distributed across it. It also shows the major technology choices and how the containers communicate with one another. It's a simple, high-level technology focussed diagram that is useful for software developers and support/operations staff alike.

**Scope**: A single software system.

**Primary elements**: Containers within the software system in scope.
Supporting elements: People and software systems directly connected to the containers.

**Intended audience**: Technical people inside and outside of the software development team; including software architects, developers and operations/support staff.

**Notes**: This diagram says nothing about deployment scenarios, clustering, replication, failover, etc.