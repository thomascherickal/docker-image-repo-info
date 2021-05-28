## `clojure:openjdk-17-boot-2.8.3`

```console
$ docker pull clojure@sha256:2d4db8e9e1fa96e7c4c8c128986f983c175d9f0b0b0574e14c6f1924d1c7aab5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-boot-2.8.3` - linux; amd64

```console
$ docker pull clojure@sha256:88ad887a5bfab20d250a96f20f0dc77f8367f62a28cfaf6d705e60009b6bf1e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.1 MB (276127852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d43e35a7893a2a51916377817c4dd9df2ee16cdae0fbf801a79dc9545c595c7`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:48:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:48:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 12 May 2021 06:48:04 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:48:04 GMT
ENV LANG=C.UTF-8
# Thu, 27 May 2021 23:30:48 GMT
ENV JAVA_VERSION=17-ea+24
# Thu, 27 May 2021 23:31:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/24/GPL/openjdk-17-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='30b8cc8945c42ab310bca47ecfe2acdf2a0285d26dfeb6bfba46ebc5947aef6e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/24/GPL/openjdk-17-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='61d192356099180ee3beec3a22cb9e97cb810c7f55f2c870a73841c3ac61abcb'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 27 May 2021 23:31:02 GMT
CMD ["jshell"]
# Thu, 27 May 2021 23:56:03 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 27 May 2021 23:56:04 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 27 May 2021 23:56:04 GMT
WORKDIR /tmp
# Thu, 27 May 2021 23:56:09 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 27 May 2021 23:56:09 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 27 May 2021 23:56:09 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 27 May 2021 23:56:41 GMT
RUN boot
# Thu, 27 May 2021 23:56:42 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2b89b6081832b112f9483322d4710c661f12135e79279dc3fb1672883ada8d`  
		Last Modified: Wed, 12 May 2021 06:58:18 GMT  
		Size: 3.3 MB (3268772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a2652fa53fe093e3b2e02b7f2d9a2837ea0791b549d005381635049293586a`  
		Last Modified: Thu, 27 May 2021 23:37:22 GMT  
		Size: 186.6 MB (186612738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6122242b0a0c3d95c02c58f142cb4de3aed68e8fc1f2eb8103a87b8d2ba50e7f`  
		Last Modified: Fri, 28 May 2021 00:00:49 GMT  
		Size: 279.7 KB (279661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a569c5a4848eca4a471b259a9d904c428690496e53b3328c58074407be8028b9`  
		Last Modified: Fri, 28 May 2021 00:00:53 GMT  
		Size: 58.8 MB (58820766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-boot-2.8.3` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:92f80ccbe500ef39ba1028a0d13518be66507fc7847d7a16bcd2ac74919c8dce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.7 MB (270725680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ea58425ee0d6dfdd3f67899127985043e33223f31e3a03009b39e224751ca37`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Thu, 27 May 2021 08:38:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 08:38:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Thu, 27 May 2021 08:38:57 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 May 2021 08:38:57 GMT
ENV LANG=C.UTF-8
# Thu, 27 May 2021 08:38:57 GMT
ENV JAVA_VERSION=17-ea+23
# Thu, 27 May 2021 08:39:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/23/GPL/openjdk-17-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='b43ffb86cad128acb9955d2dec2b254ffd0e0c7b7d2a15d8b7ad93772e8f722b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/23/GPL/openjdk-17-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='b5979d864a5c527c98adc81b5430d669672a609a4c19cd8c8b03edb84de74949'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 27 May 2021 08:39:09 GMT
CMD ["jshell"]
# Thu, 27 May 2021 14:09:56 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 27 May 2021 14:09:56 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 27 May 2021 14:09:56 GMT
WORKDIR /tmp
# Thu, 27 May 2021 14:10:01 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 27 May 2021 14:10:01 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 27 May 2021 14:10:01 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 27 May 2021 14:10:20 GMT
RUN boot
# Thu, 27 May 2021 14:10:20 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb067f13654098b66e57229fcd818a7d0f0c73bd34d158e3bedc28ee2a7b821`  
		Last Modified: Thu, 27 May 2021 08:54:42 GMT  
		Size: 3.1 MB (3118848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257d9d3e721d479d92ee9a91355ffcf19f7e099bbec28bbf4e48117341a6869f`  
		Last Modified: Thu, 27 May 2021 08:54:58 GMT  
		Size: 182.6 MB (182595734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd3fa78a6eb4d7b478c5dc9ecd7d7e99791a0ee2805dfb5adaf8edfcad61e0e`  
		Last Modified: Thu, 27 May 2021 14:20:16 GMT  
		Size: 279.5 KB (279477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4335fada020075ecd5b495a84d71d446d79a949ddada25a07b42f074849e7a`  
		Last Modified: Thu, 27 May 2021 14:20:22 GMT  
		Size: 58.8 MB (58820371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
