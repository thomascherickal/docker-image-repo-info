## `clojure:openjdk-17-tools-deps-slim-buster`

```console
$ docker pull clojure@sha256:7bdf1f5a012616c8469b84075053f9fc5f3a138e106d8b5c39d2d6d42aecd61a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-tools-deps-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:295be475e724f923fe6acef1b2cf8006cbdbcd3b85b195c0f25e3b21c632db61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.0 MB (280012121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ed9aa515f6be59068c26d4b33d276cb86b1690e0b722e44c2552b732061fab`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:19:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:23:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 26 Jan 2022 09:23:26 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:23:26 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 09:23:26 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 26 Jan 2022 09:23:49 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 26 Jan 2022 09:23:50 GMT
CMD ["jshell"]
# Fri, 04 Feb 2022 23:47:53 GMT
ENV CLOJURE_VERSION=1.10.3.1075
# Fri, 04 Feb 2022 23:47:53 GMT
WORKDIR /tmp
# Fri, 04 Feb 2022 23:48:13 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a6b72c9b23d348a0636813c5f59db5dda622e3b8dbb86124cbb51e3aced714d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 04 Feb 2022 23:48:14 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 04 Feb 2022 23:48:14 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 04 Feb 2022 23:48:14 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 04 Feb 2022 23:48:14 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa8d0f5eb646a53df0b867301afa43404e868c540fdf170240578844dfd0d6b`  
		Last Modified: Wed, 26 Jan 2022 09:43:10 GMT  
		Size: 3.3 MB (3269688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d07d03188c552a4c15bcc14429261b35c5fd4e95dba902c71a53f1bbd2cc712`  
		Last Modified: Wed, 26 Jan 2022 09:50:20 GMT  
		Size: 187.9 MB (187902911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa297b4b7d76d4540be37bd8cbb1b2371552bc514157cc9130b7debcae85653`  
		Last Modified: Fri, 04 Feb 2022 23:58:36 GMT  
		Size: 61.7 MB (61684760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdf86da0c830901d30ec5323ed38a888953a137111bf139209d8115bc96ae34`  
		Last Modified: Fri, 04 Feb 2022 23:58:27 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a262b3502d75825641384dbded1230662699e4ceb2b0620572261be0a028c77`  
		Last Modified: Fri, 04 Feb 2022 23:58:27 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-tools-deps-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4609fab6e7bd0897fa5ae6146b722d199e40fa2bd695ddc26aad20a707957e7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.9 MB (276911514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba8ff01e85b99691dbfc6878c0fdc91d88fb699dde5697454dd7d395378addf9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:51:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:55:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 26 Jan 2022 05:55:20 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:55:21 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 05:55:22 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 26 Jan 2022 05:55:37 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 26 Jan 2022 05:55:37 GMT
CMD ["jshell"]
# Fri, 04 Feb 2022 21:43:40 GMT
ENV CLOJURE_VERSION=1.10.3.1075
# Fri, 04 Feb 2022 21:43:41 GMT
WORKDIR /tmp
# Fri, 04 Feb 2022 21:43:59 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a6b72c9b23d348a0636813c5f59db5dda622e3b8dbb86124cbb51e3aced714d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 04 Feb 2022 21:44:00 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 04 Feb 2022 21:44:01 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 04 Feb 2022 21:44:01 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 04 Feb 2022 21:44:02 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a5c9716b24a17043a5d8ede1303daffeaaa07ff0393fa14caed54f01154833`  
		Last Modified: Wed, 26 Jan 2022 06:14:50 GMT  
		Size: 3.1 MB (3118858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b86e80221a9595499456cf894d6f84552e44713f10bb036cdcc9dc9b97b739`  
		Last Modified: Wed, 26 Jan 2022 06:22:23 GMT  
		Size: 186.5 MB (186533335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b03f2ba45f2edcb19fc3659f48f8e79e61d1506e352aa32e42780612d8dcaa`  
		Last Modified: Fri, 04 Feb 2022 21:56:59 GMT  
		Size: 61.3 MB (61335073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16a59b1fa4fe780ba07cf02e62e9bf96ff22432983812d5707712a5584337fb`  
		Last Modified: Fri, 04 Feb 2022 21:56:50 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32c85728dbbda8b9d7382e5876c6f5338118d92693a36e5a62003e45e08e088`  
		Last Modified: Fri, 04 Feb 2022 21:56:50 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
