## `julia:rc-windowsservercore-1809`

```console
$ docker pull julia@sha256:4a9b74f44e02ea1226fc5a30da0412a41f1bfbc36f13aa056dbbb783b726e454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `julia:rc-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull julia@sha256:bcd152877a5dc33135eb73da647abb9ff893ad8409521d02dd17413d77db2d3d
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2240037721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ff54382c8597239fc319cc72a484c7d9973793a3159bd33f3103f7533af081`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Tue, 05 Dec 2023 01:12:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 01:12:14 GMT
ENV JULIA_VERSION=1.10.0-rc2
# Tue, 05 Dec 2023 01:12:15 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.10/julia-1.10.0-rc2-win64.exe
# Tue, 05 Dec 2023 01:12:15 GMT
ENV JULIA_SHA256=e65b6b0c573c4d0539f31e86870358e12970b2cb0cb9a4c43945c19c36464187
# Tue, 05 Dec 2023 01:14:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Tue, 05 Dec 2023 01:14:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d091cd8625eb1aead26f71c81f9c3b2350cb66ba9491a7d7999c3dfd74ebbe5`  
		Last Modified: Tue, 05 Dec 2023 01:14:35 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6c5c092a0c3d27e934e0972362d988d1edcb6855028c7cf7dafba938165a57`  
		Last Modified: Tue, 05 Dec 2023 01:14:34 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb63f8f2a65903e623e0772570c36c85fb0c802475f611afc06a0115ec94be`  
		Last Modified: Tue, 05 Dec 2023 01:14:34 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c1d294332b526b8dcaed798e0cc497158017591bf31632df6574fd487acfc8`  
		Last Modified: Tue, 05 Dec 2023 01:14:34 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357db5c61333410f34884695c8b30171a216a1b7bc28e3ecc6673e7ea8895035`  
		Last Modified: Tue, 05 Dec 2023 01:14:56 GMT  
		Size: 182.6 MB (182599693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353d509e1d942d7afaf304c061e4b614a3cfc89d718020f14c7dedf32da6c89d`  
		Last Modified: Tue, 05 Dec 2023 01:14:34 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
