## `julia:windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:9da2e2371fc94b351abb94cb58316fa06bd0c475242971d81c719624abffac9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `julia:windowsservercore-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull julia@sha256:e8ae350fad38994e18e5629d416f5af53996a6c81b4566a2880394531192bb10
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2050937989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38a56be2e208eadb76cfb9d6dac21e9c668515a940a1287cda85bb27309aeaa4`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Wed, 13 Dec 2023 01:00:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 01:00:40 GMT
ENV JULIA_VERSION=1.9.4
# Wed, 13 Dec 2023 01:00:41 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.4-win64.exe
# Wed, 13 Dec 2023 01:00:42 GMT
ENV JULIA_SHA256=8a491b31a8430c3662dff34bf349653e2d13ef98a4dcf7caa740359b6c5fef3e
# Wed, 13 Dec 2023 01:01:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 13 Dec 2023 01:01:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839fc47f6e056f9e09a214230f8b7115e69419dbc74acbbb1ad6bc0caa28862`  
		Last Modified: Tue, 12 Dec 2023 18:27:40 GMT  
		Size: 500.7 MB (500674814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c3d7d9e67d19f20b517c255509f543cdc513ced1bf6e4f52e86a3c8216ff97`  
		Last Modified: Wed, 13 Dec 2023 01:01:50 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19230b1f20bc3619715a10cbe43cfe909db3c0cdde738512c62373ead8e88c30`  
		Last Modified: Wed, 13 Dec 2023 01:01:49 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0de6ec128bcc06ccd1d674892753b4f9a3f5f5374f498a2000b79877a2955e`  
		Last Modified: Wed, 13 Dec 2023 01:01:49 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d959173d16c0662324dbf72691a9129569bb673eb54d11c90e3eec8cea65ec96`  
		Last Modified: Wed, 13 Dec 2023 01:01:49 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56553cb8fb17531c1d53f4ee3634cd4cdf0c4f0d20fe58f0fcbecce687f1550`  
		Last Modified: Wed, 13 Dec 2023 01:02:10 GMT  
		Size: 161.7 MB (161657448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3cd76f5ba33226dc072de95b22e8ffd072791762784856fcbd2e42e28257ea`  
		Last Modified: Wed, 13 Dec 2023 01:01:49 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
