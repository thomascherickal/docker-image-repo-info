## `openjdk:19-ea-21-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:e97bb5c7161e754773acd45938f7e3f7d9f6b2c63e550e05f9798acc95125c0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `openjdk:19-ea-21-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull openjdk@sha256:a47257582555a77ffc03f0c9efab0e904b37301237dc8496633b7b39860b1bca
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2418527898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a42a22bfc378234bba04d9c6e6c41ace1bd69b98dc74753c2dfd9edb368f3af`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 16:55:44 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Apr 2022 16:55:45 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 13 Apr 2022 16:56:06 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 07 May 2022 01:15:04 GMT
ENV JAVA_VERSION=19-ea+21
# Sat, 07 May 2022 01:15:05 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_windows-x64_bin.zip
# Sat, 07 May 2022 01:15:06 GMT
ENV JAVA_SHA256=8445436e394bb7413fb586515b5681989aafbcbf448616a1f850550b9d07da47
# Sat, 07 May 2022 01:16:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 07 May 2022 01:16:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156288a763e09322f37d1214a5fcfaa1ebfbf8a108ee1351f5321537e137ef`  
		Last Modified: Tue, 19 Apr 2022 00:49:30 GMT  
		Size: 629.6 KB (629633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351bf1ac33e20763f11b363ce89dc94a0246c9fba4a48c2ad7f54cc49702ec37`  
		Last Modified: Tue, 19 Apr 2022 00:49:30 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48226228ba4f77ff2595c0eb2da5dbff7a0c255e2945283b32a4a6432b6a5c6`  
		Last Modified: Tue, 19 Apr 2022 00:49:30 GMT  
		Size: 559.7 KB (559710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e820539ed7ff263ca34c57bdae725d1b3c68b995d7751ab4e3d3afe023d89bb5`  
		Last Modified: Sat, 07 May 2022 01:23:19 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21b52783ccc04a16f39e2378a482dfdddb19e53c25a68dfaec3daaedc708684`  
		Last Modified: Sat, 07 May 2022 01:23:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e195e371e559652db6e1d943545190b65a237834eabb58ac74aa59304499ac3`  
		Last Modified: Sat, 07 May 2022 01:23:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d3f22f7948f8ccaad434122602ead270987236b4be78a6deed8d241d7b94c1`  
		Last Modified: Sat, 07 May 2022 01:26:33 GMT  
		Size: 190.4 MB (190375201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b616ee5fe33bb13081c55cc9e2825b0160ab445a3301e205f9218b3e7910c43`  
		Last Modified: Sat, 07 May 2022 01:23:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
