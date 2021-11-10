## `eclipse-temurin:8u312-b07-jre-windowsservercore-ltsc2016`

```console
$ docker pull eclipse-temurin@sha256:4a8d5bbc67e84f153f877a6921608a4f7b346459f034c5c8425c8a06152a3a40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `eclipse-temurin:8u312-b07-jre-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull eclipse-temurin@sha256:fa1e20ed11940f002110744342389a1a0c4833a3d35fb558a1deb74cf88f55d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6343999380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054ee0cb753acc1259553578954787b571a608d869bd7312eb12f24487e449d6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 17:14:04 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 10 Nov 2021 17:21:37 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Nov 2021 17:22:38 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:db23888e1c9322d90b869e85260905c6169cdc6c89646191d8d36f6e397f596c`  
		Last Modified: Wed, 10 Nov 2021 18:02:22 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870e504ed5fad4f27fe9096436695ca9228d6cd7707eededdf6424988a616806`  
		Last Modified: Wed, 10 Nov 2021 18:09:11 GMT  
		Size: 70.6 MB (70550663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b01412e373b145a30be45cfd2bb5a646d2261103e7bcdc687c7d7353dc2851`  
		Last Modified: Wed, 10 Nov 2021 18:07:56 GMT  
		Size: 355.0 KB (355034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
