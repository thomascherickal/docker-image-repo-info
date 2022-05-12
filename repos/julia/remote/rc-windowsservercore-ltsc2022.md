## `julia:rc-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:afcdd4313ebb314f268ac64e631296e3b11cd2464819b82d7e11c36b1c349ab9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `julia:rc-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull julia@sha256:71fff05ef72f58e4e6801fc27aeb93e1040545489a0c0dd33e617b1748124859
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2397000156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:400ac71b8721a424c79c89c789065a4e426d683006c64b71bae69ffd2652c67d`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 14:12:19 GMT
ENV JULIA_VERSION=1.8.0-beta3
# Wed, 11 May 2022 14:12:20 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-beta3-win64.exe
# Wed, 11 May 2022 14:12:21 GMT
ENV JULIA_SHA256=fdf8962e022916f2b657b1cb561f563fd5eb0dbee2e3fecf5a07d7ff5a24e2f0
# Wed, 11 May 2022 14:13:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 11 May 2022 14:13:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f936b250a4afa917a78dbe32c4579d12570380da5ca6a570cf03ec7c1ea841a`  
		Last Modified: Wed, 11 May 2022 14:24:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e3f55b3295e81957a6818e059f20da63c023a95f8dedb1e7b4d4e51bca0a4d`  
		Last Modified: Wed, 11 May 2022 14:24:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9276c230057e8feeb721263ebe96fd6fca5cc5da48a8d089c995d14f7cde00b9`  
		Last Modified: Wed, 11 May 2022 14:24:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f15ed52a79c4787e9b9b833466197c42efd634ad6874aba83945c1ac7d9a8a8`  
		Last Modified: Wed, 11 May 2022 14:27:01 GMT  
		Size: 159.5 MB (159457854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d416fc3453012851888332a6157ae2aac4f24051ef3d67f5a9ccc05fe1b025f1`  
		Last Modified: Wed, 11 May 2022 14:24:22 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
