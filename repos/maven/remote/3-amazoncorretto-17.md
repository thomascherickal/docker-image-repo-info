## `maven:3-amazoncorretto-17`

```console
$ docker pull maven@sha256:b8cd1f328e5eb3a64cbc5577eb1d556b7547cf0afc445c30e87fd1a26526fbed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17` - linux; amd64

```console
$ docker pull maven@sha256:25952ba623b0d88d2c46c636d56396df1f0c69307300f4c3c45f52d7d84042ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226591137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8a8ba59c33135f5c43569e38797acf5969879edf7c8c0161d4c9871ccf4d674`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2022 00:19:49 GMT
ADD file:33ce740675602f8911c110c617b08d74ebe9c26c82226b4815019d8c2d0a2263 in / 
# Fri, 21 Oct 2022 00:19:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 01:09:32 GMT
ARG version=17.0.5.8-1
# Fri, 21 Oct 2022 01:09:55 GMT
# ARGS: version=17.0.5.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 21 Oct 2022 01:09:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2022 01:09:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Fri, 21 Oct 2022 02:02:07 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 21 Oct 2022 02:02:08 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 21 Oct 2022 02:02:08 GMT
ARG USER_HOME_DIR=/root
# Fri, 21 Oct 2022 02:02:08 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 21 Oct 2022 02:02:08 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 21 Oct 2022 02:02:10 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 21 Oct 2022 02:02:10 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 21 Oct 2022 02:02:10 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 21 Oct 2022 02:02:10 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 21 Oct 2022 02:02:10 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 21 Oct 2022 02:02:10 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 21 Oct 2022 02:02:10 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e3cfe889ce0a44ace07ec174bd2a7e9022e493956fba0069812a53f81a6040e2`  
		Last Modified: Wed, 19 Oct 2022 18:11:43 GMT  
		Size: 62.3 MB (62306642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eefeed6fc94246b5a24b78f66026ad1ab1b1daabce49678a93c7002e4ead91`  
		Last Modified: Fri, 21 Oct 2022 01:15:00 GMT  
		Size: 151.9 MB (151911147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803bb7d9b69ceab3f4c7a9ad123608eb6b88ae3fac1cd3c7701746c70f9cba0d`  
		Last Modified: Fri, 21 Oct 2022 02:05:28 GMT  
		Size: 3.6 MB (3632629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1775ebec947f035a40c3d5d92f8deb22c6d159477180126111fabbb790a68fd7`  
		Last Modified: Fri, 21 Oct 2022 02:05:28 GMT  
		Size: 8.7 MB (8739508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d01ae6e34d7c4aff1108c643e2fad8dbd996db80c4ad57473111fa0fea76d1`  
		Last Modified: Fri, 21 Oct 2022 02:05:27 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafe0ad9eca3a71414ebaf50412f98817a52caacf5835c1dded71b164c1d87f4`  
		Last Modified: Fri, 21 Oct 2022 02:05:27 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:0e1a0e9dc93eaec6118301da40b7c4a05f249f861d53b42a2d1a818f6633c75c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.7 MB (226746346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d9bc957ce0419ed410d3da84e82ed320a95161175b810449dad13af3af90d68`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 20 Oct 2022 23:39:31 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Thu, 20 Oct 2022 23:39:32 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 10:46:27 GMT
ARG version=17.0.5.8-1
# Wed, 26 Oct 2022 10:46:45 GMT
# ARGS: version=17.0.5.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 26 Oct 2022 10:46:47 GMT
ENV LANG=C.UTF-8
# Wed, 26 Oct 2022 10:46:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Wed, 26 Oct 2022 15:20:13 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 26 Oct 2022 15:20:13 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 26 Oct 2022 15:20:13 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Oct 2022 15:20:13 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 26 Oct 2022 15:20:13 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 26 Oct 2022 15:20:15 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 26 Oct 2022 15:20:15 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Oct 2022 15:20:15 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Oct 2022 15:20:15 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 26 Oct 2022 15:20:15 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 26 Oct 2022 15:20:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Oct 2022 15:20:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701621553aa07d15d53ab04434773dad5a892efed48c098234c8b14fd4640e64`  
		Last Modified: Wed, 26 Oct 2022 10:48:39 GMT  
		Size: 150.4 MB (150443123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf89cdb93d61bff49f9a277d81e5b2dd7a3843804189e4e8af152090dec19a9`  
		Last Modified: Wed, 26 Oct 2022 15:26:06 GMT  
		Size: 3.6 MB (3642626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0466fe12ef2e563547a75267cbf75f2b004ee3b2b92f3f3d0d3dc73ae254cf69`  
		Last Modified: Wed, 26 Oct 2022 15:26:06 GMT  
		Size: 8.7 MB (8739515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b296dd2ea19e80b3f3ad983ecd9552eb1ab6b0a154d6086bb14d342b6cbe6d`  
		Last Modified: Wed, 26 Oct 2022 15:26:05 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7767715ae6df20f704dbf26881b699051d5ba29a0054e0bc1d84c2dfb3580861`  
		Last Modified: Wed, 26 Oct 2022 15:26:05 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
