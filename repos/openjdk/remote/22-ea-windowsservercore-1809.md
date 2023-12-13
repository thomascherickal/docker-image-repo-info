## `openjdk:22-ea-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:ad371488c179d65d8546fb32e22c1d52986c4d02ca5d07dec0e71b85152bad54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `openjdk:22-ea-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull openjdk@sha256:874a874950c9c19ef0604542c10d3837e9607a0f9f56622957ae092c47b4a53b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258103984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c665970237e1549e9eadc66d6fa405e4a5bd4837de6a12340e2a1cb0affe893b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 02:09:44 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Dec 2023 02:16:20 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 13 Dec 2023 02:17:31 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 13 Dec 2023 02:17:32 GMT
ENV JAVA_VERSION=22-ea+27
# Wed, 13 Dec 2023 02:17:33 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_windows-x64_bin.zip
# Wed, 13 Dec 2023 02:17:34 GMT
ENV JAVA_SHA256=522347f78607019a5c2d2478846c2ca0715ee700a7db3f78aff024e9935b1091
# Wed, 13 Dec 2023 02:19:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 13 Dec 2023 02:19:17 GMT
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
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8237cd2077ac4784fedf8ea56a9200c4f9a8cb5c1db3583e4dc52fab296873e4`  
		Last Modified: Wed, 13 Dec 2023 02:21:54 GMT  
		Size: 463.5 KB (463538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff9f4687c9439266cafea6b77d52129982ccd8070b9453dd263c7c6d9dff908`  
		Last Modified: Wed, 13 Dec 2023 02:23:51 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5f247e2575dcf7dd3e057b9f3d297a3795895bd7540ff8181dfcaab0c2811b`  
		Last Modified: Wed, 13 Dec 2023 02:23:51 GMT  
		Size: 278.0 KB (277957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8989ce550d00c4c531ef99bc4fbb0671afe532f1c929cae2492c7f0e5e9b0a83`  
		Last Modified: Wed, 13 Dec 2023 02:23:49 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce07bbc2df0316617ffdc8d8e84f44209234bc538c253170fccbeee7ace3083`  
		Last Modified: Wed, 13 Dec 2023 02:23:49 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133bcfda5a2353cbd69bc7325504f6c0dba6c7c998fbb0f7d7f3ba427828bd42`  
		Last Modified: Wed, 13 Dec 2023 02:23:49 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2ab5ad115fac51f010565f074a537ad1d3c713ca6e68ce402c304dd8dbcb57`  
		Last Modified: Wed, 13 Dec 2023 02:24:09 GMT  
		Size: 197.6 MB (197645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bac6ac173a4646d0842a0cdc74c3755bff0fde0021faaa4de6eec87a2639cf0`  
		Last Modified: Wed, 13 Dec 2023 02:23:49 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
