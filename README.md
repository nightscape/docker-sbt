Docker-SBT
============

## Summary

Repository name in Docker Hub: **[nightscape/docker-sbt](https://registry.hub.docker.com/u/nightscape/docker-sbt/)**

This repository contains Dockerized [Java](https://www.java.com/) and [SBT](http://www.scala-sbt.org), published to the public [Docker Hub](https://registry.hub.docker.com/) via **automated build** mechanism.



## Configuration

This docker image contains the following software stack:

- OS: Busybox.

- Java: Oracle JDK 1.8.0

- Scala: 2.11.4

- Sbt: 0.13.7



### Dependencies

* [jeanblanchard/busybox-java](https://github.com/jeanblanchard/docker-busybox-java)


### History

* 0.7 Fork from [William-Yeh/docker-java7](https://github.com/William-Yeh/docker-java7) and base on minimalistic [jeanblanchard/busybox-java](https://github.com/jeanblanchard/docker-busybox-java)

* 0.6 - Install sbt manually instead of deb.

* 0.5 - Support version tags.

* 0.4 - Fix APT dependency: openjdk-6-jre --> oracle-java7-installer.

* 0.3 - Change the Java dependency from [pulse00/java](https://github.com/dubture-dockerfiles/java) to [williamyeh/java7](https://github.com/William-Yeh/docker-java7).

* 0.2 - This repository was forked from [pulse00/scala](https://registry.hub.docker.com/u/pulse00/scala/).




## Installation


Latest version:

   ```
   $ docker pull nightscape/docker-sbt:latest
   ```



## Usage

Used mostly as a base image for other Scala-based applications. But if you'd like to use the CLI, here are some examples for you.


#### Run `sbt` REPL

```
$ docker run -it --rm nightscape/docker-sbt
```
