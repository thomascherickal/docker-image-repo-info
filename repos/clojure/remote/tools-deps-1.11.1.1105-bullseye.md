## `clojure:tools-deps-1.11.1.1105-bullseye`

```console
$ docker pull clojure@sha256:68785cf0d06c251b03724c7147e828f234995c71669f6181e9411cc3135c7751
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:tools-deps-1.11.1.1105-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:e87385aa320161e710a5f2b842f5f174934ee48a11440ed9991a72ea4e43326f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.5 MB (350484316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ae4bab8a24a3b0b3370b7824bad72fc083e8d7bb21d81329eb4122a36d40f2`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:15 GMT
ADD file:3a81c181c66f226bd6abd48d0c7ed8a9c599c9f521ec7229286c83161afec8c2 in / 
# Wed, 20 Apr 2022 04:43:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:57:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:57:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:58:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:47:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:50:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 20 Apr 2022 10:50:50 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:50:50 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 10:50:50 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 20 Apr 2022 10:51:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 20 Apr 2022 10:51:02 GMT
CMD ["jshell"]
# Thu, 21 Apr 2022 00:40:04 GMT
ENV CLOJURE_VERSION=1.11.1.1105
# Thu, 21 Apr 2022 00:40:04 GMT
WORKDIR /tmp
# Thu, 21 Apr 2022 00:40:11 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "5655c3ee3ea495d0778d8a87ce05a719045d3ceae9dd5cc29033379d8f82cce5 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Thu, 21 Apr 2022 00:40:11 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 21 Apr 2022 00:40:11 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 21 Apr 2022 00:40:12 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 21 Apr 2022 00:40:12 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:6aefca2dc61dcbcd268b8a9861e552f9cdb69e57242faec64ac120d2355a9c1a`  
		Last Modified: Wed, 20 Apr 2022 04:47:57 GMT  
		Size: 54.9 MB (54941777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967757d5652770cfa81b6cc7577d65e06d336173da116d1fb5b2d349d5d44127`  
		Last Modified: Wed, 20 Apr 2022 07:05:43 GMT  
		Size: 5.2 MB (5155716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c357e2c68cb3bf1e98dcb3eb6ceb16837253db71535921d6993c594588bffe04`  
		Last Modified: Wed, 20 Apr 2022 07:05:45 GMT  
		Size: 10.9 MB (10874928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c766e27afb21eddf9ab3e4349700ebe697c32a4c6ada6af4f08282277a291a28`  
		Last Modified: Wed, 20 Apr 2022 07:06:05 GMT  
		Size: 54.6 MB (54578663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e454664a629c8e4cac99685ba1b624982040c45466f197f649234a8e132803`  
		Last Modified: Wed, 20 Apr 2022 11:00:48 GMT  
		Size: 14.1 MB (14071513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303943476b6f5143642c36b70f95ce88a30634496fdbf41b8f5c5deaf16b48f7`  
		Last Modified: Wed, 20 Apr 2022 11:05:54 GMT  
		Size: 187.6 MB (187628474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882269d0662cd23b11099bdce82c34fbd46658c5614a86f861de53987dcd84f3`  
		Last Modified: Thu, 21 Apr 2022 00:59:53 GMT  
		Size: 23.2 MB (23232214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eacfbce2d88cb2c692cefcefaa0a96e2d177b5e4b4d5b1c8aa85a9dc684112f`  
		Last Modified: Thu, 21 Apr 2022 00:59:51 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a87f7274868cab1102e42dd75359da2db4e08267f1e7a35b5933540169e0e69`  
		Last Modified: Thu, 21 Apr 2022 00:59:51 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:tools-deps-1.11.1.1105-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2dfe59a8e36fe8be9c20451465711c519d4314e88d8b3dcc25d4311eaa2cc88d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.9 MB (348894335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306ab1c6c130482e6ee09180d38d2b13c8026ef6df7fc8bb99b3b358de6bfc3`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:28:55 GMT
ADD file:ece192802cbdaf1a141d04f0c2e90cfd3479e5e3e82c6a00206970684494cf48 in / 
# Wed, 20 Apr 2022 04:28:56 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:44:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:28:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 20 Apr 2022 10:28:21 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:28:22 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 10:28:23 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 20 Apr 2022 10:28:39 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 20 Apr 2022 10:28:40 GMT
CMD ["jshell"]
# Thu, 21 Apr 2022 03:32:38 GMT
ENV CLOJURE_VERSION=1.11.1.1105
# Thu, 21 Apr 2022 03:32:39 GMT
WORKDIR /tmp
# Thu, 21 Apr 2022 03:32:47 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "5655c3ee3ea495d0778d8a87ce05a719045d3ceae9dd5cc29033379d8f82cce5 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Thu, 21 Apr 2022 03:32:48 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 21 Apr 2022 03:32:49 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 21 Apr 2022 03:32:49 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 21 Apr 2022 03:32:50 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:83d5dcfea08e6927083bc886bf182fc39d87bb04b54b63002ac0c4c0b9aab682`  
		Last Modified: Wed, 20 Apr 2022 04:35:19 GMT  
		Size: 53.6 MB (53633096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfa86b7b1aca6d694057e4d42ee1440527f41c00b9e577df729244380c9eba`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 4.9 MB (4938663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79b19335f27cc78840bf9159e875322f3252ac06113c73756f9d4fba905f9b`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 10.7 MB (10656971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350ecaf08eac09037b05465ab97a1b8f7bc9b7a9b1fcef900dedd7dba9bbcf4d`  
		Last Modified: Wed, 20 Apr 2022 06:54:32 GMT  
		Size: 54.7 MB (54672934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b174d41b9ea1124e2245788f2c290f940eca707dcc0446cd302b01aaeb5c82`  
		Last Modified: Wed, 20 Apr 2022 10:45:28 GMT  
		Size: 15.5 MB (15525740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcad0d6cbc9566a9060cce10d4afebc73de9f59e90ed2ba2e9fe4e6767013600`  
		Last Modified: Wed, 20 Apr 2022 10:51:07 GMT  
		Size: 186.5 MB (186472881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c82d1a9db52605769a73f5809b71502e312a5444ee22c2b08218630aea22c6`  
		Last Modified: Thu, 21 Apr 2022 03:57:49 GMT  
		Size: 23.0 MB (22993024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5af15fc36f9c1884a2a1c841fcac48a3971d3796444d10fbcf7052ec899fb5a`  
		Last Modified: Thu, 21 Apr 2022 03:57:46 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab898845ca7360c2a01c97c9bd20e21b8fd368fc918c160a276a8a848aa1c02`  
		Last Modified: Thu, 21 Apr 2022 03:57:46 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
