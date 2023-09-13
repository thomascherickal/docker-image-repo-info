## `openjdk:22-ea-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:2976eee1f7b6d9bd0ef78fb919cf681a94cc9b54feddb08772fe88f985f50f0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `openjdk:22-ea-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull openjdk@sha256:6af90f7a207094243ba126f9fae77d2928a928b29215fe82eebe89d0353fd579
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2216206679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb1bad8ceec2aeb6af66a6d4bcf6958be320c15b7da3a3740ea82fda100ae1b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:16:37 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Sep 2023 05:16:38 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 13 Sep 2023 05:17:33 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 13 Sep 2023 05:17:34 GMT
ENV JAVA_VERSION=22-ea+14
# Wed, 13 Sep 2023 05:17:34 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/14/GPL/openjdk-22-ea+14_windows-x64_bin.zip
# Wed, 13 Sep 2023 05:17:35 GMT
ENV JAVA_SHA256=5a35fb7df33acaa4b3c14709a44966425b87a11c401c62e341d0fd8496cc11a8
# Wed, 13 Sep 2023 05:19:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 13 Sep 2023 05:19:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da151b70a7f82a6d6963a3317229ba06177114b9d44cd362e90207d42aa4d828`  
		Last Modified: Wed, 13 Sep 2023 05:26:10 GMT  
		Size: 255.5 KB (255460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f8ba7984984551020a40f5b8881b3c1fb035e9785ba3bdbae07f7c770a4f6d`  
		Last Modified: Wed, 13 Sep 2023 05:26:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0c6f3841f682fcfe5bcc0fb248fac7844337b14dd92db7132434ac8133685`  
		Last Modified: Wed, 13 Sep 2023 05:26:09 GMT  
		Size: 216.8 KB (216765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12c7d4416b5303f1443b723a956846f9b2259375ef6c3d3750ae1ae98a684b8`  
		Last Modified: Wed, 13 Sep 2023 05:26:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4a28b93868f02e57f198e121d8e79534aeb328de03f8b73b26167c5c8016f5`  
		Last Modified: Wed, 13 Sep 2023 05:26:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bb1f158b6bb8b8b6ca960499bf346c2293429836cf7c19596a77a6ed450492`  
		Last Modified: Wed, 13 Sep 2023 05:26:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb34008f32bc0b7a92cc1b68c4a8a76f9a3e2dcc51b228b94b8d8a21236de29`  
		Last Modified: Wed, 13 Sep 2023 05:26:26 GMT  
		Size: 199.4 MB (199396126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1db2aa973564c4e6def477ffd42e7bdf43599525c0d2df73f1bf6e3661d4e6`  
		Last Modified: Wed, 13 Sep 2023 05:26:07 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
