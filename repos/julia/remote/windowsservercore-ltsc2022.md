## `julia:windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:ad82dcdcb7b7c0399d3589e91e1f4b524f7e85bc9f09ec85469bab0e7f4de610
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `julia:windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull julia@sha256:0489489f78f9db7c4aaf099bfbd88894538636b101308d289d1babea94b88867
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2624214874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9375f5bff93f8ceadf6f389128c1cb6a2bd13268358ebb5ac5d007feb5a1af`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 18 Nov 2022 22:19:55 GMT
ENV JULIA_VERSION=1.8.3
# Fri, 18 Nov 2022 22:19:56 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.3-win64.exe
# Fri, 18 Nov 2022 22:19:57 GMT
ENV JULIA_SHA256=1e5cc98bf83028809f6e37d205df660e3fb27d35e95c88944c1106a6710cd909
# Fri, 18 Nov 2022 22:21:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 18 Nov 2022 22:21:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8243cf7f19002b1afbf28621277bc5fec168571001bf9b7872c1320c2d3d1f27`  
		Last Modified: Fri, 18 Nov 2022 22:27:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9f098b17c40df4ac03bc50d6d2b910210f3b68bb52c988d2be73f961a4553a`  
		Last Modified: Fri, 18 Nov 2022 22:27:29 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967793debc83d470cdcc5fd6dcc6b7bbfb17b571c463a0dc5ce876f484e7e7f3`  
		Last Modified: Fri, 18 Nov 2022 22:27:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc017eb410310d1f95101352a9f6509013d6ba40e9ca12050fde375343dc792`  
		Last Modified: Fri, 18 Nov 2022 22:28:08 GMT  
		Size: 142.4 MB (142439098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c940c22946322591ac5e910a62942ae3005d93b3b459f7a5b8ad8e6d523e18`  
		Last Modified: Fri, 18 Nov 2022 22:27:29 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
