# ECS SW 2.0 Multiple Nodes Deployments

Welcome to the Multiple Nodes installation for ECS Software 2.0. We have provided the following deployment options: 


- **[ECS Multiple Nodes Docker Deployment](https://github.com/EMCECS/ECS-CommunityEdition/blob/master/Documentation/ECS-MultiNode-Instructions.md "ECS Multiple Node Docker Deployment Information")**
- **[ECS Docker Multi Node Deployment using Docker Machine, Docker Swarm, & Docker Compose](https://github.com/emccode/ecs-dockerswarm/ "ECS Docker Multi Node Deployment using Docker Machine, Docker Swarm, & Docker Compose Deployment Information")**
- **[ECS Multiple Nodes Puppet Deployment](https://github.com/EMCECS/ECS-CommunityEdition/blob/master/Documentation/ECS-MultiNode-Puppet-Instructions.md "ECS Multiple Node Puppet Deployment Information")**
- **[Google Compute Engine Multi Node Deployment](https://github.com/EMCECS/ECS-CommunityEdition/blob/master/Documentation/ECS-GCE-MultiNode-Instructions.md "ECS GCE Deployment Information")**


## Requirements

The Host Machines should have these following minimum requirements: 

- **Operative system:** CentOS 7
- **CPU/Cores:** 3 Cores
- **Memory:** Minimum of 16 GB RAM
- **Disks:** An unpartitioned/Raw disk with at least 200 GB of Storage per disk per host. Multiple disks can be attached on each ECS Node to increase capacity and performance. Each disk need to be un-partitioned before running the installation scripts.

For multi-node deployments, the minimum number of nodes is 3.  However, installing 4 nodes is recommended if you want redundancy against node failure and erasure coding to work (EC will be disabled if less than 4 nodes are available).

We have performed testing against the following platform(s): 

|Deployment Type | OS Name | Version |
|----------------|-------|---------|
| Docker + Scripts |CentOS	| 7.1	  |
| Docker Compose |Ubuntu	| 14	  |
| Puppet |CentOS	| 7.1	  |
