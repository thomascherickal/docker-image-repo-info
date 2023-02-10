## `julia:rc-windowsservercore-1809`

```console
$ docker pull julia@sha256:6b42b2e4b6635618268678101d7bbbe9f34d5e433ed17042471c0f2b1be84447
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `julia:rc-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull julia@sha256:c84b01774711e9a5391f4ae71c8db173c78dbd9107b42b29d044cd1d1190716f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1868570307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ae443099acc375a96b181a481893032b29fc0258c89e6f1a0cb3595dad9132`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 10 Feb 2023 02:21:26 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Fri, 10 Feb 2023 02:21:27 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-beta4-win64.exe
# Fri, 10 Feb 2023 02:21:28 GMT
ENV JULIA_SHA256=c298228ad482b9941f496b88cffa4d7db516be7bae576e9d83a2bff435435ba5
# Fri, 10 Feb 2023 02:23:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 10 Feb 2023 02:23:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3116bd525a636fedba84e02e718621517d114cd385bb1252b651d9e826da07`  
		Last Modified: Fri, 10 Feb 2023 02:25:51 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6239861d345b139582cd738362767489805b29eee49b573e1227038ffefbd1`  
		Last Modified: Fri, 10 Feb 2023 02:25:51 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c7f6fe23fe1de7c3b898f3eb0497ea320133a9a65d11124878b65f8a50f35d`  
		Last Modified: Fri, 10 Feb 2023 02:25:51 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ea8096cc5ce02c3797823496b6dadb8a89a115d2b9ab1e3d3e72ded0337c40`  
		Last Modified: Fri, 10 Feb 2023 02:26:31 GMT  
		Size: 160.6 MB (160619208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db011c318070090abfe67511ebbb77a5785c5d5ae1c358bb6ab0eb99c8d3dc`  
		Last Modified: Fri, 10 Feb 2023 02:25:51 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
