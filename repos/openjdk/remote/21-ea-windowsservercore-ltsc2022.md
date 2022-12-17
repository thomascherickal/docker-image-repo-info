## `openjdk:21-ea-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:2ab946e69207c268b19f977c2c320773366155e5d8ef3e97cb0b72257e52617a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1366; amd64

### `openjdk:21-ea-windowsservercore-ltsc2022` - windows version 10.0.20348.1366; amd64

```console
$ docker pull openjdk@sha256:295ae6b80fa70e2570d45ff8ea2eca25d71bd14abd614a8b6d61a1d8d1eb6eb7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691253803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c352e2e71651888448d52b92d68f75184bb4543e471c309aa1ce5699d62d0559`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 09 Dec 2022 09:36:47 GMT
RUN Install update 10.0.20348.1366
# Tue, 13 Dec 2022 22:45:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Dec 2022 02:49:23 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Dec 2022 02:49:24 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 14 Dec 2022 02:49:56 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 16 Dec 2022 23:21:37 GMT
ENV JAVA_VERSION=21-ea+2
# Fri, 16 Dec 2022 23:21:39 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/2/GPL/openjdk-21-ea+2_windows-x64_bin.zip
# Fri, 16 Dec 2022 23:21:40 GMT
ENV JAVA_SHA256=cde0c6b624e4340dd44950e39e1bd6b5f86fefdf5f3b6367670aafe058a59d65
# Fri, 16 Dec 2022 23:22:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 16 Dec 2022 23:22:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfa20ce142ecceb471dc070d9582fff942cef447b7c8ff22f2223ffe3737c99`  
		Last Modified: Tue, 13 Dec 2022 23:54:14 GMT  
		Size: 1.0 GB (1021665190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb8b9a4ec3ca516cfaa44f64e80b1e3aaecdbde870177411ff046f81f991dd2`  
		Last Modified: Tue, 13 Dec 2022 23:51:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc6d0e6b431095ccd3ac842154ae597a56b82834441570a9c95689f517a56ea`  
		Last Modified: Wed, 14 Dec 2022 08:45:36 GMT  
		Size: 576.9 KB (576869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc9ff5976ac61d4db52625b68997e78b00950928dbf9331ad574ee8a6325ffc`  
		Last Modified: Wed, 14 Dec 2022 08:45:35 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94200dbf261bdba4d1be09e454ed78de2fd3de552ee8fe393fea2716d24d619`  
		Last Modified: Wed, 14 Dec 2022 08:45:35 GMT  
		Size: 512.8 KB (512838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fb63959de1c7ef7812fa13592a3ede29316d26ffbea9d363ec37696063a2f6`  
		Last Modified: Sat, 17 Dec 2022 02:18:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19406e0bdee1a63427e3f1b7aacacd55ae9660fa39b5cd3a684c1af40a2d0425`  
		Last Modified: Sat, 17 Dec 2022 02:18:57 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af71fb1d9ef9b2035979bf2d2fbe618b292c3918c33acdf358c53df85c8a1827`  
		Last Modified: Sat, 17 Dec 2022 02:18:57 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25633047e73ba962adf38d740cbb5e8cd8b91738a9cb050166b202da68b0a6d3`  
		Last Modified: Sat, 17 Dec 2022 02:19:20 GMT  
		Size: 194.5 MB (194492821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ed4e137b1809ea4c2ca98a5c611c5d558ed0cc75c42b7b52fb6e7a2d468b03`  
		Last Modified: Sat, 17 Dec 2022 02:18:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
