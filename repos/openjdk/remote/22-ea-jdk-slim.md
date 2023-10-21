## `openjdk:22-ea-jdk-slim`

```console
$ docker pull openjdk@sha256:df293efa34fb6afd085a275386aa57309399a76ba29be6dc1f509d59d30101a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-jdk-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:9f5ee826fcbd93e317e4a8c6243f06585221ce90ebf8bf5254e64bd048ec5a3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.7 MB (238720245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d23cb5334939226cf9676f9510acfba5482fb441e89d8bc411f47e2178eaa4f8`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 02:48:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 02:48:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Thu, 12 Oct 2023 02:48:48 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 02:48:48 GMT
ENV LANG=C.UTF-8
# Fri, 13 Oct 2023 02:03:36 GMT
ENV JAVA_VERSION=22-ea+19
# Fri, 13 Oct 2023 02:04:03 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/19/GPL/openjdk-22-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='70bc0434cc0a8e1fa5351daa062cdd86b29caa784525f22e8a0cc0028e34a157'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/19/GPL/openjdk-22-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='973d8beb242379ed3bec118f7374dc61a99699411c38875ecdf158e506b0a3c0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 13 Oct 2023 02:04:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6b4e2c8e80e7a261b67542c6655d67269b5dad6ffbef15b5e49e5589289b82`  
		Last Modified: Thu, 12 Oct 2023 02:50:10 GMT  
		Size: 4.0 MB (4017876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd08f74979c20f7ebdfdad0036141cf82830857146e31cc96299a16620ca99fe`  
		Last Modified: Fri, 13 Oct 2023 02:07:56 GMT  
		Size: 205.6 MB (205552495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-jdk-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:6a7ba478a0b9fa78020d16bad023a77aac8190cb866f8ff0029cdf761a528faf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.9 MB (236859365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dacbe7ac3634f92a42d19d31d06545df7756e94b16aefa92b2133bad3b71e593`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:50:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:50:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Wed, 11 Oct 2023 22:50:09 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:50:09 GMT
ENV LANG=C.UTF-8
# Fri, 20 Oct 2023 23:59:12 GMT
ENV JAVA_VERSION=22-ea+20
# Fri, 20 Oct 2023 23:59:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/20/GPL/openjdk-22-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='5f1627efa81951307900954bbf7b2e49d8c5303615cf116959c273e9707b0496'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/20/GPL/openjdk-22-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='8fa022a3b05cc606bccbb014baea9e821954a789ba40b6fd39b40cd4453fb9f5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 20 Oct 2023 23:59:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1addc1e1c2c75c85302c72986bed4391fe81acea06679d6de790ea18001eb6`  
		Last Modified: Wed, 11 Oct 2023 22:52:19 GMT  
		Size: 3.8 MB (3825526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69610b38a37761ebacc5b0cdad20ecacee21c792ef65765e705820245e5749dd`  
		Last Modified: Sat, 21 Oct 2023 00:05:35 GMT  
		Size: 203.9 MB (203854555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
