## `openjdk:8-jre-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:b5a14bd52ad19dc6b62cf36f010b4dc4969316dfc52b36b3cf0e1d672f478311
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `openjdk:8-jre-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull openjdk@sha256:b6a62effc7a4b188814f669c2f800f2aacef2c7c1422b843bb95d6cd85bc4892
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5780094866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e910b421be25b6c49aaa003979f439f263aca7f06a83a81051b563c3289e3b23`
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
# Wed, 13 May 2020 15:59:25 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Wed, 13 May 2020 15:59:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Wed, 13 May 2020 16:01:05 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
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
	-	`sha256:cb46085bfca00bee1f45dfadc4211a0c4fd1b195956f22cf3d1b80bd581a9184`  
		Last Modified: Wed, 13 May 2020 16:29:58 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dbef8a5ea0dd1711b578ce3475fff31e57db5c8815ad4017897a54d50ef87`  
		Last Modified: Wed, 13 May 2020 16:29:58 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c51b67616ff3f0fc9bbc2773adbd4ec7d15df1c11fda2096093e75f04f4691`  
		Last Modified: Wed, 13 May 2020 16:30:08 GMT  
		Size: 42.8 MB (42817864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
