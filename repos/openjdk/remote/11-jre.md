## `openjdk:11-jre`

```console
$ docker pull openjdk@sha256:a76453fe16ca9d1de6334bed2664ab09b2475b5ebf20a09bc57da2ce4f5a2b9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1217; amd64
	-	windows version 10.0.14393.3686; amd64

### `openjdk:11-jre` - linux; amd64

```console
$ docker pull openjdk@sha256:68d29d2a9ee17a15d288368d2031bc9ffe40cbf85a92e1420696003e46a55262
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115670576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c62a3e565bdf8a3d47b57630baa52dca98c40019a64fbc15e4fef396afef482`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:28:12 GMT
ADD file:fb54c709daa205bf9d04eb3d90ba068db4c34dfe3b6ec0d7691f677286120903 in / 
# Fri, 15 May 2020 06:28:13 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:32:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:32:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 21:03:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 21:03:31 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 21:03:31 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 15 May 2020 21:03:31 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 21:03:32 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 15 May 2020 21:03:32 GMT
ENV JAVA_VERSION=11.0.7
# Fri, 15 May 2020 21:03:32 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Fri, 15 May 2020 21:03:33 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Fri, 15 May 2020 21:03:38 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
```

-	Layers:
	-	`sha256:376057ac6fa17f65688c56977118e2e764b27c348b3f70637fa829cd2a12b200`  
		Last Modified: Fri, 15 May 2020 06:37:20 GMT  
		Size: 50.4 MB (50391294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a63a0a859d859478f30461786a49c2fca3ae7d89ab5b5ce3c81c54951d30f88`  
		Last Modified: Fri, 15 May 2020 17:50:44 GMT  
		Size: 7.8 MB (7812354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496548a8c952b37bdf149ab3654f9085d721ee126b8c73b16860778be5137f5e`  
		Last Modified: Fri, 15 May 2020 17:50:49 GMT  
		Size: 10.0 MB (9996284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b2daf7a1b5f537cba1c514f668125cbe30051a963fceee666de62352eb49ca`  
		Last Modified: Fri, 15 May 2020 21:10:23 GMT  
		Size: 5.5 MB (5529320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8058d73803f3a05ad139e4bb713b7d93fb29f671441f1be35e844bb94a47152a`  
		Last Modified: Fri, 15 May 2020 21:10:22 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc4c151e7bebd2e3066851d6bc5ed2cfa0a9299b7e89cea9181a8994fa09abc`  
		Last Modified: Fri, 15 May 2020 21:10:31 GMT  
		Size: 41.9 MB (41941113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-jre` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:14fb742ef34eae112274d8dc9fafc66f6c36664763833d7cf36c4a1f11e9983e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113376095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:335e0bc5638237f89473413f6ef68c9c281f4bd1cb7079513a09a2bdb698fac1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:22 GMT
ADD file:c49818672222185a0a985a8511744bd524fce453bddb137364d79a793dc5740f in / 
# Thu, 23 Apr 2020 00:54:26 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:37:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:38:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 15:34:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 15:34:35 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 15:34:36 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 23 Apr 2020 15:34:36 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 15:34:38 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 23 Apr 2020 15:34:38 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 23 Apr 2020 15:34:39 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 23 Apr 2020 15:34:39 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 23 Apr 2020 15:34:46 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
```

-	Layers:
	-	`sha256:6243ff87266a170a3ad584d6c9c13f9b93c3aa84bded170c0040480f6c4e4170`  
		Last Modified: Thu, 23 Apr 2020 01:03:05 GMT  
		Size: 49.2 MB (49169698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0e7aea31e932e05b2ceba046f4e670116c0e81cfc82ca24a86a41afe7f0f98`  
		Last Modified: Thu, 23 Apr 2020 03:51:42 GMT  
		Size: 7.7 MB (7681533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ee43f3d2cbd321b8fb1657fed3947ec55776292d85377636a5fd3188d42662`  
		Last Modified: Thu, 23 Apr 2020 03:51:42 GMT  
		Size: 10.0 MB (9983945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4247e8f6079e1dba65270fa53de8ab1f2b0fc485ae079374161a4a8c1ea369`  
		Last Modified: Thu, 23 Apr 2020 15:37:28 GMT  
		Size: 5.5 MB (5504371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8414f9f82498dc70f256afd55017ea317f0ee6f51fa0c6da6a8978593fc3ac7`  
		Last Modified: Thu, 23 Apr 2020 15:37:27 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954bcc28920f4e35ea8b78e14c64742a7b9af1186b6d4a7d9cbce74900087f26`  
		Last Modified: Thu, 23 Apr 2020 15:37:38 GMT  
		Size: 41.0 MB (41036336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-jre` - windows version 10.0.17763.1217; amd64

```console
$ docker pull openjdk@sha256:2a9604a00515c7484f50f090968330bdf7977450b34a536d057a70b1088aa1f1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1758121973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a992be01cf6fbc79bc7299df0dc347022cd89fffc00739926adc57b408f97f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:41:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 15:40:36 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 May 2020 15:40:59 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 13 May 2020 15:41:00 GMT
ENV JAVA_VERSION=11.0.7
# Wed, 13 May 2020 15:48:27 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Wed, 13 May 2020 15:48:28 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Wed, 13 May 2020 15:49:19 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77613e754ba9d62c0acd4ef271c4ee7d3af091b8c8b310afa404560a9d281f82`  
		Last Modified: Wed, 13 May 2020 13:00:20 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d697ee5c17f7ca6807843cf1182f2fc6186e1ceed4d513fd1d2480fdd08cd975`  
		Last Modified: Wed, 13 May 2020 16:19:35 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72742d011d4f82aae552d0a2b889c3ad4ed50703ebf87b27dbef32ad34f0e83b`  
		Last Modified: Wed, 13 May 2020 16:19:35 GMT  
		Size: 344.8 KB (344830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38758fd508ad781bb829f0ee97740dca0afbcee534ba2d334b931a36615fb7c`  
		Last Modified: Wed, 13 May 2020 16:19:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f3a8912af6322d01c34419e9a96efee6954a126f3c3f30375c7af0c5138f48`  
		Last Modified: Wed, 13 May 2020 16:25:01 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28031e47998dfb67bf4a805403b42f228b1617f8c81de8799dc9e4abedf626d`  
		Last Modified: Wed, 13 May 2020 16:25:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e83d48456acb23c4b3520302ffcd0fb1e010aa0f4e06414d94aea41a1fe88c7`  
		Last Modified: Wed, 13 May 2020 16:25:53 GMT  
		Size: 39.4 MB (39438571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-jre` - windows version 10.0.14393.3686; amd64

```console
$ docker pull openjdk@sha256:463a66cdce99aadadc75cdff16daa553f7911fedea92a975b4a3c4bbf73b96d2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5781786581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a332a3f7c18c47219a0ad5656b36bc1cd6033adb904b7de48e5ee245e40109f2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 12:34:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 15:42:48 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 May 2020 15:43:56 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 13 May 2020 15:43:57 GMT
ENV JAVA_VERSION=11.0.7
# Wed, 13 May 2020 15:49:28 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Wed, 13 May 2020 15:49:29 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Wed, 13 May 2020 15:51:18 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e3e9730c43354781e87aa51e853bff3b1e8c1ca7004f527139638a8f9d499c49`  
		Last Modified: Wed, 13 May 2020 12:59:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03a8ddd05856ecb914de50f24a846537b197783d2b9f60aadfb9573645b7afb`  
		Last Modified: Wed, 13 May 2020 16:20:20 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c70a9045d85ecc0efcdbdaeb75c307f6d92fa9dd1d166d657b96f955e39652`  
		Last Modified: Wed, 13 May 2020 16:20:21 GMT  
		Size: 5.4 MB (5380742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2da38971daa12aa35d70397c906c439b294f4c1b6aadfd8b7cfd9b46c61ee4c`  
		Last Modified: Wed, 13 May 2020 16:20:17 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ba252fba4bd13ab6ae99f2e3e124788ac065b241562dce318cf14bcbfa5851`  
		Last Modified: Wed, 13 May 2020 16:26:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aeac771f5d300808a190f1dc8d1521b0a46bf81f9bdfa07b62b55c1ebb319f`  
		Last Modified: Wed, 13 May 2020 16:26:08 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068e4d652d4d74c152504c7dfc020be5052f659b993a6f43dd1521bffafae86`  
		Last Modified: Wed, 13 May 2020 16:26:54 GMT  
		Size: 44.5 MB (44510218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
