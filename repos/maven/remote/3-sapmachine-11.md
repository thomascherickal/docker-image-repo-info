## `maven:3-sapmachine-11`

```console
$ docker pull maven@sha256:fa7541d7cb7a823aa25a6bad8eeb28b1f0ec8e68dbb2153e9dd389264b28f26a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `maven:3-sapmachine-11` - linux; amd64

```console
$ docker pull maven@sha256:b67259aee55917ce6ec2bc8bf2361a7614bc5fb33c993f9a45c3d05e79e397a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.6 MB (275562216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c973821f7acfea675fe95c954700dcb03f97cbfb0da2886fdd391f55e6fea436`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:33 GMT
ADD file:8a50ad78a668527e974b05a3dfbfd64760de3cb643ceb8a8805d21f6ceab3389 in / 
# Thu, 03 Mar 2022 20:19:33 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 23:30:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 23:30:32 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.14.1     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 23:30:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Thu, 03 Mar 2022 23:30:32 GMT
CMD ["jshell"]
# Fri, 04 Mar 2022 02:23:14 GMT
RUN apt-get update     && apt-get install -y curl git     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 02:23:15 GMT
ARG MAVEN_VERSION=3.8.4
# Fri, 04 Mar 2022 02:23:15 GMT
ARG USER_HOME_DIR=/root
# Fri, 04 Mar 2022 02:23:15 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Fri, 04 Mar 2022 02:23:15 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Fri, 04 Mar 2022 02:23:16 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 04 Mar 2022 02:23:16 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 04 Mar 2022 02:23:16 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 04 Mar 2022 02:23:16 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 04 Mar 2022 02:23:16 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 04 Mar 2022 02:23:16 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 04 Mar 2022 02:23:17 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:7c3b88808835aa80f1ef7f03083c5ae781d0f44e644537cd72de4ce6c5e62e00`  
		Last Modified: Thu, 03 Mar 2022 20:20:44 GMT  
		Size: 28.6 MB (28565751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ab19b53a1b84fb848704b282f933869153728103e9a9276d9ad881cf6a4c71`  
		Last Modified: Thu, 03 Mar 2022 23:31:22 GMT  
		Size: 8.3 MB (8318294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27de5ce49c862e59e6339d565ab8ad01196ed8fc48e6dc4f6ef06907244e133`  
		Last Modified: Thu, 03 Mar 2022 23:31:35 GMT  
		Size: 197.7 MB (197710980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3789de55b624fa7a7cbcfef4cd2c379d9599d7a60174e15a366c5150e10dd3a`  
		Last Modified: Fri, 04 Mar 2022 02:27:31 GMT  
		Size: 31.9 MB (31856158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23d40dac038586c899bdf7fc75bfa71e58b31c2927e9ce765db36fe066b5c6`  
		Last Modified: Fri, 04 Mar 2022 02:27:27 GMT  
		Size: 9.1 MB (9109824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2596dedc11dd47f1ac8a94805eb6969f69519d57a8a005ca23b6d4ce345023`  
		Last Modified: Fri, 04 Mar 2022 02:27:26 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c03f821a9807164046db2892c26000fe46cf182d164ac473a1b3c26fee0889c`  
		Last Modified: Fri, 04 Mar 2022 02:27:26 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
