## `openjdk:16-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:6f991a8cdbd0f2bcfd93b9a970ed6f12c97571f2a54358b6153c6d2f8fcb546f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:16-jdk-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:383989d8e9e29827b971704f8853e943caa02548852be5fe2d2bbe9bbd7ecb9d
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2516279760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb0b11d932c53849d07566ad283b49616f046e13169fb162ca291be23632324`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 01:45:44 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 15 Jul 2020 01:45:45 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 15 Jul 2020 01:46:14 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 01:46:14 GMT
ENV JAVA_VERSION=16-ea+5
# Wed, 15 Jul 2020 01:46:15 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/5/GPL/openjdk-16-ea+5_windows-x64_bin.zip
# Wed, 15 Jul 2020 01:46:16 GMT
ENV JAVA_SHA256=35d6b27ea5cc47f5caad0171e0a6bd120277c572c30c4e0d83d19ef63b74bc4a
# Wed, 15 Jul 2020 01:48:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 01:48:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca5cb7caf11332b67bae426682385af17fa897c718adce9713b111340eb0d71`  
		Last Modified: Wed, 15 Jul 2020 02:42:28 GMT  
		Size: 9.1 MB (9136637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13330fed5347a7e9912941992a3007161aa1fb49b13311deeecee172e5fb8dce`  
		Last Modified: Wed, 15 Jul 2020 02:42:24 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc29d35785aa1c3c0a383049b069e22805c21a9bb9cad32461bcab9457f3e69`  
		Last Modified: Wed, 15 Jul 2020 02:42:24 GMT  
		Size: 293.2 KB (293174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdf92767da0f8891b56c7a041584266effa05317f3a7b559d3494d1adf210d`  
		Last Modified: Wed, 15 Jul 2020 02:42:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5051a3b20081773b6992bd55eeb550362f9e4747bbdf8584fb114fa6d4f40c3`  
		Last Modified: Wed, 15 Jul 2020 02:42:22 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67aa71c339c714b3ac84e8be1414c7aa91a11d73a42816f9f1c2c7430381bd5`  
		Last Modified: Wed, 15 Jul 2020 02:42:22 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81988434eb0ae3d568d4c03765fc384484d85e0f4c9c950724fa5b436c7c87fc`  
		Last Modified: Wed, 15 Jul 2020 02:42:44 GMT  
		Size: 196.7 MB (196650860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef46a56a2cc955b374fe2a6f49a0283f2dd2cc8041f3170bb38262c6f923bfe`  
		Last Modified: Wed, 15 Jul 2020 02:42:22 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
