## `clojure:openjdk-15-boot-slim-buster`

```console
$ docker pull clojure@sha256:be85ee6678f54d6f6b60d1eaaab0e19573d8c9d12f4cb3afc8d9157ab935de29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-15-boot-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:7876d2f05d10f76db2c364bc3fd502e230a17f40d6a69be2e960f696510548fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285567230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f505f9453d2567b0db71fd122f69143cd9cc946e0c7c9937f5fb9d11868cf5`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:42:37 GMT
ENV JAVA_HOME=/usr/local/openjdk-15
# Wed, 05 Aug 2020 00:42:37 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:42:38 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 07 Aug 2020 23:31:58 GMT
ENV JAVA_VERSION=15
# Tue, 01 Sep 2020 01:47:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-aarch64_bin.tar.gz; 			downloadSha256=01e7e07dd8a67a65b32fdcaff75ba3f21cd9cfc749287e7c9b1c6037f96a3537; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-x64_bin.tar.gz; 			downloadSha256=bb67cadee687d7b486583d03c9850342afea4593be4f436044d785fba9508fb7; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 01 Sep 2020 01:47:08 GMT
CMD ["jshell"]
# Tue, 01 Sep 2020 21:15:12 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 01 Sep 2020 21:15:12 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 01 Sep 2020 21:15:13 GMT
WORKDIR /tmp
# Tue, 01 Sep 2020 21:15:18 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 01 Sep 2020 21:15:18 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 01 Sep 2020 21:15:18 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 01 Sep 2020 21:15:37 GMT
RUN boot
# Tue, 01 Sep 2020 21:15:37 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d928f01bcfe3ef1a57ed4d498cdf89218aa77e123cd6f78f8ec01046a6cb842`  
		Last Modified: Wed, 05 Aug 2020 00:49:13 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcaf8278534a89fbf9fe35f783ca9c66d4d3e3f77f31caa1e5c961f7d11bc50`  
		Last Modified: Tue, 01 Sep 2020 01:57:40 GMT  
		Size: 196.1 MB (196126694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836de121c469f90705b2473e56d44777f4dbafc4d656c64150b666a82757f392`  
		Last Modified: Tue, 01 Sep 2020 21:22:52 GMT  
		Size: 279.5 KB (279534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34f7122b81f062706aa133caf39d09dbc8788fcc447fbfea3709baf3da3e292`  
		Last Modified: Tue, 01 Sep 2020 21:22:56 GMT  
		Size: 58.8 MB (58820239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
