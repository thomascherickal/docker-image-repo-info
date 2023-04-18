## `maven:3-sapmachine-11`

```console
$ docker pull maven@sha256:0e158973a859ab656c5af8cc2bea89fb80efa07059cc4d9154b9a4bfc3a07811
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `maven:3-sapmachine-11` - linux; amd64

```console
$ docker pull maven@sha256:c88c42a40cd2ff8ad51c9e6590cf89735e72322aea9441bc866d65229417d5c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.3 MB (274345511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7834d9e18f55695751530a30153e4a0e367386b41b47459454f88556af2a8a6c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:18:57 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:19:26 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.18     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:19:26 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Tue, 18 Apr 2023 01:19:27 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 01:19:27 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl git --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 18 Apr 2023 01:19:27 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 18 Apr 2023 01:19:27 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Tue, 18 Apr 2023 01:19:27 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Tue, 18 Apr 2023 01:19:27 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Tue, 18 Apr 2023 01:19:27 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Tue, 18 Apr 2023 01:19:27 GMT
ARG MAVEN_VERSION=3.9.1
# Tue, 18 Apr 2023 01:19:27 GMT
ARG USER_HOME_DIR=/root
# Tue, 18 Apr 2023 01:19:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 18 Apr 2023 01:19:27 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 18 Apr 2023 01:19:27 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaa7fcf1d088a5e28885bcd22e9b185e81e5f63d784be8e835865efa147ef11`  
		Last Modified: Tue, 18 Apr 2023 01:21:26 GMT  
		Size: 7.9 MB (7917699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d1dc35b68f32b3a76b3c6fa6615d78106e3bb4ffc38e9d7ecbd420c11cbee6`  
		Last Modified: Tue, 18 Apr 2023 01:21:38 GMT  
		Size: 198.9 MB (198930476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7826f92416b0e3aab3521480fba5f946cb58a83aa714abe871b6aa443485bd6`  
		Last Modified: Tue, 18 Apr 2023 05:18:45 GMT  
		Size: 29.8 MB (29811238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bb11164c0d79061fe364a4d8642cdc501546524153d24293cb2ed56584352b`  
		Last Modified: Tue, 18 Apr 2023 05:18:41 GMT  
		Size: 9.1 MB (9106164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c73d902447e617307b4dd5c24d7324233912fa17319dc69baca9371ea342ab`  
		Last Modified: Tue, 18 Apr 2023 05:18:40 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0fb77e061bb2d576e5c624481a36b037ed2a23012c17e1e93683d564e7f85e`  
		Last Modified: Tue, 18 Apr 2023 05:18:40 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790d6c907519f9904bcad56e041e196f1c2a9ff9675dbde9284d15fc448fc5d0`  
		Last Modified: Tue, 18 Apr 2023 05:18:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-sapmachine-11` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:63142aa635a9fe53be7f637c4ef83d13beb4f15e7fb9f7fbe8cbe557fafa992a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.8 MB (270779789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19578790c6275c093f81616fdf3392917be29733798331d43e21649829c20ec`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:25:19 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:25:43 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.18     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:25:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Tue, 18 Apr 2023 02:25:45 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 02:25:45 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl git --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 18 Apr 2023 02:25:45 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 18 Apr 2023 02:25:45 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Tue, 18 Apr 2023 02:25:45 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Tue, 18 Apr 2023 02:25:45 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Tue, 18 Apr 2023 02:25:45 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Tue, 18 Apr 2023 02:25:45 GMT
ARG MAVEN_VERSION=3.9.1
# Tue, 18 Apr 2023 02:25:45 GMT
ARG USER_HOME_DIR=/root
# Tue, 18 Apr 2023 02:25:45 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 18 Apr 2023 02:25:45 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 18 Apr 2023 02:25:45 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e067d4172369eec8f6d3194c1339fa98c65b02bd1ae08f1fb5947a3792b1cb`  
		Last Modified: Tue, 18 Apr 2023 02:27:39 GMT  
		Size: 7.8 MB (7756992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f693fe6ccf712c2bc21a251ceea28d53de75ba690cfc046a240f0e3097ed0f`  
		Last Modified: Tue, 18 Apr 2023 02:27:49 GMT  
		Size: 196.9 MB (196868140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb41c656230d6efea43b49f3a5804c0f2322056a5615f40a874cbcc959d12a4`  
		Last Modified: Tue, 18 Apr 2023 03:13:06 GMT  
		Size: 29.9 MB (29850734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfb3e7931f304413785d6f72dceae61c891014c98a12ddfac5c0ee103197230`  
		Last Modified: Tue, 18 Apr 2023 03:13:05 GMT  
		Size: 9.1 MB (9106155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec24e101fc4eb49957cf1b48b6d873fff364febf9a35089ce4d37bae790d9a0`  
		Last Modified: Tue, 18 Apr 2023 03:13:03 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ebd41edc80873eb735e520c451026a6f34151998753824b4e8f71200c51021`  
		Last Modified: Tue, 18 Apr 2023 03:13:03 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c1bf4e1fcb31b004c6fb8777c962b44d3bffca21928d70d4e067d52876e67a`  
		Last Modified: Tue, 18 Apr 2023 03:13:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-sapmachine-11` - linux; ppc64le

```console
$ docker pull maven@sha256:0a904a52436123678355956156c5aa00400c57c19c92e8ddf5de4f13edf4d604
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.2 MB (273172381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b717f3e47c7dccae122e331de69cb9c5261a5e6acdc1d58d8c8471500c9d68d1`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:14:43 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:16:10 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.18     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:16:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Tue, 18 Apr 2023 01:16:15 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 01:16:15 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl git --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 18 Apr 2023 01:16:15 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 18 Apr 2023 01:16:15 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Tue, 18 Apr 2023 01:16:15 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Tue, 18 Apr 2023 01:16:15 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Tue, 18 Apr 2023 01:16:15 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Tue, 18 Apr 2023 01:16:15 GMT
ARG MAVEN_VERSION=3.9.1
# Tue, 18 Apr 2023 01:16:15 GMT
ARG USER_HOME_DIR=/root
# Tue, 18 Apr 2023 01:16:15 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 18 Apr 2023 01:16:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 18 Apr 2023 01:16:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7b240a15bddb0a3f238ea0f9dd5dcffb15162dfa03f4e233171b45b41c03e9`  
		Last Modified: Tue, 18 Apr 2023 01:22:20 GMT  
		Size: 9.3 MB (9316592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4680d4dae6266355337349d9fd4b301f24654d7ae03fe2ddb227a639b978434`  
		Last Modified: Tue, 18 Apr 2023 01:22:39 GMT  
		Size: 184.8 MB (184848643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c75f81a93e5e1989c7de57f6df2b2784e459ad9b22b15925034813eed4222`  
		Last Modified: Tue, 18 Apr 2023 02:31:50 GMT  
		Size: 36.6 MB (36598641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372119dbe857a35f3c77e8f1cae328d15d9b746ee7f3e9b522f34b8aaddbca27`  
		Last Modified: Tue, 18 Apr 2023 02:31:40 GMT  
		Size: 9.1 MB (9106160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940d2b24ff8cc0fc64e2fd7511256c6524426129b01e651cad9b2f83084a779b`  
		Last Modified: Tue, 18 Apr 2023 02:31:39 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b419dec69a76d3dfc2950911c4321796bbe308ddf0ed4fffebdd8f3b39aa673d`  
		Last Modified: Tue, 18 Apr 2023 02:31:39 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fc04cb20a721fb74f2a485e2eef0da64c20f03078a37c47d4de6eb748ee879`  
		Last Modified: Tue, 18 Apr 2023 02:31:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
