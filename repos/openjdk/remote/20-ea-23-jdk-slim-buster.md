## `openjdk:20-ea-23-jdk-slim-buster`

```console
$ docker pull openjdk@sha256:07c677b7e30d0e09a97fb6c882a0ce23cdc2c3ae12d2cee6d836a29122e4e903
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-23-jdk-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:0ab9d3742c13b9802144f87b0dedaef2113675cf7a36060e3d6c9d18937d4c99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.0 MB (229031727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a4ad8bb46807cf892c9b43dbaba13b4633929d9becbb7be4dd0abef04e9d5d`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:29:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:29:03 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 25 Oct 2022 04:29:04 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 04:29:04 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 00:57:13 GMT
ENV JAVA_VERSION=20-ea+23
# Fri, 11 Nov 2022 00:57:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Nov 2022 00:57:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04045c4766379cb0b4fc93bb96707506245d8d2e952cc00e74925a3994f6ec34`  
		Last Modified: Tue, 25 Oct 2022 04:33:18 GMT  
		Size: 3.3 MB (3275908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3a94a29557d6fe5cc2c4f1e9a23cb766f7b28df2c16b5cc70b88d26f8546a8`  
		Last Modified: Fri, 11 Nov 2022 01:03:30 GMT  
		Size: 198.6 MB (198614987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-23-jdk-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:21f82873dc4c62baff592c9ff8ce7c169eba010ae3e6aa40ea9d808fb8f8fd02
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.2 MB (226222067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b593f564717311a7dc0268e2ece09df02fc72e6a7e820b5db6d07476f93ecd3`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 00:45:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 00:45:37 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 26 Oct 2022 00:45:37 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 00:45:37 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 11:34:58 GMT
ENV JAVA_VERSION=20-ea+23
# Fri, 11 Nov 2022 11:35:10 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Nov 2022 11:35:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13616a3846ecd154918e95271126bfcebd73bd0090135c17f7836596878e708`  
		Last Modified: Wed, 26 Oct 2022 00:53:01 GMT  
		Size: 3.1 MB (3129308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aac129b05fdbc50fc37f3003296d76735f4ee855d6af4ab1d0164c370d1ae53`  
		Last Modified: Fri, 11 Nov 2022 11:40:56 GMT  
		Size: 197.2 MB (197177874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
