## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:1735612a6f53a2276971d6dafb32651b8a0254dff1f301d8eff56f1f2c85eab0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:774f24be7469aeeb6775effec0a341d3c6b341464a2ae6883cd1b6288259f785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.2 MB (150235179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c118349e4ae9804e82793fb507cc39268dc3d4ffe7b07783d356e6a5a044b260`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2022 00:19:49 GMT
ADD file:33ce740675602f8911c110c617b08d74ebe9c26c82226b4815019d8c2d0a2263 in / 
# Fri, 21 Oct 2022 00:19:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 01:08:12 GMT
ARG version=1.8.0_352.b08-1
# Fri, 21 Oct 2022 01:08:33 GMT
# ARGS: version=1.8.0_352.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 21 Oct 2022 01:08:33 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2022 01:08:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 21 Oct 2022 02:03:04 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 21 Oct 2022 02:03:04 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 21 Oct 2022 02:03:04 GMT
ARG USER_HOME_DIR=/root
# Fri, 21 Oct 2022 02:03:04 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 21 Oct 2022 02:03:04 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 21 Oct 2022 02:03:10 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 21 Oct 2022 02:03:11 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 21 Oct 2022 02:03:11 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 21 Oct 2022 02:03:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 21 Oct 2022 02:03:11 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 21 Oct 2022 02:03:11 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 21 Oct 2022 02:03:11 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 21 Oct 2022 02:03:11 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e3cfe889ce0a44ace07ec174bd2a7e9022e493956fba0069812a53f81a6040e2`  
		Last Modified: Wed, 19 Oct 2022 18:11:43 GMT  
		Size: 62.3 MB (62306642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16e5667014795f6356f1eca12b6db23f4d7b314fbbc976b833603bde6bcf1d4`  
		Last Modified: Fri, 21 Oct 2022 01:13:34 GMT  
		Size: 75.6 MB (75561784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4eef4063c88d393b2f7face14222b21af4ef94e1a5c17dc2a70db7c6e976dde`  
		Last Modified: Fri, 21 Oct 2022 02:06:15 GMT  
		Size: 3.6 MB (3626055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db3da01eba96439ac1e93de1faabe5a84f5023e26d54023c018e8ea597e4fb1`  
		Last Modified: Fri, 21 Oct 2022 02:06:11 GMT  
		Size: 8.7 MB (8739485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737653840084e5d7471cc05fba627b0712dc5b44564f8d1894e20d53e94b34fb`  
		Last Modified: Fri, 21 Oct 2022 02:06:10 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba14709a4909d43e24a6ef8a7dd5954851df73db2999841fd8fd9b69d07e9050`  
		Last Modified: Fri, 21 Oct 2022 02:06:10 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:e06fac5193cc52d174ff31935fa507e1da6c6a17c691d245fca590e0a80e35e3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.9 MB (135894590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d3e9628ebf1c8a48d528ff34869c52c1447041179f89d654413445c49faa325`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 20 Oct 2022 23:39:31 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Thu, 20 Oct 2022 23:39:32 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 10:45:39 GMT
ARG version=1.8.0_352.b08-1
# Wed, 26 Oct 2022 10:45:56 GMT
# ARGS: version=1.8.0_352.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 26 Oct 2022 10:45:57 GMT
ENV LANG=C.UTF-8
# Wed, 26 Oct 2022 10:45:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 26 Oct 2022 15:20:55 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 26 Oct 2022 15:20:56 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 26 Oct 2022 15:20:56 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Oct 2022 15:20:56 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 26 Oct 2022 15:20:56 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 26 Oct 2022 15:20:59 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 26 Oct 2022 15:20:59 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Oct 2022 15:20:59 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Oct 2022 15:20:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 26 Oct 2022 15:20:59 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 26 Oct 2022 15:20:59 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 26 Oct 2022 15:21:00 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Oct 2022 15:21:00 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0fce50e055487fffd4248a19eefeeb97d71de219bae42d71e2c4de48b703aa`  
		Last Modified: Wed, 26 Oct 2022 10:47:43 GMT  
		Size: 59.6 MB (59593844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e178adbb895d09c30638091d47c56f22eed0686c3fb4b6c212849edde82cf9`  
		Last Modified: Wed, 26 Oct 2022 15:26:45 GMT  
		Size: 3.6 MB (3640162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323257108d13125703e254832768a26fe713016bdfeed10f7cd77fa1832e2beb`  
		Last Modified: Wed, 26 Oct 2022 15:26:45 GMT  
		Size: 8.7 MB (8739505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd54a0f23cae6377720d2bf34e4d7d8e8134d32d68bb9f02ec287489915f37`  
		Last Modified: Wed, 26 Oct 2022 15:26:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e83beaf6d2a8c1850aaee0be60c7778fe60a450ce2eef67a6ecf0c3d7f34bce`  
		Last Modified: Wed, 26 Oct 2022 15:26:45 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
