## `julia:windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:69a8f4f6d5d92a7687e20f90a47a4797969ba6c83e0661e62204723cd43d86d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `julia:windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull julia@sha256:634502095de34131963e335765694be59ae89b6627a07484e900c28e6b5712dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6407122155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef7cae2fb5f208443e86f3eb67251d1eb354e5c95f69d49a7e8d3c30a79f39e8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 23 Nov 2021 01:19:24 GMT
ENV JULIA_VERSION=1.6.4
# Tue, 23 Nov 2021 01:19:25 GMT
ENV JULIA_SHA256=c9b6ecdad4feb57e5af12c9ef1a74993a96edbf87a4dc521d57e338397cee9b2
# Tue, 23 Nov 2021 01:21:30 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Tue, 23 Nov 2021 01:21:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567970bba379bc9d0742b8793b03e90ffa89398328348fbecd4190381c348917`  
		Last Modified: Tue, 23 Nov 2021 01:24:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1763e4d52f3dbc470c79470ceac40d08f6795657c7bbbeae48f6b5772547aa8`  
		Last Modified: Tue, 23 Nov 2021 01:24:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbe961709f7f3b6f70aa08ec5530a1134808299ca1cd47a7c2232a6e8dbfd37`  
		Last Modified: Tue, 23 Nov 2021 01:24:36 GMT  
		Size: 134.0 MB (134025615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f60c6cc6e7ce97d94a1c64f2ba14b35575e59b1f72d97c49cb569ada33c4fa`  
		Last Modified: Tue, 23 Nov 2021 01:24:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
