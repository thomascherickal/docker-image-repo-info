## `openjdk:20-slim`

```console
$ docker pull openjdk@sha256:5633814100924f8123f97063884781026d2389921281b86f1fa6f53092f0c5c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:83e66b4326117c50aa42395ca0cd928b96e5f34fcda45986678cd5d9db6bda1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.3 MB (230278230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff0df30d82ed034578c34854e8bf7217a29f293e0c009a4e9421fb20834339d`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:01:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:01:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 05 Oct 2022 13:01:02 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 13:01:02 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:01:02 GMT
ENV JAVA_VERSION=20-ea+17
# Wed, 05 Oct 2022 13:01:16 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='9d46acb0892a134f62ab21fca33fdef1da5d579f61ddbd0ae3ff0b4d33c5eca2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='31245b15195bf9f12a6db08474bfcbd1ddbccc76436372bf4db538c6ede8f976'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 05 Oct 2022 13:01:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d8e2bf77973a5d00e8f27539bf78d751344f63603d1463e0e7139569123611`  
		Last Modified: Wed, 05 Oct 2022 13:06:09 GMT  
		Size: 1.6 MB (1582278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c2981d6e6c5f0fcd6b5033bb7ab26df4741e0536d229ba8c90ad1448509319`  
		Last Modified: Wed, 05 Oct 2022 13:06:24 GMT  
		Size: 197.3 MB (197275850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:0b47c27e429e455ca6337c0062ae5cc40b7a05824e51d18d1ea6f55cd9f01722
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (227049820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef718a48e8be3bcd8988334edc52e69712ec434601c951a53b216e2a41d9dfe`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:26:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:26:36 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 05 Oct 2022 04:26:37 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 04:26:38 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 04:26:39 GMT
ENV JAVA_VERSION=20-ea+17
# Wed, 05 Oct 2022 04:26:53 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='9d46acb0892a134f62ab21fca33fdef1da5d579f61ddbd0ae3ff0b4d33c5eca2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='31245b15195bf9f12a6db08474bfcbd1ddbccc76436372bf4db538c6ede8f976'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 05 Oct 2022 04:26:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d821c68cde68fc1dabd765433a7ae82e1dfd40ceab9795c047d424959096651c`  
		Last Modified: Wed, 05 Oct 2022 04:35:25 GMT  
		Size: 1.4 MB (1361242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afd4a754fba1475b3e801e0b64dc2a1d19ce2c52383ba0bbe51d99d3c32fee`  
		Last Modified: Wed, 05 Oct 2022 04:35:42 GMT  
		Size: 195.6 MB (195624183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
