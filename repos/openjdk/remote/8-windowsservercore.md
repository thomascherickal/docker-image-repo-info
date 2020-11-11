## `openjdk:8-windowsservercore`

```console
$ docker pull openjdk@sha256:0f4d0cd4aabe95696e28d2d5d237c247f0d607963d9f9619a401b5bdb4439e79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `openjdk:8-windowsservercore` - windows version 10.0.17763.1577; amd64

```console
$ docker pull openjdk@sha256:cfd4f23fc8b543a7fdda686545426b335db168fdb10006b5c0c7dee6017d5b71
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2502946130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab69007c1ff0a971599f1ab67d91f8f4cd29bbdedd1184d7c2aed4770447720`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 18:13:44 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 Nov 2020 18:14:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 11 Nov 2020 18:14:23 GMT
ENV JAVA_VERSION=8u272
# Wed, 11 Nov 2020 18:14:24 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u272-b10/OpenJDK8U-jdk_x64_windows_8u272b10.zip
# Wed, 11 Nov 2020 18:15:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac -version'; javac -version; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961c113008286ec10d5b5ad6712c39a4f6893491652c16952e9ad9d6182a696d`  
		Last Modified: Wed, 11 Nov 2020 18:35:15 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4485491cb68a4d866c356a328fbcaa1122d7eb2ec55323238ff04c01659a1b49`  
		Last Modified: Wed, 11 Nov 2020 18:35:26 GMT  
		Size: 9.2 MB (9234346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bf713566e8992d35c4e5d302efb1fff3991811310266468b19dcbed275dc89`  
		Last Modified: Wed, 11 Nov 2020 18:35:15 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef67d71ac3ef4170cb4ebcfde62465f5301c43937df6db5175b484415232c25`  
		Last Modified: Wed, 11 Nov 2020 18:35:14 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312e51d5ad1a7eb43ba8ca653fcda1a4cc54ef33aba06be90ab7af246cc04ac`  
		Last Modified: Wed, 11 Nov 2020 18:37:18 GMT  
		Size: 105.7 MB (105677932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-windowsservercore` - windows version 10.0.14393.4046; amd64

```console
$ docker pull openjdk@sha256:1b15ed5c262421400b5e9b696bef782cf6b246b440dbe3f9393fce1ca161c053
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5891687332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:579a858e2130b3565c3717e5e7082ff2052aa8d342de5da506af3fb8272f7f00`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 18:15:40 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 Nov 2020 18:16:53 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 11 Nov 2020 18:16:54 GMT
ENV JAVA_VERSION=8u272
# Wed, 11 Nov 2020 18:16:55 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u272-b10/OpenJDK8U-jdk_x64_windows_8u272b10.zip
# Wed, 11 Nov 2020 18:18:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac -version'; javac -version; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864d6ab6d378108050bf02ccd849c38e57d78de73c9a59d83a550d004548aefe`  
		Last Modified: Wed, 11 Nov 2020 18:37:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699c3656ce68e9d61d5eddc7285fd7bd7cecaec9dbd0e3625290ecd2dfcf91d1`  
		Last Modified: Wed, 11 Nov 2020 18:37:40 GMT  
		Size: 10.1 MB (10080718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e52b00e18274f150039531598eafb4e338992e0d2547fd5d002b08d9f72078`  
		Last Modified: Wed, 11 Nov 2020 18:37:37 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4832b0235c62e7676ce33b7401e4e9f53be73c05b5bb7f347395efb90b2017a5`  
		Last Modified: Wed, 11 Nov 2020 18:37:37 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c765f25153a68ad4957c2ae27320b4274e14f8be172a67b5b2b46807d8e9f6f`  
		Last Modified: Wed, 11 Nov 2020 18:39:42 GMT  
		Size: 111.0 MB (111043191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
