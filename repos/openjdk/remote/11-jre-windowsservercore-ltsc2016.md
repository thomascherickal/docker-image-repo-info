## `openjdk:11-jre-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:d98d19f7137566cc4f6b8faa45461a91bdaace92c6a1ea9049ca0955e0560ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `openjdk:11-jre-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull openjdk@sha256:463a66cdce99aadadc75cdff16daa553f7911fedea92a975b4a3c4bbf73b96d2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5781786581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a332a3f7c18c47219a0ad5656b36bc1cd6033adb904b7de48e5ee245e40109f2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 12:34:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 15:42:48 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 May 2020 15:43:56 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 13 May 2020 15:43:57 GMT
ENV JAVA_VERSION=11.0.7
# Wed, 13 May 2020 15:49:28 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Wed, 13 May 2020 15:49:29 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Wed, 13 May 2020 15:51:18 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
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
	-	`sha256:c03a8ddd05856ecb914de50f24a846537b197783d2b9f60aadfb9573645b7afb`  
		Last Modified: Wed, 13 May 2020 16:20:20 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c70a9045d85ecc0efcdbdaeb75c307f6d92fa9dd1d166d657b96f955e39652`  
		Last Modified: Wed, 13 May 2020 16:20:21 GMT  
		Size: 5.4 MB (5380742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2da38971daa12aa35d70397c906c439b294f4c1b6aadfd8b7cfd9b46c61ee4c`  
		Last Modified: Wed, 13 May 2020 16:20:17 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ba252fba4bd13ab6ae99f2e3e124788ac065b241562dce318cf14bcbfa5851`  
		Last Modified: Wed, 13 May 2020 16:26:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aeac771f5d300808a190f1dc8d1521b0a46bf81f9bdfa07b62b55c1ebb319f`  
		Last Modified: Wed, 13 May 2020 16:26:08 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068e4d652d4d74c152504c7dfc020be5052f659b993a6f43dd1521bffafae86`  
		Last Modified: Wed, 13 May 2020 16:26:54 GMT  
		Size: 44.5 MB (44510218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
