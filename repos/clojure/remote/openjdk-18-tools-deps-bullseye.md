## `clojure:openjdk-18-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:cfb6d46131695f1f4dbf3fedd61501c565602eb196e69ccfcd4f92124a0e9ccc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:159decfcb436ad8c81eafb4484af5caf233b2301cc9d539da5452df6c2e5c24f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.2 MB (347153183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2938524aecb84dd3e3c97f8ba9545c02718000b5e85ad9033e233f10a8db2745`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:07 GMT
ADD file:1fedf68870782f1b44cd50691444aab4061cc0c70f24e5fabe9c562cc46eb9af in / 
# Fri, 03 Sep 2021 01:21:08 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:31:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:31:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:30:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:30:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 08:30:45 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:30:46 GMT
ENV LANG=C.UTF-8
# Sat, 25 Sep 2021 00:25:26 GMT
ENV JAVA_VERSION=18-ea+16
# Sat, 25 Sep 2021 00:25:36 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-x64_bin.tar.gz'; 			downloadSha256='ec604f7aef23624c0acdc0db346a2b226aab47d120538833070f0d5e01d571c1'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-aarch64_bin.tar.gz'; 			downloadSha256='623eff3e61bd5f74442fb5699ac3dea167dbe0ade7dd6c1fa9cdd4788e316b96'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 25 Sep 2021 00:25:37 GMT
CMD ["jshell"]
# Sat, 25 Sep 2021 01:23:20 GMT
ENV CLOJURE_VERSION=1.10.3.967
# Sat, 25 Sep 2021 01:23:20 GMT
WORKDIR /tmp
# Sat, 25 Sep 2021 01:23:28 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d1fba0cd0733b7cb66e47620845ecedfd757a9bf84e8b276fdb37ed9c272d3ae *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Sat, 25 Sep 2021 01:23:28 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:955615a668ce169f8a1443fc6b6e6215f43fe0babfb4790712a2d3171f34d366`  
		Last Modified: Fri, 03 Sep 2021 01:26:55 GMT  
		Size: 54.9 MB (54926871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2756ef5f69a5190f4308619e0f446d95f5515eef4a814dbad0bcebbbbc7b25a8`  
		Last Modified: Fri, 03 Sep 2021 06:39:22 GMT  
		Size: 5.2 MB (5153100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ea9f2bd51e53a455297e0631e18a72a86d7e2c8e1807176e80f991bde5d64`  
		Last Modified: Fri, 03 Sep 2021 06:39:23 GMT  
		Size: 10.9 MB (10871687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b0a22ee906271a6ce9ddd1754fdd7d3b59078e0b57b6cc054c7ed7ac301587`  
		Last Modified: Fri, 03 Sep 2021 06:39:45 GMT  
		Size: 54.6 MB (54566834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b79c82cab03ddf5fc88cf1ab0550217980b866ec12c52b0f16751bc45be87b6`  
		Last Modified: Fri, 03 Sep 2021 08:48:24 GMT  
		Size: 14.1 MB (14071678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1620dd942ab67022c59fcad08da73f8cbb04a9fa541518f3bb640c9dea235db`  
		Last Modified: Sat, 25 Sep 2021 00:33:56 GMT  
		Size: 188.0 MB (188011359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba30053cc0f7193bf2be5091511e7f9bffc311d9bb903c2c3e8d6e72f6666ab`  
		Last Modified: Sat, 25 Sep 2021 01:29:32 GMT  
		Size: 19.6 MB (19551654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:906a3c8699fb138ac0d1f133cc14937ed7a8fd64b5a040a39a73e90b00a99221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.1 MB (346122353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d300f0588c6de2fd211cbee0f7cb6dc3b26dcc011291958ecb73ca5e291129c`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:42:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:42:28 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 28 Sep 2021 05:42:28 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 05:42:29 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 05:42:29 GMT
ENV JAVA_VERSION=18-ea+16
# Tue, 28 Sep 2021 05:42:38 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-x64_bin.tar.gz'; 			downloadSha256='ec604f7aef23624c0acdc0db346a2b226aab47d120538833070f0d5e01d571c1'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-aarch64_bin.tar.gz'; 			downloadSha256='623eff3e61bd5f74442fb5699ac3dea167dbe0ade7dd6c1fa9cdd4788e316b96'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 05:42:38 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 02:33:34 GMT
ENV CLOJURE_VERSION=1.10.3.967
# Wed, 29 Sep 2021 02:33:35 GMT
WORKDIR /tmp
# Wed, 29 Sep 2021 02:33:42 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d1fba0cd0733b7cb66e47620845ecedfd757a9bf84e8b276fdb37ed9c272d3ae *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Wed, 29 Sep 2021 02:33:42 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7e4e85949ee45bae139f288bc1cd85a740b408abdefaaba118c4c4626b021e`  
		Last Modified: Tue, 28 Sep 2021 02:25:03 GMT  
		Size: 54.7 MB (54669786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba15136352425849a216be8c1ff09f76b7a873137b588e6be2e479ea909d966`  
		Last Modified: Tue, 28 Sep 2021 06:03:44 GMT  
		Size: 15.5 MB (15526494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37951340411e5e76fe94aef77a70780da9202848a9f312b8a0dee88fd8355027`  
		Last Modified: Tue, 28 Sep 2021 06:03:59 GMT  
		Size: 186.7 MB (186743718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6723fecd6f06634e6a2d01a057f8420fc728c2e3a1d4755fb379b5e81e51c418`  
		Last Modified: Wed, 29 Sep 2021 02:58:03 GMT  
		Size: 19.6 MB (19553262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
