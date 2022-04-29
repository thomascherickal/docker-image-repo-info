## `clojure:openjdk-19-boot-bullseye`

```console
$ docker pull clojure@sha256:f53ca72b8a51dc00886d7e6a01d4bd3e8ac71c1a761420df21374b3a1e2c8872
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-19-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:cc4ad13d298d104a134247faa7ab68c7ffb38554a9b8e10f261c92371f228071
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.2 MB (394237688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d474fc244effe3e227bed58b9c065936604a36271e514c6a1b14eadf5923b31b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:15 GMT
ADD file:3a81c181c66f226bd6abd48d0c7ed8a9c599c9f521ec7229286c83161afec8c2 in / 
# Wed, 20 Apr 2022 04:43:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:57:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:57:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:58:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:47:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:47:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 20 Apr 2022 10:47:19 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:47:19 GMT
ENV LANG=C.UTF-8
# Thu, 28 Apr 2022 23:20:52 GMT
ENV JAVA_VERSION=19-ea+20
# Thu, 28 Apr 2022 23:21:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/20/GPL/openjdk-19-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='e5667a2a1208eb3042dd0c3187dd61d10b435204e4d26e466b8f2c7a5d988ce6'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/20/GPL/openjdk-19-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='a5ff38640a2b5097e460a7dd54544f0cbe19b041262549cd3d1015fc81eec50f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 28 Apr 2022 23:21:02 GMT
CMD ["jshell"]
# Fri, 29 Apr 2022 01:19:29 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 29 Apr 2022 01:19:30 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 29 Apr 2022 01:19:30 GMT
WORKDIR /tmp
# Fri, 29 Apr 2022 01:19:33 GMT
RUN apt-get update && apt-get install -y make && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Fri, 29 Apr 2022 01:19:33 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 29 Apr 2022 01:19:33 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 29 Apr 2022 01:20:13 GMT
RUN boot
# Fri, 29 Apr 2022 01:20:13 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 29 Apr 2022 01:20:13 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 29 Apr 2022 01:20:13 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:6aefca2dc61dcbcd268b8a9861e552f9cdb69e57242faec64ac120d2355a9c1a`  
		Last Modified: Wed, 20 Apr 2022 04:47:57 GMT  
		Size: 54.9 MB (54941777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967757d5652770cfa81b6cc7577d65e06d336173da116d1fb5b2d349d5d44127`  
		Last Modified: Wed, 20 Apr 2022 07:05:43 GMT  
		Size: 5.2 MB (5155716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c357e2c68cb3bf1e98dcb3eb6ceb16837253db71535921d6993c594588bffe04`  
		Last Modified: Wed, 20 Apr 2022 07:05:45 GMT  
		Size: 10.9 MB (10874928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c766e27afb21eddf9ab3e4349700ebe697c32a4c6ada6af4f08282277a291a28`  
		Last Modified: Wed, 20 Apr 2022 07:06:05 GMT  
		Size: 54.6 MB (54578663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e454664a629c8e4cac99685ba1b624982040c45466f197f649234a8e132803`  
		Last Modified: Wed, 20 Apr 2022 11:00:48 GMT  
		Size: 14.1 MB (14071513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164406dd3998503a27a9e3d2981ab6fe8a4527feea1e275daf277431887d7ff`  
		Last Modified: Thu, 28 Apr 2022 23:29:01 GMT  
		Size: 194.8 MB (194776114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a082a407b44035025e5f7f61d3b6cacb862332a32d647a16d924b14efb8cb6f4`  
		Last Modified: Fri, 29 Apr 2022 01:25:27 GMT  
		Size: 1.0 MB (1017487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a46dc40837a44a573a43504194facda4278c0e7b422b29c6c5ffe7b4301c00`  
		Last Modified: Fri, 29 Apr 2022 01:25:30 GMT  
		Size: 58.8 MB (58821084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907c128bf6194026ca4d9cd1527e4105d982b8e11e087294f5042815d96e9ced`  
		Last Modified: Fri, 29 Apr 2022 01:25:27 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-19-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a957920f00b0c4aa18e07ddb35599c13c53a7f1e3201dd18de4cfc47a8215c12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.7 MB (392661897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3659ea75c8a89dad773fa1c7287a630e101786671b198ff03cfa76a9b831351c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:28:55 GMT
ADD file:ece192802cbdaf1a141d04f0c2e90cfd3479e5e3e82c6a00206970684494cf48 in / 
# Wed, 20 Apr 2022 04:28:56 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:44:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:24:10 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 20 Apr 2022 10:24:11 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:24:12 GMT
ENV LANG=C.UTF-8
# Thu, 28 Apr 2022 23:41:38 GMT
ENV JAVA_VERSION=19-ea+20
# Thu, 28 Apr 2022 23:41:48 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/20/GPL/openjdk-19-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='e5667a2a1208eb3042dd0c3187dd61d10b435204e4d26e466b8f2c7a5d988ce6'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/20/GPL/openjdk-19-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='a5ff38640a2b5097e460a7dd54544f0cbe19b041262549cd3d1015fc81eec50f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 28 Apr 2022 23:41:48 GMT
CMD ["jshell"]
# Fri, 29 Apr 2022 02:44:51 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 29 Apr 2022 02:44:52 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 29 Apr 2022 02:44:53 GMT
WORKDIR /tmp
# Fri, 29 Apr 2022 02:44:58 GMT
RUN apt-get update && apt-get install -y make && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Fri, 29 Apr 2022 02:44:58 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 29 Apr 2022 02:44:59 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 29 Apr 2022 02:45:15 GMT
RUN boot
# Fri, 29 Apr 2022 02:45:16 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 29 Apr 2022 02:45:16 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 29 Apr 2022 02:45:17 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:83d5dcfea08e6927083bc886bf182fc39d87bb04b54b63002ac0c4c0b9aab682`  
		Last Modified: Wed, 20 Apr 2022 04:35:19 GMT  
		Size: 53.6 MB (53633096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfa86b7b1aca6d694057e4d42ee1440527f41c00b9e577df729244380c9eba`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 4.9 MB (4938663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79b19335f27cc78840bf9159e875322f3252ac06113c73756f9d4fba905f9b`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 10.7 MB (10656971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350ecaf08eac09037b05465ab97a1b8f7bc9b7a9b1fcef900dedd7dba9bbcf4d`  
		Last Modified: Wed, 20 Apr 2022 06:54:32 GMT  
		Size: 54.7 MB (54672934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b174d41b9ea1124e2245788f2c290f940eca707dcc0446cd302b01aaeb5c82`  
		Last Modified: Wed, 20 Apr 2022 10:45:28 GMT  
		Size: 15.5 MB (15525740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28cb344818c5b2f55c5308ec92931f8aba70f9a8c843da20b990b62cbedae4c`  
		Last Modified: Thu, 28 Apr 2022 23:56:14 GMT  
		Size: 193.6 MB (193640907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09038114eb8213065bbb3438f9c73f69f8b487450f00be39320483a0abeeb08`  
		Last Modified: Fri, 29 Apr 2022 02:54:50 GMT  
		Size: 777.4 KB (777420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd29cf1b62f06687c2cf2e71dfb3adb9d2dba89de87ff90390617e0a0d540f`  
		Last Modified: Fri, 29 Apr 2022 02:54:55 GMT  
		Size: 58.8 MB (58815760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667c529fbdf756b0b0dff4ea99f08bd7f8f6f6a512bc5403a406f55689dc7376`  
		Last Modified: Fri, 29 Apr 2022 02:54:49 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
