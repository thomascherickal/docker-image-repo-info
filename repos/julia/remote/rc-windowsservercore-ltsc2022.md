## `julia:rc-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:3ce25f2da8ba133f1dd9cd15d3bc00ab64250324e7f8673ade1d24294ef80c3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `julia:rc-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull julia@sha256:6a0c782087b7448aabbd87b6439ec2becbee76657eb0f597f0bc56940dbefb7c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2477402221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744e37e7ee4c918f8c57be4bca38be5b4df7f75155e08145da1c963db400ef53`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Aug 2022 00:16:02 GMT
ENV JULIA_VERSION=1.8.0-rc4
# Fri, 12 Aug 2022 00:16:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-rc4-win64.exe
# Fri, 12 Aug 2022 00:16:05 GMT
ENV JULIA_SHA256=f874556fd3b41ce77ed51b3bf7bd7719f229bbddf454c5010c97126cece05afe
# Fri, 12 Aug 2022 00:17:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 12 Aug 2022 00:17:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b5ae4df858b6d0273352e450e4839bb7e8075e6371dcb4186c403633ed0822`  
		Last Modified: Fri, 12 Aug 2022 00:21:38 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceebd0e880544e9ac6459f0cfa43c8eef7b9e3918a8c4e6ed8c17a3438086d20`  
		Last Modified: Fri, 12 Aug 2022 00:21:38 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884fef5bcc758c8de81c11c92626d92ee8c0263f741fb6fd9e0ab3a2bb10b810`  
		Last Modified: Fri, 12 Aug 2022 00:21:38 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd1978cb37f5260578354f3be23aae2fdff5fc99fc9bce5fad306eaab13424a`  
		Last Modified: Fri, 12 Aug 2022 00:22:14 GMT  
		Size: 160.5 MB (160506026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13982e798107f9afb84dad0ab10bfd6963aec8ed18ccec50e47a6ce43cd3a68`  
		Last Modified: Fri, 12 Aug 2022 00:21:38 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
