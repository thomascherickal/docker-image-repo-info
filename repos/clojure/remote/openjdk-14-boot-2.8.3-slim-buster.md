## `clojure:openjdk-14-boot-2.8.3-slim-buster`

```console
$ docker pull clojure@sha256:46c18188193d5a7eb93bc62a3d3a944f83a423daa335a82f2486e3694b450691
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-14-boot-2.8.3-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:b8cf7b0f7a987c1177beebb9db498184e25637e62d918783d96afa8abfe2a5f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.9 MB (288912041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07295e12b2f42c2e3063503bc928fe30ec6d24cc6c4f44b9436013cbf181690`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:35:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:35:24 GMT
ENV LANG=C.UTF-8
# Wed, 29 Jul 2020 01:28:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-14
# Wed, 29 Jul 2020 01:28:13 GMT
ENV PATH=/usr/local/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jul 2020 01:28:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 29 Jul 2020 01:28:14 GMT
ENV JAVA_VERSION=14.0.2
# Wed, 29 Jul 2020 01:28:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk14.0.2/205943a0976c4ed48cb16f1043c5c647/12/GPL/openjdk-14.0.2_linux-x64_bin.tar.gz; 			downloadSha256=91310200f072045dc6cef2c8c23e7e6387b37c46e9de49623ce0fa461a24623d; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Wed, 29 Jul 2020 01:28:40 GMT
CMD ["jshell"]
# Wed, 29 Jul 2020 02:08:33 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 29 Jul 2020 02:08:34 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 29 Jul 2020 02:08:34 GMT
WORKDIR /tmp
# Wed, 29 Jul 2020 02:08:39 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 29 Jul 2020 02:08:39 GMT
ENV PATH=/usr/local/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 29 Jul 2020 02:08:39 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 29 Jul 2020 02:08:57 GMT
RUN boot
# Wed, 29 Jul 2020 02:08:57 GMT
CMD ["boot" "repl"]
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
	-	`sha256:615a5e156fd8f1d3f37f48db04ccd4d0b17809f1f1b7ed1793c41bfd97275729`  
		Last Modified: Wed, 29 Jul 2020 01:35:57 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353bd2f3c6d0e7914c26ae02426a86b4075f014592607f533637cdaf78c64302`  
		Last Modified: Wed, 29 Jul 2020 01:36:14 GMT  
		Size: 199.5 MB (199465139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff095c09a9538de8de3d0dc6df3acf9ff472f9b5f27b5270814a9910b7ffad4`  
		Last Modified: Wed, 29 Jul 2020 02:16:35 GMT  
		Size: 279.6 KB (279561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cf3fd7e199d46651017963b417e0be6038a153b4f5ef160483e79fb3dc71c5`  
		Last Modified: Wed, 29 Jul 2020 02:16:39 GMT  
		Size: 58.8 MB (58820145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
