## `clojure:openjdk-18-boot-2.8.3-slim-buster`

```console
$ docker pull clojure@sha256:9dd9743a39826441f9ec2ed9608b9ba7cd4ff34a78744a803cc8e55e990c6a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-boot-2.8.3-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:818af056ebf3b934fd55e6964ce3f3a5d104867bdc20e054b5dadf1799716206
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.0 MB (278013095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68ced611d410b39e4fdeef83e8663f07608154af4b30c0455187e525c5d8774`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:28:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:28:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 12 Oct 2021 16:28:45 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:28:45 GMT
ENV LANG=C.UTF-8
# Mon, 01 Nov 2021 18:50:33 GMT
ENV JAVA_VERSION=18-ea+21
# Mon, 01 Nov 2021 18:50:49 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/21/GPL/openjdk-18-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='c0a1fcdd389abdc8101892215f73413b10975f735f31e6d0484c9653fc9ba5e9'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/21/GPL/openjdk-18-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='a5ed86d5c7f9433360bc81b5b283d6b5fc345309d16c77125c8ceff32ed5c9a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 01 Nov 2021 18:50:50 GMT
CMD ["jshell"]
# Mon, 01 Nov 2021 19:37:58 GMT
ENV BOOT_VERSION=2.8.3
# Mon, 01 Nov 2021 19:37:58 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Mon, 01 Nov 2021 19:37:58 GMT
WORKDIR /tmp
# Mon, 01 Nov 2021 19:38:03 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Mon, 01 Nov 2021 19:38:04 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Mon, 01 Nov 2021 19:38:04 GMT
ENV BOOT_AS_ROOT=yes
# Mon, 01 Nov 2021 19:38:25 GMT
RUN boot
# Mon, 01 Nov 2021 19:38:25 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72345ef1bcc1976ef9d97f0fec94945f6957f67d796c64b3a1e92a610fe0ee10`  
		Last Modified: Tue, 12 Oct 2021 16:44:29 GMT  
		Size: 3.3 MB (3269598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669b832f4a79a98af0ed0f1f024cd2229b096d2e30b88cb3ff72c272ff08ffa2`  
		Last Modified: Mon, 01 Nov 2021 18:59:33 GMT  
		Size: 188.5 MB (188503720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1171c4ed8cab6cba60c6aa3e3c34b9093ed6a00ce081e22f787fab37e9b2d6b`  
		Last Modified: Mon, 01 Nov 2021 19:46:19 GMT  
		Size: 279.8 KB (279786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db0afe8fc9e2d13226d3f35d91904b854775ea377b9e12c907bcbafe7b133ff`  
		Last Modified: Mon, 01 Nov 2021 19:46:22 GMT  
		Size: 58.8 MB (58820481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-boot-2.8.3-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8a597bf6c1201a708013dc1683b627c97b4b0e630c66706df176db70eb179aa7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.1 MB (275125191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6a174a8866b5d3401ca7ec39de5b686314fc4f9af07b980eb80f4ccd97d3d0b`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 06:01:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:01:58 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Wed, 13 Oct 2021 06:01:59 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:02:00 GMT
ENV LANG=C.UTF-8
# Mon, 01 Nov 2021 19:19:44 GMT
ENV JAVA_VERSION=18-ea+21
# Mon, 01 Nov 2021 19:20:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/21/GPL/openjdk-18-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='c0a1fcdd389abdc8101892215f73413b10975f735f31e6d0484c9653fc9ba5e9'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/21/GPL/openjdk-18-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='a5ed86d5c7f9433360bc81b5b283d6b5fc345309d16c77125c8ceff32ed5c9a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 01 Nov 2021 19:20:02 GMT
CMD ["jshell"]
# Mon, 01 Nov 2021 20:22:35 GMT
ENV BOOT_VERSION=2.8.3
# Mon, 01 Nov 2021 20:22:36 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Mon, 01 Nov 2021 20:22:37 GMT
WORKDIR /tmp
# Mon, 01 Nov 2021 20:22:42 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Mon, 01 Nov 2021 20:22:43 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Mon, 01 Nov 2021 20:22:44 GMT
ENV BOOT_AS_ROOT=yes
# Mon, 01 Nov 2021 20:23:16 GMT
RUN boot
# Mon, 01 Nov 2021 20:23:16 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42a628bf864e5fbc07330c3cb3cbd4f73d7b9f624a52fbb7162c07185b972a4`  
		Last Modified: Wed, 13 Oct 2021 06:27:07 GMT  
		Size: 3.1 MB (3118848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9937d34cda44443b8610d52daa32dffc17d4227ad7eccde7a811d71f80114a65`  
		Last Modified: Mon, 01 Nov 2021 19:33:33 GMT  
		Size: 187.2 MB (187213863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4dfa0d7634801ee15a7b9e573c6d7b5fe2ef3cc628be9a3e6a861bcf985734`  
		Last Modified: Mon, 01 Nov 2021 20:35:03 GMT  
		Size: 67.5 KB (67533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b601f3ae6506055672e370f0a2aad6627a07245f8ed5c782fb1e40efc21cbf42`  
		Last Modified: Mon, 01 Nov 2021 20:35:10 GMT  
		Size: 58.8 MB (58816468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
