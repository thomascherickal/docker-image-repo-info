## `openjdk:22-ea-27-slim-bullseye`

```console
$ docker pull openjdk@sha256:346f600ee21fd1238957f34e55bbd53c37b2af35efeff1b6cf6bedaf5dc1ee4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:22-ea-27-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:80e3858b050add79eff0d8e20bceaa767ff8bc67d10494876f897e5d04d19be5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.8 MB (232792924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fafabe0c8510772b00bb3ccff129842d1c566229014d95d752ca3b409f2ddd66`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:30:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:30:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 21 Nov 2023 10:30:24 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 10:30:25 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 23:24:55 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 23:25:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 08 Dec 2023 23:25:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c15c180f917c66ccf40fb29716213580bb2210985872dc965325ab4182616`  
		Last Modified: Tue, 21 Nov 2023 10:32:42 GMT  
		Size: 1.6 MB (1567872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5ddba1d5855ac6033ab2dfc55bad64f061d0fa30d765b45f5709406cac34fe`  
		Last Modified: Fri, 08 Dec 2023 23:28:43 GMT  
		Size: 201.2 MB (201160929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
