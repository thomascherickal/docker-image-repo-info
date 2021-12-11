## `clojure:openjdk-18`

```console
$ docker pull clojure@sha256:d9db361062e7e9c77536cee1e1b089b74c692b7520aa379755d91901613db12f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18` - linux; amd64

```console
$ docker pull clojure@sha256:f4eb66f8afe8b7392833f5c5bf61cf9a80b6402a1a21fe2f9fce2ee9050f18ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.7 MB (278692014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5b60ed228a1353da414f999cd383698b232230aba412a6df6b250f206ff8c42`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:29:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:29:26 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 02 Dec 2021 11:29:27 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:29:27 GMT
ENV LANG=C.UTF-8
# Fri, 10 Dec 2021 21:20:50 GMT
ENV JAVA_VERSION=18-ea+27
# Fri, 10 Dec 2021 21:21:04 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='625301c146fd49d5f45dae30876079fe01ee959d84573a056426362fd6699f1f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad926dc5db48de8dce170eb97ed1539d03829b3f23cf4a2a654e0f8f296be8e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Dec 2021 21:21:05 GMT
CMD ["jshell"]
# Fri, 10 Dec 2021 22:08:16 GMT
ENV CLOJURE_VERSION=1.10.3.1040
# Fri, 10 Dec 2021 22:08:16 GMT
WORKDIR /tmp
# Fri, 10 Dec 2021 22:08:35 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "665e35e8d7dd0996edaba36220fd5048fee95f5155ec0426f628f18770239821 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 10 Dec 2021 22:08:35 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 10 Dec 2021 22:08:35 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 10 Dec 2021 22:08:36 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 10 Dec 2021 22:08:36 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9f5b9b70c2f137dc70e816256e7a568a084d066e7c34c028d30a6a45438685`  
		Last Modified: Thu, 02 Dec 2021 11:47:20 GMT  
		Size: 1.6 MB (1582045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914d992ea9c97748987f48cb0e1026e4ce7292949adee632e14e3943eba20b59`  
		Last Modified: Fri, 10 Dec 2021 21:28:43 GMT  
		Size: 189.0 MB (188954488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e0c47617130e2a32cd9d1eb446589e883e6076a464bac6377ac94635fe6233`  
		Last Modified: Fri, 10 Dec 2021 22:15:15 GMT  
		Size: 56.8 MB (56784235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d68f751746c2255282471be3147b4c7f13bf0f4514a1e93c6fb9cc04edb55be`  
		Last Modified: Fri, 10 Dec 2021 22:15:07 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9831a99ba3f7dd9eb98a5f6ed55fb4997dda869741c06e000a9e16554ce2a0`  
		Last Modified: Fri, 10 Dec 2021 22:15:07 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4747da3d6f370aa4646bad4d53b3a2b8f9f188abe62a2a8a0726bf645dd52906
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.8 MB (275789935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a84fa170ce1b94b0d00d4e662604401b0d3480e0181c3009c784fb1e87ed08`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:09 GMT
ADD file:002f2f7c6dc806b24b6c365882acd59d2b3d3fcec46d8fd99130b07a4575c88c in / 
# Thu, 02 Dec 2021 08:08:10 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:02:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 02 Dec 2021 11:02:15 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:02:16 GMT
ENV LANG=C.UTF-8
# Fri, 10 Dec 2021 21:53:01 GMT
ENV JAVA_VERSION=18-ea+27
# Fri, 10 Dec 2021 21:53:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='625301c146fd49d5f45dae30876079fe01ee959d84573a056426362fd6699f1f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad926dc5db48de8dce170eb97ed1539d03829b3f23cf4a2a654e0f8f296be8e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Dec 2021 21:53:16 GMT
CMD ["jshell"]
# Fri, 10 Dec 2021 23:20:18 GMT
ENV CLOJURE_VERSION=1.10.3.1040
# Fri, 10 Dec 2021 23:20:19 GMT
WORKDIR /tmp
# Fri, 10 Dec 2021 23:20:35 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "665e35e8d7dd0996edaba36220fd5048fee95f5155ec0426f628f18770239821 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 10 Dec 2021 23:20:36 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 10 Dec 2021 23:20:37 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 10 Dec 2021 23:20:37 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 10 Dec 2021 23:20:38 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:968621624b326084ed82349252b333e649eaab39f71866edb2b9a4f847283680`  
		Last Modified: Thu, 02 Dec 2021 08:40:45 GMT  
		Size: 30.1 MB (30056536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595058421fcb005f80f2faa2434369885cb20645caed265e7b4912808701d893`  
		Last Modified: Thu, 02 Dec 2021 11:23:15 GMT  
		Size: 1.4 MB (1361242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a57cc5bed1d3dbd9c4820e9443e6073354fa12f2044252e017748472cad145`  
		Last Modified: Fri, 10 Dec 2021 22:06:07 GMT  
		Size: 187.7 MB (187661018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6982c3cc72371e9caaa6ce143d62327404a8def55c2b333c98d636c7097084`  
		Last Modified: Fri, 10 Dec 2021 23:30:38 GMT  
		Size: 56.7 MB (56710110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b799152bfcbb0353ba0f23806e5af4dd7c1324edd9278071db6c7924c12818ac`  
		Last Modified: Fri, 10 Dec 2021 23:30:29 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e38caa82f73dc3af6ef40b53205b1a2786067d5b3b4e619a4fe2b6f371fca51`  
		Last Modified: Fri, 10 Dec 2021 23:30:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
