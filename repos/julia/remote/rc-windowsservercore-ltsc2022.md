## `julia:rc-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:506c0bcccd9e039148208a74969f364a96d95a26b76371fef2303f3b2a397fb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `julia:rc-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull julia@sha256:983ea07e4107856574c5a3fa7e42a5af1c020a25baad219a7da0aa41146ef59a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2397543857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89017b68840a3d3234a1fe32e9127499e8816a76f17b5f00479921ba755f79e7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 02 Jun 2022 18:15:26 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 02 Jun 2022 18:15:27 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-rc1-win64.exe
# Thu, 02 Jun 2022 18:15:28 GMT
ENV JULIA_SHA256=f739f4fb46030df00cbaea513afd427b436fc91b6fc6d7f4e437498cd16cc2aa
# Thu, 02 Jun 2022 18:17:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 02 Jun 2022 18:17:01 GMT
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
	-	`sha256:ba9f5fffbd70b57b4eec3fbfcd4f8a1288d24a392ae5e11a94add66fbbde1643`  
		Last Modified: Thu, 02 Jun 2022 18:20:50 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3def9dba5937e7213b5246028e80bc8112e38fdaa13d0336909be43db1f64a8f`  
		Last Modified: Thu, 02 Jun 2022 18:20:50 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76e08ee43498f0b5386766ce95caeecf9adc309147ee919b4e7dd88fc44b3c0`  
		Last Modified: Thu, 02 Jun 2022 18:20:50 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f793c8c8f284d76cc82d62b369d42420fa1c250b3c105192ee91a0f56e737f`  
		Last Modified: Thu, 02 Jun 2022 18:23:45 GMT  
		Size: 160.0 MB (160001498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25069aeb4a7ae18df5f47c9be62dc83908c86664777b53db24058de33912ffe`  
		Last Modified: Thu, 02 Jun 2022 18:20:50 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
