## Java Multistage Docker file

### Stage 1 - Compile java application and create binary

- Using openjdk-11 as a base image
- create binary from that

![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/58fd0a69-af8a-456e-a036-852beca868f4)

### Stage 2

- use distroless image
- COPY binary from base to dir
- run the app
  
![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/044af802-d25e-448e-a78d-c74dd12124bf)

### Differenece between single stage and multi-stage in terms of size

![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/56a1113c-14c3-4960-8a9d-c17f0faae6b4)
