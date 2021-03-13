## `clojure:openjdk-16-tools-deps-1.10.2.796-buster`

```console
$ docker pull clojure@sha256:5811900f81af9154d9b2f0d61c9d249040192d5f0b1c4d145a2a286e95c4584d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-16-tools-deps-1.10.2.796-buster` - linux; amd64

```console
$ docker pull clojure@sha256:ed1017fb9398b3dfb3981043597e90f6adc9db3046bd255375aad714068c6196
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.1 MB (350122161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1487913cec596de71eb9451074fd91610c1d8662987da00b9d588a59f62df8f6`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:35:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 20:56:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 20:59:40 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 09 Mar 2021 20:59:40 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:59:40 GMT
ENV LANG=C.UTF-8
# Tue, 09 Mar 2021 20:59:40 GMT
ENV JAVA_VERSION=16
# Tue, 09 Mar 2021 20:59:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-x64_bin.tar.gz'; 			downloadSha256='e952958f16797ad7dc7cd8b724edd69ec7e0e0434537d80d6b5165193e33b931'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-aarch64_bin.tar.gz'; 			downloadSha256='273d3ae0ff14af801c5ffa71fd081f1cc505354f308ce11c77af55302c83d2bf'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 20:59:50 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:52:35 GMT
ENV CLOJURE_VERSION=1.10.2.796
# Tue, 09 Mar 2021 21:52:35 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:52:46 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0ea8633c7f53eb76098132d4a4536169395be24bbdc253cff4d10251e2ea6e45 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Tue, 09 Mar 2021 21:52:47 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7467d1831b6947c294d92ee957902c3cd448b17c5ac2103ca5e79d15afb317c3`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 7.8 MB (7830684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab2c490a3cea21cc051ff29c33cc9857418edfa1be9966124b18abe1d5ae16`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 10.0 MB (9996459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15a0f46f8c38f4ca7daecf160ba9cdb3ddeafda769e2741e179851cfaa14eec`  
		Last Modified: Tue, 09 Feb 2021 04:46:23 GMT  
		Size: 51.8 MB (51830963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415655c50d52018d0916c838b59d5ee0a87aea61c2464768eae0a629075c7263`  
		Last Modified: Tue, 09 Mar 2021 21:10:07 GMT  
		Size: 13.9 MB (13921302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d07d50dc62b34aac5e18a83d03e0b853e2fc5137db535b427bac3911ef1a3b1`  
		Last Modified: Tue, 09 Mar 2021 21:14:25 GMT  
		Size: 184.9 MB (184888221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59d3522ab82e16cda091a3724b6a0ec7fffedef014c49d3fffe2db27d6fe114`  
		Last Modified: Tue, 09 Mar 2021 22:08:24 GMT  
		Size: 31.3 MB (31254334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-16-tools-deps-1.10.2.796-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ffce1171f71aecba8ad1def71c4cd36e2591e5beb85b1742d320218e95e9c3a4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343820873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098607601e26401b017f5206227eb75703d627100b33cdeebe54a60637218ea2`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:16 GMT
ADD file:b2e2cca51e131b97e6a7e02af893c7f9b1f7a491b3d5fdaafa80409ed248a706 in / 
# Fri, 12 Mar 2021 01:53:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:29:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:29:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:33:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:35:58 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Fri, 12 Mar 2021 06:35:59 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 06:36:00 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 06:36:00 GMT
ENV JAVA_VERSION=16
# Fri, 12 Mar 2021 06:36:56 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-x64_bin.tar.gz'; 			downloadSha256='e952958f16797ad7dc7cd8b724edd69ec7e0e0434537d80d6b5165193e33b931'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-aarch64_bin.tar.gz'; 			downloadSha256='273d3ae0ff14af801c5ffa71fd081f1cc505354f308ce11c77af55302c83d2bf'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 12 Mar 2021 06:36:58 GMT
CMD ["jshell"]
# Sat, 13 Mar 2021 01:08:32 GMT
ENV CLOJURE_VERSION=1.10.2.796
# Sat, 13 Mar 2021 01:08:33 GMT
WORKDIR /tmp
# Sat, 13 Mar 2021 01:08:56 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0ea8633c7f53eb76098132d4a4536169395be24bbdc253cff4d10251e2ea6e45 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Sat, 13 Mar 2021 01:08:58 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:e9742a63e95a88f8685c4f23a73f7dd15e4039ac1862ce5753c53406a5f7c04a`  
		Last Modified: Fri, 12 Mar 2021 02:01:14 GMT  
		Size: 49.2 MB (49195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90273c85fdda8648cee9282aa7b01faf0ec1f45451931985b3504c37cf1ac3e6`  
		Last Modified: Fri, 12 Mar 2021 02:43:30 GMT  
		Size: 7.7 MB (7694407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685f873e984153af9a44cf556c7679b430b9c557d901c7d476725134f28754e7`  
		Last Modified: Fri, 12 Mar 2021 02:43:30 GMT  
		Size: 10.0 MB (9984339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34041dfaf60ca49c213d83e89205fc2b7e222817c9728a4aa4f7d3f09d579c9`  
		Last Modified: Fri, 12 Mar 2021 02:43:54 GMT  
		Size: 52.2 MB (52165212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea7dd455a2166654bd3d729e78a91e18b7d2fb982780428bf02e0d1d700cb88`  
		Last Modified: Fri, 12 Mar 2021 06:44:30 GMT  
		Size: 14.7 MB (14673622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ced9001d9f355e3e501c1f689799841540890d3dad2b6ce4b80b4acf9f26e3b`  
		Last Modified: Fri, 12 Mar 2021 06:46:26 GMT  
		Size: 179.3 MB (179264185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca19345baf532823fe852a266471a73a518f582146d4d93353abc5c53d8843c`  
		Last Modified: Sat, 13 Mar 2021 01:20:16 GMT  
		Size: 30.8 MB (30843345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
