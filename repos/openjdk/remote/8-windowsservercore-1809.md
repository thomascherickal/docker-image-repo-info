## `openjdk:8-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:7cf3758a7c37c1750dcd9ee5c525deb65f39ceba60f06fc39904b540fe6c8eff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `openjdk:8-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull openjdk@sha256:187e40d24088415372ba5b1d93bf901e773206bd22385a904f78e6fed781cd1f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2321793702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddd942d92da769ce979a501db51e2ee8c80e897503d394c7bbd5a1bda2666690`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 01:30:46 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 15 Jan 2020 01:31:25 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Thu, 23 Jan 2020 00:22:38 GMT
ENV JAVA_VERSION=8u242
# Thu, 23 Jan 2020 00:22:39 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_
# Thu, 23 Jan 2020 00:22:40 GMT
ENV JAVA_URL_VERSION=8u242b08
# Thu, 23 Jan 2020 00:24:03 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac -version'; javac -version; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2d444929b943c4f4f4a475d9f25066ceec820499bc85b52c37c87831991eb9`  
		Last Modified: Wed, 15 Jan 2020 02:14:23 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e259c6c6f5b6748db8b7b81e4971e961596c683c068a25172d53849081c1fee`  
		Last Modified: Wed, 15 Jan 2020 02:14:19 GMT  
		Size: 4.5 MB (4547040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c9f508e1a37ed96518a49ccbada80c333f182ce2d65ed98fe008006398414e`  
		Last Modified: Thu, 23 Jan 2020 00:34:31 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cb0717348a121e1f633f29b4af555db4169addeae781aa48555f272b61031f`  
		Last Modified: Thu, 23 Jan 2020 00:34:32 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5dc1752a94aa7afdb0896af7c2ba2eaad7ca08b85ea4f49af39b8e6f3d52346`  
		Last Modified: Thu, 23 Jan 2020 00:34:31 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571ad3bfc1e64c801a79e7d230b206950c764d481c65d24dfc87e9892fb346c1`  
		Last Modified: Thu, 23 Jan 2020 00:34:54 GMT  
		Size: 99.8 MB (99829583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
