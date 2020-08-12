## `openjdk:8u265-jre-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:278c0c524fff29a2637f39663bf874285f733d77fd4c478a3506794702600ce2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `openjdk:8u265-jre-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull openjdk@sha256:e14239f5b4190a136e576aa4f39b645ef683732f628595e1e16a0c0595752fb1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2387107957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce8bab95b87c80b888a02cf753f849e8e73669ebf13243ff6018f73d55e79d42`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 15:56:11 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 12 Aug 2020 15:56:50 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 12 Aug 2020 15:56:51 GMT
ENV JAVA_VERSION=8u265
# Wed, 12 Aug 2020 16:02:38 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_windows_8u265b01.zip
# Wed, 12 Aug 2020 16:03:21 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04abf2de9ce532b6f8d66b98cc14471f8deed9395325454a8f2e95d21dba2e36`  
		Last Modified: Wed, 12 Aug 2020 16:22:16 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03da955294add045d3033a00b651b3f3d4ca631ba2d7d005e950377c64d91e8c`  
		Last Modified: Wed, 12 Aug 2020 16:22:19 GMT  
		Size: 9.1 MB (9144094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e49aaa82ac68fe04eff8bde8fa0a3c3332514035135314cb73314536b82f74`  
		Last Modified: Wed, 12 Aug 2020 16:22:16 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bfcb23e793051969f60c90022532fb5dff50f78604b204dc746562af45bc15`  
		Last Modified: Wed, 12 Aug 2020 16:24:04 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbd63a7ec19a472072fafc6a46d46c4c0359524ecc742c457c0b96d0331d5fc`  
		Last Modified: Wed, 12 Aug 2020 16:24:10 GMT  
		Size: 42.1 MB (42092343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
