## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:882ef4bbdf5f793958061c62a81083486070f906b4bc485dbc4b997c5bf02e51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:8e337edccff53c14e65c1fa91a78fd10e421c1e7593cc8ad8696f067c5f08a3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.3 MB (150294292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228bedbb44914558a982f1841c7c76b9d572caac7fa44f4342cdc82f7b602adc`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 09 Sep 2021 00:19:59 GMT
ADD file:bf148e5e5c33bfe39c321b4ad38c7f1068e1e4f6bfc44f5e33d3bd17f3ea65b0 in / 
# Thu, 09 Sep 2021 00:20:00 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 01:05:10 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 01:05:32 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 01:05:33 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 01:05:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Thu, 09 Sep 2021 01:25:53 GMT
ARG MAVEN_VERSION=3.8.2
# Thu, 09 Sep 2021 01:25:53 GMT
ARG USER_HOME_DIR=/root
# Thu, 09 Sep 2021 01:25:53 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Thu, 09 Sep 2021 01:25:54 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Thu, 09 Sep 2021 01:26:02 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Thu, 09 Sep 2021 01:26:04 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 09 Sep 2021 01:26:04 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 09 Sep 2021 01:26:05 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 09 Sep 2021 01:26:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Thu, 09 Sep 2021 01:26:05 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 09 Sep 2021 01:26:05 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 09 Sep 2021 01:26:05 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 09 Sep 2021 01:26:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:6b2f67060278d4a8d68cf1aaaba33c5fb108ba15b0d65d3c64c74154adb59e37`  
		Last Modified: Wed, 08 Sep 2021 08:48:25 GMT  
		Size: 62.0 MB (62000303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1def2328938d61155f42900949edc55ba0065dfb89b10b8df6b4345a90dde597`  
		Last Modified: Thu, 09 Sep 2021 01:07:20 GMT  
		Size: 75.3 MB (75313253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53a89adcfaff4739c57369df18ea445dfe34c4b0ad51d059391ec418b8ae3b4`  
		Last Modified: Thu, 09 Sep 2021 01:29:10 GMT  
		Size: 3.6 MB (3574059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513a9f91c03d3468b891714300eb7d08cff1b4ea1f9859c90a84ac5ff206dd12`  
		Last Modified: Thu, 09 Sep 2021 01:29:10 GMT  
		Size: 9.4 MB (9405466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc837cf8047b3eb23eb5aa87a69cfe24fc821a52fef660f4d40e24ffaa0a90a`  
		Last Modified: Thu, 09 Sep 2021 01:29:09 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a142fa252618cea5175f48d9ebb87b6380b303a6fe3ce55e1e805d53a1d41197`  
		Last Modified: Thu, 09 Sep 2021 01:29:09 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:638dccc86d6750f1d6e877496485bcf75026a55e5fb9c9f24876c3577342bfdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.8 MB (135848172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51baeeb3f94ab00508fd7ad5ca3dd32f77345c5d682ae70ec5e913c1f89dd4f5`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 09 Sep 2021 00:39:33 GMT
ADD file:b9ba46926c70623a28a962a14eb6ff980ce1b8dbe27b764cd8fb8f90d9de260d in / 
# Thu, 09 Sep 2021 00:39:34 GMT
CMD ["/bin/bash"]
# Thu, 09 Sep 2021 00:57:15 GMT
ARG version=1.8.0_302.b08-1
# Thu, 09 Sep 2021 00:57:36 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 09 Sep 2021 00:57:36 GMT
ENV LANG=C.UTF-8
# Thu, 09 Sep 2021 00:57:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Thu, 09 Sep 2021 02:07:14 GMT
ARG MAVEN_VERSION=3.8.2
# Thu, 09 Sep 2021 02:07:15 GMT
ARG USER_HOME_DIR=/root
# Thu, 09 Sep 2021 02:07:15 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Thu, 09 Sep 2021 02:07:15 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Thu, 09 Sep 2021 02:07:22 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Thu, 09 Sep 2021 02:07:24 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 09 Sep 2021 02:07:25 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 09 Sep 2021 02:07:25 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 09 Sep 2021 02:07:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Thu, 09 Sep 2021 02:07:25 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 09 Sep 2021 02:07:25 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 09 Sep 2021 02:07:25 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 09 Sep 2021 02:07:26 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:95c181d62dcf67412b438cf48275f91fffb0c788e3b13f41cef8dcc62842cf86`  
		Last Modified: Thu, 09 Sep 2021 00:41:06 GMT  
		Size: 63.4 MB (63430802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d7644ce683e6644a778a58cf71d3afd72066587a1faac0efaa43e346216b57`  
		Last Modified: Thu, 09 Sep 2021 00:59:24 GMT  
		Size: 59.4 MB (59403944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e1901cc4eddc9f595175c4a245df918dbce23441a38ba95406fe1167dcc950`  
		Last Modified: Thu, 09 Sep 2021 02:12:11 GMT  
		Size: 3.6 MB (3606745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad533ebf191e8a47490b907e7b48a095b87317ae573725ddf6db41bf07169dc4`  
		Last Modified: Thu, 09 Sep 2021 02:12:12 GMT  
		Size: 9.4 MB (9405466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10994988f03935d54947978783db125fbf1cd00595e1323ff2a40b373c22aa92`  
		Last Modified: Thu, 09 Sep 2021 02:12:11 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0560dfcbef106f997215f9619b4e3e7bd3d5186fc9b52e29d8a7f2092e1d11cd`  
		Last Modified: Thu, 09 Sep 2021 02:12:11 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
