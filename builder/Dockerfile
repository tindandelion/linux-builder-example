FROM java:8-jdk
MAINTAINER "Sergey Moshnikov" <info@tindandelion.com>

RUN apt-get -qq update && apt-get -qq -y install g++
ADD gradle-2.3.tar.gz /
ENV PATH=/gradle-2.3/bin:$PATH

VOLUME /workspace

CMD ["gradle", "-b", "/workspace/build.gradle", "clean", "build"]




