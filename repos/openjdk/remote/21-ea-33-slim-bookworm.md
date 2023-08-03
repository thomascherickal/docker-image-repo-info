## `openjdk:21-ea-33-slim-bookworm`

```console
$ docker pull openjdk@sha256:072c6c1a66697029df415afe5819fd3066394b37234603d98746232bf77a0cda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:21-ea-33-slim-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:048af2b0c9940acce4db5c2073746813551ecb0495e087f4fa4c2b55f6af5412
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.4 MB (237433791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85641bb04c3468f71326827fa9fd15ede41e6ee480f600403039384e19adb21a`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:10:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Fri, 28 Jul 2023 04:10:20 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 04:10:20 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 01:49:39 GMT
ENV JAVA_VERSION=21-ea+33
# Thu, 03 Aug 2023 01:50:04 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/33/GPL/openjdk-21-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='c834bec462c77e18a4ba980cc761754649ad34ee40697597ec64306918dedb0b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/33/GPL/openjdk-21-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='41295b248c50ffe8bfa522c0fce7492eabfad5d0fad5c439e7918949066f225a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 03 Aug 2023 01:50:05 GMT
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
	-	`sha256:3c38567fb9d5a86685b1141a45ff008281f854a0e2e90cf15b0ac57b2bdc621b`  
		Last Modified: Thu, 03 Aug 2023 01:57:32 GMT  
		Size: 204.3 MB (204301261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
