## `clojure:openjdk-8-tools-deps-1.11.1.1105-buster`

```console
$ docker pull clojure@sha256:853946158e392d0e9381adfc2bf0971aa1b6ee6b167f8cf700f77abe026e5c10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-8-tools-deps-1.11.1.1105-buster` - linux; amd64

```console
$ docker pull clojure@sha256:1d57794d9c0f944baf1720a953f4f1d0dcee6f37d25f05c42d77a4c2a69d83a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.1 MB (263138119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d57bfcb62bc4afe69b3e319f6cf4ed1840cb567a4dd9ffaa56ad8f70bdc75a8`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:37 GMT
ADD file:7c5789fb822bda2652d7addee832c5a3d71733f0f94f97d89b0c5570c0840829 in / 
# Wed, 20 Apr 2022 04:43:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:59:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:59:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:53:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:55:31 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 20 Apr 2022 10:55:31 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 20 Apr 2022 10:55:32 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:55:32 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 10:55:32 GMT
ENV JAVA_VERSION=8u322
# Wed, 20 Apr 2022 10:55:39 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 21 Apr 2022 00:25:54 GMT
ENV CLOJURE_VERSION=1.11.1.1105
# Thu, 21 Apr 2022 00:25:54 GMT
WORKDIR /tmp
# Thu, 21 Apr 2022 00:26:04 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "5655c3ee3ea495d0778d8a87ce05a719045d3ceae9dd5cc29033379d8f82cce5 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Thu, 21 Apr 2022 00:26:04 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 21 Apr 2022 00:26:04 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:85bed84afb9a834cf090b55d2e584abd55b4792d93b750db896f486680638344`  
		Last Modified: Wed, 20 Apr 2022 04:48:49 GMT  
		Size: 50.4 MB (50436985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdd409f4b2bf3771fac1cbc2df46d1cbb4b800b154cfc33e8e0cd23e67ab3e0`  
		Last Modified: Wed, 20 Apr 2022 07:06:56 GMT  
		Size: 7.9 MB (7856378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3069e6cecf9d5e43ace0a925b53849b2fd189ef41883d45d8f2e12213c2c06`  
		Last Modified: Wed, 20 Apr 2022 07:06:56 GMT  
		Size: 10.0 MB (9997231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee16f45eff97cbe98b74c63ca2375b2c6b2592cd765a86df098f731baab13ad`  
		Last Modified: Wed, 20 Apr 2022 07:07:14 GMT  
		Size: 51.8 MB (51843794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb306096a59de5bf0aef0ab0d3cc05698b50be3d514995ac917f1a6f448a4b6`  
		Last Modified: Wed, 20 Apr 2022 11:10:46 GMT  
		Size: 5.3 MB (5286776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96745a3c7987bb43905d9d2cf7e43231a7313ea9dcd9961d840028775cacfbcd`  
		Last Modified: Wed, 20 Apr 2022 11:15:08 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6242ca9b4df79b46503a35467aaede738b67c2e424174b2905e41fc3aef6dbe`  
		Last Modified: Wed, 20 Apr 2022 11:15:17 GMT  
		Size: 106.1 MB (106078823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815b415bd7dc5e822bbbd793fb36d7507d89dadd9d9f6bc9e7aceb725cee405`  
		Last Modified: Thu, 21 Apr 2022 00:48:50 GMT  
		Size: 31.6 MB (31637299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104ae35523e57ba8fc1c2f0e3a1314f823bb791af57eaa0a14c7d7fd46d8fb36`  
		Last Modified: Thu, 21 Apr 2022 00:48:47 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-8-tools-deps-1.11.1.1105-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:cf7503f5f1a4e6fe6b4271357ff1f438168abb166c7dd490951f38e0444a7978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.2 MB (260239118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4b8cfdaae6c699634a857e65a5dc9312a9a31aa6eb2221d11ee90830f22a949`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:22 GMT
ADD file:5286ff5db23c42ac6a437e8f2f9ef01b6ee6e523d7866c752428d54f177c7108 in / 
# Wed, 20 Apr 2022 04:29:22 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:45:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:45:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:45:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:32:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:35:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 20 Apr 2022 10:35:44 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 20 Apr 2022 10:35:44 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:35:45 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 10:35:46 GMT
ENV JAVA_VERSION=8u322
# Wed, 20 Apr 2022 10:35:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 21 Apr 2022 03:16:33 GMT
ENV CLOJURE_VERSION=1.11.1.1105
# Thu, 21 Apr 2022 03:16:34 GMT
WORKDIR /tmp
# Thu, 21 Apr 2022 03:16:46 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "5655c3ee3ea495d0778d8a87ce05a719045d3ceae9dd5cc29033379d8f82cce5 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Thu, 21 Apr 2022 03:16:47 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 21 Apr 2022 03:16:47 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:b9f330b3a7e234282d632d95bd19a655cf0e06c1a76a51d0f73b9581be8f851b`  
		Last Modified: Wed, 20 Apr 2022 04:36:12 GMT  
		Size: 49.2 MB (49227738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80651adb7e52d8ecd27d43b9e69ada9ca277071ea09607121d0076de36480b`  
		Last Modified: Wed, 20 Apr 2022 06:55:25 GMT  
		Size: 7.7 MB (7719745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b38ee622cbfb492ebc3bc598771624fba7ef1830b4e0f9737f2bbf4b6ec0ea`  
		Last Modified: Wed, 20 Apr 2022 06:55:26 GMT  
		Size: 9.8 MB (9767312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc937997baec7d2d040aba23614db074862008cbdd69b46d2baea31711d58a50`  
		Last Modified: Wed, 20 Apr 2022 06:55:45 GMT  
		Size: 52.2 MB (52174549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfcf11011f81821ca2193af2525f74f1d1fdb46b7e04cc5a661f48736a667ab`  
		Last Modified: Wed, 20 Apr 2022 10:56:36 GMT  
		Size: 5.3 MB (5277105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8bada2c3565a2a793d604df08ae9222a93ad646626487a2035d3ddc0099566`  
		Last Modified: Wed, 20 Apr 2022 11:01:19 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e813a999baedaa9476c47fcc2890d75602e6b3de3372a4388b521317f1b25f32`  
		Last Modified: Wed, 20 Apr 2022 11:01:29 GMT  
		Size: 105.1 MB (105092325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cfa8c16a0ec48df823a14c85f853ffee6e1eeac8bdfd9c8ec5ccddfcd9b219`  
		Last Modified: Thu, 21 Apr 2022 03:45:05 GMT  
		Size: 31.0 MB (30979513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f69368a7b1269aacedbe654713a532b62e7c21c43acd3bde2781bdea466cb5d`  
		Last Modified: Thu, 21 Apr 2022 03:45:02 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
