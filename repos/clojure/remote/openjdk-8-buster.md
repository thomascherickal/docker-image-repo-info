## `clojure:openjdk-8-buster`

```console
$ docker pull clojure@sha256:07542747d15047720b1059df3b24dd0e133f40b506b90c0555c6ff3fcff262f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-8-buster` - linux; amd64

```console
$ docker pull clojure@sha256:7bb8fae7f42fc1cc16097b547fccd8ac980705709523195b09c7d8d39db3b6c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262696391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dd05395d0d5ef3bffb06ec5c02ced6e6d5078986ff8308feb2e53385578e856`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:26:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:31:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:31:57 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:31:57 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:31:58 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:48:05 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:48:42 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 23:45:21 GMT
ENV CLOJURE_VERSION=1.10.3.1075
# Fri, 04 Feb 2022 23:45:22 GMT
WORKDIR /tmp
# Fri, 04 Feb 2022 23:45:36 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a6b72c9b23d348a0636813c5f59db5dda622e3b8dbb86124cbb51e3aced714d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Fri, 04 Feb 2022 23:45:36 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 04 Feb 2022 23:45:36 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c63da771697b362929cecc84777e8cfbb716ff3d575b999854d83ada039b695`  
		Last Modified: Wed, 26 Jan 2022 02:23:53 GMT  
		Size: 51.8 MB (51839910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04554298b961fe9b1471a6efe1f1c171686298a8138a4b74bfcce778504a9f7e`  
		Last Modified: Wed, 26 Jan 2022 09:52:34 GMT  
		Size: 5.3 MB (5286589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e33b0199c29b3da97d5f0c3f9abcb6f8ff01e57b4d61cbe82d02c3c387587b2`  
		Last Modified: Wed, 26 Jan 2022 09:56:53 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ad236a440b6a8f3b9e5a2c27361a2842dabe6cdae9f7553490687f9560069b`  
		Last Modified: Thu, 03 Feb 2022 21:04:01 GMT  
		Size: 106.1 MB (106078796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6c56f667d0c4a71e1e5a7280c65e7bc97d32bd39e77e77fd945e35f1499754`  
		Last Modified: Fri, 04 Feb 2022 23:57:04 GMT  
		Size: 31.2 MB (31222142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ead1ccb4407782f79e41d1302d0eccbbf474d8ddd7c7fbeb86f7ddbf7d84ea`  
		Last Modified: Fri, 04 Feb 2022 23:57:00 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-8-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c646b19949936cc5e418cc2f735388f0b3338013ce9518f910fc42326ef3846f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.8 MB (259787376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:687bbf61f2bde089c9905a8f6f00d470c74bf44661a5fbae00ac5e6bf3b53095`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:58:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:01:35 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 06:01:36 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 06:01:37 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 06:01:38 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:58:31 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:58:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 21:41:16 GMT
ENV CLOJURE_VERSION=1.10.3.1075
# Fri, 04 Feb 2022 21:41:16 GMT
WORKDIR /tmp
# Fri, 04 Feb 2022 21:41:33 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a6b72c9b23d348a0636813c5f59db5dda622e3b8dbb86124cbb51e3aced714d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Fri, 04 Feb 2022 21:41:34 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 04 Feb 2022 21:41:34 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f0325e59cadc58f4e81c6a282319b0c01f54964ef989205974a6557cf15040`  
		Last Modified: Wed, 26 Jan 2022 02:25:25 GMT  
		Size: 52.2 MB (52168727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab1b7b529fe97dbd551634a2df123f221d5ec5897d133ed78061852035deea9`  
		Last Modified: Wed, 26 Jan 2022 06:24:49 GMT  
		Size: 5.3 MB (5276627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12a0243305b3ade3c7318de1f847db764e01972bf1341c50ce386924e0f0122`  
		Last Modified: Wed, 26 Jan 2022 06:29:25 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3000a474cdd0ea1085979d5bd6cb75d3a92ae427547262e757f8e0b127a5b9b`  
		Last Modified: Thu, 03 Feb 2022 21:19:28 GMT  
		Size: 105.1 MB (105092304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e085a3f684441d84470bedf1cb2d599f1a055fc0b73d3efed99eaca1d582ebc4`  
		Last Modified: Fri, 04 Feb 2022 21:55:21 GMT  
		Size: 30.6 MB (30563431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abc83aa9dc2c3262f159e80b47f0fa441299ac56c261a064debe42f624514f7`  
		Last Modified: Fri, 04 Feb 2022 21:55:17 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
