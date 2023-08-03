## `openjdk:22-ea-8-slim-bullseye`

```console
$ docker pull openjdk@sha256:f78555f2fe1d232db8653ebccfe1a5bba476f88d6e20b8a84e45f279ef2ebd81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:22-ea-8-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:ec4c862a9835547f49342c92e725e5e5675de386d76897853716d5cfcf2f4d5c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.2 MB (238155957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c5bdc2ecee4f948e5cfba5f1d75a3daf04d35f49bb14c27c143511cd11268b`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:09:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:09:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 28 Jul 2023 04:09:43 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 04:09:43 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 01:47:43 GMT
ENV JAVA_VERSION=22-ea+8
# Thu, 03 Aug 2023 01:48:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/8/GPL/openjdk-22-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='f05e7933726ce10c3789634d099fdf1b3e61ae9d633aae85fa22ed92ed0a8bac'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/8/GPL/openjdk-22-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='ee073fed6cbf145e5e3a06384d3e8f99ee22179cbb4049e1af2dc01275290900'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 03 Aug 2023 01:48:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb66e7ec1c7a7454751d006538099f5227c45bf60b9bca6714a1f3df49c9637`  
		Last Modified: Fri, 28 Jul 2023 04:13:59 GMT  
		Size: 1.6 MB (1582416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677cfa567985944369190461082b409ba3a477402febca727b7fdf3226372d1d`  
		Last Modified: Thu, 03 Aug 2023 01:55:12 GMT  
		Size: 205.2 MB (205155939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
