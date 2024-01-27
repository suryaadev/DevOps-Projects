## Java Multistage Docker file

### Stage 1 - Compile python application and create binary

- Using python:3.10-slim as a base image
- create binary from that

  ![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/b6fe677a-4e2b-47f6-8893-2f6216770e75)


### Stage 2

- use distroless image from gcr.io python3-debian11
- COPY binary from base to dir
- run the app

  ![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/bdebcaf6-8c22-4c35-9c54-1af4ef28fc77)


### Differenece between single stage and multi-stage in terms of size

  ![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/e80da1ef-98c3-433a-a1aa-cae2880dc1ac)
