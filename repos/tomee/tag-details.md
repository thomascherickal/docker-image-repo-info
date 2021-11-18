<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `tomee`

-	[`tomee:11-jre-8.0.8-microprofile`](#tomee11-jre-808-microprofile)
-	[`tomee:11-jre-8.0.8-plume`](#tomee11-jre-808-plume)
-	[`tomee:11-jre-8.0.8-plus`](#tomee11-jre-808-plus)
-	[`tomee:11-jre-8.0.8-webprofile`](#tomee11-jre-808-webprofile)
-	[`tomee:11-jre-9.0.0-M7-microprofile`](#tomee11-jre-900-m7-microprofile)
-	[`tomee:11-jre-9.0.0-M7-plume`](#tomee11-jre-900-m7-plume)
-	[`tomee:11-jre-9.0.0-M7-plus`](#tomee11-jre-900-m7-plus)
-	[`tomee:11-jre-9.0.0-M7-webprofile`](#tomee11-jre-900-m7-webprofile)
-	[`tomee:7`](#tomee7)
-	[`tomee:7.0`](#tomee70)
-	[`tomee:7.0.9-plume`](#tomee709-plume)
-	[`tomee:7.0.9-plus`](#tomee709-plus)
-	[`tomee:7.1`](#tomee71)
-	[`tomee:7.1.4-microprofile`](#tomee714-microprofile)
-	[`tomee:7.1.4-plume`](#tomee714-plume)
-	[`tomee:7.1.4-plus`](#tomee714-plus)
-	[`tomee:7.1.4-webprofile`](#tomee714-webprofile)
-	[`tomee:8`](#tomee8)
-	[`tomee:8-jre-7.0.9-plume`](#tomee8-jre-709-plume)
-	[`tomee:8-jre-7.0.9-plus`](#tomee8-jre-709-plus)
-	[`tomee:8-jre-7.0.9-webprofile`](#tomee8-jre-709-webprofile)
-	[`tomee:8-jre-7.1.4-microprofile`](#tomee8-jre-714-microprofile)
-	[`tomee:8-jre-7.1.4-plume`](#tomee8-jre-714-plume)
-	[`tomee:8-jre-7.1.4-plus`](#tomee8-jre-714-plus)
-	[`tomee:8-jre-7.1.4-webprofile`](#tomee8-jre-714-webprofile)
-	[`tomee:8-jre-8.0.8-microprofile`](#tomee8-jre-808-microprofile)
-	[`tomee:8-jre-8.0.8-plume`](#tomee8-jre-808-plume)
-	[`tomee:8-jre-8.0.8-plus`](#tomee8-jre-808-plus)
-	[`tomee:8-jre-8.0.8-webprofile`](#tomee8-jre-808-webprofile)
-	[`tomee:8.0.8-microprofile`](#tomee808-microprofile)
-	[`tomee:8.0.8-plume`](#tomee808-plume)
-	[`tomee:8.0.8-plus`](#tomee808-plus)
-	[`tomee:8.0.8-webprofile`](#tomee808-webprofile)
-	[`tomee:9`](#tomee9)
-	[`tomee:9.0.0-M7-microprofile`](#tomee900-m7-microprofile)
-	[`tomee:9.0.0-M7-plume`](#tomee900-m7-plume)
-	[`tomee:9.0.0-M7-webprofile`](#tomee900-m7-webprofile)
-	[`tomee:9.0.0.M7-plus`](#tomee900m7-plus)
-	[`tomee:latest`](#tomeelatest)

## `tomee:11-jre-8.0.8-microprofile`

```console
$ docker pull tomee@sha256:7620cf323a60aeb99c35f97275dc95b10f0890126e5143a0e8b3fca247b12836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:11-jre-8.0.8-microprofile` - linux; amd64

```console
$ docker pull tomee@sha256:5061f541b7c9a5a880b9ae89804824b8e0ec412a8ad557d2c7555f1d56d0ea75
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.5 MB (187491585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8326521d91963a025bedf2faf47869e026f9f239338f35ba2f5464687b1f0323`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:48:28 GMT
ENV TOMEE_BUILD=microprofile
# Thu, 18 Nov 2021 12:48:35 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:36 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:36 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d111e5337bcdd4242e837b77e614da38d01b80bbbd5c70902fe1b8edff13e`  
		Last Modified: Thu, 18 Nov 2021 12:53:15 GMT  
		Size: 64.0 MB (63989426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:11-jre-8.0.8-plume`

```console
$ docker pull tomee@sha256:76cd9dc5e76694551d0ac1ac3fa7a8325123799c8e880143559b8fa9993f20c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:11-jre-8.0.8-plume` - linux; amd64

```console
$ docker pull tomee@sha256:c7f7c11f021647666f6d745968ccbc6cab626af801c238efe1353954d9e472bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.6 MB (199559111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a47415770eda92a65ed21762fc87840e6d37da25ca7277571600b710f5a5fd1`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_BUILD=plume
# Thu, 18 Nov 2021 12:48:11 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:11 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:11 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41ec1166e12b284b4b8ff79b6591f656f1c322b903b683c7874ac01f7338749`  
		Last Modified: Thu, 18 Nov 2021 12:52:47 GMT  
		Size: 76.1 MB (76056952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:11-jre-8.0.8-plus`

```console
$ docker pull tomee@sha256:0d21369b819a6ba2fde09a356b6e335f8f33bcd8746aa42a214f33109848b506
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:11-jre-8.0.8-plus` - linux; amd64

```console
$ docker pull tomee@sha256:4fb63240722a9c3b130fb2077bd794f57beeb50eadcd4b9f1ffc7d2f40d65a9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192394431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c4b3e816aabd9aeb7dd71dad13e56dece1e97130877a8dc10ffd78a3e28062`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:48:16 GMT
ENV TOMEE_BUILD=plus
# Thu, 18 Nov 2021 12:48:24 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:24 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:25 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30555b62f61dcc77487e50d27753f9fc52fb42742b5f0a68dca863f35dfb7c5a`  
		Last Modified: Thu, 18 Nov 2021 12:53:00 GMT  
		Size: 68.9 MB (68892272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:11-jre-8.0.8-webprofile`

```console
$ docker pull tomee@sha256:c4bff3f9c3220931f2e938e978e13db6f40d9056bf2e13b0950ae463886998fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:11-jre-8.0.8-webprofile` - linux; amd64

```console
$ docker pull tomee@sha256:17808945d115b73325da6bc968ac1a5cb522c17e18ffb393a11a80042c73e32d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172542472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:850fc5e5f10b12db5c551239d3ee386f18a86d7975811d69219b0e97589bbf1a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:48:39 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:48:45 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:45 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:46 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc43f1cf7fcdf28f8e12213dd41d68ffed3cca0fbb9b69d6de4a52063339078`  
		Last Modified: Thu, 18 Nov 2021 12:53:28 GMT  
		Size: 49.0 MB (49040313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:11-jre-9.0.0-M7-microprofile`

```console
$ docker pull tomee@sha256:7695a8067df502b4a12657710e4987e8cf7fe4045dab929801be9d11f40105ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:11-jre-9.0.0-M7-microprofile` - linux; amd64

```console
$ docker pull tomee@sha256:17b35e188439dcac0d1716793cd9f263a11d12f63a36dd13ddecd81ea45391ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.1 MB (189109845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a596e807fb75a5ff8c6b54547fd00b5be9bd68c049ac85ce6bf1d51aaab58cc1`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:48 GMT
ENV TOMEE_VER=9.0.0-M7
# Thu, 18 Nov 2021 12:49:11 GMT
ENV TOMEE_BUILD=microprofile
# Thu, 18 Nov 2021 12:49:18 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz   && gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz   && echo `cat tomee.tar.gz.sha512` tomee.tar.gz | sha512sum -c -   && tar -zxf tomee.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:49:19 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:49:19 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cf0877d6b664e3ab92cec263d78d35531e287f6f276435b401f90cb84523f2`  
		Last Modified: Thu, 18 Nov 2021 12:54:18 GMT  
		Size: 65.6 MB (65607686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:11-jre-9.0.0-M7-plume`

```console
$ docker pull tomee@sha256:6728f3c68f51e05fd4296433c6718395afed1e9d576a3a9e310f6eda7f282006
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:11-jre-9.0.0-M7-plume` - linux; amd64

```console
$ docker pull tomee@sha256:854e1109d2ebecc4104a4e8464133aa9e8c27ba041e1ab5e130c906a28a848e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.0 MB (201983984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f69f183d7a7ed8f97cf960e6bc51adc0d89c8852c412216a24f56f50808044d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:48 GMT
ENV TOMEE_VER=9.0.0-M7
# Thu, 18 Nov 2021 12:48:49 GMT
ENV TOMEE_BUILD=plume
# Thu, 18 Nov 2021 12:48:57 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz   && gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz   && echo `cat tomee.tar.gz.sha512` tomee.tar.gz | sha512sum -c -   && tar -zxf tomee.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:57 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:57 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd7e640aff335bd7142c477609b6779437e5ee367f35dfffbdfbca7b2d343bf`  
		Last Modified: Thu, 18 Nov 2021 12:53:49 GMT  
		Size: 78.5 MB (78481825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:11-jre-9.0.0-M7-plus`

```console
$ docker pull tomee@sha256:a40e85aabbfd48ca81f9cce980b0a8c967814f5c5bf78e1db70bdafb5a2423e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:11-jre-9.0.0-M7-plus` - linux; amd64

```console
$ docker pull tomee@sha256:d17a036c87fa9206edf59fd9fdd48d12d889567d2a1ae0465c35c920704eefa9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.0 MB (194028045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6dd28edf631503b3ee3a24aea27e1d1b473b88905446f4ca3d59ee5a2797f5d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:48 GMT
ENV TOMEE_VER=9.0.0-M7
# Thu, 18 Nov 2021 12:49:00 GMT
ENV TOMEE_BUILD=plus
# Thu, 18 Nov 2021 12:49:07 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz   && gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz   && echo `cat tomee.tar.gz.sha512` tomee.tar.gz | sha512sum -c -   && tar -zxf tomee.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:49:08 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:49:08 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1aeb075311191d82bb778bfb9d7e63d07cb9a992156ed7b451bb65edc683297`  
		Last Modified: Thu, 18 Nov 2021 12:54:04 GMT  
		Size: 70.5 MB (70525886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:11-jre-9.0.0-M7-webprofile`

```console
$ docker pull tomee@sha256:c0107232664dbc0ca025700e2a1de95e5154b755bd3a64bd30b3f56d045b21f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:11-jre-9.0.0-M7-webprofile` - linux; amd64

```console
$ docker pull tomee@sha256:d2bd3e407f48b73bc5f706de37f979595d754590274b78a22c9926c95f456731
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.1 MB (178070362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50131dcbfe666024412e11fb019e236a722a7fd45818871b83cc3c17c9027a06`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:48 GMT
ENV TOMEE_VER=9.0.0-M7
# Thu, 18 Nov 2021 12:49:22 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:49:29 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz   && gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz   && echo `cat tomee.tar.gz.sha512` tomee.tar.gz | sha512sum -c -   && tar -zxf tomee.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:49:29 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:49:29 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf246360353f18a72eb43a35c6a9f0b9ab9cb0c475ed0716cb625a1965927d82`  
		Last Modified: Thu, 18 Nov 2021 12:54:31 GMT  
		Size: 54.6 MB (54568203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:7`

```console
$ docker pull tomee@sha256:278386438b95c1e82c82276734bbeb998f5d381cae8b205a71df89db713e41c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:7` - linux; amd64

```console
$ docker pull tomee@sha256:4947e19ba78faefd666eca9e887785c3c2dcd3f2fef61d0ccf60cca6e6909844
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.5 MB (158526113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:298425ce03fb242f8104069f46949f7bac5ecb5685a05465b0fe2e9a63d7ab48`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_VER=7.1.4
# Thu, 18 Nov 2021 12:46:46 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:46:51 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6222be43da54b6e196f7cc21a835d0390b668cd845fb467b75473b04bbf8ca5c`  
		Last Modified: Thu, 18 Nov 2021 12:51:36 GMT  
		Size: 40.5 MB (40520463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:7.0`

```console
$ docker pull tomee@sha256:cb0f9f840672d8a8bbddb97c06140cf147d30b95ace9bbe0e96a179bf8ba8a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:7.0` - linux; amd64

```console
$ docker pull tomee@sha256:a89025d7de3dbd386d2894c9d608cedbaa163bb62d3eade59936d78bb854787e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156412118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9a51fb7a19879eae73430bc6207825d1ed68ac0035b25ef35c4fcc84084abf`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:45:51 GMT
ENV TOMEE_VER=7.0.9
# Thu, 18 Nov 2021 12:46:11 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:46:16 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:16 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:16 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2212e6bed3902747964550c95649f5ad251689b07e1c8074c69145341dce1c02`  
		Last Modified: Thu, 18 Nov 2021 12:50:43 GMT  
		Size: 38.4 MB (38406468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:7.0.9-plume`

```console
$ docker pull tomee@sha256:15c581efb2e6568a99f7b931658649077777a1377fa8dbc8f9a539bd41248016
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:7.0.9-plume` - linux; amd64

```console
$ docker pull tomee@sha256:c1f870100e3a4744de519fd33eeb946d5f9c81fe63d6276c0619231fc31a541c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.1 MB (181138115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42927f45b6bd37edb7a77a11c9c381ea916dcb2e03b0664d324f92d43bb67ff3`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:45:51 GMT
ENV TOMEE_VER=7.0.9
# Thu, 18 Nov 2021 12:45:51 GMT
ENV TOMEE_BUILD=plume
# Thu, 18 Nov 2021 12:45:58 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:45:58 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:45:58 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844663c5ea33ee7679c0fcb600caae1df946d4a1944ea05a6d10ad55f978f377`  
		Last Modified: Thu, 18 Nov 2021 12:50:17 GMT  
		Size: 63.1 MB (63132465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:7.0.9-plus`

```console
$ docker pull tomee@sha256:7dab204e7a7ae19b1c0e5cb520ce7327880e1b6e0325f01989c63873eecff24d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:7.0.9-plus` - linux; amd64

```console
$ docker pull tomee@sha256:e7c52b07ea691ae0fa7edc5205dbd97366420bcdbda6d8dadf57030e41deeaf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174066160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0248779b9ae1317fa7492c8f4b0e545b43ed30078dbaec90e36638bd284be092`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:45:51 GMT
ENV TOMEE_VER=7.0.9
# Thu, 18 Nov 2021 12:46:01 GMT
ENV TOMEE_BUILD=plus
# Thu, 18 Nov 2021 12:46:08 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:08 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:08 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae92206c746e99627ddcd45d7adde043c5cf228d80c832a6d2e782952ee9713`  
		Last Modified: Thu, 18 Nov 2021 12:50:30 GMT  
		Size: 56.1 MB (56060510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:7.1`

```console
$ docker pull tomee@sha256:278386438b95c1e82c82276734bbeb998f5d381cae8b205a71df89db713e41c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:7.1` - linux; amd64

```console
$ docker pull tomee@sha256:4947e19ba78faefd666eca9e887785c3c2dcd3f2fef61d0ccf60cca6e6909844
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.5 MB (158526113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:298425ce03fb242f8104069f46949f7bac5ecb5685a05465b0fe2e9a63d7ab48`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_VER=7.1.4
# Thu, 18 Nov 2021 12:46:46 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:46:51 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6222be43da54b6e196f7cc21a835d0390b668cd845fb467b75473b04bbf8ca5c`  
		Last Modified: Thu, 18 Nov 2021 12:51:36 GMT  
		Size: 40.5 MB (40520463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:7.1.4-microprofile`

```console
$ docker pull tomee@sha256:60a2295bf419ab038cba333f123f572781de6bc8c001c0ef0259dca4945fbd8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:7.1.4-microprofile` - linux; amd64

```console
$ docker pull tomee@sha256:24362c8edfd43a74457f9cd865750fa36b85b64bd8d7005a56a4b61440256e6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159038157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d5e47285eab33b0f1483b7deeef7de0a45f4324681a762e7ef8f26bebd53dc`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_VER=7.1.4
# Thu, 18 Nov 2021 12:46:38 GMT
ENV TOMEE_BUILD=microprofile
# Thu, 18 Nov 2021 12:46:43 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:43 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:43 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296514d4792bec1a071a6455adda577909c39faefbe4bf0d8edeeeccd6b6998c`  
		Last Modified: Thu, 18 Nov 2021 12:51:24 GMT  
		Size: 41.0 MB (41032507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:7.1.4-plume`

```console
$ docker pull tomee@sha256:3a2ab638443b1072ca992d228941e96442fabe5e877f2ba52341b187fc941404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:7.1.4-plume` - linux; amd64

```console
$ docker pull tomee@sha256:daa4f0899e007c64aa8cec0294ac4a543af8437d6c234debf253493f869e9eda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.2 MB (183182552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a18fce5b010b8475cb6f458f8aed717e0a86decc5dcc3be59bc9f9e1820f00d9`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_VER=7.1.4
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_BUILD=plume
# Thu, 18 Nov 2021 12:46:26 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:26 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:26 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf69920368328179572e4c3d353fcebeefd7fff3fbc643c43cf4e895a4f356b6`  
		Last Modified: Thu, 18 Nov 2021 12:50:57 GMT  
		Size: 65.2 MB (65176902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:7.1.4-plus`

```console
$ docker pull tomee@sha256:de334a36bafd0c7dccff2645bccb683bf9c6a5c00879a4a0708d84998effb6fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:7.1.4-plus` - linux; amd64

```console
$ docker pull tomee@sha256:a055b60a9a01f60870a54ee24d53c465ad7ba9d4ced9dbaf0f0fcc2896e59eed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176147777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b1985e69a1246c8e40bcb0e4c93703349d56e76e13168fa102e867943df8fb4`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_VER=7.1.4
# Thu, 18 Nov 2021 12:46:28 GMT
ENV TOMEE_BUILD=plus
# Thu, 18 Nov 2021 12:46:35 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:35 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:35 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a9cf3f74bf5a411a5854fe0ef899744a52c98335f80a0fdbdf6a9e6a912570`  
		Last Modified: Thu, 18 Nov 2021 12:51:11 GMT  
		Size: 58.1 MB (58142127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:7.1.4-webprofile`

```console
$ docker pull tomee@sha256:278386438b95c1e82c82276734bbeb998f5d381cae8b205a71df89db713e41c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:7.1.4-webprofile` - linux; amd64

```console
$ docker pull tomee@sha256:4947e19ba78faefd666eca9e887785c3c2dcd3f2fef61d0ccf60cca6e6909844
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.5 MB (158526113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:298425ce03fb242f8104069f46949f7bac5ecb5685a05465b0fe2e9a63d7ab48`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_VER=7.1.4
# Thu, 18 Nov 2021 12:46:46 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:46:51 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6222be43da54b6e196f7cc21a835d0390b668cd845fb467b75473b04bbf8ca5c`  
		Last Modified: Thu, 18 Nov 2021 12:51:36 GMT  
		Size: 40.5 MB (40520463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8`

```console
$ docker pull tomee@sha256:c4bff3f9c3220931f2e938e978e13db6f40d9056bf2e13b0950ae463886998fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8` - linux; amd64

```console
$ docker pull tomee@sha256:17808945d115b73325da6bc968ac1a5cb522c17e18ffb393a11a80042c73e32d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172542472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:850fc5e5f10b12db5c551239d3ee386f18a86d7975811d69219b0e97589bbf1a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:48:39 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:48:45 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:45 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:46 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc43f1cf7fcdf28f8e12213dd41d68ffed3cca0fbb9b69d6de4a52063339078`  
		Last Modified: Thu, 18 Nov 2021 12:53:28 GMT  
		Size: 49.0 MB (49040313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8-jre-7.0.9-plume`

```console
$ docker pull tomee@sha256:15c581efb2e6568a99f7b931658649077777a1377fa8dbc8f9a539bd41248016
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre-7.0.9-plume` - linux; amd64

```console
$ docker pull tomee@sha256:c1f870100e3a4744de519fd33eeb946d5f9c81fe63d6276c0619231fc31a541c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.1 MB (181138115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42927f45b6bd37edb7a77a11c9c381ea916dcb2e03b0664d324f92d43bb67ff3`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:45:51 GMT
ENV TOMEE_VER=7.0.9
# Thu, 18 Nov 2021 12:45:51 GMT
ENV TOMEE_BUILD=plume
# Thu, 18 Nov 2021 12:45:58 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:45:58 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:45:58 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844663c5ea33ee7679c0fcb600caae1df946d4a1944ea05a6d10ad55f978f377`  
		Last Modified: Thu, 18 Nov 2021 12:50:17 GMT  
		Size: 63.1 MB (63132465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8-jre-7.0.9-plus`

```console
$ docker pull tomee@sha256:7dab204e7a7ae19b1c0e5cb520ce7327880e1b6e0325f01989c63873eecff24d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre-7.0.9-plus` - linux; amd64

```console
$ docker pull tomee@sha256:e7c52b07ea691ae0fa7edc5205dbd97366420bcdbda6d8dadf57030e41deeaf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174066160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0248779b9ae1317fa7492c8f4b0e545b43ed30078dbaec90e36638bd284be092`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:45:51 GMT
ENV TOMEE_VER=7.0.9
# Thu, 18 Nov 2021 12:46:01 GMT
ENV TOMEE_BUILD=plus
# Thu, 18 Nov 2021 12:46:08 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:08 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:08 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae92206c746e99627ddcd45d7adde043c5cf228d80c832a6d2e782952ee9713`  
		Last Modified: Thu, 18 Nov 2021 12:50:30 GMT  
		Size: 56.1 MB (56060510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8-jre-7.0.9-webprofile`

```console
$ docker pull tomee@sha256:cb0f9f840672d8a8bbddb97c06140cf147d30b95ace9bbe0e96a179bf8ba8a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre-7.0.9-webprofile` - linux; amd64

```console
$ docker pull tomee@sha256:a89025d7de3dbd386d2894c9d608cedbaa163bb62d3eade59936d78bb854787e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156412118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9a51fb7a19879eae73430bc6207825d1ed68ac0035b25ef35c4fcc84084abf`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:45:51 GMT
ENV TOMEE_VER=7.0.9
# Thu, 18 Nov 2021 12:46:11 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:46:16 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:16 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:16 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2212e6bed3902747964550c95649f5ad251689b07e1c8074c69145341dce1c02`  
		Last Modified: Thu, 18 Nov 2021 12:50:43 GMT  
		Size: 38.4 MB (38406468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8-jre-7.1.4-microprofile`

```console
$ docker pull tomee@sha256:60a2295bf419ab038cba333f123f572781de6bc8c001c0ef0259dca4945fbd8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre-7.1.4-microprofile` - linux; amd64

```console
$ docker pull tomee@sha256:24362c8edfd43a74457f9cd865750fa36b85b64bd8d7005a56a4b61440256e6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159038157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d5e47285eab33b0f1483b7deeef7de0a45f4324681a762e7ef8f26bebd53dc`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_VER=7.1.4
# Thu, 18 Nov 2021 12:46:38 GMT
ENV TOMEE_BUILD=microprofile
# Thu, 18 Nov 2021 12:46:43 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:43 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:43 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296514d4792bec1a071a6455adda577909c39faefbe4bf0d8edeeeccd6b6998c`  
		Last Modified: Thu, 18 Nov 2021 12:51:24 GMT  
		Size: 41.0 MB (41032507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8-jre-7.1.4-plume`

```console
$ docker pull tomee@sha256:3a2ab638443b1072ca992d228941e96442fabe5e877f2ba52341b187fc941404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre-7.1.4-plume` - linux; amd64

```console
$ docker pull tomee@sha256:daa4f0899e007c64aa8cec0294ac4a543af8437d6c234debf253493f869e9eda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.2 MB (183182552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a18fce5b010b8475cb6f458f8aed717e0a86decc5dcc3be59bc9f9e1820f00d9`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_VER=7.1.4
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_BUILD=plume
# Thu, 18 Nov 2021 12:46:26 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:26 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:26 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf69920368328179572e4c3d353fcebeefd7fff3fbc643c43cf4e895a4f356b6`  
		Last Modified: Thu, 18 Nov 2021 12:50:57 GMT  
		Size: 65.2 MB (65176902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8-jre-7.1.4-plus`

```console
$ docker pull tomee@sha256:de334a36bafd0c7dccff2645bccb683bf9c6a5c00879a4a0708d84998effb6fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre-7.1.4-plus` - linux; amd64

```console
$ docker pull tomee@sha256:a055b60a9a01f60870a54ee24d53c465ad7ba9d4ced9dbaf0f0fcc2896e59eed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176147777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b1985e69a1246c8e40bcb0e4c93703349d56e76e13168fa102e867943df8fb4`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_VER=7.1.4
# Thu, 18 Nov 2021 12:46:28 GMT
ENV TOMEE_BUILD=plus
# Thu, 18 Nov 2021 12:46:35 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:35 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:35 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a9cf3f74bf5a411a5854fe0ef899744a52c98335f80a0fdbdf6a9e6a912570`  
		Last Modified: Thu, 18 Nov 2021 12:51:11 GMT  
		Size: 58.1 MB (58142127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8-jre-7.1.4-webprofile`

```console
$ docker pull tomee@sha256:278386438b95c1e82c82276734bbeb998f5d381cae8b205a71df89db713e41c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre-7.1.4-webprofile` - linux; amd64

```console
$ docker pull tomee@sha256:4947e19ba78faefd666eca9e887785c3c2dcd3f2fef61d0ccf60cca6e6909844
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.5 MB (158526113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:298425ce03fb242f8104069f46949f7bac5ecb5685a05465b0fe2e9a63d7ab48`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Thu, 18 Nov 2021 12:45:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 12:46:19 GMT
ENV TOMEE_VER=7.1.4
# Thu, 18 Nov 2021 12:46:46 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:46:51 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:46:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:46:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97645d1edb2376b7870a79eddd6598d0b6ad3e17ca98302c8495351343db07b0`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 21.4 KB (21355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6222be43da54b6e196f7cc21a835d0390b668cd845fb467b75473b04bbf8ca5c`  
		Last Modified: Thu, 18 Nov 2021 12:51:36 GMT  
		Size: 40.5 MB (40520463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8-jre-8.0.8-microprofile`

```console
$ docker pull tomee@sha256:f30ae1b5b36edfbf2bfa98e36c7716436b576d7ac4acbf6fef2c1b90373ddf66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre-8.0.8-microprofile` - linux; amd64

```console
$ docker pull tomee@sha256:35508437b0241eb6f56685a545b40e43979f9cfef067ea4bb6a61e6da71400e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.0 MB (182032016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75d08ad486aa0be1a98877462dc7d68679738fbd2efee583bc91072d09afc591`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:47:07 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:47:07 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:47:33 GMT
ENV TOMEE_BUILD=microprofile
# Thu, 18 Nov 2021 12:47:40 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:47:40 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:47:40 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba61d8fb30865abf93ebabc4e3b1e05dbcd09a9197ff99c9bc150b7c8412c39`  
		Last Modified: Thu, 18 Nov 2021 12:51:52 GMT  
		Size: 58.3 KB (58308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe3412dc58c229b833f0806c7acdefaba6f97dd2f0b673914eca795b364ac26`  
		Last Modified: Thu, 18 Nov 2021 12:52:24 GMT  
		Size: 64.0 MB (63989413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8-jre-8.0.8-plume`

```console
$ docker pull tomee@sha256:b9364f579391945978b0bb822a64441eef1a2ff84f2620ef308f843da02c665d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre-8.0.8-plume` - linux; amd64

```console
$ docker pull tomee@sha256:03018e4dba22f08f899b89f673ff4ff35fd80ada86af2488369d38b2b286cb61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.1 MB (194099515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaa3eac6985aadf0095a86b354a094eb59537a40860a92589f512938a85bb505`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:47:07 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:47:07 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:47:07 GMT
ENV TOMEE_BUILD=plume
# Thu, 18 Nov 2021 12:47:16 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:47:16 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:47:16 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba61d8fb30865abf93ebabc4e3b1e05dbcd09a9197ff99c9bc150b7c8412c39`  
		Last Modified: Thu, 18 Nov 2021 12:51:52 GMT  
		Size: 58.3 KB (58308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31488f55c3472788ddb467a4f338d4fa775d0fe84913de9643b505df2f98ca1`  
		Last Modified: Thu, 18 Nov 2021 12:51:56 GMT  
		Size: 76.1 MB (76056912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8-jre-8.0.8-plus`

```console
$ docker pull tomee@sha256:9024bb91729d655900df0b5430abdf1c2620235f74124bd33563aab69b821053
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre-8.0.8-plus` - linux; amd64

```console
$ docker pull tomee@sha256:bb8431c4af787002299211992957332f768c76beea71bea34043a62dc5302712
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.9 MB (186934920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fee859619620814e1cfc4fa9de24cd203ed034bffee34ca508239385ed96a3`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:47:07 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:47:07 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:47:21 GMT
ENV TOMEE_BUILD=plus
# Thu, 18 Nov 2021 12:47:29 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:47:30 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:47:30 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba61d8fb30865abf93ebabc4e3b1e05dbcd09a9197ff99c9bc150b7c8412c39`  
		Last Modified: Thu, 18 Nov 2021 12:51:52 GMT  
		Size: 58.3 KB (58308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae0d6d25155bde96b6ed68c1737d8911473c0acc881bee0930307cb806af542`  
		Last Modified: Thu, 18 Nov 2021 12:52:13 GMT  
		Size: 68.9 MB (68892317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8-jre-8.0.8-webprofile`

```console
$ docker pull tomee@sha256:cb489156ae4d1af2a97a0de186f03f0de6660cfb47c3f3803eff69509bcf0304
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8-jre-8.0.8-webprofile` - linux; amd64

```console
$ docker pull tomee@sha256:7fa883a4c48cf1f96fc8471e4f00cd35d34032e74ee282491c36e4b374a6801f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.1 MB (167082882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d261159f9d07defea4b7b8ef4df7198e20c87d3695bf7b274057eb9bbcd936bc`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:33:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:33:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:33:51 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:52 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 18 Nov 2021 12:45:04 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:45:05 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:45:05 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:47:07 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:47:07 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:47:44 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:47:50 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:47:50 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:47:50 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74563c2834ab88825dd581eff10b59c7a4244cce846f7046e15ad1461096`  
		Last Modified: Wed, 17 Nov 2021 09:52:30 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0455cc186e375da847448e3eb53b75c455f08940ee0b6a09178c6856ca9d03c`  
		Last Modified: Wed, 17 Nov 2021 09:52:36 GMT  
		Size: 41.4 MB (41372073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6201403ee77f29ba3f87c5007d945b45e9b194f0cb955dd234e73df026aa025d`  
		Last Modified: Thu, 18 Nov 2021 12:50:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba61d8fb30865abf93ebabc4e3b1e05dbcd09a9197ff99c9bc150b7c8412c39`  
		Last Modified: Thu, 18 Nov 2021 12:51:52 GMT  
		Size: 58.3 KB (58308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b603669a2ca7aa6b78d715d495c07a627146154198749195fb0d94503d7ecc`  
		Last Modified: Thu, 18 Nov 2021 12:52:34 GMT  
		Size: 49.0 MB (49040279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8.0.8-microprofile`

```console
$ docker pull tomee@sha256:7620cf323a60aeb99c35f97275dc95b10f0890126e5143a0e8b3fca247b12836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8.0.8-microprofile` - linux; amd64

```console
$ docker pull tomee@sha256:5061f541b7c9a5a880b9ae89804824b8e0ec412a8ad557d2c7555f1d56d0ea75
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.5 MB (187491585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8326521d91963a025bedf2faf47869e026f9f239338f35ba2f5464687b1f0323`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:48:28 GMT
ENV TOMEE_BUILD=microprofile
# Thu, 18 Nov 2021 12:48:35 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:36 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:36 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d111e5337bcdd4242e837b77e614da38d01b80bbbd5c70902fe1b8edff13e`  
		Last Modified: Thu, 18 Nov 2021 12:53:15 GMT  
		Size: 64.0 MB (63989426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8.0.8-plume`

```console
$ docker pull tomee@sha256:76cd9dc5e76694551d0ac1ac3fa7a8325123799c8e880143559b8fa9993f20c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8.0.8-plume` - linux; amd64

```console
$ docker pull tomee@sha256:c7f7c11f021647666f6d745968ccbc6cab626af801c238efe1353954d9e472bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.6 MB (199559111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a47415770eda92a65ed21762fc87840e6d37da25ca7277571600b710f5a5fd1`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_BUILD=plume
# Thu, 18 Nov 2021 12:48:11 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:11 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:11 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41ec1166e12b284b4b8ff79b6591f656f1c322b903b683c7874ac01f7338749`  
		Last Modified: Thu, 18 Nov 2021 12:52:47 GMT  
		Size: 76.1 MB (76056952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8.0.8-plus`

```console
$ docker pull tomee@sha256:0d21369b819a6ba2fde09a356b6e335f8f33bcd8746aa42a214f33109848b506
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8.0.8-plus` - linux; amd64

```console
$ docker pull tomee@sha256:4fb63240722a9c3b130fb2077bd794f57beeb50eadcd4b9f1ffc7d2f40d65a9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192394431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c4b3e816aabd9aeb7dd71dad13e56dece1e97130877a8dc10ffd78a3e28062`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:48:16 GMT
ENV TOMEE_BUILD=plus
# Thu, 18 Nov 2021 12:48:24 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:24 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:25 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30555b62f61dcc77487e50d27753f9fc52fb42742b5f0a68dca863f35dfb7c5a`  
		Last Modified: Thu, 18 Nov 2021 12:53:00 GMT  
		Size: 68.9 MB (68892272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:8.0.8-webprofile`

```console
$ docker pull tomee@sha256:c4bff3f9c3220931f2e938e978e13db6f40d9056bf2e13b0950ae463886998fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:8.0.8-webprofile` - linux; amd64

```console
$ docker pull tomee@sha256:17808945d115b73325da6bc968ac1a5cb522c17e18ffb393a11a80042c73e32d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172542472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:850fc5e5f10b12db5c551239d3ee386f18a86d7975811d69219b0e97589bbf1a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:48:39 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:48:45 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:45 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:46 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc43f1cf7fcdf28f8e12213dd41d68ffed3cca0fbb9b69d6de4a52063339078`  
		Last Modified: Thu, 18 Nov 2021 12:53:28 GMT  
		Size: 49.0 MB (49040313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:9`

```console
$ docker pull tomee@sha256:c0107232664dbc0ca025700e2a1de95e5154b755bd3a64bd30b3f56d045b21f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:9` - linux; amd64

```console
$ docker pull tomee@sha256:d2bd3e407f48b73bc5f706de37f979595d754590274b78a22c9926c95f456731
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.1 MB (178070362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50131dcbfe666024412e11fb019e236a722a7fd45818871b83cc3c17c9027a06`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:48 GMT
ENV TOMEE_VER=9.0.0-M7
# Thu, 18 Nov 2021 12:49:22 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:49:29 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz   && gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz   && echo `cat tomee.tar.gz.sha512` tomee.tar.gz | sha512sum -c -   && tar -zxf tomee.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:49:29 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:49:29 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf246360353f18a72eb43a35c6a9f0b9ab9cb0c475ed0716cb625a1965927d82`  
		Last Modified: Thu, 18 Nov 2021 12:54:31 GMT  
		Size: 54.6 MB (54568203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:9.0.0-M7-microprofile`

```console
$ docker pull tomee@sha256:7695a8067df502b4a12657710e4987e8cf7fe4045dab929801be9d11f40105ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:9.0.0-M7-microprofile` - linux; amd64

```console
$ docker pull tomee@sha256:17b35e188439dcac0d1716793cd9f263a11d12f63a36dd13ddecd81ea45391ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.1 MB (189109845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a596e807fb75a5ff8c6b54547fd00b5be9bd68c049ac85ce6bf1d51aaab58cc1`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:48 GMT
ENV TOMEE_VER=9.0.0-M7
# Thu, 18 Nov 2021 12:49:11 GMT
ENV TOMEE_BUILD=microprofile
# Thu, 18 Nov 2021 12:49:18 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz   && gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz   && echo `cat tomee.tar.gz.sha512` tomee.tar.gz | sha512sum -c -   && tar -zxf tomee.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:49:19 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:49:19 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cf0877d6b664e3ab92cec263d78d35531e287f6f276435b401f90cb84523f2`  
		Last Modified: Thu, 18 Nov 2021 12:54:18 GMT  
		Size: 65.6 MB (65607686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:9.0.0-M7-plume`

```console
$ docker pull tomee@sha256:6728f3c68f51e05fd4296433c6718395afed1e9d576a3a9e310f6eda7f282006
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:9.0.0-M7-plume` - linux; amd64

```console
$ docker pull tomee@sha256:854e1109d2ebecc4104a4e8464133aa9e8c27ba041e1ab5e130c906a28a848e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.0 MB (201983984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f69f183d7a7ed8f97cf960e6bc51adc0d89c8852c412216a24f56f50808044d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:48 GMT
ENV TOMEE_VER=9.0.0-M7
# Thu, 18 Nov 2021 12:48:49 GMT
ENV TOMEE_BUILD=plume
# Thu, 18 Nov 2021 12:48:57 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz   && gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz   && echo `cat tomee.tar.gz.sha512` tomee.tar.gz | sha512sum -c -   && tar -zxf tomee.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:57 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:57 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd7e640aff335bd7142c477609b6779437e5ee367f35dfffbdfbca7b2d343bf`  
		Last Modified: Thu, 18 Nov 2021 12:53:49 GMT  
		Size: 78.5 MB (78481825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:9.0.0-M7-webprofile`

```console
$ docker pull tomee@sha256:c0107232664dbc0ca025700e2a1de95e5154b755bd3a64bd30b3f56d045b21f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:9.0.0-M7-webprofile` - linux; amd64

```console
$ docker pull tomee@sha256:d2bd3e407f48b73bc5f706de37f979595d754590274b78a22c9926c95f456731
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.1 MB (178070362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50131dcbfe666024412e11fb019e236a722a7fd45818871b83cc3c17c9027a06`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:48 GMT
ENV TOMEE_VER=9.0.0-M7
# Thu, 18 Nov 2021 12:49:22 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:49:29 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz   && gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz   && echo `cat tomee.tar.gz.sha512` tomee.tar.gz | sha512sum -c -   && tar -zxf tomee.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:49:29 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:49:29 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf246360353f18a72eb43a35c6a9f0b9ab9cb0c475ed0716cb625a1965927d82`  
		Last Modified: Thu, 18 Nov 2021 12:54:31 GMT  
		Size: 54.6 MB (54568203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:9.0.0.M7-plus`

```console
$ docker pull tomee@sha256:a40e85aabbfd48ca81f9cce980b0a8c967814f5c5bf78e1db70bdafb5a2423e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:9.0.0.M7-plus` - linux; amd64

```console
$ docker pull tomee@sha256:d17a036c87fa9206edf59fd9fdd48d12d889567d2a1ae0465c35c920704eefa9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.0 MB (194028045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6dd28edf631503b3ee3a24aea27e1d1b473b88905446f4ca3d59ee5a2797f5d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:48 GMT
ENV TOMEE_VER=9.0.0-M7
# Thu, 18 Nov 2021 12:49:00 GMT
ENV TOMEE_BUILD=plus
# Thu, 18 Nov 2021 12:49:07 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz   && gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz   && echo `cat tomee.tar.gz.sha512` tomee.tar.gz | sha512sum -c -   && tar -zxf tomee.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:49:08 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:49:08 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1aeb075311191d82bb778bfb9d7e63d07cb9a992156ed7b451bb65edc683297`  
		Last Modified: Thu, 18 Nov 2021 12:54:04 GMT  
		Size: 70.5 MB (70525886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `tomee:latest`

```console
$ docker pull tomee@sha256:c4bff3f9c3220931f2e938e978e13db6f40d9056bf2e13b0950ae463886998fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `tomee:latest` - linux; amd64

```console
$ docker pull tomee@sha256:17808945d115b73325da6bc968ac1a5cb522c17e18ffb393a11a80042c73e32d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172542472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:850fc5e5f10b12db5c551239d3ee386f18a86d7975811d69219b0e97589bbf1a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:30:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:30:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:30:43 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:30:43 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:30:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 18 Nov 2021 12:47:53 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 12:47:54 GMT
RUN mkdir -p /usr/local/tomee
# Thu, 18 Nov 2021 12:47:54 GMT
WORKDIR /usr/local/tomee
# Thu, 18 Nov 2021 12:48:02 GMT
RUN set -xe;   for key in   9056B710F1E332780DE7AF34CBAEBE39A46C4CA1   F067B8140F5DD80E1D3B5D92318242FE9A0B1183   223D3A74B068ECA354DC385CE126833F9CF64915   DBCCD103B8B24F86FFAAB025C8BB472CD297D428   7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF   B8B301E6105DF628076BD92C5483E55897ABD9B9   FAA603D58B1BA4EDF65896D0ED340E0E6D545F97   A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1   82D8419BA697F0E7FB85916EE91287822FDB81B1   B7574789F5018690043E6DD9C212662E12F3E1DD   C23A3F6F595EBD0F960270CC997C8F1A5BE6E4C1   678F2D98F1FD9643811639FB622B8F2D043F71D8   BDD0BBEB753192957EFC5F896A62FC8EF17D8FEF   D11DF12CC2CA4894BDE638B967C1227A2678363C   C92604B0DEC5C62CFF5801E73D4683C24EDC64D1   626C542EDA7C113814B77AF09C04914D63645D20   3948829384B269D333CC5B98358807C52B4B0E23   ; do     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done
# Thu, 18 Nov 2021 12:48:02 GMT
ENV TOMEE_VER=8.0.8
# Thu, 18 Nov 2021 12:48:39 GMT
ENV TOMEE_BUILD=webprofile
# Thu, 18 Nov 2021 12:48:45 GMT
RUN set -x   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.sha512 -o tomee.tar.gz.sha512   && curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && gpg --batch --verify tomee.tar.gz.asc apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && echo `cat tomee.tar.gz.sha512` | sha512sum -c -   && tar -zxf apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee   && rm apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz   && rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}   && rm bin/*.bat   && rm bin/*.exe   && rm bin/*.tar.gz*   && rm tomee.tar.gz.asc   && rm tomee.tar.gz*
# Thu, 18 Nov 2021 12:48:45 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 12:48:46 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3accde8486ae548a316be3d9277ab3e9e33374f7cfe9e7331973cde22ce0e82f`  
		Last Modified: Wed, 17 Nov 2021 09:48:58 GMT  
		Size: 5.7 MB (5653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98877a5f005f3bd196e69f002a8ce9e0ec54f380cddd12ed1062e02c67220f9`  
		Last Modified: Wed, 17 Nov 2021 09:48:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a549665034cc904cf990a58028b187e532789de2bb27a18696a56573599019`  
		Last Modified: Wed, 17 Nov 2021 09:49:07 GMT  
		Size: 46.8 MB (46831653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1965d44a42b4e78ad10fc731f89e2e715880dcac9d3a851e6e05a9ff422e45`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2313c0fad650aa12b15ed1bfd0755c8f8cf15ef8d87901ed3c92a77f1714d5`  
		Last Modified: Thu, 18 Nov 2021 12:52:42 GMT  
		Size: 58.3 KB (58285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc43f1cf7fcdf28f8e12213dd41d68ffed3cca0fbb9b69d6de4a52063339078`  
		Last Modified: Thu, 18 Nov 2021 12:53:28 GMT  
		Size: 49.0 MB (49040313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
