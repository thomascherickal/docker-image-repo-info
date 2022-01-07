## `clojure:openjdk-17-tools-deps-1.10.3.1058-slim-buster`

```console
$ docker pull clojure@sha256:9bd5b197c6dbb1b31fd9d3639519be53822029acee3231e0842fc6011fa33a19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-tools-deps-1.10.3.1058-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:8bd117ff6ea7acce224b68468b54262caf419cdb964d60b4b80974304cfd7563
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.2 MB (279190204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e08414a02f022e3653c72aaec63c6f16f84aee787440369bfa3ff6992189aa3`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 22:58:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:01:28 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 21 Dec 2021 23:01:29 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:01:29 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:01:29 GMT
ENV JAVA_VERSION=17.0.1
# Tue, 21 Dec 2021 23:01:45 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='1c0a73cbb863aad579b967316bf17673b8f98a9bb938602a140ba2e5c38f880a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='86653d48787e5a1c029df10da7808194fe8bd931ddd72ff3d42850bf1afb317e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 21 Dec 2021 23:01:46 GMT
CMD ["jshell"]
# Fri, 07 Jan 2022 20:22:09 GMT
ENV CLOJURE_VERSION=1.10.3.1058
# Fri, 07 Jan 2022 20:22:09 GMT
WORKDIR /tmp
# Fri, 07 Jan 2022 20:22:27 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "980168025a3827bd7ed9d5ab1681ce29808ac8e6cbced3ab6683db8b365b54df *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 07 Jan 2022 20:22:28 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 07 Jan 2022 20:22:28 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 07 Jan 2022 20:22:28 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 07 Jan 2022 20:22:28 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c983bcc370920d99695dc288c345343be841987206e4ce762a4e7599f28c96`  
		Last Modified: Tue, 21 Dec 2021 23:16:09 GMT  
		Size: 3.3 MB (3269567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2dd1934c7e37cb0dd1aa7edb2a85416feeb6ef8fb75c26de2a963b9e5c1efd`  
		Last Modified: Tue, 21 Dec 2021 23:22:31 GMT  
		Size: 187.5 MB (187548485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bceafea1a936e81b0c8d4abea064513856ac144e93efaea09745156c1ef3de73`  
		Last Modified: Fri, 07 Jan 2022 20:31:04 GMT  
		Size: 61.2 MB (61217396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965eca3468cfc1b345e6b75cc7aed3d799a80e12afbe527ac814cf30936cd94e`  
		Last Modified: Fri, 07 Jan 2022 20:30:56 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514ebad98a27f287158989ec11ea3fc5a33c3e72d15bc79fa95130ee77520c77`  
		Last Modified: Fri, 07 Jan 2022 20:30:56 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-tools-deps-1.10.3.1058-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:3a7534c780a9df4f3fd87ee8ac75459b5f1180cdc17cf4762b4b03ac766aee6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.1 MB (276056307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b31f7a9f1dbb342a64068f36b62e56b6c451456a1fd69fa78c1880cf9e968b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:54:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:58:53 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 21 Dec 2021 02:58:54 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:58:55 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 02:58:56 GMT
ENV JAVA_VERSION=17.0.1
# Tue, 21 Dec 2021 02:59:11 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='1c0a73cbb863aad579b967316bf17673b8f98a9bb938602a140ba2e5c38f880a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='86653d48787e5a1c029df10da7808194fe8bd931ddd72ff3d42850bf1afb317e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 21 Dec 2021 02:59:11 GMT
CMD ["jshell"]
# Fri, 07 Jan 2022 20:43:03 GMT
ENV CLOJURE_VERSION=1.10.3.1058
# Fri, 07 Jan 2022 20:43:03 GMT
WORKDIR /tmp
# Fri, 07 Jan 2022 20:43:26 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "980168025a3827bd7ed9d5ab1681ce29808ac8e6cbced3ab6683db8b365b54df *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 07 Jan 2022 20:43:27 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 07 Jan 2022 20:43:28 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 07 Jan 2022 20:43:28 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 07 Jan 2022 20:43:29 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c74145b5f237a66007b7c0d55f2ffe3d54c07bf5e09c19bebd4ec94b00005e`  
		Last Modified: Tue, 21 Dec 2021 03:17:41 GMT  
		Size: 3.1 MB (3118854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3f14d4fc26eea37b6d16d78a92f75e786a6efa868ec35267a831bfe148f318`  
		Last Modified: Tue, 21 Dec 2021 03:25:05 GMT  
		Size: 186.1 MB (186146523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcc309ed723ecacc5992069da88e70bb3623b1ee8021668dd034b73a90ee8fc`  
		Last Modified: Fri, 07 Jan 2022 20:56:34 GMT  
		Size: 60.9 MB (60866750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec0d615c55a44a4babcffc942c4d9e77ac055ecd52fa892e4ea8f92e6df4a4c`  
		Last Modified: Fri, 07 Jan 2022 20:56:25 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ffffafbdc6693d0c411290f9f8145a9570ca2c3c5b39e4d279385ff4c6456f`  
		Last Modified: Fri, 07 Jan 2022 20:56:25 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
