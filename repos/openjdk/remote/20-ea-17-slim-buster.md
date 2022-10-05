## `openjdk:20-ea-17-slim-buster`

```console
$ docker pull openjdk@sha256:c4a00fdf45119865f7d9ddf7d55a41bb7bfddf4ad54f308a9053fc5c6286e909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-17-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:afa4f3f7314e7913cf3cc7daaa974eec753c453cb251ba8e6e016c0e57ea3c75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.7 MB (227685638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e9d3d6bcc650cde1a0945dc3b3eb36ffa4bac9a3edc4b49afe9fd2e004937e`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:01:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:01:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 05 Oct 2022 13:01:50 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 13:01:50 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:01:50 GMT
ENV JAVA_VERSION=20-ea+17
# Wed, 05 Oct 2022 13:02:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='9d46acb0892a134f62ab21fca33fdef1da5d579f61ddbd0ae3ff0b4d33c5eca2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='31245b15195bf9f12a6db08474bfcbd1ddbccc76436372bf4db538c6ede8f976'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 05 Oct 2022 13:02:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e42b9ceb9670d3b07bff56104ed6b09d0fc403302f1722dbc879ad64349d2f1`  
		Last Modified: Wed, 05 Oct 2022 13:07:32 GMT  
		Size: 3.3 MB (3273408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1822bbd2bf5921c6c4e2af4c1a406606a83220d1f18cbab49ff757e7e5cf42`  
		Last Modified: Wed, 05 Oct 2022 13:07:46 GMT  
		Size: 197.3 MB (197274187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-17-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:1986db8883bdfaee1183a56345889f2fb8054ffe4f869494abccf826357f48b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.7 MB (224669597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:252cf63ac5eb5cc692af79212f6b381e3ca1a0e8d397702cc479cec433bd42fc`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:10 GMT
ADD file:5395cc8536f80a7cce6fbae552f35b892b152e1db2fce6274fc514d8fc77d7c9 in / 
# Tue, 04 Oct 2022 23:45:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:27:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:27:47 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 05 Oct 2022 04:27:48 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 04:27:49 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 04:27:50 GMT
ENV JAVA_VERSION=20-ea+17
# Wed, 05 Oct 2022 04:28:04 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='9d46acb0892a134f62ab21fca33fdef1da5d579f61ddbd0ae3ff0b4d33c5eca2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='31245b15195bf9f12a6db08474bfcbd1ddbccc76436372bf4db538c6ede8f976'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 05 Oct 2022 04:28:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2c1ba50780a9bc2b2a8f3d639ceca4285c97f51fd1c51c783fe34e150ff35e60`  
		Last Modified: Tue, 04 Oct 2022 23:51:14 GMT  
		Size: 25.9 MB (25911903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a81927bc22acfe9508e423675967ad20111ed2c4daa880d6b1e9ac555cc7a7`  
		Last Modified: Wed, 05 Oct 2022 04:37:04 GMT  
		Size: 3.1 MB (3126082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9742e2a49cd08655e9889ad96d9c5ab3fedfea14f304090d6c6ec7d2033b14`  
		Last Modified: Wed, 05 Oct 2022 04:37:21 GMT  
		Size: 195.6 MB (195631612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
