## Java Multistage Docker file

### Stage 1 - Compile python application and create binary

- Using python:3.10-slim as a base image
- create binary from that

### Stage 2

- use distroless image from gcr.io python3-debian11
- COPY binary from base to dir
- run the app

### Differenece between single stage and multi-stage in terms of size
