## `clojure:openjdk-18-boot`

```console
$ docker pull clojure@sha256:65f3fdf1fe2a93ffe2adfe4fe85d05c424ca8fa17bfefcc65af04f11fe9a8098
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-boot` - linux; amd64

```console
$ docker pull clojure@sha256:29fed8ea231036d8a339a8addbfc37aa50f358d1cabf8166ebcf4cb6453e7c63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.3 MB (280333987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9dac7794a8c96a2c13e7353505364fbbd66d8502efc06faf73af98268d4d351`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:21 GMT
ADD file:19d7ba0fceddd7fc78b5fb96cf8110e5d10e0e5d2554030dfe640d161379cb79 in / 
# Fri, 03 Sep 2021 01:21:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:31:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:31:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 08:31:20 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:31:20 GMT
ENV LANG=C.UTF-8
# Sat, 25 Sep 2021 00:25:42 GMT
ENV JAVA_VERSION=18-ea+16
# Sat, 25 Sep 2021 00:25:55 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-x64_bin.tar.gz'; 			downloadSha256='ec604f7aef23624c0acdc0db346a2b226aab47d120538833070f0d5e01d571c1'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-aarch64_bin.tar.gz'; 			downloadSha256='623eff3e61bd5f74442fb5699ac3dea167dbe0ade7dd6c1fa9cdd4788e316b96'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 25 Sep 2021 00:25:56 GMT
CMD ["jshell"]
# Sat, 25 Sep 2021 01:21:51 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 25 Sep 2021 01:21:52 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 25 Sep 2021 01:21:52 GMT
WORKDIR /tmp
# Sat, 25 Sep 2021 01:21:56 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 25 Sep 2021 01:21:56 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 25 Sep 2021 01:21:57 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 25 Sep 2021 01:22:20 GMT
RUN boot
# Sat, 25 Sep 2021 01:22:20 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:f8416d8bac72cefc0ce17bd2dc0c03aa43e123d309db92ee23be9382192cf2ed`  
		Last Modified: Fri, 03 Sep 2021 01:27:25 GMT  
		Size: 31.4 MB (31368702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ae0b0c4c13e1ebacfd091b8e226cc8aa92df8937632e3bec2b03a877bf2d87`  
		Last Modified: Fri, 03 Sep 2021 08:49:03 GMT  
		Size: 1.6 MB (1582002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90416dc6dd4ab7f0222694d32e64bba4e610c0cd0dcf2227cc3631e39d4f3ea0`  
		Last Modified: Sat, 25 Sep 2021 00:34:30 GMT  
		Size: 188.3 MB (188279789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025bf23355b61c491701aefff1d2f0b2188d61ca22f1064bb6f721618f129e27`  
		Last Modified: Sat, 25 Sep 2021 01:28:38 GMT  
		Size: 283.1 KB (283056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83878ca6030ca909ab97404119940b28eae5e779e69146d1af02ccaa37fb50f6`  
		Last Modified: Sat, 25 Sep 2021 01:28:41 GMT  
		Size: 58.8 MB (58820438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-boot` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:fa11b36e732270f5e3a1247d55cf899555f061044dd892424b9307bf0ea4f231
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.7 MB (277740926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0d03ccc9e56d713bf90060f7fde5789372f7ddad76c44c909268cb9bf959b4`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:43 GMT
ADD file:6472ab63529e688735f77634402740e08fdbd5bfa788c150915027993df7e8ec in / 
# Tue, 28 Sep 2021 01:40:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 05:42:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:42:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 28 Sep 2021 05:42:51 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 05:42:51 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 05:42:51 GMT
ENV JAVA_VERSION=18-ea+16
# Tue, 28 Sep 2021 05:43:03 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-x64_bin.tar.gz'; 			downloadSha256='ec604f7aef23624c0acdc0db346a2b226aab47d120538833070f0d5e01d571c1'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-aarch64_bin.tar.gz'; 			downloadSha256='623eff3e61bd5f74442fb5699ac3dea167dbe0ade7dd6c1fa9cdd4788e316b96'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 05:43:04 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 02:32:08 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 29 Sep 2021 02:32:08 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 29 Sep 2021 02:32:09 GMT
WORKDIR /tmp
# Wed, 29 Sep 2021 02:32:13 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 29 Sep 2021 02:32:13 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 29 Sep 2021 02:32:13 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 29 Sep 2021 02:32:34 GMT
RUN boot
# Wed, 29 Sep 2021 02:32:34 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:2f8871a8654eb1158cb626f8dc69992dba7e4bd8796fae6aa7cf967f951f5fe9`  
		Last Modified: Tue, 28 Sep 2021 01:48:25 GMT  
		Size: 30.1 MB (30055408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc69e286af9edc8fb3518a0692316edc953730d4b65004457f37972b70873fe1`  
		Last Modified: Tue, 28 Sep 2021 06:04:25 GMT  
		Size: 1.6 MB (1566191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d48028112f2af20bfa2863589ad5231ced228799108fbbc4460280a1d3a0bb1`  
		Last Modified: Tue, 28 Sep 2021 06:04:43 GMT  
		Size: 187.0 MB (187015722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c0e061b3780cc3b92291f28a6c287b4935db2971c92af19f90fab20f5a0c6d`  
		Last Modified: Wed, 29 Sep 2021 02:56:58 GMT  
		Size: 283.0 KB (282995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce00a06e27ba0188decc41ef811721816260a104df76060ce2f950333fb1254d`  
		Last Modified: Wed, 29 Sep 2021 02:57:02 GMT  
		Size: 58.8 MB (58820610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
