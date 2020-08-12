## `openjdk:8u265-jre-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:5a358e86b5e9de97f53e5710f6c25b09618f99d5ab5c73a8032f8fd441969ff6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `openjdk:8u265-jre-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull openjdk@sha256:ddd01a366e0de0b8a7880726e1e69804eef67b2cd747ef5588cbfa9e2c20c0f5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5795286536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3758d88508f9bf0953c91adac91dd5f77dae5de92c0e058b3cfe8becd90c3c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Aug 2020 20:31:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 15:58:10 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 12 Aug 2020 15:59:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 12 Aug 2020 15:59:23 GMT
ENV JAVA_VERSION=8u265
# Wed, 12 Aug 2020 16:03:29 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_windows_8u265b01.zip
# Wed, 12 Aug 2020 16:05:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32838d9637dc39d4acee78700b0f93d6c8c9d2db755f12c8009c1b51687d3fbd`  
		Last Modified: Tue, 11 Aug 2020 20:54:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2785dc5ba8107135b4e1c3a8709ebe4838c24deab58b743d2dd94ec05eee2881`  
		Last Modified: Wed, 12 Aug 2020 16:22:51 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484711f5757749de8c97caa8f632d669911c1bb5c6a31eb08123e3e3a89221d9`  
		Last Modified: Wed, 12 Aug 2020 16:22:54 GMT  
		Size: 9.9 MB (9869230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d66838d1245feb00bdbd58ac1bbeb128973bcf5570fdef979801d7f55394867`  
		Last Modified: Wed, 12 Aug 2020 16:22:50 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f636e547a1dc2b198a91d5b2279db4643ad03e198939d3de4bb97f4ebc841`  
		Last Modified: Wed, 12 Aug 2020 16:24:21 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78b1566e7134786e267545c171a3344c23b09105b4c78a32d90101df325fd62`  
		Last Modified: Wed, 12 Aug 2020 16:24:29 GMT  
		Size: 47.3 MB (47265240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
