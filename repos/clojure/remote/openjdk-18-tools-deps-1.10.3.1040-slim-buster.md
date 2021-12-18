## `clojure:openjdk-18-tools-deps-1.10.3.1040-slim-buster`

```console
$ docker pull clojure@sha256:563f224116da3f1fe1d0ae45890c5895a712b6400a25a8bcfaa947e5368c3598
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-tools-deps-1.10.3.1040-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:3ef1c826ae7e87c17c4ec75b10418c7bcb8fb48e4eb54847c5926ae9d861df47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.9 MB (277875799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a1a724428021db5d17ba6ccfb5d3835a4b10b358950e2150ac71e456b1af61`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:30:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:30:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 02 Dec 2021 11:30:51 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:30:51 GMT
ENV LANG=C.UTF-8
# Sat, 18 Dec 2021 04:11:52 GMT
ENV JAVA_VERSION=18-ea+28
# Sat, 18 Dec 2021 04:12:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='7e5f0e54c799f8c155a934e61d88f4fef3a70a641c1636c925158622c7bd9341'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='e29aa39763ebcfe5f037cc4fe47c6b9eb34cbe482f6ea57e93de89070255e22b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 18 Dec 2021 04:12:07 GMT
CMD ["jshell"]
# Sat, 18 Dec 2021 06:51:48 GMT
ENV CLOJURE_VERSION=1.10.3.1040
# Sat, 18 Dec 2021 06:51:48 GMT
WORKDIR /tmp
# Sat, 18 Dec 2021 06:52:10 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "665e35e8d7dd0996edaba36220fd5048fee95f5155ec0426f628f18770239821 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 18 Dec 2021 06:52:11 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Sat, 18 Dec 2021 06:52:11 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Sat, 18 Dec 2021 06:52:11 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 18 Dec 2021 06:52:12 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169731f46e61fb8aef8f7ed809068db98d3feb2466197e9680dbbdbb80d8ed90`  
		Last Modified: Thu, 02 Dec 2021 11:48:59 GMT  
		Size: 3.3 MB (3269625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fcca4b8a0d7e8f5eaa98fdcf97f0e34def478e6fd8229f64a3ea47c7b8caf7`  
		Last Modified: Sat, 18 Dec 2021 04:25:43 GMT  
		Size: 189.0 MB (189011855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a2daecb1a2b8303b9097c576eed35c875bb26ba23184fe08a743ea9ac0b043`  
		Last Modified: Sat, 18 Dec 2021 06:59:39 GMT  
		Size: 58.4 MB (58439559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b07e0d5873ca277880d650c06d48491cc5612dc82d5eebb2fb24cf4c5ab5e6`  
		Last Modified: Sat, 18 Dec 2021 06:59:30 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce590a5f308f0839679589f52876937d721da83d01d74fa3fbc499f43e03cab`  
		Last Modified: Sat, 18 Dec 2021 06:59:30 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-tools-deps-1.10.3.1040-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2af1bd43fd86ab458284299f579c1bfa68a1998e7da47a4c7a44aadbfa608c76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.9 MB (274870694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ad897cc96a3512df435c4ebd20502b87452ddfdebb7fbb1bffe5813910c1bc`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:03:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:03:23 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 02 Dec 2021 11:03:24 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:03:25 GMT
ENV LANG=C.UTF-8
# Fri, 17 Dec 2021 23:45:06 GMT
ENV JAVA_VERSION=18-ea+28
# Fri, 17 Dec 2021 23:45:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='7e5f0e54c799f8c155a934e61d88f4fef3a70a641c1636c925158622c7bd9341'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='e29aa39763ebcfe5f037cc4fe47c6b9eb34cbe482f6ea57e93de89070255e22b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 17 Dec 2021 23:45:20 GMT
CMD ["jshell"]
# Sat, 18 Dec 2021 00:31:54 GMT
ENV CLOJURE_VERSION=1.10.3.1040
# Sat, 18 Dec 2021 00:31:55 GMT
WORKDIR /tmp
# Sat, 18 Dec 2021 00:32:13 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "665e35e8d7dd0996edaba36220fd5048fee95f5155ec0426f628f18770239821 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 18 Dec 2021 00:32:15 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Sat, 18 Dec 2021 00:32:16 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Sat, 18 Dec 2021 00:32:16 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 18 Dec 2021 00:32:17 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7c7f43e0be8e395071a65cf4a7b754dc421cf18e5de6bde1fab5e7376f8d28`  
		Last Modified: Thu, 02 Dec 2021 11:24:55 GMT  
		Size: 3.1 MB (3118874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edef99cacc4b0a23fd5f6b9fddbd12345d270199685bb97304918f0f7f3b6ff`  
		Last Modified: Sat, 18 Dec 2021 00:05:13 GMT  
		Size: 187.7 MB (187740634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecb5bd1f54de471c37c242f852fdd58e00408a68bbae80f6f5c85c7dd9eb9f5`  
		Last Modified: Sat, 18 Dec 2021 00:43:25 GMT  
		Size: 58.1 MB (58087017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd529a2375f6c7be3033b4d1f5c1a9e2fa6e1e7c8e592df8728577747b0ae9b`  
		Last Modified: Sat, 18 Dec 2021 00:43:17 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb6f6110a8ce69cf0ee3fcbe9aebc192b320e6f80f46da7b47d91a145a4303f`  
		Last Modified: Sat, 18 Dec 2021 00:43:17 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
