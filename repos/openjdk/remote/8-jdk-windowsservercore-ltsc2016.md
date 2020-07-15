## `openjdk:8-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:f962ff5a3c821b275ee9dcbdd84d6060635c9bf6367fa98332f59655f2e71120
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `openjdk:8-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull openjdk@sha256:7782ebdf8635067155793eb6eb35ed2cbabe30ba36cb8754d230d07064a53e2a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5856880283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27c5afd324e2524cab20c89624d1813c7fdca1cdffdadf8921eb6d0243a63948`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 02:29:56 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 15 Jul 2020 02:31:27 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 02:31:28 GMT
ENV JAVA_VERSION=8u252
# Wed, 15 Jul 2020 02:31:29 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Wed, 15 Jul 2020 02:31:31 GMT
ENV JAVA_URL_VERSION=8u252b09
# Wed, 15 Jul 2020 02:33:51 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac -version'; javac -version; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a507ee4c5f1710265ef802239c6b751e4038de0880d1199939f60e9a55b852`  
		Last Modified: Wed, 15 Jul 2020 02:54:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f508a80c49db228b8b105873dc5f16dcab73be484890fc688db12a14646d0b9e`  
		Last Modified: Wed, 15 Jul 2020 02:54:01 GMT  
		Size: 9.8 MB (9848518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb57449db94f282f29d3b41741b7b624399cb9fc753ccbbe77da93115440bdc5`  
		Last Modified: Wed, 15 Jul 2020 02:53:59 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e011b2caf5c7b955215e7b1f5b50f9ad529cad1a8e7c9fcb9d32557c5ac500`  
		Last Modified: Wed, 15 Jul 2020 02:53:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149ac9938eec70456439db474217447b303bd18c27e6db0ea69e2d0606009892`  
		Last Modified: Wed, 15 Jul 2020 02:53:58 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35042e0c2863127a190bb9f36a71b1c3062ea5ef74c32ebee1f2b71e28f94544`  
		Last Modified: Wed, 15 Jul 2020 02:54:12 GMT  
		Size: 109.6 MB (109563950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
