## `julia:1-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:37a24acd1e7ac7912581603172dfc4ec274a2687137b723669f2b88dd55c8825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `julia:1-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull julia@sha256:56d65550cf8e6a8a9c5ee36000b8db8aa7a983964756d62a8ac33b61e4fb62ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2021529529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac15eaca4d9e58d5c6ec2baf5d430bb8ce7b7b0d9256199e720d62ece978bb4`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 06:01:24 GMT
ENV JULIA_VERSION=1.9.3
# Wed, 11 Oct 2023 06:01:24 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.3-win64.exe
# Wed, 11 Oct 2023 06:01:25 GMT
ENV JULIA_SHA256=eb5a6464dcb1653143caf117a76f9e9126da8c960b737d1c82e4c46d165061f0
# Wed, 11 Oct 2023 06:02:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 11 Oct 2023 06:02:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5329a4bcc0b48e75a781a40fe527b4c69e7c8bc46c370a7f553a74bc356dca72`  
		Last Modified: Wed, 11 Oct 2023 06:10:44 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f187c6b341cbb91b979b289d1401c6a8b6d547cfca78a27086d93927a4d87915`  
		Last Modified: Wed, 11 Oct 2023 06:10:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f3c53a6fcfe6496ddc27076db5c2893e623877342f2b56d73b5c535f6fe9e2`  
		Last Modified: Wed, 11 Oct 2023 06:10:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c105c81e17f00e0da42bb85a63d65b640f86bcff5c6f241a46deec9ea0fa8ec8`  
		Last Modified: Wed, 11 Oct 2023 06:11:18 GMT  
		Size: 161.7 MB (161679399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfac0329d1bb8c5f67f7c9b893d7aa7c6329e6c85e6ce73fcc197d87714fc13`  
		Last Modified: Wed, 11 Oct 2023 06:10:43 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
