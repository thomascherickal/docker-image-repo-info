## `openjdk:8-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:bd245afb1641ddfea67475df357d57281025604454f7d1328f8afca1045966fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `openjdk:8-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull openjdk@sha256:e64c9a60babe0898b957d210feccdc15d9fd72b30dd5af2f9b7be5678c6972f0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5859124524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:943711b036df7daf9180157e6798d18994f73ef5159eafceb303602a6152d768`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Sep 2020 21:16:03 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 08 Sep 2020 21:17:28 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 08 Sep 2020 21:17:29 GMT
ENV JAVA_VERSION=8u265
# Tue, 08 Sep 2020 21:17:30 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_windows_8u265b01.zip
# Tue, 08 Sep 2020 21:19:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac -version'; javac -version; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3358b74428811280b1f3dda3449fde85aa183b9ab00c8c2544314f6dd6f95c6`  
		Last Modified: Tue, 08 Sep 2020 22:43:08 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe579e67c19d6eb6c16d0505037dd4c354bebc669d4f7fcbc665850b5fe93bc3`  
		Last Modified: Tue, 08 Sep 2020 22:43:11 GMT  
		Size: 9.9 MB (9880038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60f0fbc101f430aae5765a2b407a78cb246f06456704a6e7e8c57ffa637ec1e`  
		Last Modified: Tue, 08 Sep 2020 22:43:08 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcc78dcdb7806ee6be106966aa8852ee2dc450be0ac301f81d6a791b3177c05`  
		Last Modified: Tue, 08 Sep 2020 22:43:08 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361c8532418376a3f55e4713a9830f2d5c7431a9ceaf88dd4e4b557a35ebed5e`  
		Last Modified: Tue, 08 Sep 2020 22:43:21 GMT  
		Size: 110.0 MB (109985501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
