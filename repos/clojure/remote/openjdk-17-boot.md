## `clojure:openjdk-17-boot`

```console
$ docker pull clojure@sha256:c887c8a493a52789c7f4da29767698377de26f6848eba2cc26d3298434f66e67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-boot` - linux; amd64

```console
$ docker pull clojure@sha256:99469a33c0b3078ed1f5f264c1eea096d75adb1b9d9ecb3ca1fe7b2fc8116511
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.1 MB (277061279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c3511e7858b357ef1d6ac09a5f0a84c078bbdabed664b7a769c0413a458f2e`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:00:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:01:12 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 23 Jun 2021 08:01:12 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 08:01:12 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 08:01:12 GMT
ENV JAVA_VERSION=17-ea+27
# Wed, 23 Jun 2021 08:01:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='7e1042e3daf741aad75ebda0ea38650111475a810be8fedf38f554732d7750f4'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='88bdeb49442e85c19e126b720bd810bc59007973c6fc06aa6e62b609c1c44d53'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 23 Jun 2021 08:01:30 GMT
CMD ["jshell"]
# Thu, 24 Jun 2021 02:45:33 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 24 Jun 2021 02:45:33 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 24 Jun 2021 02:45:33 GMT
WORKDIR /tmp
# Thu, 24 Jun 2021 02:45:38 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 24 Jun 2021 02:45:38 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 24 Jun 2021 02:45:39 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 24 Jun 2021 02:45:58 GMT
RUN boot
# Thu, 24 Jun 2021 02:45:59 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee45ae9730633057cf9bd12924f9a1bf2b590631d3d085b14c96f4466557794`  
		Last Modified: Wed, 23 Jun 2021 08:12:04 GMT  
		Size: 3.3 MB (3268886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aded171439b9acb04d47c919182bd77c6d2365bf28cf402ee2db0e3821f7342b`  
		Last Modified: Wed, 23 Jun 2021 08:14:13 GMT  
		Size: 187.5 MB (187546175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3770fb7e6b15a83a36ae082664d2fa4e5b339c4de28237b5ebd397d9334d669`  
		Last Modified: Thu, 24 Jun 2021 02:55:57 GMT  
		Size: 279.9 KB (279850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc70133c69b3373c2d983a1827e37cca722c824be82847665a6c5176b322763e`  
		Last Modified: Thu, 24 Jun 2021 02:56:01 GMT  
		Size: 58.8 MB (58820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-boot` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2edd7c128dd74a4b05fbb2f816a0549f391d966fafc4c9b99589f9340dc6500d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.5 MB (274491301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32af877d14c565136d727a360f8737318e67f97d2c49ce6501a43ee036d1d0fb`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 04:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 04:57:10 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 23 Jun 2021 04:57:10 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 04:57:10 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 04:57:10 GMT
ENV JAVA_VERSION=17-ea+27
# Wed, 23 Jun 2021 04:57:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='7e1042e3daf741aad75ebda0ea38650111475a810be8fedf38f554732d7750f4'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='88bdeb49442e85c19e126b720bd810bc59007973c6fc06aa6e62b609c1c44d53'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 23 Jun 2021 04:57:23 GMT
CMD ["jshell"]
# Wed, 23 Jun 2021 20:01:14 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 23 Jun 2021 20:01:14 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 23 Jun 2021 20:01:14 GMT
WORKDIR /tmp
# Wed, 23 Jun 2021 20:01:19 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 23 Jun 2021 20:01:19 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 23 Jun 2021 20:01:19 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 23 Jun 2021 20:01:39 GMT
RUN boot
# Wed, 23 Jun 2021 20:01:40 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb5c013aa648ff2c30dafc35db9efb2faa7f9fa6f1c98a2f31c1b5fee0334dc`  
		Last Modified: Wed, 23 Jun 2021 05:11:10 GMT  
		Size: 3.1 MB (3118894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cc1fe036d48b434be9ff64dcce132db5120a6f2c84577f627ca47e01e62879`  
		Last Modified: Wed, 23 Jun 2021 05:13:28 GMT  
		Size: 186.4 MB (186357568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9b27be4befc520d19270a92e389ddaa6b47588fbdaf4b0204a399ed24e9131`  
		Last Modified: Wed, 23 Jun 2021 20:12:11 GMT  
		Size: 279.6 KB (279557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f20eb3834f22a2240a4c00b556f5e71d2eefdfb9aa9bdc9a194ad166fa3585`  
		Last Modified: Wed, 23 Jun 2021 20:12:16 GMT  
		Size: 58.8 MB (58820289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
