## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:0ec7efc01d8fe5085ffeca6137c838136653f2ccabb9e559673f6c434d5fdb5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull julia@sha256:43a8d54d0cbcc2aa3e06c5a039a9108b00134452cc5aca95f9396d196617f4b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2853325068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11caf055cae43b0ba6a173ab39c48cd13f008856fe22350f291acec445bf241`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Dec 2021 18:17:51 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:17:53 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Mon, 27 Dec 2021 18:17:54 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Mon, 27 Dec 2021 18:20:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Mon, 27 Dec 2021 18:20:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f615b27269f4ae47361f0dd3e1c0e7dade7a798c84bd8daf0541c92bdf32b30d`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43777aee21a90dd7ae16e744498ba3423b5c4255698acf3a17318187ed569c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ecc579854a79b3d24c95a127fcda7b58d39985a47783d4b9abffd82f7a8c8c`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161382cf4a878de820374c84f6a07ad62d59d3f2f47a21ca7b70e2899223886c`  
		Last Modified: Mon, 27 Dec 2021 18:28:33 GMT  
		Size: 144.7 MB (144713562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ea14bc61d7ae1ec49427472d4ee7f8135d7aa1a095325e3222b3a32318bca0`  
		Last Modified: Mon, 27 Dec 2021 18:28:02 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
