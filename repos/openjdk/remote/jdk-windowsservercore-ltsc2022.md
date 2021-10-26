## `openjdk:jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:41575574cc7b1bd7d3866db879d94fd1572cbe16fe19f19e39dcb274ee90e01e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.288; amd64

### `openjdk:jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.288; amd64

```console
$ docker pull openjdk@sha256:23090965885da7d97277212b4fe8d7a7f3974a8319d3813f53b9aa62da8112a2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2325346439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce45e8bdee7982bb0a3cfb1bb5e90a0afda17591ed63b6123b3e62e6b35affd2`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 07 Oct 2021 11:33:56 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Oct 2021 12:26:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 25 Oct 2021 23:16:39 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Mon, 25 Oct 2021 23:18:54 GMT
ENV JAVA_HOME=C:\openjdk-17
# Mon, 25 Oct 2021 23:19:20 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 25 Oct 2021 23:19:21 GMT
ENV JAVA_VERSION=17.0.1
# Mon, 25 Oct 2021 23:19:22 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_windows-x64_bin.zip
# Mon, 25 Oct 2021 23:19:23 GMT
ENV JAVA_SHA256=329900a6673b237b502bdcf77bc334da34bc91355c5fd2d457fc00f53fd71ef1
# Mon, 25 Oct 2021 23:20:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 25 Oct 2021 23:20:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b03bbc71f9254a4ad2fba472595c859655b9d0cfefa638928416e277e0f0d497`  
		Size: 889.8 MB (889767519 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b201e45e5b11128e36517715f5b6ae98e5782737c1b112a5fae2aa83206f57bf`  
		Last Modified: Wed, 13 Oct 2021 13:23:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a947ce19e17c924828c9323a0de0ab956cabefde1b9245295f097feaff9f13a`  
		Last Modified: Tue, 26 Oct 2021 01:22:57 GMT  
		Size: 628.9 KB (628862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975f70b9a82216783c0c0e21b408fb16e21e38fb53b161c0130b5b27e07f91f4`  
		Last Modified: Tue, 26 Oct 2021 01:26:51 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a1b71adffea85a6872cbab45b665ce2c9bd024455f48a4fd7d9e101a77d543`  
		Last Modified: Tue, 26 Oct 2021 01:26:52 GMT  
		Size: 560.1 KB (560068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9de0db196c4c6fe23d7cfc2049c328e0636b41439d0518c5ee7ab0467eae65`  
		Last Modified: Tue, 26 Oct 2021 01:26:49 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51dc2a4df21428c8879a9e0f793937a5462063a043c9a2b71dd4851493eed5a`  
		Last Modified: Tue, 26 Oct 2021 01:26:49 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8f5f62694d9168bea84e754ed56ed6eb486067cb8d681596a3f6b6f8c6de0a`  
		Last Modified: Tue, 26 Oct 2021 01:26:49 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0717b43cbeaaee71964fb2d14edcbbdb04f9ade90c7caaad0d7d8af1b9a42e4`  
		Last Modified: Tue, 26 Oct 2021 01:27:10 GMT  
		Size: 182.7 MB (182682473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbcf74ba27d2280bdd84230c3fbcd74d6f73976e5bcb11ee344dc0dd255af8c`  
		Last Modified: Tue, 26 Oct 2021 01:26:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
