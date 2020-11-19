## `openjdk:8-jre`

```console
$ docker pull openjdk@sha256:315ebe39e23eb2aed74f218ec74d6f3b82309cd1a43811ea6188120df110e9d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `openjdk:8-jre` - linux; amd64

```console
$ docker pull openjdk@sha256:7ee341dd70298e4ad59e1c0c1b00648aaaa097a9e6f1ae1c66af1e4b9c473737
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115036673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f48bacf78ccd8e2c03d40daf4230adfa6a00e4d6b1fc9ebe630c2443382ca9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:58 GMT
ADD file:9a4fd72d749f4a791e75e0f6fc6028d0771e3381b6d84a8d0b07a4887bc7c641 in / 
# Tue, 17 Nov 2020 20:20:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:30:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:30:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 19 Nov 2020 03:06:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 03:06:45 GMT
ENV LANG=C.UTF-8
# Thu, 19 Nov 2020 03:07:31 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 19 Nov 2020 03:07:31 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 03:07:32 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 19 Nov 2020 03:07:32 GMT
ENV JAVA_VERSION=8u275
# Thu, 19 Nov 2020 03:07:38 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
```

-	Layers:
	-	`sha256:756975cb9c7e7933d824af9319b512dd72a50894232761d06ef3be59981df838`  
		Last Modified: Tue, 17 Nov 2020 20:27:06 GMT  
		Size: 50.4 MB (50397725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77915b4e630d47296770ce4cf481894885978072432456615172af463433cc5`  
		Last Modified: Wed, 18 Nov 2020 00:49:42 GMT  
		Size: 7.8 MB (7811717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f37a0a41b6b03489dd7de0aa2a79e369fd8b219bbc36b52f3f9790dc128e74b`  
		Last Modified: Wed, 18 Nov 2020 00:49:42 GMT  
		Size: 10.0 MB (9996233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713f7746108e0e07f616eec5ac22de7d9981c7e5087a3d63d92193b71d3e98e3`  
		Last Modified: Thu, 19 Nov 2020 03:12:18 GMT  
		Size: 5.5 MB (5529433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba38f0ad15ed007b8974fb97b174e2f3e0418a49a03c215e237812c058006714`  
		Last Modified: Thu, 19 Nov 2020 03:12:53 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef0ecdbb4512b269e1df4a3a65f0ff50bbfbdbfe16779256f3f3954f36eb61b`  
		Last Modified: Thu, 19 Nov 2020 03:12:58 GMT  
		Size: 41.3 MB (41301352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jre` - windows version 10.0.17763.1577; amd64

```console
$ docker pull openjdk@sha256:454a0881d85220bb74d33e2e6e5c937ddb8f649fe13682f7dae7d39599b0b68e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2440185913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03ecd3e5cf449013495ebff0cdcbd4e54e54daa06a20babf3ab846add2e0b4ed`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 18:13:44 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 Nov 2020 18:14:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Thu, 12 Nov 2020 01:34:35 GMT
ENV JAVA_VERSION=8u275
# Thu, 12 Nov 2020 01:39:04 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_windows_8u275b01.zip
# Thu, 12 Nov 2020 01:39:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961c113008286ec10d5b5ad6712c39a4f6893491652c16952e9ad9d6182a696d`  
		Last Modified: Wed, 11 Nov 2020 18:35:15 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4485491cb68a4d866c356a328fbcaa1122d7eb2ec55323238ff04c01659a1b49`  
		Last Modified: Wed, 11 Nov 2020 18:35:26 GMT  
		Size: 9.2 MB (9234346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be0d7b941c4cc39629a0b0f78c4aa565c0b1a7798acbfc5ec0365e62d0ea4c`  
		Last Modified: Thu, 12 Nov 2020 01:57:14 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c2156462c26adf9e5c781bce4bce636ac93cdd145e00d79dafb5ca633e195`  
		Last Modified: Thu, 12 Nov 2020 02:00:25 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140202478dc068edf29123898b136ea9b4633ef2c40268f842e48a5ce283b886`  
		Last Modified: Thu, 12 Nov 2020 02:00:31 GMT  
		Size: 42.9 MB (42917707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jre` - windows version 10.0.14393.4046; amd64

```console
$ docker pull openjdk@sha256:1655f064c3c6ad37b09d73ee5d4f89a519d5a10ab40ac5ac0e414815d23dc535
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5828887192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b37648db14645c5518fd7aac506c39e86e3343b1f2cc0140a79d62b03b0a7f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 18:15:40 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 Nov 2020 18:16:53 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Thu, 12 Nov 2020 01:36:01 GMT
ENV JAVA_VERSION=8u275
# Thu, 12 Nov 2020 01:39:55 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_windows_8u275b01.zip
# Thu, 12 Nov 2020 01:41:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864d6ab6d378108050bf02ccd849c38e57d78de73c9a59d83a550d004548aefe`  
		Last Modified: Wed, 11 Nov 2020 18:37:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699c3656ce68e9d61d5eddc7285fd7bd7cecaec9dbd0e3625290ecd2dfcf91d1`  
		Last Modified: Wed, 11 Nov 2020 18:37:40 GMT  
		Size: 10.1 MB (10080718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17338a5c062bee677d2a8a14e27c2dbeedb6b44519ba560b618b7f8c736bcdf4`  
		Last Modified: Thu, 12 Nov 2020 01:57:44 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18237a144c3efca51338810fbe94dee80183ca3805d7abd00a9ecee9a4894cbd`  
		Last Modified: Thu, 12 Nov 2020 02:00:42 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef729ad546f3ea1636ae1f90fd00345fa94ff0988c29b2a79b0137801634ed1`  
		Last Modified: Thu, 12 Nov 2020 02:00:51 GMT  
		Size: 48.2 MB (48243090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
