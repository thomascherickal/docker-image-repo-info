## `clojure:openjdk-18-tools-deps-1.10.3.967-slim-buster`

```console
$ docker pull clojure@sha256:00681f02d329011540abd09d9d3897bf1ee49755cb3bf5c08084ead735f341ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-tools-deps-1.10.3.967-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:f3c8a3830efc392d98c47b96cb433ae8b1c11b3ac0dca52a8a9f3ec128e8bddb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.1 MB (277121745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5520834af181da6f80437046b6724593fdb108d72a8f80e79e1697de8ae9db4f`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:32:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:32:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 08:32:42 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:32:42 GMT
ENV LANG=C.UTF-8
# Sat, 25 Sep 2021 00:26:15 GMT
ENV JAVA_VERSION=18-ea+16
# Sat, 25 Sep 2021 00:26:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-x64_bin.tar.gz'; 			downloadSha256='ec604f7aef23624c0acdc0db346a2b226aab47d120538833070f0d5e01d571c1'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-aarch64_bin.tar.gz'; 			downloadSha256='623eff3e61bd5f74442fb5699ac3dea167dbe0ade7dd6c1fa9cdd4788e316b96'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 25 Sep 2021 00:26:30 GMT
CMD ["jshell"]
# Sat, 25 Sep 2021 01:19:01 GMT
ENV CLOJURE_VERSION=1.10.3.967
# Sat, 25 Sep 2021 01:19:01 GMT
WORKDIR /tmp
# Sat, 25 Sep 2021 01:19:20 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d1fba0cd0733b7cb66e47620845ecedfd757a9bf84e8b276fdb37ed9c272d3ae *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 25 Sep 2021 01:19:20 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb538b78785f115f86e312f41ac522a9b30e0cb77d061dd273f331e57ae2e471`  
		Last Modified: Fri, 03 Sep 2021 08:50:36 GMT  
		Size: 3.3 MB (3269611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39de3f8ba0601a94ebc366f5a916de4aaec9d842925bf77229cb7ac55331bcd2`  
		Last Modified: Sat, 25 Sep 2021 00:35:52 GMT  
		Size: 188.3 MB (188286967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df89338f5cdb2e7cce5dfd69d61e81fb5de338b884f0a257a5c731b7ac57f5df`  
		Last Modified: Sat, 25 Sep 2021 01:27:34 GMT  
		Size: 58.4 MB (58419323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-tools-deps-1.10.3.967-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:463a960a3495ba11f9fca6e72a9c9eb6fd8e6878a41cd657d5c28fb424df89f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.3 MB (274319600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a8c5990ba6a5d2efd7dfc8c3d4556e92513e4d1e1586a61ad63d43ff635b26`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:13 GMT
ADD file:3e2426765cfe2b896fc847bcb435624930753c72ac00b87d2c73f4a81c813fd4 in / 
# Tue, 28 Sep 2021 01:41:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 05:43:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:43:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 28 Sep 2021 05:43:46 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 05:43:46 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 05:43:46 GMT
ENV JAVA_VERSION=18-ea+16
# Tue, 28 Sep 2021 05:43:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-x64_bin.tar.gz'; 			downloadSha256='ec604f7aef23624c0acdc0db346a2b226aab47d120538833070f0d5e01d571c1'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-aarch64_bin.tar.gz'; 			downloadSha256='623eff3e61bd5f74442fb5699ac3dea167dbe0ade7dd6c1fa9cdd4788e316b96'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 05:43:59 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 02:23:00 GMT
ENV CLOJURE_VERSION=1.10.3.967
# Wed, 29 Sep 2021 02:23:00 GMT
WORKDIR /tmp
# Wed, 29 Sep 2021 02:23:16 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d1fba0cd0733b7cb66e47620845ecedfd757a9bf84e8b276fdb37ed9c272d3ae *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 29 Sep 2021 02:23:16 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:896f18f54b28590b15a0f3354b13e8ea2f88a05f13de4117720f88cef30206ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:22 GMT  
		Size: 25.9 MB (25915039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f844c3c3d3fdf0c62ff77a82ed24a2a010ad55e3206255c75275457b868825`  
		Last Modified: Tue, 28 Sep 2021 06:06:17 GMT  
		Size: 3.1 MB (3119080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6019d6a94042b363999f573da4846ecfff708548c5470f0fddebacc67e0fa896`  
		Last Modified: Tue, 28 Sep 2021 06:06:33 GMT  
		Size: 187.0 MB (187011891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30059c5a84f395bb7594b14b2deea3abe72625b502dd84a4fa92fcb6079184c9`  
		Last Modified: Wed, 29 Sep 2021 02:48:55 GMT  
		Size: 58.3 MB (58273590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
