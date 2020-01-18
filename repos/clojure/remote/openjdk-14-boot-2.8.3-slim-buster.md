## `clojure:openjdk-14-boot-2.8.3-slim-buster`

```console
$ docker pull clojure@sha256:d2697c52ad444575e585f3daa187baf0fc76c0f85881399d836d315203ebb502
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-14-boot-2.8.3-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:53e7bdd4668fa72dfe502df13bfb95b207e65cc1ae29937f2b8594dae6dcbc2a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.8 MB (288801492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b861549e78fdac1cc30a41557ff32cecb4ffc274e423ca26e636307ea3ed4a3`
-	Default Command: `["boot","repl"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:50:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:50:14 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 08:52:35 GMT
ENV JAVA_HOME=/usr/java/openjdk-14
# Sat, 28 Dec 2019 08:52:35 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 08:52:36 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 17 Jan 2020 23:41:57 GMT
ENV JAVA_VERSION=14-ea+32
# Fri, 17 Jan 2020 23:41:58 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk14/32/GPL/openjdk-14-ea+32_linux-x64_bin.tar.gz
# Fri, 17 Jan 2020 23:41:58 GMT
ENV JAVA_SHA256=a5ebd5f004508a1617849b598d8fe8c599ed1b255d34a2c4c4776cb00260a8e5
# Fri, 17 Jan 2020 23:42:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Fri, 17 Jan 2020 23:42:19 GMT
CMD ["jshell"]
# Sat, 18 Jan 2020 00:08:48 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 18 Jan 2020 00:08:48 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 18 Jan 2020 00:08:48 GMT
WORKDIR /tmp
# Sat, 18 Jan 2020 00:08:53 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && echo "f717ef381f2863a4cad47bf0dcc61e923b3d2afb *boot.sh" | sha1sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get remove -y --purge wget && apt-get autoremove -y
# Sat, 18 Jan 2020 00:08:54 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 18 Jan 2020 00:08:54 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 18 Jan 2020 00:09:44 GMT
RUN boot
# Sat, 18 Jan 2020 00:09:44 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e866b0959566a21a8fa7eb2f7f12da0d12aa3498d6c31bb25a6ede1fa632ac2`  
		Last Modified: Sat, 28 Dec 2019 08:58:53 GMT  
		Size: 3.2 MB (3249103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab72a68614df7d0d9d800dc8bc5b3378c9d144c38bdf0865dbdb5d13bce631a`  
		Last Modified: Sat, 28 Dec 2019 08:59:58 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ad778c003423c5084800ce1c17cd70ead6bf725a44640a6e7d1fa6b99a15a9`  
		Last Modified: Fri, 17 Jan 2020 23:47:57 GMT  
		Size: 199.4 MB (199359368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970e2fab23945493216bd42fb0ac6420769999d4beb110e1c111f7b9e524f704`  
		Last Modified: Sat, 18 Jan 2020 00:13:04 GMT  
		Size: 279.6 KB (279616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34482ac45a6a452b1573937f78ed9048d16fbf734a72b40369b4ca9eb8409df`  
		Last Modified: Sat, 18 Jan 2020 00:13:08 GMT  
		Size: 58.8 MB (58820920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
