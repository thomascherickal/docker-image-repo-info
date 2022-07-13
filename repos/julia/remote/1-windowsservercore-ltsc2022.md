## `julia:1-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:3efda70b9300bf76704fa78f609c6697bd95e90ad27b03059a294606f3bd6458
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `julia:1-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull julia@sha256:450192ea5a42b7304a3d88775ee3f140a6bca534b4199e672c23697d3dcc2382
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2445476198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da683d1f8c68e3c9cd8e7bfc7fa5e943d407ab42d7cc3a37166813ac80612ddd`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jul 2022 14:26:12 GMT
ENV JULIA_VERSION=1.7.3
# Wed, 13 Jul 2022 14:26:13 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.3-win64.exe
# Wed, 13 Jul 2022 14:26:14 GMT
ENV JULIA_SHA256=ef5915eaf35bb71359072e8c41f84fa73f1059fecb198e7fc838270d4ba5bbae
# Wed, 13 Jul 2022 14:27:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 13 Jul 2022 14:27:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fec97d72036299b74f6cd664d86d2854659e963c3a99d7438d6b4b5c7d8f9`  
		Last Modified: Wed, 13 Jul 2022 14:37:14 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b35b3e65f8276073def2c2e0210ccac45332e25d1f58a09f6232ac82e0ace8`  
		Last Modified: Wed, 13 Jul 2022 14:37:14 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fd0b0962c9165d7ae7e18c108416bd23897f38fab692e7d0ca6c0af18a5ccf`  
		Last Modified: Wed, 13 Jul 2022 14:37:14 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99b0cd229b0fca1feab1c78b2386e8c5d230a894296fff51ca4d07d839f4e7a`  
		Last Modified: Wed, 13 Jul 2022 14:37:45 GMT  
		Size: 145.2 MB (145237520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6e86e4b2f10551e64e5e93ca6b1a7b854215dc1b4b298568d5e14bb45bcae3`  
		Last Modified: Wed, 13 Jul 2022 14:37:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
