## `openjdk:20-slim`

```console
$ docker pull openjdk@sha256:b62f4e97f8215e20bd44d24a582fc8615f39fc6792958beb0ee779821e48fdaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:22efbce4bf171b850713a1517bfcc2d382111f857d511dd199b070469a77128d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231650363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee4bf7b13dff3c50213701eee27a225172b62a43606ea65f53aa097669ec724a`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:37:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:37:09 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 15 Nov 2022 13:37:09 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 13:37:09 GMT
ENV LANG=C.UTF-8
# Fri, 18 Nov 2022 01:42:22 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:42:37 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='f73656bed38d61eb8b7c771a59ad326adeb625e5f18e92b7fd11f657d1005d54'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='58fb9a1ea196a73f54b3ab94189cb6eaece44105eb82d113db57b6ab51aca5e6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Nov 2022 01:42:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54e66bc569588bf6945416d9455248d373e1db9ffe9428a75b3963b798662d6`  
		Last Modified: Tue, 15 Nov 2022 13:42:10 GMT  
		Size: 1.6 MB (1583981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0cc1fba6c64751a74a09efeb49576f911f3d6eb754c00a53e177558d69b467`  
		Last Modified: Fri, 18 Nov 2022 01:47:35 GMT  
		Size: 198.7 MB (198653752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:445535935860b3fa199b30e6d0a94cad6567e2f6369db5b7b1b51f64f046ddc9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.8 MB (228849054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec3e0e1375ced94170a44194ceafd7f5dfe55f508c6a1648cbd9e2e72a2919d`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:59:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:59:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 15 Nov 2022 06:59:21 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 06:59:21 GMT
ENV LANG=C.UTF-8
# Fri, 18 Nov 2022 01:58:21 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:58:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='f73656bed38d61eb8b7c771a59ad326adeb625e5f18e92b7fd11f657d1005d54'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='58fb9a1ea196a73f54b3ab94189cb6eaece44105eb82d113db57b6ab51aca5e6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Nov 2022 01:58:35 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bb8ead4542ac0732ce51843584ff03141aa14c30f7161cc4856f3caa5d7a95`  
		Last Modified: Tue, 15 Nov 2022 07:04:17 GMT  
		Size: 1.6 MB (1567467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0bf1051b3fea8298aae2fc428294d9cfc9b8ca7fc36468028e41653c2fd6b4`  
		Last Modified: Fri, 18 Nov 2022 02:03:27 GMT  
		Size: 197.2 MB (197220982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
