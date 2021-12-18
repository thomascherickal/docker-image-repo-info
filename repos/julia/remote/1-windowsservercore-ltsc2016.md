## `julia:1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:7be2f183a0a2eeea9f9cd100ae0aeca7b151534343c355a33cc7e622751b74f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `julia:1-windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull julia@sha256:2a0b341c83a654c45cf5fe25ab2d3e8791e5aaf094922b9c9430e49be595fbc4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6419307394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52f6cd9fffabe7e228fc335d1b1b55acae995d4e64d95ed029a8ae7cefbb5f7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 04:10:16 GMT
ENV JULIA_VERSION=1.7.0
# Sat, 18 Dec 2021 04:10:17 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.0-win64.exe
# Sat, 18 Dec 2021 04:10:18 GMT
ENV JULIA_SHA256=40c6704a9f27031729610e177aa1cae5386336c7fea9c2e021e3b14d230498d5
# Sat, 18 Dec 2021 04:12:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 04:12:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f936ff5c0386e64bdb6f444b59d15ca03cbdd6151f82cd920abde7f2ee06f2`  
		Last Modified: Sat, 18 Dec 2021 04:22:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8619047d3d7443340e690928023f4fbfe07e1f59236a191f2d493e900bd12190`  
		Last Modified: Sat, 18 Dec 2021 04:22:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41826699f3aae700d362551d16ec48a5915b98efe72f78bc3d30844418fda18`  
		Last Modified: Sat, 18 Dec 2021 04:22:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb88c260cf7ee312e0236eaf8e5881b3896775b5f5c08b5b0a7dfa44685cee96`  
		Last Modified: Sat, 18 Dec 2021 04:25:15 GMT  
		Size: 144.6 MB (144585538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d796f2255897643868017250892ac06756cb3a38c5f8ef447344ec9bbe7ba3`  
		Last Modified: Sat, 18 Dec 2021 04:22:35 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
