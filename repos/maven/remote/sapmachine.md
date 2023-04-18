## `maven:sapmachine`

```console
$ docker pull maven@sha256:a76666b8a983bef81303d2a8a143ec0064c5b3bc842b267830803812c7b4fdcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `maven:sapmachine` - linux; amd64

```console
$ docker pull maven@sha256:7a0c1438d34097123ae946e180dbb46a24c84759e3f0b72414074a66b63fb778
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.5 MB (273495458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d86fea7c4a85e5ac9b5e711f6be05ba6e5d4e02d0124a0bd27089f35cfb4dba8`
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
# Tue, 18 Apr 2023 01:20:06 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.6     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:20:06 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Tue, 18 Apr 2023 01:20:06 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 01:20:06 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl git --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 18 Apr 2023 01:20:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 18 Apr 2023 01:20:06 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Tue, 18 Apr 2023 01:20:06 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Tue, 18 Apr 2023 01:20:06 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Tue, 18 Apr 2023 01:20:06 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Tue, 18 Apr 2023 01:20:06 GMT
ARG MAVEN_VERSION=3.9.1
# Tue, 18 Apr 2023 01:20:06 GMT
ARG USER_HOME_DIR=/root
# Tue, 18 Apr 2023 01:20:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 18 Apr 2023 01:20:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 18 Apr 2023 01:20:06 GMT
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
	-	`sha256:97af029ef0ba5a27d6027cb52ca458497a95b2a8d5494c4053aafb503193315a`  
		Last Modified: Tue, 18 Apr 2023 01:22:00 GMT  
		Size: 198.1 MB (198080507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219924a94c9a232b15f7bec253b2988518ce2a11785a0574faf1f52c894a1a8a`  
		Last Modified: Tue, 18 Apr 2023 05:18:59 GMT  
		Size: 29.8 MB (29811159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d983d523ee2d01890cb8cc2461a02502ad1c3ab92ff00e26a61bc96a3dbfc568`  
		Last Modified: Tue, 18 Apr 2023 05:18:55 GMT  
		Size: 9.1 MB (9106161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9c1ff398efbaa2f12b42ee420fdf38f9a4f5078bd4eaa5114647a6eb664f0`  
		Last Modified: Tue, 18 Apr 2023 05:18:54 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a4543408c507e18aa38d1a549534fce2204340148c11cb3146305018decf3d`  
		Last Modified: Tue, 18 Apr 2023 05:18:54 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7988005ef50219d88cec7fe2ebe4f8dd2127b609d3ee84c5ea3bbd20d8f0d51f`  
		Last Modified: Tue, 18 Apr 2023 05:18:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:sapmachine` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:2fb95ec74b9c439fb283d2079d2e870ed1fa3a81e0619d46ed1e95970185c0ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.0 MB (270020222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74d1fdaaad78351fc41d96503dad84e2b0bcef45b59a9308d3a20c82211b8c7`
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
# Tue, 18 Apr 2023 02:26:16 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.6     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:26:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Tue, 18 Apr 2023 02:26:18 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 02:26:18 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl git --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 18 Apr 2023 02:26:18 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 18 Apr 2023 02:26:18 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Tue, 18 Apr 2023 02:26:18 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Tue, 18 Apr 2023 02:26:18 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Tue, 18 Apr 2023 02:26:18 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Tue, 18 Apr 2023 02:26:18 GMT
ARG MAVEN_VERSION=3.9.1
# Tue, 18 Apr 2023 02:26:18 GMT
ARG USER_HOME_DIR=/root
# Tue, 18 Apr 2023 02:26:18 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 18 Apr 2023 02:26:18 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 18 Apr 2023 02:26:18 GMT
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
	-	`sha256:42985978055623606d5a7473d3be8cee620713021ac4cefb3dfd16c98cb2d6bc`  
		Last Modified: Tue, 18 Apr 2023 02:28:08 GMT  
		Size: 196.1 MB (196108617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b653c155eec4aa741d55bd20fe1fc166970a492d06e3ee94899848697361153a`  
		Last Modified: Tue, 18 Apr 2023 03:13:20 GMT  
		Size: 29.9 MB (29850691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1345386dba3d0e9f78c1d92119d894d95192979345fb5e7538c12c62b04ea5b9`  
		Last Modified: Tue, 18 Apr 2023 03:13:17 GMT  
		Size: 9.1 MB (9106155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0f4fbb7bab30f1491dd1bc9d60a583dd2d2679d934f9f80d61f8a369afc306`  
		Last Modified: Tue, 18 Apr 2023 03:13:16 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b932c4fb45265fa1060bebe279d955c54a251761e009e4267244ea1df308e`  
		Last Modified: Tue, 18 Apr 2023 03:13:16 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc2dcabb01e9c310248d65bbc4c527ffa6dde90ebdaf31ec9c93186102cecda`  
		Last Modified: Tue, 18 Apr 2023 03:13:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:sapmachine` - linux; ppc64le

```console
$ docker pull maven@sha256:381dc2328f8baae57a690cb274074632b386e8ff79422f85fc4e3fc482cfe92f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.5 MB (286547561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79eb545169c48a8a81c457417a7970f554b24836b584c95fc7fd8e5b74de567e`
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
# Tue, 18 Apr 2023 01:18:03 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.6     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:18:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Tue, 18 Apr 2023 01:18:08 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 01:18:08 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl git --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 18 Apr 2023 01:18:08 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 18 Apr 2023 01:18:08 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Tue, 18 Apr 2023 01:18:08 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Tue, 18 Apr 2023 01:18:08 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Tue, 18 Apr 2023 01:18:08 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Tue, 18 Apr 2023 01:18:08 GMT
ARG MAVEN_VERSION=3.9.1
# Tue, 18 Apr 2023 01:18:08 GMT
ARG USER_HOME_DIR=/root
# Tue, 18 Apr 2023 01:18:08 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 18 Apr 2023 01:18:08 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 18 Apr 2023 01:18:08 GMT
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
	-	`sha256:18569d6a9c5078185f28c33f6ee8624e6cf685f2b6ad30cd706b7be4573b1cf4`  
		Last Modified: Tue, 18 Apr 2023 01:23:16 GMT  
		Size: 198.2 MB (198223906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4cce1879cae7f02846e05edd224a6675173c3f5608013e03c82e13315505a`  
		Last Modified: Tue, 18 Apr 2023 02:32:12 GMT  
		Size: 36.6 MB (36598551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54af0f284ef8d6f2f6fbf0c4da3ac22de8b575c29bb52aaf19a91da3a265a086`  
		Last Modified: Tue, 18 Apr 2023 02:32:03 GMT  
		Size: 9.1 MB (9106161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aad7b4f4c884a239cbd60f21ef63c7d7e9758c27f1b56fcc5672f0604a3dd05`  
		Last Modified: Tue, 18 Apr 2023 02:32:02 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02f41387cdb2f50ba8366e0a997d6520bfc2b459ed8c020fd5b1ffab47046d5`  
		Last Modified: Tue, 18 Apr 2023 02:32:01 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc42462f6f3450f91424263fbc55c7f1cfcd119b44660e23e6b8bdfedbb80b8a`  
		Last Modified: Tue, 18 Apr 2023 02:32:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
