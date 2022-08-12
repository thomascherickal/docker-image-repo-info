## `maven:3-amazoncorretto-18`

```console
$ docker pull maven@sha256:460e712416c459b41b9ce9a28b23e8b4df22550d73564a08bc37c141910aeb91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-18` - linux; amd64

```console
$ docker pull maven@sha256:fe31c5d7e26b909c1467b953ec5fc3294d015af2a9690e93e2ae27002a5941d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227379774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:722d2ddadd4f08e3a6381653e64db9ac04475a27faa3ecd1e2fd71cb2ea4eba9`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 12 Aug 2022 00:20:15 GMT
ADD file:56a385790046ac5dfb85932009eb1e99c8593221e306b937274c477c05cc9886 in / 
# Fri, 12 Aug 2022 00:20:15 GMT
CMD ["/bin/bash"]
# Fri, 12 Aug 2022 03:01:29 GMT
ARG version=18.0.2.9-1
# Fri, 12 Aug 2022 03:01:55 GMT
# ARGS: version=18.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-18-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-18-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 12 Aug 2022 03:01:56 GMT
ENV LANG=C.UTF-8
# Fri, 12 Aug 2022 03:01:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-18-amazon-corretto
# Fri, 12 Aug 2022 04:14:52 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 12 Aug 2022 04:14:52 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 12 Aug 2022 04:14:52 GMT
ARG USER_HOME_DIR=/root
# Fri, 12 Aug 2022 04:14:52 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 12 Aug 2022 04:14:53 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 12 Aug 2022 04:14:56 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 12 Aug 2022 04:14:56 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 12 Aug 2022 04:14:56 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 12 Aug 2022 04:14:56 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 12 Aug 2022 04:14:57 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 12 Aug 2022 04:14:57 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 12 Aug 2022 04:14:57 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5e0be87f98fb0e8a6ecddb6b717178ddc6555638e6e89d39929d47654b79739d`  
		Last Modified: Mon, 01 Aug 2022 22:09:03 GMT  
		Size: 62.3 MB (62316216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188a28cedc43dd2a2fb4b59c6bc7b5a07186690557cfb49f2750f1378654b259`  
		Last Modified: Fri, 12 Aug 2022 03:05:34 GMT  
		Size: 152.7 MB (152698531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4ca0faafcd263e4489dcba618bce153844907cdbca4584bdbd6412b94ec0cc`  
		Last Modified: Fri, 12 Aug 2022 04:17:26 GMT  
		Size: 3.6 MB (3624326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fd568edd4dc84cd51f5ff2d12f02a9d2b58739319d5d446b2d9f44f32670ed`  
		Last Modified: Fri, 12 Aug 2022 04:17:27 GMT  
		Size: 8.7 MB (8739488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787ff1a102cd8011583eed093a85f62da9e380000e263627b7048ab32de81909`  
		Last Modified: Fri, 12 Aug 2022 04:17:26 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8e896181ca41a050e49dd94cde5505215af3980c0c692a5fb560023cbb7c41`  
		Last Modified: Fri, 12 Aug 2022 04:17:26 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-18` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:685c6902262346711dc2b0d448d52f567f8a2bb21ae0f168f951fd529eba8be3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.7 MB (227651055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a7c0135784f65a382c57d69d1399c3fbc1ffd15e58e786be5a3c5988220807`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
# Wed, 20 Jul 2022 06:01:54 GMT
ARG version=18.0.2.9-1
# Wed, 20 Jul 2022 06:02:13 GMT
# ARGS: version=18.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-18-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-18-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 20 Jul 2022 06:02:13 GMT
ENV LANG=C.UTF-8
# Wed, 20 Jul 2022 06:02:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-18-amazon-corretto
# Thu, 21 Jul 2022 15:41:58 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Thu, 21 Jul 2022 15:41:58 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 21 Jul 2022 15:41:59 GMT
ARG USER_HOME_DIR=/root
# Thu, 21 Jul 2022 15:42:00 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 21 Jul 2022 15:42:01 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 21 Jul 2022 15:42:09 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 21 Jul 2022 15:42:09 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 21 Jul 2022 15:42:10 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 21 Jul 2022 15:42:12 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 21 Jul 2022 15:42:13 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 21 Jul 2022 15:42:13 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 21 Jul 2022 15:42:14 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bc5f828d044d382ed3806efb3ad9219b30d4bda213a4ca8897a42940755c10`  
		Last Modified: Wed, 20 Jul 2022 06:04:54 GMT  
		Size: 151.4 MB (151352322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b134023bf2157cb723241ab53e6f5455a760c10caf7737f4365c28fe6316b751`  
		Last Modified: Thu, 21 Jul 2022 15:45:41 GMT  
		Size: 3.6 MB (3639406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5672f406b628b859990cd9e0228ef7154459270de3c59f3349dee92e6cabe932`  
		Last Modified: Thu, 21 Jul 2022 15:45:42 GMT  
		Size: 8.7 MB (8739469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa986bdaf594ebc4398d5b582274971ae7163afdddc405f80a7823b28e78f8fa`  
		Last Modified: Thu, 21 Jul 2022 15:45:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e978000ebf2feed970484d600ddc0cc00e0b805b5c98dfa8a9a282026eef0fa4`  
		Last Modified: Thu, 21 Jul 2022 15:45:41 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
