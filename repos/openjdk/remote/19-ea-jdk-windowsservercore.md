## `openjdk:19-ea-jdk-windowsservercore`

```console
$ docker pull openjdk@sha256:2e691ed82723a4154afcd57c17f77869984aa13f5cf7773d8944ccfa2b7c96f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `openjdk:19-ea-jdk-windowsservercore` - windows version 10.0.20348.643; amd64

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

### `openjdk:19-ea-jdk-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull openjdk@sha256:09175f597378d46aa3941df886490a5f4800535b9902b2802d2cf8a4d9211d58
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2906771985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64081bcac5783899493dbfc92f46a94de5f7193dfa1a847425285168f1f30ea1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 16:58:06 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Apr 2022 16:58:07 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 13 Apr 2022 16:59:01 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 07 May 2022 01:16:32 GMT
ENV JAVA_VERSION=19-ea+21
# Sat, 07 May 2022 01:16:33 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_windows-x64_bin.zip
# Sat, 07 May 2022 01:16:34 GMT
ENV JAVA_SHA256=8445436e394bb7413fb586515b5681989aafbcbf448616a1f850550b9d07da47
# Sat, 07 May 2022 01:18:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 07 May 2022 01:18:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25b7048e3be90e8d3856a943edfe91e214649883ffeabdf6fcebcea7b3053e2`  
		Last Modified: Tue, 19 Apr 2022 00:53:10 GMT  
		Size: 366.7 KB (366674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f218e98479db3f32c0db578928d63948fc1a4d83a3525921b9f9a7f4c999de53`  
		Last Modified: Tue, 19 Apr 2022 00:53:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4898bdb62896a1acbb34025e03c775d3d5f0f7299ae3f01875842d74e0e7984b`  
		Last Modified: Tue, 19 Apr 2022 00:53:10 GMT  
		Size: 322.4 KB (322423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ac2257d311eac5e1ffdf1d2ce3bb5ea26c3a2093b36557b0fc854e57d6349`  
		Last Modified: Sat, 07 May 2022 01:26:54 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbdccfbdde9b388d718d57e00bda3eb10c5b3954b226acf31d01ef72354e354`  
		Last Modified: Sat, 07 May 2022 01:26:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac671174b5cd9e0180818ccb5a8d6c64e09b40d82e8ed15d35f12850df116ec`  
		Last Modified: Sat, 07 May 2022 01:26:54 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f9e5f41b24f288c07be816cc21509dfcbf0d70c379e85b033cc2145e97c79d`  
		Last Modified: Sat, 07 May 2022 01:30:20 GMT  
		Size: 190.2 MB (190153991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bcc1d561dd154d0a850f559fd333d6014e32589ee5ff70ac4458dffa3002b2`  
		Last Modified: Sat, 07 May 2022 01:26:54 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
