BoardGaming.Club
=================

Currently, just a mono-repo to house my gaming group's infra and app config. Perhaps something that
will evolve into a SaaS that board gaming groups can use to organize their own gaming groups.

The Plan
--------

Curate a collection of tools, apps, and niceties that can help make communication, collaboration, 
and scheduling simpler and more enjoyable. 

### Basic Infra

Current plan is to run everything on a k3s cluster of raspbery-pis. but it would likely need to 
evolve into something with a little more horsepower at somepoint in the future. 

#### Cluster

- 4x RPI4 8gb each with 1TB SSD
- 1x RPI5 8gb with 256GB NVMe

#### Proxmox

I would like to have a hypervisor to administer all the compute through a single pane of glass, 
but proxmox does not currently support rpi4/5 as a platform. 


### Services

1. Reverse Proxy
    [Treafik](https://treafik.io)
2. static site hosting
    [nginx](https://nginx.org)
3. Chat
    [matrix](https://matrix.org)
    [synapse](https://github.com/element-hq/synapse)
    [conduit](https://conduit.rs)
    [element](https://element.io)
4. Database
    [postgres](https://www.postgresql.org)
5. Calendar/scheduling
    ???

