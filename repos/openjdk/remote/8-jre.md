## `openjdk:8-jre`

```console
$ docker pull openjdk@sha256:15e26185a7f4af3d9cbff470cd83a6afed53594816dd6aa8681896236f544abf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `openjdk:8-jre` - linux; amd64

```console
$ docker pull openjdk@sha256:efbc039452d932e5d0cb5f1851ee68bec8f0856d363eab96d3619589bf1ce511
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.0 MB (117955465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d073328e94a87ac7c43965a572ef0a658175c3bdc332757abb5da1d1973e1578`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:30 GMT
ADD file:aea313ae50ce6474a3df142b34d4dcba4e7e0186ea6fe55389cb2ea903b9ebbb in / 
# Tue, 12 Oct 2021 01:20:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:42:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 16:34:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:36:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 12 Oct 2021 16:36:57 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 12 Oct 2021 16:36:58 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:36:58 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:36:58 GMT
ENV JAVA_VERSION=8u302
# Tue, 12 Oct 2021 16:37:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
```

-	Layers:
	-	`sha256:bb7d5a84853b217ac05783963f12b034243070c1c9c8d2e60ada47444f3cce04`  
		Last Modified: Tue, 12 Oct 2021 01:25:37 GMT  
		Size: 54.9 MB (54917520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02b617c6a8c415a175f44d7e2c5d3b521059f2a6112c5f022e005a44a759f2d`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 5.2 MB (5153273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32e17419b7ee61bbd89c2f0d2833a99cf45e594257d15cb567e4cf7771ce34a`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 10.9 MB (10871935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab18cfab55f9b2e1184b3f5b90de6574c96bdf1c4c782f4e1879437c38541af9`  
		Last Modified: Tue, 12 Oct 2021 16:53:01 GMT  
		Size: 5.7 MB (5653928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793716e93ecb3dc756176dea4353c0fd34b83be7fe04582df89283781c0e2bdf`  
		Last Modified: Tue, 12 Oct 2021 16:56:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7471530a63ae5624808eb1ddc31e1f84a0c041ffb879f79f9c106ade1d41dd2a`  
		Last Modified: Tue, 12 Oct 2021 16:56:24 GMT  
		Size: 41.4 MB (41358598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jre` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:676ad89b58c8324622a370b128d8c8f5ca38284a4a4f80ab0b53889fc4f81be6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115881116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924a8aea1e6cb4d618f95d715d149faba63ae9b44c014ca085f2465384e72df2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:04 GMT
ADD file:1529ae12e334fd992892d3fb97c103297cff7e0115b0475bec4c093939a2bff7 in / 
# Tue, 12 Oct 2021 01:41:04 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:10:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:10:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 06:11:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:15:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 13 Oct 2021 06:15:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 13 Oct 2021 06:15:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:15:16 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 06:15:17 GMT
ENV JAVA_VERSION=8u302
# Wed, 13 Oct 2021 06:15:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
```

-	Layers:
	-	`sha256:1c47a423366578e5ce665d03788914bf0459485a627a27896fa9c5663ce55cdf`  
		Last Modified: Tue, 12 Oct 2021 01:47:41 GMT  
		Size: 53.6 MB (53603015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580c36351f836fd83ee4aee909834823b15f90ce0ec580f869717dc3679a020b`  
		Last Modified: Tue, 12 Oct 2021 02:18:53 GMT  
		Size: 5.1 MB (5142731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b655be758028f8234aab1f828dc2f79ee5abf3ce0a85560430b5f7c806367d1`  
		Last Modified: Tue, 12 Oct 2021 02:18:53 GMT  
		Size: 10.9 MB (10872848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685e801adad0b6a144db48e53949b8f0c2e7eb8cd8e802e8e667ccfe21d8df8d`  
		Last Modified: Wed, 13 Oct 2021 06:41:02 GMT  
		Size: 5.6 MB (5647116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc8df60f4347accf6231ab821581ec184b7b4fc3e55b6f1136c3a7e35412827`  
		Last Modified: Wed, 13 Oct 2021 06:45:36 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aba2616e7c28e15cb64bbfc3e1d8e73ad5e968b2c8ff3291eaed537b9c27af7`  
		Last Modified: Wed, 13 Oct 2021 06:45:42 GMT  
		Size: 40.6 MB (40615195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jre` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:adbf2086f0ba395e000cce9bd343d442c0592e4d886799612d44ec04272de06a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2725548954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58c79f0c229a98bb83dd0a47a3e37f6a89ed1e5e179a4a556e8df0d21d7b5ecc`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 00:31:04 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 01:03:45 GMT
ENV JAVA_HOME=C:\openjdk-8
# Thu, 14 Oct 2021 01:04:55 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 01:04:56 GMT
ENV JAVA_VERSION=8u302
# Thu, 14 Oct 2021 01:10:05 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_windows_8u302b08.zip
# Thu, 14 Oct 2021 01:11:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3778f0ab9c363534bcf1068a50329066ca025f6499401dd667a232ffdd9687e4`  
		Last Modified: Sat, 16 Oct 2021 00:35:18 GMT  
		Size: 349.3 KB (349328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562322d8904b5f4201b83a278bcad8ac93931de36ab6d4f4fc398938e1793828`  
		Last Modified: Sat, 16 Oct 2021 00:49:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c83dfb5768f71697f2053162176ba51b0c34f3835fc4cc567bbd96c74d1c32`  
		Last Modified: Sat, 16 Oct 2021 00:49:47 GMT  
		Size: 312.4 KB (312377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3fcc2d803f1a7cc121d85237b2c97637d0024479cdd22d614ee2555aac3e33`  
		Last Modified: Sat, 16 Oct 2021 00:49:47 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7932ab186011f3cd2d376f0a91553a2866f3a10059b69270e9326e765bd15d4`  
		Last Modified: Sat, 16 Oct 2021 00:52:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed95b4cc77ccabaa4c35601f88b8568ae91dd503b5cad0e94e9985eb96ac062`  
		Last Modified: Sat, 16 Oct 2021 00:52:52 GMT  
		Size: 38.6 MB (38562780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jre` - windows version 10.0.14393.4704; amd64

```console
$ docker pull openjdk@sha256:5e95e30812221ae959acf1196b0f339ab3b82d33a3d1674bf4cec0c5af140e32
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6312039108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0524d3ae56a7babbeabe2c4c5801b96873ba1638b252bafdee24f1a4bd97e7e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 12:40:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 00:35:32 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 01:06:30 GMT
ENV JAVA_HOME=C:\openjdk-8
# Thu, 14 Oct 2021 01:07:35 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 01:07:36 GMT
ENV JAVA_VERSION=8u302
# Thu, 14 Oct 2021 01:11:32 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_windows_8u302b08.zip
# Thu, 14 Oct 2021 01:12:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6974b1bd85ba3f9ce16d86231eced43f720fed9c13411d37584dfe7193bcde60`  
		Last Modified: Wed, 13 Oct 2021 13:27:57 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df06f60babff5e4f22bec0a3230e7cb06b975eee8a07f9541607a63c6f54ec1`  
		Last Modified: Sat, 16 Oct 2021 00:35:57 GMT  
		Size: 352.3 KB (352290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0c4d3b2ec873e55c039f51a197f4de61458d4f05a18fbc82eeebe00b1b5886`  
		Last Modified: Sat, 16 Oct 2021 00:50:13 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8b9c7731d764fa4e12975893be5abd39526f8ecc73b00ad2113009751e70c`  
		Last Modified: Sat, 16 Oct 2021 00:50:13 GMT  
		Size: 348.4 KB (348382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4ce1dccba2a2d699f13b831ecba8da857b410a935538aa72a3bf38bbe251f6`  
		Last Modified: Sat, 16 Oct 2021 00:50:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf32e9a46c96a9dceacc27a86efec66f50f97e76536df2c107414360539a6aa`  
		Last Modified: Sat, 16 Oct 2021 00:53:06 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c15710c1dfa3b56cfb23d30a34920c041f3b85519e20088ff0ef77b6bf623c3`  
		Last Modified: Sat, 16 Oct 2021 00:53:12 GMT  
		Size: 38.6 MB (38566351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
