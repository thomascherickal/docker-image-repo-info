## `clojure:openjdk-17-boot-slim-buster`

```console
$ docker pull clojure@sha256:72f35e40820c503fdac9e0490cc4f8b23842a3439d7e0600f66c0907d62c162e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-boot-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:5dd04a0f564311f11ae859c3e0b511f7222df6cac37b7d417ac3a5629ac95914
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.0 MB (277038731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4153f3a9c5db6828afdf5e5f007eb89b1c05dfd724828130e9ccbc5b88a3fa68`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:32:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:34:42 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Fri, 03 Sep 2021 08:34:42 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:34:42 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:34:43 GMT
ENV JAVA_VERSION=17
# Fri, 03 Sep 2021 08:34:57 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 03 Sep 2021 08:34:58 GMT
CMD ["jshell"]
# Sat, 04 Sep 2021 10:02:17 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 04 Sep 2021 10:02:17 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 04 Sep 2021 10:02:18 GMT
WORKDIR /tmp
# Sat, 04 Sep 2021 10:02:22 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 04 Sep 2021 10:02:22 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 04 Sep 2021 10:02:23 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 04 Sep 2021 10:02:42 GMT
RUN boot
# Sat, 04 Sep 2021 10:02:42 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb538b78785f115f86e312f41ac522a9b30e0cb77d061dd273f331e57ae2e471`  
		Last Modified: Fri, 03 Sep 2021 08:50:36 GMT  
		Size: 3.3 MB (3269611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f283494c72c90c2f29b73123ccefa9bd75e713930e39f9ee9ce4885d8c73d`  
		Last Modified: Fri, 03 Sep 2021 08:53:23 GMT  
		Size: 187.5 MB (187523165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9dac9421195daca94cde51cac16ad2c5268ae722902aef0b97608f84b6cec7`  
		Last Modified: Sat, 04 Sep 2021 10:14:46 GMT  
		Size: 279.7 KB (279743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972e9d24934f3c09cd55a9960aa4ae88a1b71dd577e02e1258b6e4f93e6af631`  
		Last Modified: Sat, 04 Sep 2021 10:14:50 GMT  
		Size: 58.8 MB (58820368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-boot-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a81099b68b539a30ebcb242eaa3d529e8f4d80a6d3dec27e6330e76f408bbbe6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.5 MB (274473549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e46c96fcdacf8cdfebe96b63a11be50cef98f48d8ec43041e3f0ca1a08cb2d`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:13 GMT
ADD file:3e2426765cfe2b896fc847bcb435624930753c72ac00b87d2c73f4a81c813fd4 in / 
# Tue, 28 Sep 2021 01:41:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 05:43:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:45:16 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 28 Sep 2021 05:45:16 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 05:45:16 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 05:45:16 GMT
ENV JAVA_VERSION=17
# Tue, 28 Sep 2021 05:45:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 05:45:29 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 02:18:57 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 29 Sep 2021 02:18:58 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 29 Sep 2021 02:18:58 GMT
WORKDIR /tmp
# Wed, 29 Sep 2021 02:19:03 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 29 Sep 2021 02:19:03 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 29 Sep 2021 02:19:03 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 29 Sep 2021 02:19:27 GMT
RUN boot
# Wed, 29 Sep 2021 02:19:27 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:896f18f54b28590b15a0f3354b13e8ea2f88a05f13de4117720f88cef30206ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:22 GMT  
		Size: 25.9 MB (25915039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f844c3c3d3fdf0c62ff77a82ed24a2a010ad55e3206255c75275457b868825`  
		Last Modified: Tue, 28 Sep 2021 06:06:17 GMT  
		Size: 3.1 MB (3119080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5b5cc49cb0464110d1d44eb9be8ba1effa059f6bc1f48a7c7da9949b37337b`  
		Last Modified: Tue, 28 Sep 2021 06:09:21 GMT  
		Size: 186.3 MB (186339348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ae07584bc69652b5eadbb84a9685fefa7f7d3e57aa114447315d61d65d072c`  
		Last Modified: Wed, 29 Sep 2021 02:46:37 GMT  
		Size: 279.6 KB (279555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4eabe8d12826d3bbf946ecd136ec8d4bdc3382bccb3bd6beb89d68d14a1b30`  
		Last Modified: Wed, 29 Sep 2021 02:46:42 GMT  
		Size: 58.8 MB (58820527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
