## `julia:rc-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:5a3d46338747480775eaee1e7c5dbd6a6e1a26059972b252ced28e67eca9fe54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `julia:rc-windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull julia@sha256:3fb5a907eafeeff67d2e56b3e76380521f49a6e1e33665b752cc1276b1a5cfdf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636588006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae8c503d59b2e966221a7efb4bb58f3a3597012fdecd3ecc3ff4eacef3e8d09`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 18 Nov 2022 22:14:23 GMT
ENV JULIA_VERSION=1.9.0-alpha1
# Fri, 18 Nov 2022 22:14:24 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-alpha1-win64.exe
# Fri, 18 Nov 2022 22:14:26 GMT
ENV JULIA_SHA256=b9cf18544d67e015fc8679e10deac29bef56758f1a88021ed485b5719bca7eae
# Fri, 18 Nov 2022 22:16:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 18 Nov 2022 22:16:15 GMT
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
	-	`sha256:60d0bfe3b39cdda5f721c9ea441d6dc83fd2ff6631dac275b841bb069b3feb46`  
		Last Modified: Fri, 18 Nov 2022 22:25:50 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405317f7b8a3e05e9763ba45b21c35262598c2495b446c7818532cb6c602bc87`  
		Last Modified: Fri, 18 Nov 2022 22:25:50 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e09d9e2e3db36377f72a07ce34af9fcb90dc3f4645856fa877fcda879daaf0`  
		Last Modified: Fri, 18 Nov 2022 22:25:50 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de006715b00b5ae9716ce4a3e3ec4aacee009f3c81e317679f4de75b3364993`  
		Last Modified: Fri, 18 Nov 2022 22:26:29 GMT  
		Size: 154.8 MB (154812245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773933f8a814ece8ccf94f04679dee85c425d0e161da53ab6f5b402592194eb3`  
		Last Modified: Fri, 18 Nov 2022 22:25:51 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
