## `clojure:openjdk-15-boot-buster`

```console
$ docker pull clojure@sha256:6e396970ba735a0d6625b557709560f3b504c4bcf07d407854bef26004d6c45b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-15-boot-buster` - linux; amd64

```console
$ docker pull clojure@sha256:605b56cfe7b5348b82a703eb728cb7bd55d7cf79c849bdbbb5901764dd36e1c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.7 MB (388712849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8b13a62cd0b1615133e547f734609acde9f6befc8daceb5a6db5f496ef542e`
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
# Tue, 09 Mar 2021 20:56:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 21:01:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-15
# Tue, 09 Mar 2021 21:01:20 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 09 Mar 2021 21:01:20 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 21:01:20 GMT
ENV LANG=C.UTF-8
# Tue, 09 Mar 2021 21:01:21 GMT
ENV JAVA_VERSION=15.0.2
# Tue, 09 Mar 2021 21:01:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='91ac6fc353b6bf39d995572b700e37a20e119a87034eeb939a6f24356fbcd207'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='3958f01858f9290c48c23e7804a0af3624e8eca6749b085c425df4c4f2f7dcbc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 21:01:31 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:49:31 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 09 Mar 2021 21:49:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 09 Mar 2021 21:49:31 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:49:32 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Tue, 09 Mar 2021 21:49:32 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 09 Mar 2021 21:49:33 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 09 Mar 2021 21:49:55 GMT
RUN boot
# Tue, 09 Mar 2021 21:49:55 GMT
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
	-	`sha256:415655c50d52018d0916c838b59d5ee0a87aea61c2464768eae0a629075c7263`  
		Last Modified: Tue, 09 Mar 2021 21:10:07 GMT  
		Size: 13.9 MB (13921302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f105276800877ff54c00b0db7fd825a11fc817dde638df7985d7fda75545a9b`  
		Last Modified: Tue, 09 Mar 2021 21:17:07 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ab0a9f2c59cb4d600f76d1f646b3bab0446d6bc6b3519d438873ea9d42de4b`  
		Last Modified: Tue, 09 Mar 2021 21:17:23 GMT  
		Size: 195.9 MB (195905697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a208f1addf25a64fa49a5047c5a136b60aae08180cdfba9350f4b0f7d2a6b94d`  
		Last Modified: Tue, 09 Mar 2021 22:04:00 GMT  
		Size: 6.9 KB (6922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c446fda47a1b7161a5c27ef9782c7b8934bbfd25f9999beb958c03a0e2ae9a0`  
		Last Modified: Tue, 09 Mar 2021 22:04:05 GMT  
		Size: 58.8 MB (58820414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-15-boot-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ed0dc1f61439144d9126d44774dd1e8db3c365658eaeb1f0fbca487a997f0900
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.5 MB (367542934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffc2d0b31f019abcf75b619c709744d82e3df88441924427c298bf142c2f51f`
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
# Fri, 12 Mar 2021 06:33:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:37:53 GMT
ENV JAVA_HOME=/usr/local/openjdk-15
# Fri, 12 Mar 2021 06:37:55 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 06:37:56 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 06:37:56 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 06:37:57 GMT
ENV JAVA_VERSION=15.0.2
# Fri, 12 Mar 2021 06:38:34 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='91ac6fc353b6bf39d995572b700e37a20e119a87034eeb939a6f24356fbcd207'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='3958f01858f9290c48c23e7804a0af3624e8eca6749b085c425df4c4f2f7dcbc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 12 Mar 2021 06:38:36 GMT
CMD ["jshell"]
# Sat, 13 Mar 2021 01:00:41 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 13 Mar 2021 01:00:43 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 13 Mar 2021 01:00:46 GMT
WORKDIR /tmp
# Sat, 13 Mar 2021 01:00:52 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Sat, 13 Mar 2021 01:00:54 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 13 Mar 2021 01:00:55 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 13 Mar 2021 01:01:28 GMT
RUN boot
# Sat, 13 Mar 2021 01:01:32 GMT
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
	-	`sha256:bea7dd455a2166654bd3d729e78a91e18b7d2fb982780428bf02e0d1d700cb88`  
		Last Modified: Fri, 12 Mar 2021 06:44:30 GMT  
		Size: 14.7 MB (14673622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5b3c61fce08c8fcf2b274c105f4ce74bfcf88a42d84cd266e46675a49551f5`  
		Last Modified: Fri, 12 Mar 2021 06:47:21 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2fbf33443b755809172420d7cecdf218922f75f006929e975f4610067f671e`  
		Last Modified: Fri, 12 Mar 2021 06:47:47 GMT  
		Size: 175.0 MB (175002100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4912389f38bfb79418de3354a0403bd5fc280f0c5f52b0aa0e1b48d3afb4a9a5`  
		Last Modified: Sat, 13 Mar 2021 01:18:10 GMT  
		Size: 6.9 KB (6922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7746ccace721a25a338f1a53fd1577f0c61a24a26d0a2093ec18de960ce847`  
		Last Modified: Sat, 13 Mar 2021 01:18:16 GMT  
		Size: 58.8 MB (58820358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
