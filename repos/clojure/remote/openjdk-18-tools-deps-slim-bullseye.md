## `clojure:openjdk-18-tools-deps-slim-bullseye`

```console
$ docker pull clojure@sha256:9691593a00369c06b860dffe061003029805ceedea24fd65a29d1f5a871e2477
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-18-tools-deps-slim-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:f7247e6526fdb8db7ce5171da71a1671ee2d2bf58c6d36661c17f8db8d2cf7db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.5 MB (277496210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d88ae93fa78fa7453e912f030de10cf66c013f2f606bbbfb64c3d64a44e5b040`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:21 GMT
ADD file:19d7ba0fceddd7fc78b5fb96cf8110e5d10e0e5d2554030dfe640d161379cb79 in / 
# Fri, 03 Sep 2021 01:21:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:31:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:31:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 08:31:20 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:31:20 GMT
ENV LANG=C.UTF-8
# Sat, 04 Sep 2021 09:42:18 GMT
ENV JAVA_VERSION=18-ea+13
# Sat, 04 Sep 2021 09:42:31 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/13/GPL/openjdk-18-ea+13_linux-x64_bin.tar.gz'; 			downloadSha256='396584ea555ad439176473f4e22c146817290a8eeaad02e3072dfb398ba786e0'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/13/GPL/openjdk-18-ea+13_linux-aarch64_bin.tar.gz'; 			downloadSha256='4601ee9811daa3bf282753e1fa6b8caffd869d0e56c9acfe95e1670bc580ed34'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 04 Sep 2021 09:42:32 GMT
CMD ["jshell"]
# Thu, 09 Sep 2021 19:34:31 GMT
ENV CLOJURE_VERSION=1.10.3.967
# Thu, 09 Sep 2021 19:34:31 GMT
WORKDIR /tmp
# Thu, 09 Sep 2021 19:34:48 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d1fba0cd0733b7cb66e47620845ecedfd757a9bf84e8b276fdb37ed9c272d3ae *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Sep 2021 19:34:48 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:f8416d8bac72cefc0ce17bd2dc0c03aa43e123d309db92ee23be9382192cf2ed`  
		Last Modified: Fri, 03 Sep 2021 01:27:25 GMT  
		Size: 31.4 MB (31368702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ae0b0c4c13e1ebacfd091b8e226cc8aa92df8937632e3bec2b03a877bf2d87`  
		Last Modified: Fri, 03 Sep 2021 08:49:03 GMT  
		Size: 1.6 MB (1582002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25baa4d26f4c51077d9f4064945d9e80538961a0548091534e19f6b026db4374`  
		Last Modified: Sat, 04 Sep 2021 09:51:04 GMT  
		Size: 187.8 MB (187781630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0482960be916bfc6735146a16bb5113c38158b82696ef3f21c567b7c76916ac`  
		Last Modified: Thu, 09 Sep 2021 19:51:03 GMT  
		Size: 56.8 MB (56763876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
