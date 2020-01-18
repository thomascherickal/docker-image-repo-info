## `clojure:openjdk-14-boot-2.8.3-buster`

```console
$ docker pull clojure@sha256:1096588064451cc6241adaecf40a055c9aeaacc946e3c629c2613c176b4fcdd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-14-boot-2.8.3-buster` - linux; amd64

```console
$ docker pull clojure@sha256:f8e7616a9438574a345fedf34edeb97741ddf248a9b24aca9807d1321287a6cc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.8 MB (391820810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e0e70a81cecfbe602f915ffff6d66b40dc7169c5af3cb47fe485b5c7ad68ad`
-	Default Command: `["boot","repl"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:47:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:49:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:49:14 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 08:50:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-14
# Sat, 28 Dec 2019 08:50:51 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 08:50:52 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 17 Jan 2020 23:41:37 GMT
ENV JAVA_VERSION=14-ea+32
# Fri, 17 Jan 2020 23:41:37 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk14/32/GPL/openjdk-14-ea+32_linux-x64_bin.tar.gz
# Fri, 17 Jan 2020 23:41:37 GMT
ENV JAVA_SHA256=a5ebd5f004508a1617849b598d8fe8c599ed1b255d34a2c4c4776cb00260a8e5
# Fri, 17 Jan 2020 23:41:53 GMT
RUN set -eux; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Fri, 17 Jan 2020 23:41:53 GMT
CMD ["jshell"]
# Sat, 18 Jan 2020 00:09:51 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 18 Jan 2020 00:09:51 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 18 Jan 2020 00:09:51 GMT
WORKDIR /tmp
# Sat, 18 Jan 2020 00:09:52 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && echo "f717ef381f2863a4cad47bf0dcc61e923b3d2afb *boot.sh" | sha1sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Sat, 18 Jan 2020 00:09:52 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 18 Jan 2020 00:09:53 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 18 Jan 2020 00:10:42 GMT
RUN boot
# Sat, 18 Jan 2020 00:10:42 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918eaefd9de8a1595f56900fdb8ab65a03d64b1da1078da7c0b0bf6f7552a14`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 7.8 MB (7811715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bf3e3107f525b7dea5b3cdfd15f62666066202105a0aaddbab2a02aefad1f7`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 10.0 MB (9996202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27622921edb2aae9e0cb64f71a81b4a7cfef8f6a6c766514a018815834ba4e14`  
		Last Modified: Sat, 28 Dec 2019 05:02:00 GMT  
		Size: 51.8 MB (51790562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6522e32240cc901e3fc4dd0a386015b12118789e80eaaff2a864f0e096be6b00`  
		Last Modified: Sat, 28 Dec 2019 08:58:29 GMT  
		Size: 13.9 MB (13920215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57162a26a4826bf91a221b1aee8be41308e7a4fbf827b12b3dc52c9455cbce60`  
		Last Modified: Sat, 28 Dec 2019 08:59:29 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409bcbc5b08b2f2f579b3e1d5d3c0212fd36ba3015f24d7d04eab7fc86319e9d`  
		Last Modified: Fri, 17 Jan 2020 23:47:14 GMT  
		Size: 199.1 MB (199094415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57134119496dfc3f986edf73b0d40e2b9724da35fb3f98f7fc841e5b563475c`  
		Last Modified: Sat, 18 Jan 2020 00:13:14 GMT  
		Size: 6.9 KB (6895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fa1c18970a4d62c54ad0edf38110f1fa313e44b6e50f17574fbefe7254b1f4`  
		Last Modified: Sat, 18 Jan 2020 00:13:23 GMT  
		Size: 58.8 MB (58820875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
