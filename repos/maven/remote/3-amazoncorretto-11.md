## `maven:3-amazoncorretto-11`

```console
$ docker pull maven@sha256:d73e758eff62c447dccfa8ab27ce68be88d00e36b562b171d2b8102fa25bac66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-11` - linux; amd64

```console
$ docker pull maven@sha256:53c5ba3425281c7235ccaf0a8d4b7831cec77bb739312152bde9fb609be44abe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221457575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3beaba9188dd65c285a30d5d71c9e78eabd6b4945dcfe51ef49e31dd7757b2fc`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 21 Oct 2021 22:19:45 GMT
ADD file:7aef897e53c30ca977c42dd7692208abbd381b7d2e7e07a91d929f3f0ac4ea5c in / 
# Thu, 21 Oct 2021 22:19:46 GMT
CMD ["/bin/bash"]
# Thu, 21 Oct 2021 23:28:10 GMT
ARG version=11.0.13.8-1
# Thu, 21 Oct 2021 23:28:33 GMT
# ARGS: version=11.0.13.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 21 Oct 2021 23:28:34 GMT
ENV LANG=C.UTF-8
# Thu, 21 Oct 2021 23:28:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Tue, 23 Nov 2021 01:05:28 GMT
ARG MAVEN_VERSION=3.8.4
# Tue, 23 Nov 2021 01:05:28 GMT
ARG USER_HOME_DIR=/root
# Tue, 23 Nov 2021 01:05:28 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Tue, 23 Nov 2021 01:05:29 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Tue, 23 Nov 2021 01:05:42 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Tue, 23 Nov 2021 01:05:52 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 23 Nov 2021 01:05:52 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 23 Nov 2021 01:05:52 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 23 Nov 2021 01:05:52 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 23 Nov 2021 01:05:53 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 23 Nov 2021 01:05:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 23 Nov 2021 01:05:53 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5263c4cb36ce7acd05658a221ec502b376a281d7a6075ad09beb23ac02a7668c`  
		Last Modified: Wed, 20 Oct 2021 18:03:24 GMT  
		Size: 62.0 MB (61976108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9fa85bea77510327bc7908e11b491f6298bdc25fab855d9265928c2f0a9283`  
		Last Modified: Thu, 21 Oct 2021 23:32:02 GMT  
		Size: 146.8 MB (146770732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c868b9a5a83eaf0bc95347e0f670fbd76b758cb650b3562dabfa8866f291ca3`  
		Last Modified: Tue, 23 Nov 2021 01:13:13 GMT  
		Size: 3.6 MB (3599720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38c67eb365e21a6157e983e1d88ea8b2d7810752cf9845a2b33aa229545ce9e`  
		Last Modified: Tue, 23 Nov 2021 01:13:13 GMT  
		Size: 9.1 MB (9109803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33cc7064c09b11528b8a860b94ae466de05acc004ec15b0a2c08e2b6b009ee8`  
		Last Modified: Tue, 23 Nov 2021 01:13:12 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fca29d4e63be8b8782003a7bcfe4ebee73e071f4fc397463679d53e92a26b31`  
		Last Modified: Tue, 23 Nov 2021 01:13:13 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-11` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:4aadcff22ecb474847ed637be2e1d24ff29a47d55444b8951c79614bbd08bd82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.3 MB (220268497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a8cf28ffd8bfffe3acd9c03da50de44a1635903bdd5734160b33791d00bfc3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 21 Oct 2021 21:39:54 GMT
ADD file:d9148106dadecc4050f37ebf22ea9e7e56102619349368d1ce40d36f5e2fadd1 in / 
# Thu, 21 Oct 2021 21:39:55 GMT
CMD ["/bin/bash"]
# Fri, 22 Oct 2021 02:02:14 GMT
ARG version=11.0.13.8-1
# Fri, 22 Oct 2021 02:02:31 GMT
# ARGS: version=11.0.13.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 22 Oct 2021 02:02:31 GMT
ENV LANG=C.UTF-8
# Fri, 22 Oct 2021 02:02:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Tue, 23 Nov 2021 01:11:18 GMT
ARG MAVEN_VERSION=3.8.4
# Tue, 23 Nov 2021 01:11:18 GMT
ARG USER_HOME_DIR=/root
# Tue, 23 Nov 2021 01:11:19 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Tue, 23 Nov 2021 01:11:20 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Tue, 23 Nov 2021 01:11:26 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Tue, 23 Nov 2021 01:11:45 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 23 Nov 2021 01:11:45 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 23 Nov 2021 01:11:46 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 23 Nov 2021 01:11:48 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 23 Nov 2021 01:11:49 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 23 Nov 2021 01:11:49 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 23 Nov 2021 01:11:50 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e20b44047a77430ceb5678bf23278ca2841835a1b18a72adaace3d3a11c56031`  
		Last Modified: Thu, 21 Oct 2021 21:40:44 GMT  
		Size: 63.6 MB (63606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1e16f0b5b1bca9c76f0e5b214a6125a30f4a670ac4de220530010565098437`  
		Last Modified: Fri, 22 Oct 2021 02:04:58 GMT  
		Size: 143.9 MB (143929529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabc662f08a0d0f26c94c1f6c4ec5c2c681a6534df7543cb8d7e0163141ff682`  
		Last Modified: Tue, 23 Nov 2021 01:19:37 GMT  
		Size: 3.6 MB (3621096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2582869b60c84019bada94c528144cf79fcbe5d3f0caf0893166727551e23de`  
		Last Modified: Tue, 23 Nov 2021 01:19:37 GMT  
		Size: 9.1 MB (9109778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f97e87c75d9b882d019f5c2d96fb278f5a9fc5e4c492d16bccea8314b282864`  
		Last Modified: Tue, 23 Nov 2021 01:19:36 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53936aed0fdbe6b1caa77e39ecb0caf3708b964fefd852b0e0d6d0370adcceed`  
		Last Modified: Tue, 23 Nov 2021 01:19:37 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
