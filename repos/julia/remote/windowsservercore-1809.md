## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:c72611e6cce79bcf49a5cd17fe3caeecfab0852fee938a219ef20302f8b5c0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull julia@sha256:ced337da7c3824d9ae8e8b7654db837b7fb60769d80355e691d9458539140f2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812184912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f68fdcb08072a2eb9826fcccc0685c0aa24e99d3b5ec2320db60f595a11138`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 06 Jul 2023 20:24:30 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.2-win64.exe
# Thu, 06 Jul 2023 20:24:31 GMT
ENV JULIA_SHA256=bcc8a0eb217ee128638e12b756e1f41df5c83cff6c6749839d081618f6c79e57
# Thu, 06 Jul 2023 20:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 06 Jul 2023 20:25:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aba1725eb1cb630298f0d3c691a2c5c108e89082756ea5f57aee779d508c95`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117c43b3314970d865f9cf204ceafcbf96e12e8ec5004a7dc05523b8949e7a`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722f427fa71695bf3bf994fd27ab41814eaf8721b2e825cd86ed2fdc82ab3c88`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa7236ecf253f99b449281a56466ca3af33a4b9d6c011ca6b696b94823221cc`  
		Last Modified: Thu, 06 Jul 2023 20:28:05 GMT  
		Size: 161.4 MB (161441046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3985434a400fa1112eb170b179ff0c5457a56d90415609bcab24c72942c68`  
		Last Modified: Thu, 06 Jul 2023 20:27:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
