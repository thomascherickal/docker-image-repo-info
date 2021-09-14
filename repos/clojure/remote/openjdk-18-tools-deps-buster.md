## `clojure:openjdk-18-tools-deps-buster`

```console
$ docker pull clojure@sha256:3d40c3876e056c10475dc949d69bbc9e734703b3cc60dcbdc065571e36c967f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-tools-deps-buster` - linux; amd64

```console
$ docker pull clojure@sha256:5ba89bc5f7b67919396bb6ccda5d981ae959e6e3d1beabf765e9f95951cca425
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.5 MB (349549989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4840e06a4c905c228230c7b1d68e81392b93db812dc919698199c4631389723c`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:33:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:32:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 08:32:04 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:32:05 GMT
ENV LANG=C.UTF-8
# Tue, 14 Sep 2021 01:32:44 GMT
ENV JAVA_VERSION=18-ea+14
# Tue, 14 Sep 2021 01:32:53 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/14/GPL/openjdk-18-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='6aee5779ac7488dbd6988658662ca683704ac98cee6b8dde8df3ddffac76142e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/14/GPL/openjdk-18-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='88a106afe903b8f5d552ceae108294d8b36cbc0656a744f84525ccae542c5029'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 14 Sep 2021 01:32:54 GMT
CMD ["jshell"]
# Tue, 14 Sep 2021 02:15:19 GMT
ENV CLOJURE_VERSION=1.10.3.967
# Tue, 14 Sep 2021 02:15:19 GMT
WORKDIR /tmp
# Tue, 14 Sep 2021 02:15:29 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d1fba0cd0733b7cb66e47620845ecedfd757a9bf84e8b276fdb37ed9c272d3ae *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Tue, 14 Sep 2021 02:15:30 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e5f66f5d0e1c97622f33d44fb04efb42bd3562bdc3482537d121040c789f9a`  
		Last Modified: Fri, 03 Sep 2021 06:40:37 GMT  
		Size: 7.8 MB (7833606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c8f1c77d6674046d7deb41be1ca07f25cb43fd67f87e879ee79cc6586087f0`  
		Last Modified: Fri, 03 Sep 2021 06:40:37 GMT  
		Size: 10.0 MB (9997249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5095cab277710f0c2883844158323ad986c763ffc37353ddff874dd85585d9b6`  
		Last Modified: Fri, 03 Sep 2021 06:40:55 GMT  
		Size: 51.8 MB (51840968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee27e112836c56c7a7f0e8a1986512005c433ddddbe7aaff39133b826a04844`  
		Last Modified: Fri, 03 Sep 2021 08:50:02 GMT  
		Size: 13.9 MB (13921260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89857ce3f39017cfcae77a5aa5ef0065be326d5b27d066c4140b4c775eca4aea`  
		Last Modified: Tue, 14 Sep 2021 01:41:47 GMT  
		Size: 187.6 MB (187558832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f607aa2c9e130844ee0cc0e33520cc7df43ef7d50dd1e8880d6552b4ba14fa23`  
		Last Modified: Tue, 14 Sep 2021 02:24:46 GMT  
		Size: 28.0 MB (27962181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-tools-deps-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:37d253d8dda71571cc4584f260dbec35cd85bd3c80f19c32a000b6bbc251adbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.6 MB (347583900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:575aab0f53ffd2cecf0568f89f0a24be917da2edfc2fca656ac4958f56d7ba0a`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:44 GMT
ADD file:1d6e5f5349752ab5c5888d38637821d2943472188c06bd14ea2bdf7a676ea19b in / 
# Fri, 03 Sep 2021 00:40:44 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:33:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:33:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 04:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 10:45:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 10:45:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 10:45:01 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 10:45:01 GMT
ENV LANG=C.UTF-8
# Tue, 14 Sep 2021 01:59:04 GMT
ENV JAVA_VERSION=18-ea+14
# Tue, 14 Sep 2021 01:59:12 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/14/GPL/openjdk-18-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='6aee5779ac7488dbd6988658662ca683704ac98cee6b8dde8df3ddffac76142e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/14/GPL/openjdk-18-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='88a106afe903b8f5d552ceae108294d8b36cbc0656a744f84525ccae542c5029'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 14 Sep 2021 01:59:13 GMT
CMD ["jshell"]
# Tue, 14 Sep 2021 02:39:57 GMT
ENV CLOJURE_VERSION=1.10.3.967
# Tue, 14 Sep 2021 02:39:57 GMT
WORKDIR /tmp
# Tue, 14 Sep 2021 02:40:07 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d1fba0cd0733b7cb66e47620845ecedfd757a9bf84e8b276fdb37ed9c272d3ae *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Tue, 14 Sep 2021 02:40:08 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:e3c1991bf0816d8624d8191a43732b869478319ed39c5f218e5878ed1ee05d58`  
		Last Modified: Fri, 03 Sep 2021 00:49:16 GMT  
		Size: 49.2 MB (49222144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529bf6c2a9fdb0edf93a87f6fbc959069a0068fe2ed046af546fca48e8ed6ffe`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 7.7 MB (7695770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9703bfb802a7157134df39897b2625906f8057c03e52daa3e8298ca41dfd7b`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 10.0 MB (9984267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a64745ecb3a1d83570e6c503995c0eb3f97176e23bd91210bf235e5646a4e96`  
		Last Modified: Fri, 03 Sep 2021 04:42:38 GMT  
		Size: 52.2 MB (52167858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a619afbd5fbf8751bdfe501f2c76be064cd35c66bc77c681698f60417a131a`  
		Last Modified: Fri, 03 Sep 2021 11:05:51 GMT  
		Size: 14.7 MB (14673457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e8c1323638d2f6705a6849427671a35427d900a540166991096421996a880f`  
		Last Modified: Tue, 14 Sep 2021 02:15:11 GMT  
		Size: 186.3 MB (186297602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c013b605a039c87b927263427ad27d19c2331ced6546bc3fc2a163d8c75307`  
		Last Modified: Tue, 14 Sep 2021 02:52:28 GMT  
		Size: 27.5 MB (27542802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
