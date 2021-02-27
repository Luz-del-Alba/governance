# Welcome to Luz del Alba™ Governance

# Platform

![alt text][logo]

[logo]: assets/diagram.png

# Infrastructure

![alt text][azure]

[azure]: assets/azure.png

Luz del Alba™ platform is mounted in an Ubuntu VM instance on Azure cloud.

Since we are using docker to release the artifacts, within the VM we are using `Docker Swarm`.

### CI/CD

Every project contains this file

```
.github/workflows/deploy.yml 
```

This file is allowing us to perform Continuous Integration and Continuous Deployment out of the box via `GitHub Actions`, so,  every time you commit on `master` you code is being deployed to our environment.

### Services

On this platform where are using several services like `redis`, `mongodb`, `postgresql` and they are maintained by us, you will
be able to stand up/tear down the services that we are using.

Please refer

```
https://github.com/Luz-del-Alba/infrastructure
```

# Application Architecture

We are using microservice fashion architecture for our platform.

Microservices are described down below: 

gateway: |

```
    API Gateway
```

app: |

```
    Frontend App
``` 

rate: |

```
   Microservice that is using MongoDB that is performing the evaluation of the prospects, given the information they provided on the frontend.
```

policy: |

```
    Microservice that is using PostgreSQL that is in charge of managing the transactional data such as customer information as well as the policy management.
```

# How Platform works

### Dashboard

![alt text][dashboard]

[dashboard]: assets/image1.jpg

This is the dashboard, the principal view where customer can see what are the types of insurance Luz del Alba™ offers.

We have a reactive comunication with `rate` service, this because if new coverages are created, this will immediately be reflected in the frontend.

Once you click on Details, you will be able to see the coverages available for that module. e.g. :

![alt text][module-detail]

[module-detail]: assets/image2.jpg

If you decided to go ahead and request a quote click on "Get a Quote", a form similar to this will be shown

![alt text][form-for-quota]

[form-for-quota]: assets/image3.jpg

When you fill all the requested inputs, the rate for you will be shown, pleace click on "Buy" to start enjoying of your new insurance.

![alt text][buy]

[buy]: assets/image4.jpg