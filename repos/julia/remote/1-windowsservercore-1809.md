## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:a9d96dd8cbfe19b50834b16cec262b7508e047167f1aa0d35da3f5c039e739ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull julia@sha256:3549988210b26719ff630803677d1220956eee3417d1fdfe19c056f2d320f76f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2920806512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:331f783cd45e9c425270bbe722f58c32abd9c7bd7a407e52481944d256ac391d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 18 Nov 2022 22:21:39 GMT
ENV JULIA_VERSION=1.8.3
# Fri, 18 Nov 2022 22:21:40 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.3-win64.exe
# Fri, 18 Nov 2022 22:21:41 GMT
ENV JULIA_SHA256=1e5cc98bf83028809f6e37d205df660e3fb27d35e95c88944c1106a6710cd909
# Fri, 18 Nov 2022 22:24:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 18 Nov 2022 22:24:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc8bd5935ff251b091be055ef91254d404fa372c2ed6954dc6b2f50cf0c08ac`  
		Last Modified: Fri, 18 Nov 2022 22:28:21 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d16e49d92a471fa8fda7127a99b988b8f7f65b9ada7d73ced12a07e70201ed`  
		Last Modified: Fri, 18 Nov 2022 22:28:21 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4887f10f37908d925fe874b1c4b141fc534454cebbc9a7fbf7c659f62e50d15`  
		Last Modified: Fri, 18 Nov 2022 22:28:21 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e2c42ca412926612eb9097118f08105845e78d273e8b1e82fc697b7f40fd9d`  
		Last Modified: Fri, 18 Nov 2022 22:28:57 GMT  
		Size: 142.2 MB (142212599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e995eb3a2e75acd0339fc9a806e5fa780c9c403ecd1b964d9a979e67bdd770`  
		Last Modified: Fri, 18 Nov 2022 22:28:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
