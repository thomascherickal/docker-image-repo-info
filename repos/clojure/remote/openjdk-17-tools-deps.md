## `clojure:openjdk-17-tools-deps`

```console
$ docker pull clojure@sha256:94ae79913b5822703125ca4d9ec086eddffd63f2c6e5e51d348c44169201987d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-tools-deps` - linux; amd64

```console
$ docker pull clojure@sha256:cc8ef41a950aab5172fa547868a1ea805b2f2b20c4014f5ac1c80a43a19ab15c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.3 MB (256348694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa170292282f5fdbfdd41f5cdb150e99b88be46c2f541831466331414c3ae17`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 13:33:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:34:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Thu, 22 Jul 2021 13:34:21 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:34:21 GMT
ENV LANG=C.UTF-8
# Fri, 30 Jul 2021 18:51:00 GMT
ENV JAVA_VERSION=17-ea+33
# Fri, 30 Jul 2021 18:51:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/33/GPL/openjdk-17-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='d89e04f161553560c454bf263924dc49c5c2529698ef8131baff632355baea18'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/33/GPL/openjdk-17-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='d361654c87bae6712f36d7f0d27914c63fbe31f10a9a0d5316072b3c69ed2263'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 30 Jul 2021 18:51:14 GMT
CMD ["jshell"]
# Fri, 30 Jul 2021 20:22:24 GMT
ENV CLOJURE_VERSION=1.10.3.933
# Fri, 30 Jul 2021 20:22:24 GMT
WORKDIR /tmp
# Fri, 30 Jul 2021 20:22:40 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0559cc25d08c3c25c3c0b734aba3a6c80f9b5d2760fdbddf08a4df886873528e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 30 Jul 2021 20:22:41 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d5ef013a6164e3b6c391252d0a26dbd18a3c564f734d771b4033a83f6d84a9`  
		Last Modified: Thu, 22 Jul 2021 13:43:45 GMT  
		Size: 3.3 MB (3268756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b3fbe93f72c0ef70aaae3d0ef6d42330d8aebfbcff151eafc291d117e24a4a`  
		Last Modified: Fri, 30 Jul 2021 19:01:10 GMT  
		Size: 187.5 MB (187515558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300ba801eb84bfc01212b7ab5be51f14fa4c9218514ff3d959fd5949cd71af43`  
		Last Modified: Fri, 30 Jul 2021 20:28:32 GMT  
		Size: 38.4 MB (38418585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-tools-deps` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c2fd29566e7388486c9a4a140a22ecb715ceab33042e97835f835f6478e70f79
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.2 MB (253247427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15b8574e3839f4a52fef6bb6926ab7b01edf052be4a93f86075b32f77fd94f94`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 05:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 05:16:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Thu, 22 Jul 2021 05:16:48 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 05:16:48 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 18:50:04 GMT
ENV JAVA_VERSION=17-ea+32
# Fri, 23 Jul 2021 18:50:16 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/32/GPL/openjdk-17-ea+32_linux-x64_bin.tar.gz'; 			downloadSha256='9e5b6c4e27d2adda491036edeed79fafea2961c78a96265a34dd4bb82d7bbf0b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/32/GPL/openjdk-17-ea+32_linux-aarch64_bin.tar.gz'; 			downloadSha256='28445241fd8ac0a8572f1dc202f7b492389c3a28d510b8c23cf7538a53b17eab'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jul 2021 18:50:17 GMT
CMD ["jshell"]
# Fri, 23 Jul 2021 19:56:38 GMT
ENV CLOJURE_VERSION=1.10.3.855
# Fri, 23 Jul 2021 19:56:39 GMT
WORKDIR /tmp
# Fri, 23 Jul 2021 19:56:54 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4bafe3c7343b7d4ef44bd0145bf4203be1c144a30d99a1db53ab67abb2568e2b *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 23 Jul 2021 19:56:55 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e464611cad28e3191fb5458b5b6b9bbcfd879d9863a4aa29debea8bf188cc100`  
		Last Modified: Thu, 22 Jul 2021 05:30:12 GMT  
		Size: 3.1 MB (3118880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4923092351acf021bf904e2a6008cd0998b7a0fb343bb3869d5223d96a01944e`  
		Last Modified: Fri, 23 Jul 2021 19:02:57 GMT  
		Size: 186.3 MB (186310233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd562cfe0d0b08facfb632e7791140cdd1612a078d3851076b8b7b195e6f9a8`  
		Last Modified: Fri, 23 Jul 2021 20:02:21 GMT  
		Size: 37.9 MB (37903520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
