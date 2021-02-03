<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rapidoid`

-	[`rapidoid:5`](#rapidoid5)
-	[`rapidoid:5.4`](#rapidoid54)
-	[`rapidoid:5.4.6`](#rapidoid546)
-	[`rapidoid:latest`](#rapidoidlatest)

## `rapidoid:5`

```console
$ docker pull rapidoid@sha256:ab0735787e46b137be758c0a292b80f1fe8c82516f0fda6412de5c18b4ed3dea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `rapidoid:5` - linux; arm64 variant v8

```console
$ docker pull rapidoid@sha256:caaf2185ded6e242605bbafe735dce572a0fe6b927702fd58b140c9a5f79ae40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83914069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff166b35f84c89947de28dd53abfe28122ddc85c997c3e9589004282544d835`
-	Entrypoint: `["\/opt\/entrypoint.sh"]`

```dockerfile
# Wed, 08 May 2019 08:49:02 GMT
ADD file:fadb1563a7cd043d96e76895bb1bb3920f9a9262206eb9bcd4ef4b5aec8d9b35 in / 
# Wed, 08 May 2019 08:49:03 GMT
CMD ["bash"]
# Fri, 17 May 2019 22:45:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 17 May 2019 22:49:44 GMT
ENV LANG=C.UTF-8
# Fri, 17 May 2019 22:49:46 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 17 May 2019 22:49:47 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 17 May 2019 22:51:43 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Fri, 17 May 2019 22:51:44 GMT
ENV JAVA_VERSION=8u212
# Fri, 17 May 2019 22:51:44 GMT
ENV JAVA_DEBIAN_VERSION=8u212-b01-1~deb9u1
# Fri, 17 May 2019 22:52:10 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Wed, 16 Sep 2020 21:04:19 GMT
MAINTAINER Nikolche Mihajlovski
# Wed, 16 Sep 2020 21:04:20 GMT
ENV GPG_KEY=E306FEF548C686C23DC00242B9B08D8F616EF49C
# Wed, 16 Sep 2020 21:04:21 GMT
ENV RAPIDOID_JAR=/opt/rapidoid.jar
# Wed, 16 Sep 2020 21:04:22 GMT
ENV RAPIDOID_TMP=/tmp/rapidoid
# Wed, 16 Sep 2020 21:04:24 GMT
WORKDIR /opt
# Wed, 16 Sep 2020 21:04:25 GMT
EXPOSE 8888
# Wed, 16 Sep 2020 21:04:26 GMT
VOLUME [/data]
# Wed, 16 Sep 2020 21:04:27 GMT
ENV RAPIDOID_VERSION=5.4.6
# Wed, 16 Sep 2020 21:04:29 GMT
ENV RAPIDOID_URL=https://repo1.maven.org/maven2/org/rapidoid/rapidoid-platform/5.4.6/rapidoid-platform-5.4.6.jar
# Wed, 16 Sep 2020 21:04:29 GMT
COPY file:54eb4a0f21aca6721ebea0745a2cbfeb12c799c7a0902f588f490fc0afa8e8ea in /opt/ 
# Wed, 16 Sep 2020 21:05:04 GMT
RUN set -xe     && apt-get update     && apt-get install -y --no-install-recommends         ca-certificates curl dirmngr gnupg     && mkdir /platform     && mkdir -p "$RAPIDOID_TMP" 	&& curl -SL "$RAPIDOID_URL" -o $RAPIDOID_JAR 	&& curl -SL "$RAPIDOID_URL.asc" -o $RAPIDOID_JAR.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys $GPG_KEY 	&& gpg --batch --verify $RAPIDOID_JAR.asc $RAPIDOID_JAR 	&& rm -rf "$GNUPGHOME" 	&& rm "$RAPIDOID_JAR.asc" 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 21:05:05 GMT
ENTRYPOINT ["/opt/entrypoint.sh"]
```

