## `openjdk:18-ea-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:0c733a47ea57fcad89f331f471233f5822d7617bc302af3ea597be9ffba2dbcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `openjdk:18-ea-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull openjdk@sha256:a312a5386071493ef9258bbb94b8435a5a134f12c2bed58de2d768ddb6334efc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6457980469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6e4cd5df2751a121a10f5d5288243e7e6fa7f629362a50eb4eb7d92f62b141`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:29:09 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 10 Nov 2021 20:29:10 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 10 Nov 2021 20:30:05 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 03 Dec 2021 23:11:33 GMT
ENV JAVA_VERSION=18-ea+26
# Fri, 03 Dec 2021 23:11:34 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/26/GPL/openjdk-18-ea+26_windows-x64_bin.zip
# Fri, 03 Dec 2021 23:11:35 GMT
ENV JAVA_SHA256=ca0f08726d07f4f0514c35b0e30268cf229e8564aceab51d288f237a5ea9b309
# Fri, 03 Dec 2021 23:13:24 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 03 Dec 2021 23:13:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f998978d6856e995f1d9c4942941c32a17a4d88aff023bd7b9c78fc2a16c252e`  
		Last Modified: Wed, 10 Nov 2021 21:07:51 GMT  
		Size: 355.7 KB (355709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efceaabe52cac09e507c97b920e08a9358526f82a968e0123516aab06c1ac57b`  
		Last Modified: Wed, 10 Nov 2021 21:07:50 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b2835ec5caac2405ac77407ac306d4269c837a329e31ef3e1e8ff58363dec8`  
		Last Modified: Wed, 10 Nov 2021 21:07:51 GMT  
		Size: 346.8 KB (346841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f149866530f13ac1baa43eeb7638eb792174aafcd4b233a6f08d2890dc7d1b5f`  
		Last Modified: Fri, 03 Dec 2021 23:34:10 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ee3d7a044a5be6ad513dcb34a16962a775de2bd928331e926c54fbbdc3ce26`  
		Last Modified: Fri, 03 Dec 2021 23:34:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67b0531b394b4f627a52cedd92f5247680005080f8e6c2cae4f9a4acedcfeac`  
		Last Modified: Fri, 03 Dec 2021 23:34:10 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026e0b5a1efbe76a76475ce9a81722900b617362047a207cccb986be6068d02f`  
		Last Modified: Fri, 03 Dec 2021 23:37:22 GMT  
		Size: 184.2 MB (184178511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4ba727ad1beeb9d06dfaa04b9bd6415e90ad1fc7dea99f5362d5ee7bd6cb1e`  
		Last Modified: Fri, 03 Dec 2021 23:34:10 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
