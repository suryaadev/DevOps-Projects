## Java Multistage Docker file

### Stage 1 - Compile java application and create binary

- Using openjdk-11 as a base image
- create binary from that

### Stage 2

- use distroless image
- COPY binary from base to dir
- run the app
