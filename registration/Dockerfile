FROM gradle:jdk11 as build
RUN mkdir -p /opt/RememberMe
WORKDIR /opt/RememberMe
COPY . .
RUN ./gradlew installDist

FROM openjdk:11.0.4-jre-slim
COPY --from=build /opt/RememberMe/build/install /opt/RememberMe/build/
CMD ["/opt/RememberMe/build/registration/bin/registration"]
