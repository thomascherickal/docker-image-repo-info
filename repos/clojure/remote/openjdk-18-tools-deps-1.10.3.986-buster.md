## `clojure:openjdk-18-tools-deps-1.10.3.986-buster`

```console
$ docker pull clojure@sha256:a6a542baa17749a77d2b2b6ff3e0e536ac74a5c6d90fd1b7f0a79edd6a0e4124
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-tools-deps-1.10.3.986-buster` - linux; amd64

```console
$ docker pull clojure@sha256:414a2caf6a92ea7b9481f69b7228a2436024d3fb64ec17215a922812258c2316
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.2 MB (350195626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a615dcb0c2ed143e7945ab6436a0023f2a9be6ec06368eedf2b87a6df9344e`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:44:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:44:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 15:44:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:28:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:28:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 12 Oct 2021 16:28:21 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:28:21 GMT
ENV LANG=C.UTF-8
# Mon, 01 Nov 2021 18:50:17 GMT
ENV JAVA_VERSION=18-ea+21
# Mon, 01 Nov 2021 18:50:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/21/GPL/openjdk-18-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='c0a1fcdd389abdc8101892215f73413b10975f735f31e6d0484c9653fc9ba5e9'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/21/GPL/openjdk-18-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='a5ed86d5c7f9433360bc81b5b283d6b5fc345309d16c77125c8ceff32ed5c9a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 01 Nov 2021 18:50:29 GMT
CMD ["jshell"]
# Mon, 01 Nov 2021 19:39:18 GMT
ENV CLOJURE_VERSION=1.10.3.986
# Mon, 01 Nov 2021 19:39:18 GMT
WORKDIR /tmp
# Mon, 01 Nov 2021 19:39:29 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "f2a271d6892fb04f7377148f6770185486ca194245721ab34a62ae03e8d1149f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Mon, 01 Nov 2021 19:39:29 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cef1aa2170c001b320769bf8b018ed82d2c94a673e3010ea1ffe152e107419`  
		Last Modified: Tue, 12 Oct 2021 15:54:16 GMT  
		Size: 7.8 MB (7833862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a51f13be8e69cfc526b671d0bbf621b985b0932acd1523050e2995777b5926`  
		Last Modified: Tue, 12 Oct 2021 15:54:17 GMT  
		Size: 10.0 MB (9997204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def39d67a1a77adaac93be02cc61a57145a5a6273cd061d97660f30ef1e09bc1`  
		Last Modified: Tue, 12 Oct 2021 15:54:37 GMT  
		Size: 51.8 MB (51840680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6028bcac0bf13daf952fdab1ea1dc3341f884e2243e08aeace7206a75c9feb65`  
		Last Modified: Tue, 12 Oct 2021 16:43:50 GMT  
		Size: 13.9 MB (13921295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab5fe1454290004d1cebe69e0ae7e06ebd8c5a614ea3697558e7dfb9cf3e5aa`  
		Last Modified: Mon, 01 Nov 2021 18:58:57 GMT  
		Size: 188.2 MB (188236263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951848424c153e42165894547404deda7bd1a90128fe06a8be55f2c05754ea60`  
		Last Modified: Mon, 01 Nov 2021 19:47:04 GMT  
		Size: 27.9 MB (27929630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-tools-deps-1.10.3.986-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:55b0fdd5a326ba11149a621b15010641108d77aaf5510eb589c60b8c21293787
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.0 MB (347955905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0ed38afe0feadc9239ed28ed4bc96bbc806c84bdb19dfab073d1f18f286ed7c`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:59:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:59:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:00:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 04:07:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 04:07:15 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Sat, 16 Oct 2021 04:07:16 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Oct 2021 04:07:17 GMT
ENV LANG=C.UTF-8
# Mon, 01 Nov 2021 19:19:23 GMT
ENV JAVA_VERSION=18-ea+21
# Mon, 01 Nov 2021 19:19:37 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/21/GPL/openjdk-18-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='c0a1fcdd389abdc8101892215f73413b10975f735f31e6d0484c9653fc9ba5e9'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/21/GPL/openjdk-18-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='a5ed86d5c7f9433360bc81b5b283d6b5fc345309d16c77125c8ceff32ed5c9a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 01 Nov 2021 19:19:38 GMT
CMD ["jshell"]
# Mon, 01 Nov 2021 20:24:21 GMT
ENV CLOJURE_VERSION=1.10.3.986
# Mon, 01 Nov 2021 20:24:21 GMT
WORKDIR /tmp
# Mon, 01 Nov 2021 20:24:32 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "f2a271d6892fb04f7377148f6770185486ca194245721ab34a62ae03e8d1149f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Mon, 01 Nov 2021 20:24:33 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7324ea4098419bc5fa2ac5a138522230bf12cef3996d1740dd00f9d4737d004`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 7.7 MB (7695063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e213c33a07316d84d829be685bd3b02e1e2bc135f7748c932050e6ed6a3a0d3`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 9.8 MB (9767289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c82db586c3ef7a5c4716aeca2d6e779ec11c568c84c8ef7e6df7bd72512c80`  
		Last Modified: Sat, 16 Oct 2021 03:15:56 GMT  
		Size: 52.2 MB (52167277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca5f2ea6ae2690d6893716729208342b96e3108dcbbc9e492305d11869aa54e`  
		Last Modified: Sat, 16 Oct 2021 04:22:43 GMT  
		Size: 14.7 MB (14671047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb20e5eb8d79436d86b43ab5273b00adf57966130ee2142bbd833c2d4ef7f5b7`  
		Last Modified: Mon, 01 Nov 2021 19:32:50 GMT  
		Size: 187.2 MB (187160504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624c91572a428bf74834652d6bd94ec509a63800ae22f30cfb15644c03019f8`  
		Last Modified: Mon, 01 Nov 2021 20:35:59 GMT  
		Size: 27.3 MB (27271969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
