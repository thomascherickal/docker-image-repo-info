## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:32634730ec95cd7dc3b1c2bcc1dc7b4700c9c4f64881cea27c1f84b01c4ded91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull julia@sha256:2e0382eb569eb7615d480ffd9a23ea12ca4bc9374bc488e8a3dba9db4a0c6e3d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2840190150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4938a9a5d5690583da4796159c013ced05e4435e16441dcbc18f28278d0c366f`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 23 Nov 2021 01:16:57 GMT
ENV JULIA_VERSION=1.6.4
# Tue, 23 Nov 2021 01:16:58 GMT
ENV JULIA_SHA256=c9b6ecdad4feb57e5af12c9ef1a74993a96edbf87a4dc521d57e338397cee9b2
# Tue, 23 Nov 2021 01:19:06 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Tue, 23 Nov 2021 01:19:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb41f4249d9110eae98c897d297b7ae5d9988bd70dabb4157834c6a4c831907`  
		Last Modified: Tue, 23 Nov 2021 01:23:24 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353c3e9f06956a6065b66db76d2207ab0ee4a08f84826750c7434572a5ae195d`  
		Last Modified: Tue, 23 Nov 2021 01:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976d486dc620c406ebc996ed0ff5148d2d52e4dc1aab04a30891dfd639ad4d2e`  
		Last Modified: Tue, 23 Nov 2021 01:23:53 GMT  
		Size: 134.1 MB (134063322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f6007b948d03c31617fa0176e19e243d148676098f79e405a28a4a4977401c`  
		Last Modified: Tue, 23 Nov 2021 01:23:24 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
