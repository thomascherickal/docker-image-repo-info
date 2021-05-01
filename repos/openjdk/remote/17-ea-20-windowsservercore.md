## `openjdk:17-ea-20-windowsservercore`

```console
$ docker pull openjdk@sha256:f8cee47d2a96b0180f757725753e2c5c8427611654a7c22086c7e395f15c69cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `openjdk:17-ea-20-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull openjdk@sha256:c496db7cd58ad55c78d2bf73024eb1a2703e5c4ed7c1d40b47071bef376f6502
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2656511521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd95a16c91d0d2071d4931f4d0670dd74994ad95d4e9c83ef31cc9f7575162c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 16:45:00 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Apr 2021 16:45:01 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Apr 2021 16:45:32 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 30 Apr 2021 21:15:26 GMT
ENV JAVA_VERSION=17-ea+20
# Fri, 30 Apr 2021 21:15:27 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_windows-x64_bin.zip
# Fri, 30 Apr 2021 21:15:27 GMT
ENV JAVA_SHA256=dc5e49aa398cd724454363f811da6a3e1c33c484b5fd72c350468cdec4ed2f65
# Fri, 30 Apr 2021 21:16:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 30 Apr 2021 21:16:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3d005d273e9763b53b5f1034b1284bcce913f8dbd1855d70f561efc09be849`  
		Last Modified: Wed, 14 Apr 2021 17:36:21 GMT  
		Size: 5.1 MB (5074608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ab40deb7e8f2f68f8ddebdcf9a4ccf7112615246fd6c75d400cd491cdac535`  
		Last Modified: Wed, 14 Apr 2021 17:36:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3fa76ecf2e81ab47fe24f1aeab9427a58be444cc60cf90038197c769d046a0`  
		Last Modified: Wed, 14 Apr 2021 17:36:21 GMT  
		Size: 319.5 KB (319514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9879a084f33e9060917429f103c2af303a182286673c6088b8eeffa770d808dd`  
		Last Modified: Fri, 30 Apr 2021 21:24:54 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0162e852ed74e90c499becbc3527efb4f1cf401ad3d7c8430dd5bf492d1b33`  
		Last Modified: Fri, 30 Apr 2021 21:24:54 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fac70cfd78095624f4d92ee03cfabbc18d4a085a74a2f3b30255bafee93fb4`  
		Last Modified: Fri, 30 Apr 2021 21:24:54 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6370414fff3baf42f55452f9b40d3f167947481783e5b00f0730e60ffda7de46`  
		Last Modified: Fri, 30 Apr 2021 21:25:16 GMT  
		Size: 181.4 MB (181355013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bfc4fc22e8f4b6d36fe6c32558c9d8447ec1e7a8447b55593c817f8c0c93a`  
		Last Modified: Fri, 30 Apr 2021 21:24:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-20-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull openjdk@sha256:64ad61fab5e47a71c4a2ed828521df7c065e312b8afc9046842e1b516f1db874
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5992747280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84a3a61a231d1187a0f550813960776238571c6b247b5039e152cbe2b51302a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 16:48:32 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Apr 2021 16:48:33 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Apr 2021 16:50:24 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 30 Apr 2021 21:16:51 GMT
ENV JAVA_VERSION=17-ea+20
# Fri, 30 Apr 2021 21:16:52 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_windows-x64_bin.zip
# Fri, 30 Apr 2021 21:16:53 GMT
ENV JAVA_SHA256=dc5e49aa398cd724454363f811da6a3e1c33c484b5fd72c350468cdec4ed2f65
# Fri, 30 Apr 2021 21:18:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 30 Apr 2021 21:18:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e39566a6e39d3a16eac2642132dd97b58680502417c33529cb3b20734e62ffd`  
		Last Modified: Wed, 14 Apr 2021 17:37:12 GMT  
		Size: 5.6 MB (5648642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501b89977f05abcd65cccdbfec96af4495b33ee4acc7932a4bf2a77874b2d40`  
		Last Modified: Wed, 14 Apr 2021 17:37:09 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e79ef171c9bf6c1503c79940d0393f3121096ad7a3a91bc2d65c511c78175e8`  
		Last Modified: Wed, 14 Apr 2021 17:37:11 GMT  
		Size: 5.6 MB (5595448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72f30b2a2e44d123d89a3a4eabad9e86f7799cee2c2de61a9ae4345c992c0b5`  
		Last Modified: Fri, 30 Apr 2021 21:25:38 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5978d30d2ef0e9dbe7d2467c3778c9548df6c6d8b80d5463a535b49304e68855`  
		Last Modified: Fri, 30 Apr 2021 21:25:38 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0fa34f2bd5a759cb5c6dbfc7638f8bbe8cdc0fd80613fea4a78020300f26a4`  
		Last Modified: Fri, 30 Apr 2021 21:25:38 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a3fd91ec4d2a5a3688139bd7168cfba42e0aa6358b3bfcaabfdb367675e947`  
		Last Modified: Fri, 30 Apr 2021 21:25:59 GMT  
		Size: 186.6 MB (186610858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3705bbc87ee897ce4613b485eac3a3fe96c65cc3e2666d900238acae6f066f4`  
		Last Modified: Fri, 30 Apr 2021 21:25:38 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
