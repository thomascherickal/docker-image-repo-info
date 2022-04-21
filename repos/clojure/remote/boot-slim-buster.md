## `clojure:boot-slim-buster`

```console
$ docker pull clojure@sha256:037f3dac08e7bf971785121dce00cf57536c2b195fa658866eb08780632c2ccc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:boot-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:b89ca00758f476f3e7d4dc45ee20cb6adc878a2adc50691912767a361962af8f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.4 MB (277417423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d48c72089aaa411d0b3deec033b52c6db9de2e6890b397dc699c32840db736`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:48:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:51:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 20 Apr 2022 10:51:43 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:51:43 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 10:51:43 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 20 Apr 2022 10:51:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 20 Apr 2022 10:51:59 GMT
CMD ["jshell"]
# Thu, 21 Apr 2022 00:29:06 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 21 Apr 2022 00:29:06 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 21 Apr 2022 00:29:07 GMT
WORKDIR /tmp
# Thu, 21 Apr 2022 00:29:11 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 21 Apr 2022 00:29:11 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 21 Apr 2022 00:29:11 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 21 Apr 2022 00:29:38 GMT
RUN boot
# Thu, 21 Apr 2022 00:29:38 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 21 Apr 2022 00:29:38 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 21 Apr 2022 00:29:38 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b97724dec0639ffbe1d30e60defc8ff8fc2e27a3844e7c6173e64cb73e25b88`  
		Last Modified: Wed, 20 Apr 2022 11:02:57 GMT  
		Size: 3.3 MB (3273257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a8e5c4d31807097cbd665b38de64e8a7d442e0e99b9cca01b3800bb803a164`  
		Last Modified: Wed, 20 Apr 2022 11:08:24 GMT  
		Size: 187.9 MB (187902684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d8e82eaa308ad3632df530dac8faf46b4f45c42e14185f5d14ea3ba8d3e220`  
		Last Modified: Thu, 21 Apr 2022 00:51:23 GMT  
		Size: 279.8 KB (279755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc88b4f636fdaab08b0f7f16c2f018ad4d46699746b9c1468cf4db93ec37cc48`  
		Last Modified: Thu, 21 Apr 2022 00:51:26 GMT  
		Size: 58.8 MB (58820659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea9b10032f94275cc453d2823f1bc3cf60774d0b796d57afafe68880f8772f8`  
		Last Modified: Thu, 21 Apr 2022 00:51:23 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:boot-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:92fa64e90f93b0b5e06d1cd72802fc968f37e7eb7bfd3ab8e395153f7806347c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.5 MB (274450916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c58787a1c3a25ff16b1862283f87e805c39b78c6078544d11f2ad3f36d87cad7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:25:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:29:40 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 20 Apr 2022 10:29:40 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:29:41 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 10:29:42 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 20 Apr 2022 10:29:55 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 20 Apr 2022 10:29:55 GMT
CMD ["jshell"]
# Thu, 21 Apr 2022 03:21:08 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 21 Apr 2022 03:21:08 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 21 Apr 2022 03:21:09 GMT
WORKDIR /tmp
# Thu, 21 Apr 2022 03:21:14 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 21 Apr 2022 03:21:15 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 21 Apr 2022 03:21:16 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 21 Apr 2022 03:21:29 GMT
RUN boot
# Thu, 21 Apr 2022 03:21:31 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 21 Apr 2022 03:21:31 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 21 Apr 2022 03:21:32 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef4c0391a581a54e4ae08706ac3173bf39e99722f6efe3a9094dbe8916d7bfd`  
		Last Modified: Wed, 20 Apr 2022 10:47:49 GMT  
		Size: 3.1 MB (3125683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2ff3da472d3e74705427c6b8ac620684ee8c6d130060777a70dd139cd89254`  
		Last Modified: Wed, 20 Apr 2022 10:53:53 GMT  
		Size: 186.5 MB (186533409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31656444e2d0801ba1e6d0583975628f736b831aeee818e683090dbd8d5a2d4`  
		Last Modified: Thu, 21 Apr 2022 03:48:00 GMT  
		Size: 67.5 KB (67508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164ee98495e59397de783933d54200e877e33a5d7748e65cf4bc45e0a81c2272`  
		Last Modified: Thu, 21 Apr 2022 03:48:04 GMT  
		Size: 58.8 MB (58815561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e432e02ed396ff5ce4ada2bb9fa3328ca0efca287f2c89bdeaa906da91c3fe20`  
		Last Modified: Thu, 21 Apr 2022 03:48:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
