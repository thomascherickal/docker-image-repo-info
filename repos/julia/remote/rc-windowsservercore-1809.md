## `julia:rc-windowsservercore-1809`

```console
$ docker pull julia@sha256:e41c7ab3956d78afa8c57ab1074e6b819c34c27cc9437a4d692bace48de083e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `julia:rc-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull julia@sha256:2b07dde2770d54e2af27b5f81b60f8c8eb6a20129d44f63facfb7c166487b948
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2663399587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbfd5b5b453bdf4bbe2419131be8fcc14dede2872a8856517725d5a42c8befe7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 14:14:02 GMT
ENV JULIA_VERSION=1.8.0-beta3
# Wed, 11 May 2022 14:14:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-beta3-win64.exe
# Wed, 11 May 2022 14:14:04 GMT
ENV JULIA_SHA256=fdf8962e022916f2b657b1cb561f563fd5eb0dbee2e3fecf5a07d7ff5a24e2f0
# Wed, 11 May 2022 14:15:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 11 May 2022 14:15:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b7c9e65514b9ffc8718869c199228263fb05d1c320b5a847bfd36b07bb78db`  
		Last Modified: Wed, 11 May 2022 14:27:10 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee4a07f8074fef07f4e3974075415b07e033eb9631981370c8009d246d0a36c`  
		Last Modified: Wed, 11 May 2022 14:27:10 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5102f13612bf4ef8607347b61c3df9ac7731bc9524b578b9d7f58c24a68a93c4`  
		Last Modified: Wed, 11 May 2022 14:27:10 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a979790608ca941b4b9ffd54ba48d40d497bd95202bab447d729c964264d90`  
		Last Modified: Wed, 11 May 2022 14:29:57 GMT  
		Size: 159.3 MB (159336702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666d303a1cb6db6be6f795de4ecba253779a66c6e8b21db816bc9bbfc3ac34a0`  
		Last Modified: Wed, 11 May 2022 14:27:10 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
