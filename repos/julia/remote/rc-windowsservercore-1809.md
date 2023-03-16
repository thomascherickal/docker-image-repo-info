## `julia:rc-windowsservercore-1809`

```console
$ docker pull julia@sha256:efdaebfc1a69a6fd5e8ecf90f09eb6ecafd14c299c22e649207ec3daecccbbc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `julia:rc-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull julia@sha256:00fffb28e1000e8935ac615023c771cd1674cae417dd47a021522571a4ea9066
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2174800441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2f0b03004e64ba01edce93f6a13ac78a54b9e7fc957a40599eadd9c5665b320`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 07:20:06 GMT
ENV JULIA_VERSION=1.9.0-rc1
# Thu, 16 Mar 2023 07:20:07 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-rc1-win64.exe
# Thu, 16 Mar 2023 07:20:08 GMT
ENV JULIA_SHA256=8bcb9ac062b86407c16f21052c05cc4a414a2623e708ccf4c41394857c849063
# Thu, 16 Mar 2023 07:23:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 16 Mar 2023 07:23:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a82d12251bcae9056bf6a6f14747ada9fcdf40428483e075e9be108ca5fd2f9`  
		Last Modified: Thu, 16 Mar 2023 07:35:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf31eddd4d173e07844fb9f65e557a1007a73ff38547e8a04c8d9fae0f1075f9`  
		Last Modified: Thu, 16 Mar 2023 07:35:54 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac9b4231675af55156ec7e72b036fde2dd179c361952d3dcea9238f06245dfb`  
		Last Modified: Thu, 16 Mar 2023 07:35:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e799e4d617c85ef3c77f7ace87d13cdf6bd3e3ef134669c4e48f86d3e3f82c`  
		Last Modified: Thu, 16 Mar 2023 07:36:37 GMT  
		Size: 161.3 MB (161284359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a667a31e1e4ce2707e0421cb3b81fa9175d73e48b4af1850251cb79b867ffab4`  
		Last Modified: Thu, 16 Mar 2023 07:35:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
