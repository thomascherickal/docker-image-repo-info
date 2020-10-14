## `clojure:openjdk-14-boot-2.8.3-slim-buster`

```console
$ docker pull clojure@sha256:a3b76a7ca6e8af7efe8841a3578b1846de9e39110baa4f788087c9efd254e1ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-14-boot-2.8.3-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:441d3b41e3ec3d6aabdf5110a85d83f199cd7bbab618a953bbdecfdab7af37e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.9 MB (288906967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8afa376ff2935daeb143360e32d887ed9c1ea6b01d51c325e05bbc044087f8f`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:58:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:58:53 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 09:01:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-14
# Tue, 13 Oct 2020 09:01:51 GMT
ENV PATH=/usr/local/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 09:01:52 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 13 Oct 2020 09:01:52 GMT
ENV JAVA_VERSION=14.0.2
# Tue, 13 Oct 2020 09:02:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk14.0.2/205943a0976c4ed48cb16f1043c5c647/12/GPL/openjdk-14.0.2_linux-x64_bin.tar.gz; 			downloadSha256=91310200f072045dc6cef2c8c23e7e6387b37c46e9de49623ce0fa461a24623d; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Oct 2020 09:02:22 GMT
CMD ["jshell"]
# Wed, 14 Oct 2020 05:33:25 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 14 Oct 2020 05:33:25 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 14 Oct 2020 05:33:25 GMT
WORKDIR /tmp
# Wed, 14 Oct 2020 05:33:30 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 14 Oct 2020 05:33:30 GMT
ENV PATH=/usr/local/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 14 Oct 2020 05:33:31 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 14 Oct 2020 05:33:48 GMT
RUN boot
# Wed, 14 Oct 2020 05:33:48 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00028440d132be6f9dd59a787bc5d1372d575a539c19954651757f12912f2e65`  
		Last Modified: Tue, 13 Oct 2020 09:08:08 GMT  
		Size: 3.2 MB (3248445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7865553c3609b81c17f53c118feac93b812fbe48f2927e86247119b0c5f38859`  
		Last Modified: Tue, 13 Oct 2020 09:10:22 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03464def664221d5eae2df26f46afc21f8cbb59a7f32b5ac724172c5ccf16f7b`  
		Last Modified: Tue, 13 Oct 2020 09:10:48 GMT  
		Size: 199.5 MB (199466486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31522a33313325103c6bf137f3f5efa3f6742ec03730da176855b6a4f2bb0fc`  
		Last Modified: Wed, 14 Oct 2020 05:44:34 GMT  
		Size: 279.6 KB (279555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b792c0380fc12f1267f64f6cc551bd52b8d5ff3c035c71276c8674ae4e9c1447`  
		Last Modified: Wed, 14 Oct 2020 05:44:38 GMT  
		Size: 58.8 MB (58820043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
