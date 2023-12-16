## `openjdk:22-jdk-windowsservercore`

```console
$ docker pull openjdk@sha256:a50eda3577b249f10eb21be440cd130076b71bd6aebcdd44f08168727c9c78c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `openjdk:22-jdk-windowsservercore` - windows version 10.0.20348.2159; amd64

```console
$ docker pull openjdk@sha256:5108e37312d8d57b1f367490d761c259096631f4308a06631a0abd85b90d64fe
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087855688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38f81ffe6720ddeb44b3308efa22acba5abbe0826dfec9159e42f9456ff30d0e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Fri, 15 Dec 2023 22:14:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 15 Dec 2023 22:14:16 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:14:17 GMT
ENV JAVA_HOME=C:\openjdk-22
# Fri, 15 Dec 2023 22:14:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:14:23 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 15 Dec 2023 22:14:24 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_windows-x64_bin.zip
# Fri, 15 Dec 2023 22:14:25 GMT
ENV JAVA_SHA256=522347f78607019a5c2d2478846c2ca0715ee700a7db3f78aff024e9935b1091
# Fri, 15 Dec 2023 22:15:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:15:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839fc47f6e056f9e09a214230f8b7115e69419dbc74acbbb1ad6bc0caa28862`  
		Last Modified: Tue, 12 Dec 2023 18:27:40 GMT  
		Size: 500.7 MB (500674814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469eae946945ee926852d89bdb55b3ff7c8fb84a8255432d184b1dca3c42ddae`  
		Last Modified: Fri, 15 Dec 2023 22:15:21 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a58e72de81796b9c7ccdfa55ca9e400dec7c20f216ba3b941bcaf673301a854`  
		Last Modified: Fri, 15 Dec 2023 22:15:21 GMT  
		Size: 504.1 KB (504050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ace084ec98d59e05cd39afdd8b0e5018c624ad6c1770afdd6d21259bc0eb89b`  
		Last Modified: Fri, 15 Dec 2023 22:15:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0969a116040f91ebab6e6be3237a287dee8db52d38187eced24f1d88ca789b`  
		Last Modified: Fri, 15 Dec 2023 22:15:21 GMT  
		Size: 356.0 KB (356043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a44fb5cb11c659b0e000e66fa7ef41a671a07932d6a18366dd6f128fce99c2f`  
		Last Modified: Fri, 15 Dec 2023 22:15:20 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9605a9702c25dd3c072a4d8ee07388f8cda99f4b46ff062c68db61d7d754b56`  
		Last Modified: Fri, 15 Dec 2023 22:15:20 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20858b9539a907011e3efb53da83b3da5f379128731585ed478cd982030d744e`  
		Last Modified: Fri, 15 Dec 2023 22:15:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbba622edc2ed253bea3da11fef94117ee80e630b1092458fc5b44f26e645597`  
		Last Modified: Fri, 15 Dec 2023 22:15:32 GMT  
		Size: 197.7 MB (197714102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10b1c0daec01c30d65bf5578997d41bb7445f1927c725cfe2b326c69ae0b6f`  
		Last Modified: Fri, 15 Dec 2023 22:15:20 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-jdk-windowsservercore` - windows version 10.0.17763.5206; amd64

```console
$ docker pull openjdk@sha256:5645c45accf8db625ce2600e4ec6fb88d7a48d80bc1ab9e9da14399c7eab4705
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258274569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd4fa34dcaea35d73a637057d30ede81abab87286c3961797da61593c6a162c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Fri, 15 Dec 2023 22:15:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 15 Dec 2023 22:16:23 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:16:24 GMT
ENV JAVA_HOME=C:\openjdk-22
# Fri, 15 Dec 2023 22:16:45 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:16:46 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 15 Dec 2023 22:16:46 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_windows-x64_bin.zip
# Fri, 15 Dec 2023 22:16:46 GMT
ENV JAVA_SHA256=522347f78607019a5c2d2478846c2ca0715ee700a7db3f78aff024e9935b1091
# Fri, 15 Dec 2023 22:17:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:17:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920fd32a001461d7c9331191a04c5a9e69424e94cb5633a07078ca1dab410d22`  
		Last Modified: Fri, 15 Dec 2023 22:17:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784b640e5ca3dd98cbc4e57493773e97299e88db7230c789fb49ea2013b47f2f`  
		Last Modified: Fri, 15 Dec 2023 22:17:31 GMT  
		Size: 500.4 KB (500415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d511c2f122a81118bfe6d2cb580b4c320e17ab1b9998790e1a5ecff74f7f031d`  
		Last Modified: Fri, 15 Dec 2023 22:17:31 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef706a4276fa8f38ec1bc6992082af0bdf9597a4e42295f8bfdccdd387b27d33`  
		Last Modified: Fri, 15 Dec 2023 22:17:32 GMT  
		Size: 344.7 KB (344690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d2e2e0d5c08e58029c8c15fcbdf48a4e8fb66c488850f2fd1d0a691ea313bc`  
		Last Modified: Fri, 15 Dec 2023 22:17:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3664bd7324f9dbba04161398d494adc2a50efe641f2ac1b136c5c2adda0c2bd`  
		Last Modified: Fri, 15 Dec 2023 22:17:30 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf3044eac13c2e7115315b2318fc0c20cb67967efbca69130bb74395eea256a`  
		Last Modified: Fri, 15 Dec 2023 22:17:30 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cad8a06bf5c36b555afcd6d427b797e071e0ba609257652e6004e3d5e1966c`  
		Last Modified: Fri, 15 Dec 2023 22:17:42 GMT  
		Size: 197.7 MB (197712226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2927a6c56e0649525eb61aea9236ac43162fc84f3436dd1f08fd2138fe3b6151`  
		Last Modified: Fri, 15 Dec 2023 22:17:30 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
