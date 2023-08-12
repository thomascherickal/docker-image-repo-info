## `openjdk:21-rc-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:3520551ad1d14def368350a0157a81fbc64982e219d12a2c63b63d514489b4bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `openjdk:21-rc-jdk-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull openjdk@sha256:521a4cff8e7ac4f8e6f4fce7c17def13da5aad72985460324a6bf66aa0f5f3fa
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2194929924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d3d755968f0fcffa4d0841ab6264f346e826df28cae191f62566333eff2bcca`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:39:19 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 10 Aug 2023 02:44:28 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 10 Aug 2023 02:45:24 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 12 Aug 2023 00:04:51 GMT
ENV JAVA_VERSION=21
# Sat, 12 Aug 2023 00:04:52 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_windows-x64_bin.zip
# Sat, 12 Aug 2023 00:04:53 GMT
ENV JAVA_SHA256=5434faaf029e66e7ce6e75770ca384de476750984a7d2881ef7686894c4b4944
# Sat, 12 Aug 2023 00:06:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 12 Aug 2023 00:06:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82556c0499019c0d63fc48880317518db1b5694401f0d8420ea2c4961effcee4`  
		Last Modified: Thu, 10 Aug 2023 02:49:35 GMT  
		Size: 250.9 KB (250879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e209df0c7d77cd6a6e02e637fa04e5eb4a165589d5b412e7b010bf0e612c2c4a`  
		Last Modified: Thu, 10 Aug 2023 02:51:33 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567c0183a0fd1cdeb87e458ff06bb946e60513a946914e135db33acc4181aef0`  
		Last Modified: Thu, 10 Aug 2023 02:51:34 GMT  
		Size: 246.7 KB (246701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99aa34e54f4af59ce1d61e0abda0fc2a5ec37c66cd99d9e2cf7bf6484b01865`  
		Last Modified: Sat, 12 Aug 2023 00:11:10 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160b0b3b66b8519443bb69819bfacda9b4c7a78ce1b2503490feb010e9102fa`  
		Last Modified: Sat, 12 Aug 2023 00:11:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fd62968bead6cfa7a7083c151cd4639a3bc7abfed9d3c38ccde47973341aef`  
		Last Modified: Sat, 12 Aug 2023 00:11:10 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aeeee7a2a832067326f4f8d4e432f58e7d2da08e2ad331913a23594b069fb3b`  
		Last Modified: Sat, 12 Aug 2023 00:11:31 GMT  
		Size: 198.5 MB (198468632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623d95c625a1cd19e3a8947e3e148b9124f593c00822f3ade43ca7945fae396e`  
		Last Modified: Sat, 12 Aug 2023 00:11:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
