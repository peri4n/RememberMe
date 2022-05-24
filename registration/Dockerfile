FROM openjdk:8-jdk-alpine
CMD mkdir -p /opt/RememberMe
WORKDIR /opt/RememberMe
COPY ./build/install/registration .
ENTRYPOINT ["/bin/ash -c", "registration"]
# ENTRYPOINT ["ash"]