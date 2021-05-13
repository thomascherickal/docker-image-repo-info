## `clojure:openjdk-11-tools-deps-1.10.3.822`

```console
$ docker pull clojure@sha256:f9ffaf0e38f928c592186dae0fff03ccd7487b4a7abfc2f7032391e87159a8f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-11-tools-deps-1.10.3.822` - linux; amd64

```console
$ docker pull clojure@sha256:8625c4e2c8bf0e702508b9f900127a4de59be64415949e1087be8387074f692c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.3 MB (355348519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1616db1ed6362a9a4be81adf3ff0ca06976c1e5f5e344df1c56355b779daa057`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:49:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:49:53 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:49:56 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:49:56 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:49:56 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:49:57 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:50:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 12 May 2021 06:50:20 GMT
CMD ["jshell"]
# Thu, 13 May 2021 04:37:33 GMT
ENV CLOJURE_VERSION=1.10.3.822
# Thu, 13 May 2021 04:37:33 GMT
WORKDIR /tmp
# Thu, 13 May 2021 04:37:46 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ebc820fe0e74de4bd77e6d5bd7db4a262ec1902efdf4d0553309485afcd75abf *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Thu, 13 May 2021 04:37:46 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d943ee54c1fa196b54ab9a6673174c66eea04cfa1a4ac5b0328b74f066a4d9`  
		Last Modified: Wed, 12 May 2021 02:05:07 GMT  
		Size: 51.8 MB (51841468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da20b77f10accb6bbe77d0a222b481d7a083efa84c2cb9ee752723ad4fca2cf4`  
		Last Modified: Wed, 12 May 2021 07:01:49 GMT  
		Size: 5.3 MB (5286520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8669a096f083b397ec8949a2da592616f90bbd22bd612927db3becd457747829`  
		Last Modified: Wed, 12 May 2021 07:01:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c0a5e9ce88aa01049ae5788512abb561b34cf649940e8a87cb58f14919f603`  
		Last Modified: Wed, 12 May 2021 07:02:05 GMT  
		Size: 202.9 MB (202930541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f116864d6af34394a06af92a54b06dfa41cd8365e4f24639750bf9b765ee072`  
		Last Modified: Thu, 13 May 2021 04:48:04 GMT  
		Size: 27.0 MB (27026442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-11-tools-deps-1.10.3.822` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a648cbbb76f3c947a8a89b4477cc91f1724ce195c946e4f38d8d568465d85b65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351509402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be801d4deb185b056d727f98e1f22cc53cd6c7205e75d6312d501c9d059cfbb3`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Wed, 12 May 2021 00:50:48 GMT
ADD file:ff9983cd659b3fc32ddfbbdeda76a971afd7d399e6d8b98faea3a9ead0e598f6 in / 
# Wed, 12 May 2021 00:50:52 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:34:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:34:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:35:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:18:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:18:53 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:18:56 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:18:56 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:18:57 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:18:59 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:19:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 12 May 2021 06:19:22 GMT
CMD ["jshell"]
# Thu, 13 May 2021 03:28:02 GMT
ENV CLOJURE_VERSION=1.10.3.822
# Thu, 13 May 2021 03:28:03 GMT
WORKDIR /tmp
# Thu, 13 May 2021 03:28:31 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ebc820fe0e74de4bd77e6d5bd7db4a262ec1902efdf4d0553309485afcd75abf *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Thu, 13 May 2021 03:28:33 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:c54d9402d498e45ed396b5b6fe836f55e4ccadbad745decda3e9f83d880bc677`  
		Last Modified: Wed, 12 May 2021 01:01:40 GMT  
		Size: 49.2 MB (49225351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91bbb3592d6685d1c683c8c20e60901274c636605800608685274c194d43d25`  
		Last Modified: Wed, 12 May 2021 01:48:24 GMT  
		Size: 7.7 MB (7695057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d8c28b9129321858810cff4cd78385949579ed18d991f98c77f912c7a754f8`  
		Last Modified: Wed, 12 May 2021 01:48:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70b3803033bfb8e0c8ab31f286ca427ccb8a47b7c63ca8e6d05d23ff7231733`  
		Last Modified: Wed, 12 May 2021 01:48:46 GMT  
		Size: 52.2 MB (52168431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205569750a80f2b705a2e4a96ffd1c98adf60ff45ae6afe47a1ca7eff35ae18`  
		Last Modified: Wed, 12 May 2021 06:29:44 GMT  
		Size: 5.3 MB (5277765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13f11c70479156d92297a5856c057dd8d1bb534802c4830dffbf0d36c8ee2b6`  
		Last Modified: Wed, 12 May 2021 06:29:42 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165cdcf04178580d3e3812e5e49d7a002e6113958dfbbfee8ea0074fbe96bc35`  
		Last Modified: Wed, 12 May 2021 06:30:12 GMT  
		Size: 200.5 MB (200547647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf637f6a59492a9a30641e64a95791f4e811df53d5d8764a3081ea9be1a86f2b`  
		Last Modified: Thu, 13 May 2021 03:42:01 GMT  
		Size: 26.6 MB (26610596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
