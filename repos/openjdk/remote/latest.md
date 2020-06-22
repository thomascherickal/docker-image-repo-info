## `openjdk:latest`

```console
$ docker pull openjdk@sha256:802e85bf23de5af422f63fedfb01554898de31830a99cf87d7ddb8331a1d3274
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `openjdk:latest` - linux; amd64

```console
$ docker pull openjdk@sha256:f43d68430b197ef5eb66a0d90e3844115d332a91e9d8d5f5a303c125f86ba52c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.4 MB (257370984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dee15a342cac109255097c908378f6e84245ad22c588809105911dcac54f860e`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Wed, 10 Jun 2020 18:22:32 GMT
ADD file:79bb5b8b89fe54ba99fd9d42d4f8774bfb9c1319ac3ead17a2005a3bde852451 in / 
# Wed, 10 Jun 2020 18:22:32 GMT
CMD ["/bin/bash"]
# Wed, 10 Jun 2020 18:39:27 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 10 Jun 2020 18:39:28 GMT
ENV LANG=en_US.UTF-8
# Wed, 10 Jun 2020 18:40:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-14
# Wed, 10 Jun 2020 18:40:21 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 18:40:21 GMT
ENV JAVA_VERSION=14.0.1
# Mon, 22 Jun 2020 20:23:17 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk14.0.1/664493ef4a6946b186ff29eb326336a2/7/GPL/openjdk-14.0.1_linux-x64_bin.tar.gz; 			downloadSha256=22ce248e0bd69f23028625bede9d1b3080935b68d011eaaf9e241f84d6b9c4cc; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java --version; 	javac --version
# Mon, 22 Jun 2020 20:23:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fa926a7d213a8145d6a906d68a085b21909a4b26871f142804e68b322bf8881f`  
		Last Modified: Wed, 10 Jun 2020 18:23:43 GMT  
		Size: 43.5 MB (43457466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22aed8993d2fb0bb3a658c631a1dfbd05c0e5d42218f419d18238996bd06ea08`  
		Last Modified: Wed, 10 Jun 2020 18:42:25 GMT  
		Size: 14.8 MB (14760261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82415e630b3538e083d5ce5e9a20e5e55d7878e9daa01efd09fbaba620a989b8`  
		Last Modified: Mon, 22 Jun 2020 20:27:41 GMT  
		Size: 199.2 MB (199153257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:latest` - windows version 10.0.17763.1282; amd64

```console
$ docker pull openjdk@sha256:4995cbd80788700220e6532d0d871fa7dca08999f247c141954891cde7b92874
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2493218856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5706efd86a84af36e20d71d1aea7cb5e2e22a8127dbdd33721acdb8c2ef7703a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 09 Jun 2020 22:34:11 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 09 Jun 2020 22:44:26 GMT
ENV JAVA_HOME=C:\openjdk-14
# Tue, 09 Jun 2020 22:44:50 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 09 Jun 2020 22:44:50 GMT
ENV JAVA_VERSION=14.0.1
# Tue, 09 Jun 2020 22:44:51 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk14.0.1/664493ef4a6946b186ff29eb326336a2/7/GPL/openjdk-14.0.1_windows-x64_bin.zip
# Tue, 09 Jun 2020 22:44:52 GMT
ENV JAVA_SHA256=26255f3f2fe7168ec0dce9d9f3825649c18540ba86279a7506c7f17dd3e537f9
# Tue, 09 Jun 2020 22:46:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 09 Jun 2020 22:46:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d8ec06304524cdb2b900879af7ed2db71d5e36e5f2306b46859250255390d`  
		Last Modified: Tue, 09 Jun 2020 23:17:51 GMT  
		Size: 4.8 MB (4765053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1cd1e30100fcdafa1c863d0c55f1cd8da38a93c7b2ec0de93e7069f60c466b`  
		Last Modified: Tue, 09 Jun 2020 23:23:05 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854cd79c2af1ace701acd352328961214b4a245ffa4f7e3f92c85e7760931366`  
		Last Modified: Tue, 09 Jun 2020 23:23:05 GMT  
		Size: 289.9 KB (289911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1149060594298e158344ea6679ac552ce84a4d569e4d59e5733322cd2dfba3ed`  
		Last Modified: Tue, 09 Jun 2020 23:23:03 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de6e36cf814a0af3f619cf6aaf64a933ff89769f3fe034f594526cdacc954be`  
		Last Modified: Tue, 09 Jun 2020 23:23:02 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3588db0a22b21319b168097d1043db6cf5556674cae8c472f305e537d9bdb9f`  
		Last Modified: Tue, 09 Jun 2020 23:23:02 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a691f020d33126fc477cd0dfccd4e07a8e0d4d19f7b072320aba8156570435`  
		Last Modified: Tue, 09 Jun 2020 23:23:22 GMT  
		Size: 194.2 MB (194243056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8670c17caac3f21f4385314fa111b6bd731be0d2b38b5386bf7a339f447ca203`  
		Last Modified: Tue, 09 Jun 2020 23:23:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:latest` - windows version 10.0.14393.3750; amd64

```console
$ docker pull openjdk@sha256:53ad3a03b2fb240b6c494339821e6638cd44c989bcf26ec4d51a6a52f7518c1d
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5944087908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0374e9876c019fa7eedb6f72885e430683752a03f973173a5222d979847f0ca5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 09 Jun 2020 22:38:24 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 09 Jun 2020 22:46:38 GMT
ENV JAVA_HOME=C:\openjdk-14
# Tue, 09 Jun 2020 22:48:02 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 09 Jun 2020 22:48:03 GMT
ENV JAVA_VERSION=14.0.1
# Tue, 09 Jun 2020 22:48:04 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk14.0.1/664493ef4a6946b186ff29eb326336a2/7/GPL/openjdk-14.0.1_windows-x64_bin.zip
# Tue, 09 Jun 2020 22:48:05 GMT
ENV JAVA_SHA256=26255f3f2fe7168ec0dce9d9f3825649c18540ba86279a7506c7f17dd3e537f9
# Tue, 09 Jun 2020 22:50:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 09 Jun 2020 22:50:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20399ac1a4e75ca1edbca4b2438a810ea66dbe6bdd128414ab987881b5ed641`  
		Last Modified: Tue, 09 Jun 2020 23:18:34 GMT  
		Size: 5.4 MB (5393368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5700b3b478012f44dcea5290744706546d56c75814e32e0445454ae3305553bc`  
		Last Modified: Tue, 09 Jun 2020 23:23:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb40f628ad8e35c2287456c5ef3851a53c4214f32fa70c71aba9b083ecdc223`  
		Last Modified: Tue, 09 Jun 2020 23:23:53 GMT  
		Size: 5.4 MB (5366819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5281de3fb51d4f84dd759c54d9f2c072f0fa2b0843a10ce35de72c7bc329a0`  
		Last Modified: Tue, 09 Jun 2020 23:23:48 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a34cf5d8f174d4ba0022f3370d972e15feef72b6ece08bd081d6e334075988`  
		Last Modified: Tue, 09 Jun 2020 23:23:48 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711926fbbbf4e9a886557be4eec5cfa9726813ecc4ab5c58f4817b538e54eb27`  
		Last Modified: Tue, 09 Jun 2020 23:23:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c5882b12fb7972b4c6e2d4ff309624867d118af7c27e5b59cefe064110eaa1`  
		Last Modified: Tue, 09 Jun 2020 23:24:09 GMT  
		Size: 199.3 MB (199323198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bb24c70b5b6ddd0ea00261b7094028bf434f954eb77b24bbff1ea1980a9c1a`  
		Last Modified: Tue, 09 Jun 2020 23:23:48 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
