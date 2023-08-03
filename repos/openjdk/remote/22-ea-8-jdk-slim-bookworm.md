## `openjdk:22-ea-8-jdk-slim-bookworm`

```console
$ docker pull openjdk@sha256:fcb36e929c096ad70fe07a3498f29391dc0a994492b489ee330d0e44cb013601
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:22-ea-8-jdk-slim-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:a5c1f3f87728210b0699f45413c5c45a797d7574230c2c035d19c35ae6abd1b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.3 MB (238282262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:525dcbeb16d04122867a687aeb3d23669e9dac14959c909fcb1f001a71d12f3b`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:08:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 28 Jul 2023 04:08:55 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 04:08:55 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 01:46:40 GMT
ENV JAVA_VERSION=22-ea+8
# Thu, 03 Aug 2023 01:47:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/8/GPL/openjdk-22-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='f05e7933726ce10c3789634d099fdf1b3e61ae9d633aae85fa22ed92ed0a8bac'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/8/GPL/openjdk-22-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='ee073fed6cbf145e5e3a06384d3e8f99ee22179cbb4049e1af2dc01275290900'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 03 Aug 2023 01:47:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0240addcdc3176ff8e69de0608d99fa8e2e530a860fb05c187d7e292b3f119b8`  
		Last Modified: Fri, 28 Jul 2023 04:12:44 GMT  
		Size: 4.0 MB (4007998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffaf34982de27d8e67fd35e9764b7fb45ee2e2cc4448ec61556322de77af9b2`  
		Last Modified: Thu, 03 Aug 2023 01:53:57 GMT  
		Size: 205.1 MB (205149732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
