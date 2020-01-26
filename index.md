Introduction
============

`pattoo` stores timeseries data in a database and makes it available for users via a GraphQL API.

Data can be collected from a number of sources. The `pattoo-agents` repository provides a number standard data collection agents for:

- Linux
- SNMP
- Modbus
- BACnet
- OPC UA

`pattoo` was originally created to assist DevOps and building facilities
management teams to monitor the performance of servers, applications and
electro-mechanical systems. It is flexible enough to chart a wide variety of
data that changes over time by creating custom agents.

`pattoo` currently only runs on Linux systems.

Getting Started
===============

There are four primary components to `pattoo`. These are:

- `pattoo-shared`: A shared set of software libraries used by all `pattoo`
applications.
- `pattoo`: The central system that receives data from `pattoo-agents` and
makes it available over the network via a web API.
- `pattoo-agents`: Data collection agents that report data to the `pattoo`
server.
- `pattoo-web`: A web UI that allows you to view the data stored on the
`pattoo` server.

Installation
============

Each component has detailed documentation which is listed below. The
recommended order of installation is:

- `pattoo`
- `pattoo-agents`
- `pattoo-web`

Documentation
=============

There are a number of sets of documents that cover the `pattoo`
portfolio.

Pattoo
------

The data collection server that acts as the central repository of data
provided by the `pattoo` agents.

-   The [Pattoo Server documentation](https://pattoo.readthedocs.io/)
    can be found here.
-   Visit the [Pattoo Server GitHub
    site](https://github.com/PalisadoesFoundation/pattoo) to see the
    code.

Pattoo-Agents
-------------

`pattoo` agents collect data from a variety of sources and send them to
the central `pattoo` server over HTTP. We provide a few standard agents,
but you can create your own. (See Pattoo-Shared for details)

-   The [Pattoo Agents
    documentation](https://pattoo-agents.readthedocs.io/) can be found
    here.
-   Visit the [Pattoo Agents GitHub
    site](https://github.com/PalisadoesFoundation/pattoo-agents) to see
    the code.

Pattoo-Web
----------

The web user interface to use to get access to the `pattoo` data.

-   The [Pattoo Web documentation](https://pattoo-web.readthedocs.io/)
    can be found here.
-   Visit the [Pattoo Web GitHub
    site](https://github.com/PalisadoesFoundation/pattoo-web) to see the
    code.

Pattoo-Shared
-------------

All other `pattoo` components use this shared python library. This must be
pre-installed using `pip3` for them to work. Fortunately the each component's
installation scripts automatically does this for you.

You can use the `pattoo-shared` documentation to learn the basics of
creating your own custom `pattoo-agents` to feed data to the `pattoo`
server

-   The [Pattoo Shared
    documentation](https://pattoo-shared.readthedocs.io/) can be found
    here.
-   Visit the [Pattoo Shared GitHub
    site](https://github.com/PalisadoesFoundation/pattoo-shared) to see
    the code.


About The Palisadoes Foundation
===============================

`pattoo` is based on the original `infoset` code created by the
[Palisadoes Foundation](http://www.palisadoes.org) as part of its annual
Calico Challenge program. Calico provides paid summer internships for
Jamaican university students to work on selected open source projects.
They are mentored by software professionals and receive stipends based
on the completion of predefined milestones. Calico was started in 2015.
