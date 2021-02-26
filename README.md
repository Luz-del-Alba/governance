# Welcome to Luz del Alba™ Governance

# Architecture

![alt text][logo]

[logo]: assets/diagram.png

# Infrastructure

![alt text][azure]

[azure]: assets/azure.png

The platform is mounted in Ubuntu VM instance on azure cloud.

Since we are using docker to release the artifacts, within the VM we are managing Docker Swarm.

### CI/CD

Every project contains this file

```
.github/workflows/deploy.yml 
```

This file is allowing us to perform Continuous Integration and Continuous Deployment out of the box via `GitHub Actions`

This enables us to deploy to our environment every time you commit on `master`

### Services

On this platform where are using several servis like `redis`, `mongodb`, `postgresql` and is maintained by us, you will
be able to stand up/tear down the services that we are using.

Please refer

```
https://github.com/Luz-del-Alba/infrastructure
```

# Application architecture

We are using microservice fashion arquitecture to out platform.

as righ now, we are using only two microsevices

gateway: |

```
    API Gateway
```

rate: |

```
   Microservice using MongoDB that is performing the evaluation of the prospects, given the information they provided on the frontend.
```

policy: |

```
    Microservice that is in charge of managing the transactional data such as customer information as well as the policy management.
```

app: |

```
    Frontend App
``` 

# How the platform works

