## `clojure:openjdk-15-boot-buster`

```console
$ docker pull clojure@sha256:ad42bb9df9a403da9bc51774c5a01848feefbc16f579f030c0e9e601bb81f485
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-15-boot-buster` - linux; amd64

```console
$ docker pull clojure@sha256:c365773ff7dc796efd1d13c08255b3411b9fd4c1ff9340e67df4662a2e8c7bf2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.7 MB (388675962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0892366ab6ebc5c168d056469f14d2cbe0f27678c429cb022d6ead4089fe4ad1`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 16:58:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:49:57 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:50:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-15
# Fri, 18 Dec 2020 04:50:50 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:50:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:50:51 GMT
ENV JAVA_VERSION=15.0.1
# Fri, 18 Dec 2020 04:51:03 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.1/51f4f36ad4ef43e39d0dfdbaf6549e32/9/GPL/openjdk-15.0.1_linux-aarch64_bin.tar.gz; 			downloadSha256=6a62b7ec065280bad978a3322733a089153dec5ebf5ba81fd2fa361382dbc7b0; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.1/51f4f36ad4ef43e39d0dfdbaf6549e32/9/GPL/openjdk-15.0.1_linux-x64_bin.tar.gz; 			downloadSha256=83ec3a7b1649a6b31e021cde1e58ab447b07fb8173489f27f427e731c89ed84a; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Dec 2020 04:51:03 GMT
CMD ["jshell"]
# Fri, 18 Dec 2020 07:50:57 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 18 Dec 2020 07:50:57 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 18 Dec 2020 07:50:57 GMT
WORKDIR /tmp
# Fri, 18 Dec 2020 07:50:58 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Fri, 18 Dec 2020 07:50:59 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 18 Dec 2020 07:50:59 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 18 Dec 2020 07:51:18 GMT
RUN boot
# Fri, 18 Dec 2020 07:51:19 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d599c07d28e6c920ef615f4f9b5cd0d52eb106fcd20c3a7daef389f14edd4ef5`  
		Last Modified: Thu, 17 Dec 2020 17:26:19 GMT  
		Size: 51.8 MB (51829485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fa4eb1e951cd03e1e1ada47951e6cee0ec635dd8ab218565664a8973b12901`  
		Last Modified: Fri, 18 Dec 2020 04:55:16 GMT  
		Size: 13.9 MB (13920463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa8dbf6480a1d6f12f9fb61244f98c27a9b236f5145d58643928d1ade1bfcfb`  
		Last Modified: Fri, 18 Dec 2020 04:56:24 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcef78132cef7f08eff79bada6d433f2936ef4a83573a048c8ed08933820bb6`  
		Last Modified: Fri, 18 Dec 2020 04:56:43 GMT  
		Size: 195.9 MB (195892446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d489f26385a93c5187192d2c8b8854c41599b50f3973e15d171f8aaccf53ad`  
		Last Modified: Fri, 18 Dec 2020 07:56:09 GMT  
		Size: 6.9 KB (6897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57b383f6e3dc01a8e38fac6b41e0537ccbaeae64293bfe50fd03e654225b291`  
		Last Modified: Fri, 18 Dec 2020 07:56:12 GMT  
		Size: 58.8 MB (58820239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
