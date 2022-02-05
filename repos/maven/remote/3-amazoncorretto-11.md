## `maven:3-amazoncorretto-11`

```console
$ docker pull maven@sha256:648a38dce9cbdeadbdf7738aa50034b340dea3890ef267a9d8e9898dd8ebcc5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-11` - linux; amd64

```console
$ docker pull maven@sha256:6b8e3ab0904a2df6725b69005f7049fb9ce4cea065bc3de1d7393a1b08937488
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.8 MB (221839418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3211cfdad699f1d7c21655c1fb5b926bb4438687486b09221fa5c1d3ab4971`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
# Sat, 05 Feb 2022 06:32:30 GMT
ARG version=11.0.14.9-1
# Sat, 05 Feb 2022 06:32:55 GMT
# ARGS: version=11.0.14.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 05 Feb 2022 06:32:56 GMT
ENV LANG=C.UTF-8
# Sat, 05 Feb 2022 06:32:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Sat, 05 Feb 2022 07:37:59 GMT
ARG MAVEN_VERSION=3.8.4
# Sat, 05 Feb 2022 07:37:59 GMT
ARG USER_HOME_DIR=/root
# Sat, 05 Feb 2022 07:37:59 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Sat, 05 Feb 2022 07:37:59 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Sat, 05 Feb 2022 07:38:11 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Sat, 05 Feb 2022 07:38:14 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 05 Feb 2022 07:38:14 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 05 Feb 2022 07:38:14 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 05 Feb 2022 07:38:15 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 05 Feb 2022 07:38:15 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 05 Feb 2022 07:38:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 05 Feb 2022 07:38:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6cf8541f1bf614954d9904dbfc3395eec63297d0f089d94cc13165c458b49`  
		Last Modified: Sat, 05 Feb 2022 06:35:59 GMT  
		Size: 146.9 MB (146871660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5013a1603aefc424bb5f8f71ae091e82051dcc820d76380390bc2742f0e3b4`  
		Last Modified: Sat, 05 Feb 2022 07:40:44 GMT  
		Size: 3.6 MB (3618900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d394b0a0b82ed8f50efd917cab6b189291f937e4e88bea75f59805bba00e6d`  
		Last Modified: Sat, 05 Feb 2022 07:40:44 GMT  
		Size: 9.1 MB (9109804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddeba6e9c03e5419580ebb2eb5521214006247f78d50cacafbda4a6c1cab726`  
		Last Modified: Sat, 05 Feb 2022 07:40:43 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01be82c3b9888b6f03865b46d60535c7b4ee561edcadc6c795386c1613ca721b`  
		Last Modified: Sat, 05 Feb 2022 07:40:43 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-11` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:89b59474641a76587a97d99e2ee7917a23e7bfb413d297984406429b8770a97e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220699962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25f3590435f04490314ddea1a2abf52773e9db350979764269493d3c5cc296cc`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 04 Feb 2022 21:33:28 GMT
ADD file:38bb92c68a8a2ac1145ea8d422911f6f0d9c62cccc02b3bdeda096047efecef5 in / 
# Fri, 04 Feb 2022 21:33:29 GMT
CMD ["/bin/bash"]
# Sat, 05 Feb 2022 00:11:17 GMT
ARG version=11.0.14.9-1
# Sat, 05 Feb 2022 00:11:34 GMT
# ARGS: version=11.0.14.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 05 Feb 2022 00:11:34 GMT
ENV LANG=C.UTF-8
# Sat, 05 Feb 2022 00:11:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Sat, 05 Feb 2022 07:08:42 GMT
ARG MAVEN_VERSION=3.8.4
# Sat, 05 Feb 2022 07:08:42 GMT
ARG USER_HOME_DIR=/root
# Sat, 05 Feb 2022 07:08:43 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Sat, 05 Feb 2022 07:08:44 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Sat, 05 Feb 2022 07:08:50 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Sat, 05 Feb 2022 07:08:59 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 05 Feb 2022 07:09:00 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 05 Feb 2022 07:09:01 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 05 Feb 2022 07:09:03 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 05 Feb 2022 07:09:04 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 05 Feb 2022 07:09:04 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 05 Feb 2022 07:09:05 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:591d91c97b5df29e14efc53ca38020094df8fa114d32d412bb8f02344aad2411`  
		Last Modified: Fri, 28 Jan 2022 02:04:32 GMT  
		Size: 63.9 MB (63857619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc71349709571db1b767f749e129bb8478cea56beff4f872d29c7ea4cd99750`  
		Last Modified: Sat, 05 Feb 2022 00:13:22 GMT  
		Size: 144.1 MB (144085880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8daca65a44d24cac64db4a0913e073449c8ccd4e364a38dd075c328793344d22`  
		Last Modified: Sat, 05 Feb 2022 07:13:02 GMT  
		Size: 3.6 MB (3645470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597fe027569d832e72e1d05a34236f2d177b176312c32a47981f496c9fce6054`  
		Last Modified: Sat, 05 Feb 2022 07:13:02 GMT  
		Size: 9.1 MB (9109775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09722b5e7a87356784ef737e9408209ee3a1398c7ff7e5288fab8c9959c8451d`  
		Last Modified: Sat, 05 Feb 2022 07:13:01 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f967704f9b5589ca17e4931f4c66755259c6df0bf16b6a9de221bfe4e72f1062`  
		Last Modified: Sat, 05 Feb 2022 07:13:01 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
