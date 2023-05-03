## `julia:rc-windowsservercore-1809`

```console
$ docker pull julia@sha256:69761715859a06045f1b7e946422e6395ed202a4e43fba887a38f0b2034eab12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `julia:rc-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull julia@sha256:639df0ed6593ac2b90a9eac9c97386501bb2cf4ec165382ae594e5954f1bdf94
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2232876780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4848a6172d0f359d68592eb48714ccfcaf4b07318140f9e8229f80a509793fdb`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 02 May 2023 23:20:39 GMT
ENV JULIA_VERSION=1.9.0-rc3
# Tue, 02 May 2023 23:20:41 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-rc3-win64.exe
# Tue, 02 May 2023 23:20:43 GMT
ENV JULIA_SHA256=5cfee20b00591abb548ca32f4931e52284e831c783238cba72e6f9622bf5e76e
# Tue, 02 May 2023 23:22:48 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Tue, 02 May 2023 23:22:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b3af92349ccad0542786df5d6ada208a965a7e4d11215a74de62b13c7d34e7`  
		Last Modified: Tue, 02 May 2023 23:24:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1887f492c565ebc342382574cda9415c163fdf0826a907ac77c0a683293171bf`  
		Last Modified: Tue, 02 May 2023 23:24:45 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3505d9d1cfd37abcb7a52c180414af9c0b4179f9978789bc51cf52de99b4202c`  
		Last Modified: Tue, 02 May 2023 23:24:45 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a127ab115c4d17240a7669dcd37309a37d588ef5426e8a2dc690621299de65c`  
		Last Modified: Tue, 02 May 2023 23:25:21 GMT  
		Size: 161.6 MB (161578444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbbed9dc8b7b8299d230391905d310b72918675f23c9c7fbf07f4de6be8849c`  
		Last Modified: Tue, 02 May 2023 23:24:45 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
