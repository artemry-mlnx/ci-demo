# Run on arm64 (aarch64) host - e.g. hpc-arm-01
# docker build --no-cache --network=host --rm --force-rm -t harbor.mellanox.com/swx-storage/jenkins-arm-slave-jnlp .
# docker login harbor.mellanox.com/swx-storage
# docker push harbor.mellanox.com/swx-storage/jenkins-arm-slave-jnlp

FROM harbor.mellanox.com/swx-storage/jenkins-arm-slave:latest
LABEL Description="This is a base image, which allows connecting Jenkins agents via JNLP protocols" Vendor="Jenkins project" Version="4.6"
COPY jenkins-slave /usr/local/bin/jenkins-slave
ENTRYPOINT ["jenkins-slave"]
