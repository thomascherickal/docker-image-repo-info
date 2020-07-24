## `clojure:openjdk-15-boot-2.8.3-buster`

```console
$ docker pull clojure@sha256:2c5b67e344eba5eecfed46590586c65e2227c6fa225fa34758e2afd0205fc3e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-15-boot-2.8.3-buster` - linux; amd64

```console
$ docker pull clojure@sha256:af90a0da3a6144ded33ec8dd44da3171df512b2be87ec999a5df8c64803f1469
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.6 MB (388644895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430cdeb1f9a1726872b83320e3d2148104be58eeea1837806dab4b40fe014a59`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:16 GMT
ADD file:89dfd7d3ed77fd5e05f20a0ab631142207ae462f5bbd877f8745d3930c751d87 in / 
# Wed, 22 Jul 2020 02:03:16 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 03:00:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 03:00:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 03:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:34:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:34:22 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 22:36:32 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Wed, 22 Jul 2020 22:36:32 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 22:36:33 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 24 Jul 2020 19:15:42 GMT
ENV JAVA_VERSION=15-ea+33
# Fri, 24 Jul 2020 19:16:24 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/33/GPL/openjdk-15-ea+33_linux-aarch64_bin.tar.gz; 			downloadSha256=124fd9ba4611895460ff1547df282cd49b0e9ba2f00c9ead211b59142cc642c4; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/33/GPL/openjdk-15-ea+33_linux-x64_bin.tar.gz; 			downloadSha256=6de169c1de7d37e6c5d5b59a12410a908f22576c07f98d9915a586d91909fc12; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Fri, 24 Jul 2020 19:16:24 GMT
CMD ["jshell"]
# Fri, 24 Jul 2020 20:47:27 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 24 Jul 2020 20:47:27 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 24 Jul 2020 20:47:27 GMT
WORKDIR /tmp
# Fri, 24 Jul 2020 20:47:28 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Fri, 24 Jul 2020 20:47:28 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 24 Jul 2020 20:47:29 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 24 Jul 2020 20:47:46 GMT
RUN boot
# Fri, 24 Jul 2020 20:47:46 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:31dd5ebca5efc5e96a425402fa85e492b02c8fe757dfd3edfdea2a7c67322909`  
		Last Modified: Wed, 22 Jul 2020 02:09:37 GMT  
		Size: 50.4 MB (50390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed641c4ae9821ca3c399071ea82ae667237acbcaad1e367c3e1e87fc967834c`  
		Last Modified: Wed, 22 Jul 2020 03:16:28 GMT  
		Size: 7.8 MB (7811702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd57146431eae70720cf24877e818256ae1a30b9c1c9e7d0ad093c945ca0af2`  
		Last Modified: Wed, 22 Jul 2020 03:16:28 GMT  
		Size: 10.0 MB (9996319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac34a4d7c330794ec24a76e7e58b50d4c8f6a2fc77ca958d83092c8962e7d6d7`  
		Last Modified: Wed, 22 Jul 2020 03:16:44 GMT  
		Size: 51.8 MB (51829832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca8eb5acf18e7b4ad9db90f79975b06b18325e8658a637c682f1cb13ed67997`  
		Last Modified: Wed, 22 Jul 2020 22:44:05 GMT  
		Size: 13.9 MB (13920343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81ece9319a60bd93f204ea486d5e2a72cf146eaf2d653e9d8ae8121e76c44ca`  
		Last Modified: Wed, 22 Jul 2020 22:45:05 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f8a67791e6349342ef74ba0e6924df41012476918a8a52a96fa42d85c11bff`  
		Last Modified: Fri, 24 Jul 2020 19:20:33 GMT  
		Size: 195.9 MB (195869076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ca1d3addd617104928292019ee9d0386f6f9d1a8253ee62c3aaf48d6021267`  
		Last Modified: Fri, 24 Jul 2020 20:50:31 GMT  
		Size: 6.9 KB (6892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeebf6473105b2d8564f3ce8faec79ed13bc198470ad8ed023bdc57bdf86570`  
		Last Modified: Fri, 24 Jul 2020 20:50:36 GMT  
		Size: 58.8 MB (58820197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
