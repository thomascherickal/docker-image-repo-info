## `openjdk:22-jdk-bullseye`

```console
$ docker pull openjdk@sha256:ac64352f1e44b89c2e121653a59d7670c75127a9e1a93db0217484598d08b137
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `openjdk:22-jdk-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:fffa442d1e14368020593d147f6e974d8f5a1a330f8f6683a9b029bbffb5b467
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.3 MB (342329137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5507b134becbad203ee38d4999389764da9db809eddb73d8295984db83d84d`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:54:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 08 Dec 2023 19:48:25 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Dec 2023 19:48:25 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7b1e60e9d5a0f16eb1f998245666f7a64a44f8b1f2317bd31e8a658150c23d3`  
		Last Modified: Tue, 21 Nov 2023 10:02:45 GMT  
		Size: 54.6 MB (54595728 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:297f281b63ad85def56078fb60e9d7ffabb4e1383341864e4d4367a7672f9d87`  
		Last Modified: Fri, 15 Dec 2023 22:05:50 GMT  
		Size: 14.1 MB (14073046 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c0547d73925a5b7056213eb56c897000d0b344baf320aa618a5789a3cc44c52`  
		Last Modified: Fri, 15 Dec 2023 22:05:53 GMT  
		Size: 202.8 MB (202838213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-jdk-bullseye` - unknown; unknown

```console
$ docker pull openjdk@sha256:b25e8aca6c6e6b49a2e6613f2c38cc1bab71f75cf5f70ee91b26a81df16f9175
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6974959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a20f27bacbaad89c6581f98ab2300b5d5a9795ccd3e2cbef154120bfa0385dfd`

```dockerfile
```

-	Layers:
	-	`sha256:8fc109eea625e20a30144c7db19909e12e3af55e2225c6f4e6cec64437e46801`  
		Last Modified: Fri, 15 Dec 2023 22:05:50 GMT  
		Size: 7.0 MB (6956052 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:10118fc60e61520110423b0d3c0440a916bc27b73a0cc600a5a7e313fe638c1c`  
		Last Modified: Fri, 15 Dec 2023 22:05:49 GMT  
		Size: 18.9 KB (18907 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:22-jdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:2a6247bc7b32321b0255aa69e8fa9a61c517e70132c01a05867b41d706928234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.6 MB (340575202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45d4a1ff02bdd8a5a410d1d352f9595ec6e7e7511e56255d7062744d0b2836f2`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:59:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 08 Dec 2023 19:48:25 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Dec 2023 19:48:25 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1e860a4a6ca9e583881322c2e78baef1911e4d61bc607563e8ad9891e2d91f9`  
		Last Modified: Tue, 21 Nov 2023 08:07:01 GMT  
		Size: 15.8 MB (15750113 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1a9d2006a8ea812285a7be34dfc82465b2a592d6217f4d385d373c298de4642`  
		Last Modified: Tue, 21 Nov 2023 08:07:16 GMT  
		Size: 54.7 MB (54700129 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebc85cb84d79c3e3594b521045571bbae857e3a968aea20d3f8da0ccc3b21b10`  
		Last Modified: Fri, 15 Dec 2023 23:24:25 GMT  
		Size: 15.5 MB (15527435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b6c8511c27759a843df14a7ac5f55e8163c081cdbd08f94888f5fd87b28f3e0`  
		Last Modified: Fri, 15 Dec 2023 23:30:45 GMT  
		Size: 200.9 MB (200889653 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-jdk-bullseye` - unknown; unknown

```console
$ docker pull openjdk@sha256:e77bfba7b3038e5fe39e7e13d8172b15971ae311204e82515f3b46666034e704
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7062124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab30bc71f4942735f19062dba2a1dfed00c6430f548375e9b59ecaebd0776461`

```dockerfile
```

-	Layers:
	-	`sha256:26b3220137b3edff906d794376e87a15871c689fbb3f1443cd26781ffb4fad31`  
		Last Modified: Fri, 15 Dec 2023 23:30:39 GMT  
		Size: 7.0 MB (7043700 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:59d7629d0942af87e3dbcd70c506cef49d744ffe978757b8fd4be8126e2ffe23`  
		Last Modified: Fri, 15 Dec 2023 23:30:39 GMT  
		Size: 18.4 KB (18424 bytes)  
		MIME: application/vnd.in-toto+json
