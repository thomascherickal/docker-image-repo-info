## `clojure:openjdk-15-tools-deps-1.10.1.590`

```console
$ docker pull clojure@sha256:6bf970f5576d15deb3a191ce1309a09b37a17f342e3f0b6c689781b6ed600dd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-15-tools-deps-1.10.1.590` - linux; amd64

```console
$ docker pull clojure@sha256:4430139976b6b614128ad95f6a55c7e28e93bd77fd7970a9a6614e255a34572b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (268988339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:616e67f9cbf60beca400ede8d5b36786059b21bb33f3b28f908918928587605f`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:35:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:35:24 GMT
ENV LANG=C.UTF-8
# Wed, 29 Jul 2020 01:26:03 GMT
ENV JAVA_HOME=/usr/local/openjdk-15
# Wed, 29 Jul 2020 01:26:03 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jul 2020 01:26:04 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 29 Jul 2020 01:26:04 GMT
ENV JAVA_VERSION=15-ea+33
# Wed, 29 Jul 2020 01:26:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/33/GPL/openjdk-15-ea+33_linux-aarch64_bin.tar.gz; 			downloadSha256=124fd9ba4611895460ff1547df282cd49b0e9ba2f00c9ead211b59142cc642c4; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/33/GPL/openjdk-15-ea+33_linux-x64_bin.tar.gz; 			downloadSha256=6de169c1de7d37e6c5d5b59a12410a908f22576c07f98d9915a586d91909fc12; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Wed, 29 Jul 2020 01:26:33 GMT
CMD ["jshell"]
# Wed, 29 Jul 2020 02:11:41 GMT
ENV CLOJURE_VERSION=1.10.1.590
# Wed, 29 Jul 2020 02:11:41 GMT
WORKDIR /tmp
# Wed, 29 Jul 2020 02:12:01 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "92a606c1b373ddee338c209f9fecd6f0a40b3354b5eb762962b9cc64f226ce53 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 29 Jul 2020 02:12:01 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa4e9b7780660af457791b3bbbd51d1d25c8d9681c1f7ebe5e3a59e0179cecd`  
		Last Modified: Wed, 22 Jul 2020 22:44:33 GMT  
		Size: 3.2 MB (3248441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb9bb9b7d051e91eee43856c2c35d5c940bc296414fd9a560794f48a17687e6`  
		Last Modified: Wed, 29 Jul 2020 01:34:09 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09833c6a4bdaf5ac37c2adbf9b69db0ab56904a3aa187ed2bc96ba3051e2c7c`  
		Last Modified: Wed, 29 Jul 2020 01:34:26 GMT  
		Size: 196.1 MB (196132334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890921c6d099b290106d88f48b7b76948dd645e895643080e64bd1bc3f4fe99b`  
		Last Modified: Wed, 29 Jul 2020 02:17:47 GMT  
		Size: 42.5 MB (42508811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
