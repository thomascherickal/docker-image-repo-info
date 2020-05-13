## `openjdk:11-jre-windowsservercore`

```console
$ docker pull openjdk@sha256:59049fff6844806063ae9a043b81bc9020427eab0991a4319286cc68b855751b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64
	-	windows version 10.0.14393.3686; amd64

### `openjdk:11-jre-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull openjdk@sha256:2a9604a00515c7484f50f090968330bdf7977450b34a536d057a70b1088aa1f1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1758121973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a992be01cf6fbc79bc7299df0dc347022cd89fffc00739926adc57b408f97f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:41:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 15:40:36 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 May 2020 15:40:59 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 13 May 2020 15:41:00 GMT
ENV JAVA_VERSION=11.0.7
# Wed, 13 May 2020 15:48:27 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Wed, 13 May 2020 15:48:28 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Wed, 13 May 2020 15:49:19 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77613e754ba9d62c0acd4ef271c4ee7d3af091b8c8b310afa404560a9d281f82`  
		Last Modified: Wed, 13 May 2020 13:00:20 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d697ee5c17f7ca6807843cf1182f2fc6186e1ceed4d513fd1d2480fdd08cd975`  
		Last Modified: Wed, 13 May 2020 16:19:35 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72742d011d4f82aae552d0a2b889c3ad4ed50703ebf87b27dbef32ad34f0e83b`  
		Last Modified: Wed, 13 May 2020 16:19:35 GMT  
		Size: 344.8 KB (344830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38758fd508ad781bb829f0ee97740dca0afbcee534ba2d334b931a36615fb7c`  
		Last Modified: Wed, 13 May 2020 16:19:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f3a8912af6322d01c34419e9a96efee6954a126f3c3f30375c7af0c5138f48`  
		Last Modified: Wed, 13 May 2020 16:25:01 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28031e47998dfb67bf4a805403b42f228b1617f8c81de8799dc9e4abedf626d`  
		Last Modified: Wed, 13 May 2020 16:25:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e83d48456acb23c4b3520302ffcd0fb1e010aa0f4e06414d94aea41a1fe88c7`  
		Last Modified: Wed, 13 May 2020 16:25:53 GMT  
		Size: 39.4 MB (39438571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-jre-windowsservercore` - windows version 10.0.14393.3686; amd64

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
