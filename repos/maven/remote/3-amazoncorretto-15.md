## `maven:3-amazoncorretto-15`

```console
$ docker pull maven@sha256:3280a9fda49682ea06dcfc12481554726da11ba6fd7074a4b83968e95a355e3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-15` - linux; amd64

```console
$ docker pull maven@sha256:162e4b2377296d1aa14b16b124c24e5e289a17155c1531f45d8343dc1f76203c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230828672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caeed490c4d346f1c5735058efdc5434e20081e344698f13025b1d8ffd3a5b62`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:09 GMT
ADD file:15991ffbefc01e13f134972ce0eabc6b7901ea9ab4d56347bee5057302cf4848 in / 
# Wed, 23 Dec 2020 20:20:09 GMT
CMD ["/bin/bash"]
# Fri, 22 Jan 2021 23:20:01 GMT
ARG version=15.0.2.7-1
# Fri, 22 Jan 2021 23:20:19 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 22 Jan 2021 23:20:20 GMT
ENV LANG=C.UTF-8
# Fri, 22 Jan 2021 23:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
# Fri, 22 Jan 2021 23:38:59 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 22 Jan 2021 23:38:59 GMT
ARG USER_HOME_DIR=/root
# Fri, 22 Jan 2021 23:39:00 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 22 Jan 2021 23:39:00 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 22 Jan 2021 23:39:08 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 22 Jan 2021 23:39:17 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 22 Jan 2021 23:39:17 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 22 Jan 2021 23:39:17 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 22 Jan 2021 23:39:17 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 22 Jan 2021 23:39:18 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 22 Jan 2021 23:39:18 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 22 Jan 2021 23:39:18 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:4232b9ee675bb1f9a32337ec3f266a570b75c54c3c3f173b1abb998e9984ad8c`  
		Last Modified: Wed, 23 Dec 2020 20:21:42 GMT  
		Size: 62.0 MB (62007428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75963262766311d0a7d40f30c07fffa202b9e5b32f35d6cfb70ad51ce630e0f6`  
		Last Modified: Fri, 22 Jan 2021 23:21:25 GMT  
		Size: 155.7 MB (155666746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56a23309a30bcd1ffa081bc09e5c40a156662f4169a58fbd370d2a95b4b54f8`  
		Last Modified: Fri, 22 Jan 2021 23:41:12 GMT  
		Size: 3.6 MB (3572094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b25722381b9ec9e87d256bfeb6f9884989f98e7e78980ae0a7834b5f3d5ff8e`  
		Last Modified: Fri, 22 Jan 2021 23:41:13 GMT  
		Size: 9.6 MB (9581190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8ddd9e407a058037dbb098eda17d33f4bcd081635d072f568bb65430630e4b`  
		Last Modified: Fri, 22 Jan 2021 23:41:12 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdc2a03cb6d3e084946547dc5ffebc29a244167645b68cc8aceee3c7d7d8fda`  
		Last Modified: Fri, 22 Jan 2021 23:41:12 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-15` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:90ac865e6d4b7bec187d46ebfce5f1da9e95301e58a47ef1defadea9098de178
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232406192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea165413422696ab4500f16652ff8d6fffbfe4e40e603ad004950f8c12ba6c84`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 23 Dec 2020 19:39:59 GMT
ADD file:d991483ad4376be5e4327b3789511ab9266db8b87fc4b5327f0cabd1016ba00a in / 
# Wed, 23 Dec 2020 19:40:02 GMT
CMD ["/bin/bash"]
# Fri, 22 Jan 2021 23:39:43 GMT
ARG version=15.0.2.7-1
# Fri, 22 Jan 2021 23:40:19 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 22 Jan 2021 23:40:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Jan 2021 23:40:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
# Sat, 23 Jan 2021 00:04:39 GMT
ARG MAVEN_VERSION=3.6.3
# Sat, 23 Jan 2021 00:04:39 GMT
ARG USER_HOME_DIR=/root
# Sat, 23 Jan 2021 00:04:40 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Sat, 23 Jan 2021 00:04:41 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Sat, 23 Jan 2021 00:04:53 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Sat, 23 Jan 2021 00:04:57 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 23 Jan 2021 00:04:58 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 23 Jan 2021 00:04:59 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 23 Jan 2021 00:04:59 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 23 Jan 2021 00:05:00 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 23 Jan 2021 00:05:01 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 23 Jan 2021 00:05:02 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3307d2ab2034125075f0b058dcc32d6bf3e2c0595f1306de08d9e4a0287ddd76`  
		Last Modified: Wed, 23 Dec 2020 19:40:59 GMT  
		Size: 63.7 MB (63707914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97903ed68d862654dd466114bfa7e540200c8cdced49a5d6dc002e7cdd346f38`  
		Last Modified: Fri, 22 Jan 2021 23:41:13 GMT  
		Size: 155.5 MB (155538960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21e77b8d52e6857ddfac006b323acaa2028d752946b3fe85246ffa0b7e90cb9`  
		Last Modified: Sat, 23 Jan 2021 00:06:32 GMT  
		Size: 3.6 MB (3576900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcb87aa729077107f9b3914b918c77a3be16402b9bfe160f84b69f472cfe796`  
		Last Modified: Sat, 23 Jan 2021 00:06:32 GMT  
		Size: 9.6 MB (9581201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9ce3312ea1ff26e8619ca135de66b74d208dfc268891ab496b8432e7b939c6`  
		Last Modified: Sat, 23 Jan 2021 00:06:31 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b480c1e9f50a56e6a1ea8583fb2756c07a1784e0836534686d312c3ed6e316b4`  
		Last Modified: Sat, 23 Jan 2021 00:06:31 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
