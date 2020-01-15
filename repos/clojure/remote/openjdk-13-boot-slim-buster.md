## `clojure:openjdk-13-boot-slim-buster`

```console
$ docker pull clojure@sha256:82829b337dfa334d3cfb71512218cc1ba12d7b4ca41ed507077ae72111d7fd90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-13-boot-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:402cf4f5b5bb406867e8276e9b936d096c2fa4ce82f81ddc7aeef36fe72ccf82
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286117557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7880eaec85949e16e4877dc4e6bd3c3a6f52c31deedc7a1ae0629c4422bb377c`
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
# Sat, 28 Dec 2019 08:54:07 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Sat, 28 Dec 2019 08:54:08 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 08:54:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 14 Jan 2020 23:25:13 GMT
ENV JAVA_VERSION=13.0.2
# Tue, 14 Jan 2020 23:25:13 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Tue, 14 Jan 2020 23:25:13 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Tue, 14 Jan 2020 23:25:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Tue, 14 Jan 2020 23:25:30 GMT
CMD ["jshell"]
# Wed, 15 Jan 2020 00:05:31 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 15 Jan 2020 00:05:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 15 Jan 2020 00:05:32 GMT
WORKDIR /tmp
# Wed, 15 Jan 2020 00:05:37 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && echo "f717ef381f2863a4cad47bf0dcc61e923b3d2afb *boot.sh" | sha1sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get remove -y --purge wget && apt-get autoremove -y
# Wed, 15 Jan 2020 00:05:37 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 15 Jan 2020 00:05:37 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 15 Jan 2020 00:06:41 GMT
RUN boot
# Wed, 15 Jan 2020 00:06:41 GMT
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
	-	`sha256:cb5f37227b87c0b96a46435e5f02e7b6ee1d336ade4e987032482e24f673cc12`  
		Last Modified: Sat, 28 Dec 2019 09:01:05 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f246661328ac5dd6941774168ed113fa4d61471d23245509a193842aeecdb7f5`  
		Last Modified: Tue, 14 Jan 2020 23:28:12 GMT  
		Size: 196.7 MB (196675194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1687d5f5c321f30af581fdedea3f5de00e4547bd994b63aedfdd411f3581936`  
		Last Modified: Wed, 15 Jan 2020 00:09:47 GMT  
		Size: 279.7 KB (279666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79228fb661ede2bf3b7aa7115137cf0b3638626797508d848c338df5e23e71a5`  
		Last Modified: Wed, 15 Jan 2020 00:09:51 GMT  
		Size: 58.8 MB (58821109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
