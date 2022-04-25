## `clojure:openjdk-19-boot-2.8.3`

```console
$ docker pull clojure@sha256:ae6c29eff156be74335382fa679b010e3750183fe85a4dc756a66ba7e71c709f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-19-boot-2.8.3` - linux; amd64

```console
$ docker pull clojure@sha256:a237a2963727e401142ce04c832762d9ae7c220909f4715e0ff81258ae0015d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.1 MB (287060667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9459309f3d931987d1ed3cb3e6b494315069d42427973b2d191aa2dac3b0fb`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:47:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:47:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 20 Apr 2022 10:47:39 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:47:40 GMT
ENV LANG=C.UTF-8
# Mon, 25 Apr 2022 18:23:24 GMT
ENV JAVA_VERSION=19-ea+19
# Mon, 25 Apr 2022 18:23:47 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5920845cb577a0883cfbd0bc3a781b5b0a4f71b19a870525c653f9815fa0596b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad9457964256d9d43d6246a0da743a73450231506d0a8a711e28b996b7e6e6e3'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 25 Apr 2022 18:23:48 GMT
CMD ["jshell"]
# Mon, 25 Apr 2022 19:06:09 GMT
ENV BOOT_VERSION=2.8.3
# Mon, 25 Apr 2022 19:06:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Mon, 25 Apr 2022 19:06:09 GMT
WORKDIR /tmp
# Mon, 25 Apr 2022 19:06:13 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Mon, 25 Apr 2022 19:06:13 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Mon, 25 Apr 2022 19:06:13 GMT
ENV BOOT_AS_ROOT=yes
# Mon, 25 Apr 2022 19:06:35 GMT
RUN boot
# Mon, 25 Apr 2022 19:06:36 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Mon, 25 Apr 2022 19:06:36 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 25 Apr 2022 19:06:36 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3aa8d076675d49d85180b0ced9daef210fe4fdff4bdbb422b9cf384e591d0`  
		Last Modified: Wed, 20 Apr 2022 11:01:25 GMT  
		Size: 1.6 MB (1582162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4da7eb4501e852e7e9b34d60f5e860576c81b3d23aa925e8848800cd75fb39`  
		Last Modified: Mon, 25 Apr 2022 18:34:50 GMT  
		Size: 195.0 MB (194995411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae2660b64e65f5a712c25215cc900cb9b80f46cf0fcc463405d14bcd0b2a9cd`  
		Last Modified: Mon, 25 Apr 2022 19:15:06 GMT  
		Size: 283.1 KB (283139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000e76a445b8a4d83a2d1445b2c640d5b903db2abf3b25bf664faa3c3fbedddd`  
		Last Modified: Mon, 25 Apr 2022 19:15:09 GMT  
		Size: 58.8 MB (58820570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db00baddfa61e31236bb2eb876e74950aeeffaef95ed198e2828cec9b9ca31cd`  
		Last Modified: Mon, 25 Apr 2022 19:15:06 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-19-boot-2.8.3` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9d77d133f180e09425c4f89f9116ba5b4e4c4562746a3632e1d51b396885fa15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.9 MB (283933966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c364bfd06ea143149f6d6e99726be5b0ba890bb5b1ba8f19bd3b8a92a61e5a9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:24:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:24:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 20 Apr 2022 10:24:40 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:24:41 GMT
ENV LANG=C.UTF-8
# Mon, 25 Apr 2022 18:41:51 GMT
ENV JAVA_VERSION=19-ea+19
# Mon, 25 Apr 2022 18:42:03 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5920845cb577a0883cfbd0bc3a781b5b0a4f71b19a870525c653f9815fa0596b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad9457964256d9d43d6246a0da743a73450231506d0a8a711e28b996b7e6e6e3'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 25 Apr 2022 18:42:04 GMT
CMD ["jshell"]
# Mon, 25 Apr 2022 19:35:27 GMT
ENV BOOT_VERSION=2.8.3
# Mon, 25 Apr 2022 19:35:27 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Mon, 25 Apr 2022 19:35:28 GMT
WORKDIR /tmp
# Mon, 25 Apr 2022 19:35:33 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Mon, 25 Apr 2022 19:35:33 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Mon, 25 Apr 2022 19:35:34 GMT
ENV BOOT_AS_ROOT=yes
# Mon, 25 Apr 2022 19:35:47 GMT
RUN boot
# Mon, 25 Apr 2022 19:35:49 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Mon, 25 Apr 2022 19:35:49 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 25 Apr 2022 19:35:50 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59f13dc084e185af417a4c6d1be2534adaff0c4f35ac2166a539260f4e8e945`  
		Last Modified: Wed, 20 Apr 2022 10:46:08 GMT  
		Size: 1.4 MB (1361221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762a965b36a14508cc17ff80baed915039381b471ad8671a763702d4a12114fe`  
		Last Modified: Mon, 25 Apr 2022 18:59:25 GMT  
		Size: 193.6 MB (193623751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b860a17594303fa72a569e1c6ddd8b2b431b7bfb2b9815b45957a4c397c77edc`  
		Last Modified: Mon, 25 Apr 2022 19:48:24 GMT  
		Size: 67.2 KB (67240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3a85a6bb5c5f18c0af919e2b65d927b2cd71b459718e8a7c4569e4b9bd6ceb`  
		Last Modified: Mon, 25 Apr 2022 19:48:29 GMT  
		Size: 58.8 MB (58815546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb045f6d7843b9ab39c60884f648e6c9ca007a50f1d5e29f4aad7813e1e0d34a`  
		Last Modified: Mon, 25 Apr 2022 19:48:24 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
