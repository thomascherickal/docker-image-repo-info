## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:de4e1c777ea15caa036256483c3aebba5f171f0b79b06e161920b7185c4f0568
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:ea9488d1e0b948bf0c758c175431cbada7cc930bdc476f576306e45bfb4e0669
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150077204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a4f4f9920ec0288565c1cadeb9ade7094fb5f0b70b5a13b48af3bb8e3f54e74`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:19:28 GMT
ARG version=1.8.0_272.b10-3
# Wed, 28 Oct 2020 00:19:52 GMT
# ARGS: version=1.8.0_272.b10-3
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:19:52 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:19:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 28 Oct 2020 00:51:09 GMT
ARG MAVEN_VERSION=3.6.3
# Wed, 28 Oct 2020 00:51:10 GMT
ARG USER_HOME_DIR=/root
# Wed, 28 Oct 2020 00:51:10 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Wed, 28 Oct 2020 00:51:10 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Wed, 28 Oct 2020 00:51:27 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 28 Oct 2020 00:51:37 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 28 Oct 2020 00:51:37 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 28 Oct 2020 00:51:37 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 28 Oct 2020 00:51:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 28 Oct 2020 00:51:38 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 28 Oct 2020 00:51:39 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 28 Oct 2020 00:51:39 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 28 Oct 2020 00:51:40 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a3c2059a8a90e1819eafb917f66ddf3baae20fcfd47bb182749d9d7ca8a2d4`  
		Last Modified: Wed, 28 Oct 2020 00:21:51 GMT  
		Size: 75.2 MB (75241034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8068fdb1f54e8e5a21b1954404f6bc49eee80c9dd0a6f0c60b5f733d678046`  
		Last Modified: Wed, 28 Oct 2020 00:54:24 GMT  
		Size: 3.5 MB (3537208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfd4b5ecc7ae8447f67d36b9fd9eae6dde95f2000ae8c66e91df551b58e9b7a`  
		Last Modified: Wed, 28 Oct 2020 00:54:25 GMT  
		Size: 9.6 MB (9581208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db23b27296847d1baf727b2c0ccfafffa9101475b39124cafa8b2de5efad631a`  
		Last Modified: Wed, 28 Oct 2020 00:54:23 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7dc21f63062697f54f831fe5fc6cb39076e41c9d1ce19a6a0ee9ca642ae377`  
		Last Modified: Wed, 28 Oct 2020 00:54:23 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:140ba64e5c15a4d90a7440830566a3287f154d5a4367643d0bfad5d58ccb8df1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.8 MB (135831955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3bfb818457459757a7179eb4339a9c14a8db59e2e3332f9d2637590144d478b`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Fri, 06 Nov 2020 23:39:33 GMT
ARG version=1.8.0_275.b01-1
# Fri, 06 Nov 2020 23:40:03 GMT
# ARGS: version=1.8.0_275.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 06 Nov 2020 23:40:04 GMT
ENV LANG=C.UTF-8
# Fri, 06 Nov 2020 23:40:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Sat, 07 Nov 2020 00:16:08 GMT
ARG MAVEN_VERSION=3.6.3
# Sat, 07 Nov 2020 00:16:09 GMT
ARG USER_HOME_DIR=/root
# Sat, 07 Nov 2020 00:16:11 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Sat, 07 Nov 2020 00:16:12 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Sat, 07 Nov 2020 00:16:32 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Sat, 07 Nov 2020 00:16:37 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 07 Nov 2020 00:16:38 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 07 Nov 2020 00:16:39 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 07 Nov 2020 00:16:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Sat, 07 Nov 2020 00:16:40 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 07 Nov 2020 00:16:41 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 07 Nov 2020 00:16:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 07 Nov 2020 00:16:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87433f2cdf56429cf79382ba8c1ae0b2aacb1ca00f4b11e52d3f38922b83943d`  
		Last Modified: Fri, 06 Nov 2020 23:41:26 GMT  
		Size: 59.3 MB (59332826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f6e312c67663233b663957beea590784354adfccb3f8f73a3d9765ec5e4888`  
		Last Modified: Sat, 07 Nov 2020 00:18:03 GMT  
		Size: 3.6 MB (3562575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34c34a7af0d219fe89aa65377cd33f59499bf4f83b7d08d6b95a461f116cf84`  
		Last Modified: Sat, 07 Nov 2020 00:18:02 GMT  
		Size: 9.6 MB (9581203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7775cda3a7d9c42d1cf37b393a2aca6573778141bfb63528cb96f42c948e237`  
		Last Modified: Sat, 07 Nov 2020 00:18:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8fd9741e2fd096df060e9065bd3ceba58133a3c0c11b38d0fe72b3e71cb987`  
		Last Modified: Sat, 07 Nov 2020 00:18:01 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
