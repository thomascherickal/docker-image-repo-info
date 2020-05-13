## `openjdk:8u252-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:767a16941c7a79c7b4a43d544466e24737095572810ee186a9e17f7fd801ab76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `openjdk:8u252-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull openjdk@sha256:1a4f1fbac2d83f91722db95beaaaeaf8f64db07b83c2ef6310f6a014249f41da
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5842410576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f16c13ac6bf39c103695cfe279923e3f3761ba7d00c7ee65d4eeeedd27321c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 12:34:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 15:53:40 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 May 2020 15:54:50 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 13 May 2020 15:54:51 GMT
ENV JAVA_VERSION=8u252
# Wed, 13 May 2020 15:54:53 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Wed, 13 May 2020 15:54:54 GMT
ENV JAVA_URL_VERSION=8u252b09
# Wed, 13 May 2020 15:57:02 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac -version'; javac -version; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e3e9730c43354781e87aa51e853bff3b1e8c1ca7004f527139638a8f9d499c49`  
		Last Modified: Wed, 13 May 2020 12:59:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9807e911923955127143c7fb9ee8b23f92bdbef94ab9fa7faedef3a14ff5ac45`  
		Last Modified: Wed, 13 May 2020 16:28:40 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef6a7748e6a61e27cd66c8fcf61448526139e56ae02669a1aec151e56061372`  
		Last Modified: Wed, 13 May 2020 16:28:39 GMT  
		Size: 5.4 MB (5381574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c720773fc1438fb72c62dc0dff34f460c26b01c1e0dcfe2f9003c492b359fde2`  
		Last Modified: Wed, 13 May 2020 16:28:38 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a665184e6fef0d9ffbf6d4673f0b4d45008483dca6e65667e83bd545d5b9d77`  
		Last Modified: Wed, 13 May 2020 16:28:37 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5b4f0e36525625c889750a6088562472cfd21688138f2e0905c2f61692eae6`  
		Last Modified: Wed, 13 May 2020 16:28:38 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c0b96f382b81f7982b38cb0bd129dc2affee8695418d668b6c49ab321f7133`  
		Last Modified: Wed, 13 May 2020 16:28:55 GMT  
		Size: 105.1 MB (105133643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
