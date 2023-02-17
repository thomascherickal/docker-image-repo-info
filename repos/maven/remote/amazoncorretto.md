## `maven:amazoncorretto`

```console
$ docker pull maven@sha256:c86596e8d22deedcbb0bf3ddac2f98bfd12f4b5f962e1a618069c062ac07eb9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:amazoncorretto` - linux; amd64

```console
$ docker pull maven@sha256:a4214b123855b741fbfdde2f5bfa6ee139d35cfed1ec143279e8f50d5e6fec88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.9 MB (222882772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9fb29dd92db235f6637e2bf783fbe60de9b7e421e5f11d0e71050293a24ca56`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 16 Feb 2023 21:20:09 GMT
ADD file:29cd40b7c56d98385ece53bcbadfefd25bc70ccf0326777986ef6a5720bdfe83 in / 
# Thu, 16 Feb 2023 21:20:10 GMT
CMD ["/bin/bash"]
# Thu, 16 Feb 2023 21:39:40 GMT
ARG version=11.0.18.10-1
# Thu, 16 Feb 2023 21:40:07 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 16 Feb 2023 21:40:08 GMT
ENV LANG=C.UTF-8
# Thu, 16 Feb 2023 21:40:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Thu, 16 Feb 2023 22:29:28 GMT
ARG MAVEN_VERSION=3.9.0
# Thu, 16 Feb 2023 22:29:28 GMT
ARG USER_HOME_DIR=/root
# Thu, 16 Feb 2023 22:29:28 GMT
ARG SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd
# Thu, 16 Feb 2023 22:29:29 GMT
ARG BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries
# Thu, 16 Feb 2023 22:29:29 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 16 Feb 2023 22:29:29 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 16 Feb 2023 22:29:44 GMT
# ARGS: BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries MAVEN_VERSION=3.9.0 SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd USER_HOME_DIR=/root
RUN set -x   && yum install -y tar which gzip   && yum clean all   && rm -rf /var/cache/yum/*   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  apache-maven-${MAVEN_VERSION}-bin.tar.gz" | sha512sum -c -   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys   6A814B1F869C2BBEAB7CB7271A2A1C94BDE89688   29BEA2A645F2D6CED7FB12E02B172E3E156466E8   && gpg --batch --verify apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz   && mkdir -p ${MAVEN_HOME} ${MAVEN_HOME}/ref   && tar -xzf apache-maven-${MAVEN_VERSION}-bin.tar.gz -C ${MAVEN_HOME} --strip-components=1   && (rm -rf "$GNUPGHOME" apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz || true)   && ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn   && mvn --version
# Thu, 16 Feb 2023 22:29:44 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 16 Feb 2023 22:29:44 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 16 Feb 2023 22:29:45 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 16 Feb 2023 22:29:45 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d78505e615251c4f4af6eaa9507b67917d263d23551dcc5a1eed3c012d32a54d`  
		Last Modified: Wed, 15 Feb 2023 00:09:42 GMT  
		Size: 62.4 MB (62386320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faa7f030066f9d4df33cb43a964f7fca01e19c2263d1aed8fbb17fa30265232`  
		Last Modified: Thu, 16 Feb 2023 21:44:19 GMT  
		Size: 147.8 MB (147791436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6438e34cae0f61cf9d7445cd4430a00f5c65055944c168bcca9e9b4bbcd06c29`  
		Last Modified: Thu, 16 Feb 2023 22:32:24 GMT  
		Size: 12.7 MB (12703810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864ab37b35856cd38a7ac2fddc751a311dfb8c073629694ccbba7355fe80bab9`  
		Last Modified: Thu, 16 Feb 2023 22:32:23 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620baf9d47559fdc054b957ca25851f6611a27e580bda0882bd8cd461445794d`  
		Last Modified: Thu, 16 Feb 2023 22:32:23 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:2e2a9cf9fbcf140546fd2f41a6feb2f38ccc2b3585dd03401f3c1a18e9bb384b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221693129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98525c3a0fa27aeb336d769e39d92f3c398cd10d58720d1c7383f14b1b1fc403`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 16 Feb 2023 20:39:31 GMT
ADD file:17574026c2754afa903450c59a6d8f7d0905209b174cbe9c13252a61d5a6f916 in / 
# Thu, 16 Feb 2023 20:39:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Feb 2023 21:05:47 GMT
ARG version=11.0.18.10-1
# Thu, 16 Feb 2023 21:06:07 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 16 Feb 2023 21:06:08 GMT
ENV LANG=C.UTF-8
# Thu, 16 Feb 2023 21:06:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Thu, 16 Feb 2023 21:32:50 GMT
ARG MAVEN_VERSION=3.9.0
# Thu, 16 Feb 2023 21:32:50 GMT
ARG USER_HOME_DIR=/root
# Thu, 16 Feb 2023 21:32:50 GMT
ARG SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd
# Thu, 16 Feb 2023 21:32:50 GMT
ARG BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries
# Thu, 16 Feb 2023 21:32:50 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 16 Feb 2023 21:32:50 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 16 Feb 2023 21:33:05 GMT
# ARGS: BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries MAVEN_VERSION=3.9.0 SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd USER_HOME_DIR=/root
RUN set -x   && yum install -y tar which gzip   && yum clean all   && rm -rf /var/cache/yum/*   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  apache-maven-${MAVEN_VERSION}-bin.tar.gz" | sha512sum -c -   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys   6A814B1F869C2BBEAB7CB7271A2A1C94BDE89688   29BEA2A645F2D6CED7FB12E02B172E3E156466E8   && gpg --batch --verify apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz   && mkdir -p ${MAVEN_HOME} ${MAVEN_HOME}/ref   && tar -xzf apache-maven-${MAVEN_VERSION}-bin.tar.gz -C ${MAVEN_HOME} --strip-components=1   && (rm -rf "$GNUPGHOME" apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz || true)   && ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn   && mvn --version
# Thu, 16 Feb 2023 21:33:05 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 16 Feb 2023 21:33:05 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 16 Feb 2023 21:33:05 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 16 Feb 2023 21:33:05 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:71343c2791199c6e2c19c308cff6493497a02f57e225c11405e1934dc7428b3c`  
		Last Modified: Wed, 15 Feb 2023 03:16:17 GMT  
		Size: 64.0 MB (64003805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2f94ae48211bd1a594568459c26544ed87add671819456bfa5fe2bc2f1d741`  
		Last Modified: Thu, 16 Feb 2023 21:08:24 GMT  
		Size: 145.0 MB (144955124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886e2bf7b23f0af7dcf5230508d4e0091111f99284ecb486e36c43d550f5f598`  
		Last Modified: Thu, 16 Feb 2023 21:35:25 GMT  
		Size: 12.7 MB (12732992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9aeb27f854649d180d039f34fee0e5d176f8534803280e2580935cb78ffb9f`  
		Last Modified: Thu, 16 Feb 2023 21:35:24 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659ac1d36cbada3a5131f99c9e34e291c747650cc8a6599bb30021264068d449`  
		Last Modified: Thu, 16 Feb 2023 21:35:24 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