-	Layers:
	-	`sha256:29b80961214d7f0c89081fe8134e6e8e14ccfa1afe001357539f59930ff9e3ef`  
		Last Modified: Wed, 08 May 2019 08:55:12 GMT  
		Size: 20.3 MB (20333815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392e0924564e298648b4a7b2ebc774103f98526dd2afd1c948697b4c6686300f`  
		Last Modified: Fri, 17 May 2019 22:55:11 GMT  
		Size: 441.1 KB (441065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15c6e01e710610402034472504e3628bdd00c2b0907f3ec4364f8e71a38d8c0`  
		Last Modified: Fri, 17 May 2019 22:58:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acba4335cd44174a82b7a5d29d7b9dacc9e0b19f066b622c972c573edeb4dddd`  
		Last Modified: Fri, 17 May 2019 22:58:52 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59618f8b2b956f7305c3963ec555282c1346b658cfde0252fc1f0402132a9c0d`  
		Last Modified: Fri, 17 May 2019 23:00:40 GMT  
		Size: 48.3 MB (48338807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915607a345b1aaf32b97c81d3cc15da8da53b5e76d31f87700919a0926a50735`  
		Last Modified: Wed, 16 Sep 2020 21:05:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5aca1ca4b68c6c22c42e16e7d777a3b89508893ddd25845f89ad5dd53941e27`  
		Last Modified: Wed, 16 Sep 2020 21:05:23 GMT  
		Size: 14.8 MB (14799636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rapidoid:5.4`

```console
$ docker pull rapidoid@sha256:5c4ea426e8151756ed9d5796aeefed783f228d3b220acded47ef3f76256a3344
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rapidoid:5.4` - linux; amd64

```console
$ docker pull rapidoid@sha256:a2ff81fe806b3e0236ae2e3db0023e773add322ec9c09272f995a168cf25b9a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (88040840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a7f9a2a2e4abc30d2ca82d0cef914bb0b3a969334b202a86add55990c4a2d1`
-	Entrypoint: `["\/opt\/entrypoint.sh"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:53:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 01 Feb 2021 19:56:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Mon, 01 Feb 2021 19:56:57 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Mon, 01 Feb 2021 19:56:58 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Feb 2021 19:56:58 GMT
ENV LANG=C.UTF-8
# Mon, 01 Feb 2021 19:56:58 GMT
ENV JAVA_VERSION=8u282
# Mon, 01 Feb 2021 19:57:42 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jre_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Mon, 01 Feb 2021 22:15:27 GMT
MAINTAINER Nikolche Mihajlovski
# Mon, 01 Feb 2021 22:15:27 GMT
ENV GPG_KEY=E306FEF548C686C23DC00242B9B08D8F616EF49C
# Mon, 01 Feb 2021 22:15:27 GMT
ENV RAPIDOID_JAR=/opt/rapidoid.jar
# Mon, 01 Feb 2021 22:15:27 GMT
ENV RAPIDOID_TMP=/tmp/rapidoid
# Mon, 01 Feb 2021 22:15:27 GMT
WORKDIR /opt
# Mon, 01 Feb 2021 22:15:28 GMT
EXPOSE 8888
# Mon, 01 Feb 2021 22:15:28 GMT
VOLUME [/data]
# Mon, 01 Feb 2021 22:15:28 GMT
ENV RAPIDOID_VERSION=5.4.6
# Mon, 01 Feb 2021 22:15:28 GMT
ENV RAPIDOID_URL=https://repo1.maven.org/maven2/org/rapidoid/rapidoid-platform/5.4.6/rapidoid-platform-5.4.6.jar
# Mon, 01 Feb 2021 22:15:28 GMT
COPY file:54eb4a0f21aca6721ebea0745a2cbfeb12c799c7a0902f588f490fc0afa8e8ea in /opt/ 
# Mon, 01 Feb 2021 22:15:41 GMT
RUN set -xe     && apt-get update     && apt-get install -y --no-install-recommends         ca-certificates curl dirmngr gnupg     && mkdir /platform     && mkdir -p "$RAPIDOID_TMP" 	&& curl -SL "$RAPIDOID_URL" -o $RAPIDOID_JAR 	&& curl -SL "$RAPIDOID_URL.asc" -o $RAPIDOID_JAR.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys $GPG_KEY 	&& gpg --batch --verify $RAPIDOID_JAR.asc $RAPIDOID_JAR 	&& rm -rf "$GNUPGHOME" 	&& rm "$RAPIDOID_JAR.asc" 	&& rm -rf /var/lib/apt/lists/*
# Mon, 01 Feb 2021 22:15:41 GMT
ENTRYPOINT ["/opt/entrypoint.sh"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943d8acaac04a2b66af03bcc85abe1cd3f50e06d7e193634e04d4e55c4fc7cc8`  
		Last Modified: Tue, 12 Jan 2021 11:07:22 GMT  
		Size: 3.2 MB (3248558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf659c946760b22203efd07517094398c96b09cf88600f4fa5246e91aeafe21`  
		Last Modified: Mon, 01 Feb 2021 20:11:24 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a1f3c619047861843d3b26e2dd68858d324eb1aed3d99c8f6a5077571ebbca`  
		Last Modified: Mon, 01 Feb 2021 20:12:09 GMT  
		Size: 41.6 MB (41590978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60d2788be5dbe8bd39f18f2465ba8a9ddcf28444145e89fab3289dfcfbf8ce2`  
		Last Modified: Mon, 01 Feb 2021 22:15:51 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad54500a7bc8bc1f1a470714f5308f9ad80abb285ede629aec00142178f98da0`  
		Last Modified: Mon, 01 Feb 2021 22:15:52 GMT  
		Size: 16.1 MB (16092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rapidoid:5.4` - linux; arm64 variant v8

```console
$ docker pull rapidoid@sha256:caaf2185ded6e242605bbafe735dce572a0fe6b927702fd58b140c9a5f79ae40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83914069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff166b35f84c89947de28dd53abfe28122ddc85c997c3e9589004282544d835`
-	Entrypoint: `["\/opt\/entrypoint.sh"]`

```dockerfile
# Wed, 08 May 2019 08:49:02 GMT
ADD file:fadb1563a7cd043d96e76895bb1bb3920f9a9262206eb9bcd4ef4b5aec8d9b35 in / 
# Wed, 08 May 2019 08:49:03 GMT
CMD ["bash"]
# Fri, 17 May 2019 22:45:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 17 May 2019 22:49:44 GMT
ENV LANG=C.UTF-8
# Fri, 17 May 2019 22:49:46 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 17 May 2019 22:49:47 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 17 May 2019 22:51:43 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Fri, 17 May 2019 22:51:44 GMT
ENV JAVA_VERSION=8u212
# Fri, 17 May 2019 22:51:44 GMT
ENV JAVA_DEBIAN_VERSION=8u212-b01-1~deb9u1
# Fri, 17 May 2019 22:52:10 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Wed, 16 Sep 2020 21:04:19 GMT
MAINTAINER Nikolche Mihajlovski
# Wed, 16 Sep 2020 21:04:20 GMT
ENV GPG_KEY=E306FEF548C686C23DC00242B9B08D8F616EF49C
# Wed, 16 Sep 2020 21:04:21 GMT
ENV RAPIDOID_JAR=/opt/rapidoid.jar
# Wed, 16 Sep 2020 21:04:22 GMT
ENV RAPIDOID_TMP=/tmp/rapidoid
# Wed, 16 Sep 2020 21:04:24 GMT
WORKDIR /opt
# Wed, 16 Sep 2020 21:04:25 GMT
EXPOSE 8888
# Wed, 16 Sep 2020 21:04:26 GMT
VOLUME [/data]
# Wed, 16 Sep 2020 21:04:27 GMT
ENV RAPIDOID_VERSION=5.4.6
# Wed, 16 Sep 2020 21:04:29 GMT
ENV RAPIDOID_URL=https://repo1.maven.org/maven2/org/rapidoid/rapidoid-platform/5.4.6/rapidoid-platform-5.4.6.jar
# Wed, 16 Sep 2020 21:04:29 GMT
COPY file:54eb4a0f21aca6721ebea0745a2cbfeb12c799c7a0902f588f490fc0afa8e8ea in /opt/ 
# Wed, 16 Sep 2020 21:05:04 GMT
RUN set -xe     && apt-get update     && apt-get install -y --no-install-recommends         ca-certificates curl dirmngr gnupg     && mkdir /platform     && mkdir -p "$RAPIDOID_TMP" 	&& curl -SL "$RAPIDOID_URL" -o $RAPIDOID_JAR 	&& curl -SL "$RAPIDOID_URL.asc" -o $RAPIDOID_JAR.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys $GPG_KEY 	&& gpg --batch --verify $RAPIDOID_JAR.asc $RAPIDOID_JAR 	&& rm -rf "$GNUPGHOME" 	&& rm "$RAPIDOID_JAR.asc" 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 21:05:05 GMT
ENTRYPOINT ["/opt/entrypoint.sh"]
```

-	Layers:
	-	`sha256:29b80961214d7f0c89081fe8134e6e8e14ccfa1afe001357539f59930ff9e3ef`  
		Last Modified: Wed, 08 May 2019 08:55:12 GMT  
		Size: 20.3 MB (20333815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392e0924564e298648b4a7b2ebc774103f98526dd2afd1c948697b4c6686300f`  
		Last Modified: Fri, 17 May 2019 22:55:11 GMT  
		Size: 441.1 KB (441065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15c6e01e710610402034472504e3628bdd00c2b0907f3ec4364f8e71a38d8c0`  
		Last Modified: Fri, 17 May 2019 22:58:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acba4335cd44174a82b7a5d29d7b9dacc9e0b19f066b622c972c573edeb4dddd`  
		Last Modified: Fri, 17 May 2019 22:58:52 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59618f8b2b956f7305c3963ec555282c1346b658cfde0252fc1f0402132a9c0d`  
		Last Modified: Fri, 17 May 2019 23:00:40 GMT  
		Size: 48.3 MB (48338807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915607a345b1aaf32b97c81d3cc15da8da53b5e76d31f87700919a0926a50735`  
		Last Modified: Wed, 16 Sep 2020 21:05:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5aca1ca4b68c6c22c42e16e7d777a3b89508893ddd25845f89ad5dd53941e27`  
		Last Modified: Wed, 16 Sep 2020 21:05:23 GMT  
		Size: 14.8 MB (14799636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rapidoid:5.4.6`

```console
$ docker pull rapidoid@sha256:5c4ea426e8151756ed9d5796aeefed783f228d3b220acded47ef3f76256a3344
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rapidoid:5.4.6` - linux; amd64

```console
$ docker pull rapidoid@sha256:a2ff81fe806b3e0236ae2e3db0023e773add322ec9c09272f995a168cf25b9a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (88040840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a7f9a2a2e4abc30d2ca82d0cef914bb0b3a969334b202a86add55990c4a2d1`
-	Entrypoint: `["\/opt\/entrypoint.sh"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:53:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 01 Feb 2021 19:56:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Mon, 01 Feb 2021 19:56:57 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Mon, 01 Feb 2021 19:56:58 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Feb 2021 19:56:58 GMT
ENV LANG=C.UTF-8
# Mon, 01 Feb 2021 19:56:58 GMT
ENV JAVA_VERSION=8u282
# Mon, 01 Feb 2021 19:57:42 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jre_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Mon, 01 Feb 2021 22:15:27 GMT
MAINTAINER Nikolche Mihajlovski
# Mon, 01 Feb 2021 22:15:27 GMT
ENV GPG_KEY=E306FEF548C686C23DC00242B9B08D8F616EF49C
# Mon, 01 Feb 2021 22:15:27 GMT
ENV RAPIDOID_JAR=/opt/rapidoid.jar
# Mon, 01 Feb 2021 22:15:27 GMT
ENV RAPIDOID_TMP=/tmp/rapidoid
# Mon, 01 Feb 2021 22:15:27 GMT
WORKDIR /opt
# Mon, 01 Feb 2021 22:15:28 GMT
EXPOSE 8888
# Mon, 01 Feb 2021 22:15:28 GMT
VOLUME [/data]
# Mon, 01 Feb 2021 22:15:28 GMT
ENV RAPIDOID_VERSION=5.4.6
# Mon, 01 Feb 2021 22:15:28 GMT
ENV RAPIDOID_URL=https://repo1.maven.org/maven2/org/rapidoid/rapidoid-platform/5.4.6/rapidoid-platform-5.4.6.jar
# Mon, 01 Feb 2021 22:15:28 GMT
COPY file:54eb4a0f21aca6721ebea0745a2cbfeb12c799c7a0902f588f490fc0afa8e8ea in /opt/ 
# Mon, 01 Feb 2021 22:15:41 GMT
RUN set -xe     && apt-get update     && apt-get install -y --no-install-recommends         ca-certificates curl dirmngr gnupg     && mkdir /platform     && mkdir -p "$RAPIDOID_TMP" 	&& curl -SL "$RAPIDOID_URL" -o $RAPIDOID_JAR 	&& curl -SL "$RAPIDOID_URL.asc" -o $RAPIDOID_JAR.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys $GPG_KEY 	&& gpg --batch --verify $RAPIDOID_JAR.asc $RAPIDOID_JAR 	&& rm -rf "$GNUPGHOME" 	&& rm "$RAPIDOID_JAR.asc" 	&& rm -rf /var/lib/apt/lists/*
# Mon, 01 Feb 2021 22:15:41 GMT
ENTRYPOINT ["/opt/entrypoint.sh"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943d8acaac04a2b66af03bcc85abe1cd3f50e06d7e193634e04d4e55c4fc7cc8`  
		Last Modified: Tue, 12 Jan 2021 11:07:22 GMT  
		Size: 3.2 MB (3248558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf659c946760b22203efd07517094398c96b09cf88600f4fa5246e91aeafe21`  
		Last Modified: Mon, 01 Feb 2021 20:11:24 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a1f3c619047861843d3b26e2dd68858d324eb1aed3d99c8f6a5077571ebbca`  
		Last Modified: Mon, 01 Feb 2021 20:12:09 GMT  
		Size: 41.6 MB (41590978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60d2788be5dbe8bd39f18f2465ba8a9ddcf28444145e89fab3289dfcfbf8ce2`  
		Last Modified: Mon, 01 Feb 2021 22:15:51 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad54500a7bc8bc1f1a470714f5308f9ad80abb285ede629aec00142178f98da0`  
		Last Modified: Mon, 01 Feb 2021 22:15:52 GMT  
		Size: 16.1 MB (16092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rapidoid:5.4.6` - linux; arm64 variant v8

```console
$ docker pull rapidoid@sha256:caaf2185ded6e242605bbafe735dce572a0fe6b927702fd58b140c9a5f79ae40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83914069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff166b35f84c89947de28dd53abfe28122ddc85c997c3e9589004282544d835`
-	Entrypoint: `["\/opt\/entrypoint.sh"]`

```dockerfile
# Wed, 08 May 2019 08:49:02 GMT
ADD file:fadb1563a7cd043d96e76895bb1bb3920f9a9262206eb9bcd4ef4b5aec8d9b35 in / 
# Wed, 08 May 2019 08:49:03 GMT
CMD ["bash"]
# Fri, 17 May 2019 22:45:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 17 May 2019 22:49:44 GMT
ENV LANG=C.UTF-8
# Fri, 17 May 2019 22:49:46 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 17 May 2019 22:49:47 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 17 May 2019 22:51:43 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Fri, 17 May 2019 22:51:44 GMT
ENV JAVA_VERSION=8u212
# Fri, 17 May 2019 22:51:44 GMT
ENV JAVA_DEBIAN_VERSION=8u212-b01-1~deb9u1
# Fri, 17 May 2019 22:52:10 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Wed, 16 Sep 2020 21:04:19 GMT
MAINTAINER Nikolche Mihajlovski
# Wed, 16 Sep 2020 21:04:20 GMT
ENV GPG_KEY=E306FEF548C686C23DC00242B9B08D8F616EF49C
# Wed, 16 Sep 2020 21:04:21 GMT
ENV RAPIDOID_JAR=/opt/rapidoid.jar
# Wed, 16 Sep 2020 21:04:22 GMT
ENV RAPIDOID_TMP=/tmp/rapidoid
# Wed, 16 Sep 2020 21:04:24 GMT
WORKDIR /opt
# Wed, 16 Sep 2020 21:04:25 GMT
EXPOSE 8888
# Wed, 16 Sep 2020 21:04:26 GMT
VOLUME [/data]
# Wed, 16 Sep 2020 21:04:27 GMT
ENV RAPIDOID_VERSION=5.4.6
# Wed, 16 Sep 2020 21:04:29 GMT
ENV RAPIDOID_URL=https://repo1.maven.org/maven2/org/rapidoid/rapidoid-platform/5.4.6/rapidoid-platform-5.4.6.jar
# Wed, 16 Sep 2020 21:04:29 GMT
COPY file:54eb4a0f21aca6721ebea0745a2cbfeb12c799c7a0902f588f490fc0afa8e8ea in /opt/ 
# Wed, 16 Sep 2020 21:05:04 GMT
RUN set -xe     && apt-get update     && apt-get install -y --no-install-recommends         ca-certificates curl dirmngr gnupg     && mkdir /platform     && mkdir -p "$RAPIDOID_TMP" 	&& curl -SL "$RAPIDOID_URL" -o $RAPIDOID_JAR 	&& curl -SL "$RAPIDOID_URL.asc" -o $RAPIDOID_JAR.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys $GPG_KEY 	&& gpg --batch --verify $RAPIDOID_JAR.asc $RAPIDOID_JAR 	&& rm -rf "$GNUPGHOME" 	&& rm "$RAPIDOID_JAR.asc" 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 21:05:05 GMT
ENTRYPOINT ["/opt/entrypoint.sh"]
```

-	Layers:
	-	`sha256:29b80961214d7f0c89081fe8134e6e8e14ccfa1afe001357539f59930ff9e3ef`  
		Last Modified: Wed, 08 May 2019 08:55:12 GMT  
		Size: 20.3 MB (20333815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392e0924564e298648b4a7b2ebc774103f98526dd2afd1c948697b4c6686300f`  
		Last Modified: Fri, 17 May 2019 22:55:11 GMT  
		Size: 441.1 KB (441065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15c6e01e710610402034472504e3628bdd00c2b0907f3ec4364f8e71a38d8c0`  
		Last Modified: Fri, 17 May 2019 22:58:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acba4335cd44174a82b7a5d29d7b9dacc9e0b19f066b622c972c573edeb4dddd`  
		Last Modified: Fri, 17 May 2019 22:58:52 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59618f8b2b956f7305c3963ec555282c1346b658cfde0252fc1f0402132a9c0d`  
		Last Modified: Fri, 17 May 2019 23:00:40 GMT  
		Size: 48.3 MB (48338807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915607a345b1aaf32b97c81d3cc15da8da53b5e76d31f87700919a0926a50735`  
		Last Modified: Wed, 16 Sep 2020 21:05:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5aca1ca4b68c6c22c42e16e7d777a3b89508893ddd25845f89ad5dd53941e27`  
		Last Modified: Wed, 16 Sep 2020 21:05:23 GMT  
		Size: 14.8 MB (14799636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rapidoid:latest`

```console
$ docker pull rapidoid@sha256:5c4ea426e8151756ed9d5796aeefed783f228d3b220acded47ef3f76256a3344
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rapidoid:latest` - linux; amd64

```console
$ docker pull rapidoid@sha256:a2ff81fe806b3e0236ae2e3db0023e773add322ec9c09272f995a168cf25b9a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (88040840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a7f9a2a2e4abc30d2ca82d0cef914bb0b3a969334b202a86add55990c4a2d1`
-	Entrypoint: `["\/opt\/entrypoint.sh"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:53:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 01 Feb 2021 19:56:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Mon, 01 Feb 2021 19:56:57 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Mon, 01 Feb 2021 19:56:58 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Feb 2021 19:56:58 GMT
ENV LANG=C.UTF-8
# Mon, 01 Feb 2021 19:56:58 GMT
ENV JAVA_VERSION=8u282
# Mon, 01 Feb 2021 19:57:42 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jre_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Mon, 01 Feb 2021 22:15:27 GMT
MAINTAINER Nikolche Mihajlovski
# Mon, 01 Feb 2021 22:15:27 GMT
ENV GPG_KEY=E306FEF548C686C23DC00242B9B08D8F616EF49C
# Mon, 01 Feb 2021 22:15:27 GMT
ENV RAPIDOID_JAR=/opt/rapidoid.jar
# Mon, 01 Feb 2021 22:15:27 GMT
ENV RAPIDOID_TMP=/tmp/rapidoid
# Mon, 01 Feb 2021 22:15:27 GMT
WORKDIR /opt
# Mon, 01 Feb 2021 22:15:28 GMT
EXPOSE 8888
# Mon, 01 Feb 2021 22:15:28 GMT
VOLUME [/data]
# Mon, 01 Feb 2021 22:15:28 GMT
ENV RAPIDOID_VERSION=5.4.6
# Mon, 01 Feb 2021 22:15:28 GMT
ENV RAPIDOID_URL=https://repo1.maven.org/maven2/org/rapidoid/rapidoid-platform/5.4.6/rapidoid-platform-5.4.6.jar
# Mon, 01 Feb 2021 22:15:28 GMT
COPY file:54eb4a0f21aca6721ebea0745a2cbfeb12c799c7a0902f588f490fc0afa8e8ea in /opt/ 
# Mon, 01 Feb 2021 22:15:41 GMT
RUN set -xe     && apt-get update     && apt-get install -y --no-install-recommends         ca-certificates curl dirmngr gnupg     && mkdir /platform     && mkdir -p "$RAPIDOID_TMP" 	&& curl -SL "$RAPIDOID_URL" -o $RAPIDOID_JAR 	&& curl -SL "$RAPIDOID_URL.asc" -o $RAPIDOID_JAR.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys $GPG_KEY 	&& gpg --batch --verify $RAPIDOID_JAR.asc $RAPIDOID_JAR 	&& rm -rf "$GNUPGHOME" 	&& rm "$RAPIDOID_JAR.asc" 	&& rm -rf /var/lib/apt/lists/*
# Mon, 01 Feb 2021 22:15:41 GMT
ENTRYPOINT ["/opt/entrypoint.sh"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943d8acaac04a2b66af03bcc85abe1cd3f50e06d7e193634e04d4e55c4fc7cc8`  
		Last Modified: Tue, 12 Jan 2021 11:07:22 GMT  
		Size: 3.2 MB (3248558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf659c946760b22203efd07517094398c96b09cf88600f4fa5246e91aeafe21`  
		Last Modified: Mon, 01 Feb 2021 20:11:24 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a1f3c619047861843d3b26e2dd68858d324eb1aed3d99c8f6a5077571ebbca`  
		Last Modified: Mon, 01 Feb 2021 20:12:09 GMT  
		Size: 41.6 MB (41590978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60d2788be5dbe8bd39f18f2465ba8a9ddcf28444145e89fab3289dfcfbf8ce2`  
		Last Modified: Mon, 01 Feb 2021 22:15:51 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad54500a7bc8bc1f1a470714f5308f9ad80abb285ede629aec00142178f98da0`  
		Last Modified: Mon, 01 Feb 2021 22:15:52 GMT  
		Size: 16.1 MB (16092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rapidoid:latest` - linux; arm64 variant v8

```console
$ docker pull rapidoid@sha256:caaf2185ded6e242605bbafe735dce572a0fe6b927702fd58b140c9a5f79ae40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83914069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff166b35f84c89947de28dd53abfe28122ddc85c997c3e9589004282544d835`
-	Entrypoint: `["\/opt\/entrypoint.sh"]`

```dockerfile
# Wed, 08 May 2019 08:49:02 GMT
ADD file:fadb1563a7cd043d96e76895bb1bb3920f9a9262206eb9bcd4ef4b5aec8d9b35 in / 
# Wed, 08 May 2019 08:49:03 GMT
CMD ["bash"]
# Fri, 17 May 2019 22:45:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 17 May 2019 22:49:44 GMT
ENV LANG=C.UTF-8
# Fri, 17 May 2019 22:49:46 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 17 May 2019 22:49:47 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 17 May 2019 22:51:43 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Fri, 17 May 2019 22:51:44 GMT
ENV JAVA_VERSION=8u212
# Fri, 17 May 2019 22:51:44 GMT
ENV JAVA_DEBIAN_VERSION=8u212-b01-1~deb9u1
# Fri, 17 May 2019 22:52:10 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Wed, 16 Sep 2020 21:04:19 GMT
MAINTAINER Nikolche Mihajlovski
# Wed, 16 Sep 2020 21:04:20 GMT
ENV GPG_KEY=E306FEF548C686C23DC00242B9B08D8F616EF49C
# Wed, 16 Sep 2020 21:04:21 GMT
ENV RAPIDOID_JAR=/opt/rapidoid.jar
# Wed, 16 Sep 2020 21:04:22 GMT
ENV RAPIDOID_TMP=/tmp/rapidoid
# Wed, 16 Sep 2020 21:04:24 GMT
WORKDIR /opt
# Wed, 16 Sep 2020 21:04:25 GMT
EXPOSE 8888
# Wed, 16 Sep 2020 21:04:26 GMT
VOLUME [/data]
# Wed, 16 Sep 2020 21:04:27 GMT
ENV RAPIDOID_VERSION=5.4.6
# Wed, 16 Sep 2020 21:04:29 GMT
ENV RAPIDOID_URL=https://repo1.maven.org/maven2/org/rapidoid/rapidoid-platform/5.4.6/rapidoid-platform-5.4.6.jar
# Wed, 16 Sep 2020 21:04:29 GMT
COPY file:54eb4a0f21aca6721ebea0745a2cbfeb12c799c7a0902f588f490fc0afa8e8ea in /opt/ 
# Wed, 16 Sep 2020 21:05:04 GMT
RUN set -xe     && apt-get update     && apt-get install -y --no-install-recommends         ca-certificates curl dirmngr gnupg     && mkdir /platform     && mkdir -p "$RAPIDOID_TMP" 	&& curl -SL "$RAPIDOID_URL" -o $RAPIDOID_JAR 	&& curl -SL "$RAPIDOID_URL.asc" -o $RAPIDOID_JAR.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys $GPG_KEY 	&& gpg --batch --verify $RAPIDOID_JAR.asc $RAPIDOID_JAR 	&& rm -rf "$GNUPGHOME" 	&& rm "$RAPIDOID_JAR.asc" 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 21:05:05 GMT
ENTRYPOINT ["/opt/entrypoint.sh"]
```

-	Layers:
	-	`sha256:29b80961214d7f0c89081fe8134e6e8e14ccfa1afe001357539f59930ff9e3ef`  
		Last Modified: Wed, 08 May 2019 08:55:12 GMT  
		Size: 20.3 MB (20333815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392e0924564e298648b4a7b2ebc774103f98526dd2afd1c948697b4c6686300f`  
		Last Modified: Fri, 17 May 2019 22:55:11 GMT  
		Size: 441.1 KB (441065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15c6e01e710610402034472504e3628bdd00c2b0907f3ec4364f8e71a38d8c0`  
		Last Modified: Fri, 17 May 2019 22:58:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acba4335cd44174a82b7a5d29d7b9dacc9e0b19f066b622c972c573edeb4dddd`  
		Last Modified: Fri, 17 May 2019 22:58:52 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59618f8b2b956f7305c3963ec555282c1346b658cfde0252fc1f0402132a9c0d`  
		Last Modified: Fri, 17 May 2019 23:00:40 GMT  
		Size: 48.3 MB (48338807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915607a345b1aaf32b97c81d3cc15da8da53b5e76d31f87700919a0926a50735`  
		Last Modified: Wed, 16 Sep 2020 21:05:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5aca1ca4b68c6c22c42e16e7d777a3b89508893ddd25845f89ad5dd53941e27`  
		Last Modified: Wed, 16 Sep 2020 21:05:23 GMT  
		Size: 14.8 MB (14799636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
