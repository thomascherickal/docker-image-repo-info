## `clojure:openjdk-8-tools-deps-1.10.3.967-buster`

```console
$ docker pull clojure@sha256:5f1cb35ad59e23738e41b5f7de4c47841d97a31723e91179e01253ec31511f6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-8-tools-deps-1.10.3.967-buster` - linux; amd64

```console
$ docker pull clojure@sha256:1ce3e97d4688c8b87e4cdf972555a87ac189bad05ab6761499b6f60b8fa4f263
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.3 MB (259346606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ddf907250d91bae1f509fb3ccce995b3e143c1a953922150854c643abf22756`
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
# Fri, 03 Sep 2021 08:38:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:41:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 03 Sep 2021 08:41:52 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 03 Sep 2021 08:41:52 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:41:52 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:41:53 GMT
ENV JAVA_VERSION=8u302
# Fri, 03 Sep 2021 08:41:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 09 Sep 2021 19:21:21 GMT
ENV CLOJURE_VERSION=1.10.3.967
# Thu, 09 Sep 2021 19:21:21 GMT
WORKDIR /tmp
# Thu, 09 Sep 2021 19:21:33 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d1fba0cd0733b7cb66e47620845ecedfd757a9bf84e8b276fdb37ed9c272d3ae *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Thu, 09 Sep 2021 19:21:33 GMT
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
	-	`sha256:9ffbb70985069a18b6cb99f75ac2e6b3210b011fdd55f60dfa98ca3389d566c7`  
		Last Modified: Fri, 03 Sep 2021 08:59:03 GMT  
		Size: 5.3 MB (5286452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc339866e15682e2b6469e399f0ac4dc764f7affe5027f7ab6793e93863800b7`  
		Last Modified: Fri, 03 Sep 2021 09:06:25 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68bf95a3f96b7f824f6571aa054358b628fba5a2df2ff91cd8522a309f53989`  
		Last Modified: Fri, 03 Sep 2021 09:06:38 GMT  
		Size: 106.0 MB (105992983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2150e87e5777edc063878389a42a726650185c3366ef5cb6c8f1b65322141897`  
		Last Modified: Thu, 09 Sep 2021 19:39:06 GMT  
		Size: 28.0 MB (27959247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
