## `clojure:boot-buster`

```console
$ docker pull clojure@sha256:6e47bc4171b780f37a6722dea098e094455329d9e75451368b3311963cae3274
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:boot-buster` - linux; amd64

```console
$ docker pull clojure@sha256:7bdf67d734399ebbbfaa59ce887f78eb099545f733212fd665f5a42b7dff269a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.0 MB (386975264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5584d7b91dc59b061135bee591a1a059bf0a8d075a65be8436bc02a98acc7fdf`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:35:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 21:02:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 21:02:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 09 Mar 2021 21:02:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 09 Mar 2021 21:02:42 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 21:02:43 GMT
ENV LANG=C.UTF-8
# Tue, 09 Mar 2021 21:02:43 GMT
ENV JAVA_VERSION=11.0.10
# Tue, 09 Mar 2021 21:02:53 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_11.0.10_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.10_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 21:02:54 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:46:56 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 09 Mar 2021 21:46:56 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 09 Mar 2021 21:46:56 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:46:58 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Tue, 09 Mar 2021 21:46:58 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 09 Mar 2021 21:46:58 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 09 Mar 2021 21:47:23 GMT
RUN boot
# Tue, 09 Mar 2021 21:47:24 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7467d1831b6947c294d92ee957902c3cd448b17c5ac2103ca5e79d15afb317c3`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 7.8 MB (7830684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab2c490a3cea21cc051ff29c33cc9857418edfa1be9966124b18abe1d5ae16`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 10.0 MB (9996459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15a0f46f8c38f4ca7daecf160ba9cdb3ddeafda769e2741e179851cfaa14eec`  
		Last Modified: Tue, 09 Feb 2021 04:46:23 GMT  
		Size: 51.8 MB (51830963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4735181ba0c236211ac3061b9b64a3c6b6c49be666302913fd5fb9c5a9ef113`  
		Last Modified: Tue, 09 Mar 2021 21:20:32 GMT  
		Size: 5.3 MB (5286471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfee37d01c31f60d071f54f2414c0da25597fe2cc5c490ce13920824dc1e23c`  
		Last Modified: Tue, 09 Mar 2021 21:20:31 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84289cf02da5745f71612d8ab7b9759a0db726244997235c102e9600cc6ef175`  
		Last Modified: Tue, 09 Mar 2021 21:20:47 GMT  
		Size: 202.8 MB (202802773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fd098983bf901dc8dc61e4426ac1e173de5bb38b82cd6f27fe17d7278c2085`  
		Last Modified: Tue, 09 Mar 2021 22:01:08 GMT  
		Size: 6.9 KB (6931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a021b1a75ed122bffa329d24fbc908d68bb827c09051c7069ea5165dfe6ec8`  
		Last Modified: Tue, 09 Mar 2021 22:01:12 GMT  
		Size: 58.8 MB (58820573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:boot-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:0569978bdd2b3dd273f7e99f72b728b6201256dff323859b810482305cffe929
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.5 MB (383541929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85cc74a77f57569504d11520e3a61f20f21f0a71d38622bffbd02551267fe8ba`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:16 GMT
ADD file:b2e2cca51e131b97e6a7e02af893c7f9b1f7a491b3d5fdaafa80409ed248a706 in / 
# Fri, 12 Mar 2021 01:53:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:29:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:29:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:39:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:39:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 12 Mar 2021 06:39:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 06:39:52 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 06:39:53 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 06:39:54 GMT
ENV JAVA_VERSION=11.0.10
# Fri, 12 Mar 2021 06:40:12 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_11.0.10_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.10_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 12 Mar 2021 06:40:14 GMT
CMD ["jshell"]
# Sat, 13 Mar 2021 00:54:58 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 13 Mar 2021 00:54:59 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 13 Mar 2021 00:55:02 GMT
WORKDIR /tmp
# Sat, 13 Mar 2021 00:55:06 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Sat, 13 Mar 2021 00:55:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 13 Mar 2021 00:55:11 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 13 Mar 2021 00:55:41 GMT
RUN boot
# Sat, 13 Mar 2021 00:55:43 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:e9742a63e95a88f8685c4f23a73f7dd15e4039ac1862ce5753c53406a5f7c04a`  
		Last Modified: Fri, 12 Mar 2021 02:01:14 GMT  
		Size: 49.2 MB (49195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90273c85fdda8648cee9282aa7b01faf0ec1f45451931985b3504c37cf1ac3e6`  
		Last Modified: Fri, 12 Mar 2021 02:43:30 GMT  
		Size: 7.7 MB (7694407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685f873e984153af9a44cf556c7679b430b9c557d901c7d476725134f28754e7`  
		Last Modified: Fri, 12 Mar 2021 02:43:30 GMT  
		Size: 10.0 MB (9984339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34041dfaf60ca49c213d83e89205fc2b7e222817c9728a4aa4f7d3f09d579c9`  
		Last Modified: Fri, 12 Mar 2021 02:43:54 GMT  
		Size: 52.2 MB (52165212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e9f2998e0b670218d576b34308a475046c45448c1fe4c381f7a1debd15c85b`  
		Last Modified: Fri, 12 Mar 2021 06:49:15 GMT  
		Size: 5.3 MB (5277857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3119238b58e7cb540b8d20c130c97953db0998db81a0a10733bc0467efb2b54a`  
		Last Modified: Fri, 12 Mar 2021 06:49:14 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0613829c6b40e5128274b62c14b09ce33430233d5968b9ccffb29f75885ffab`  
		Last Modified: Fri, 12 Mar 2021 06:49:45 GMT  
		Size: 200.4 MB (200396702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de57b1c86e0000585754dcbffeb92713e5294d635c6164d4a0fb60b00bea709`  
		Last Modified: Sat, 13 Mar 2021 01:16:09 GMT  
		Size: 6.9 KB (6931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59198224360bdb9b83277e64050957cd0ea2ce70c94adff2f7cd3bac1b97b79`  
		Last Modified: Sat, 13 Mar 2021 01:16:16 GMT  
		Size: 58.8 MB (58820507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
