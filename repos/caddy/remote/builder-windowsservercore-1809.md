## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:400b57963363cf511d64bfc6600baf5da26b08a9b5c00a8c454492ed1b42f0a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:9b312efe7309c3718f7329ad585bac045841698280521eeb3899e97f2d6b5f89
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2257313697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bed9373becad1f9de986ced4fc7f6fb229d0f01548cb064a5863d6f71d4ff5f7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:22:56 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:22:57 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:24:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:24:15 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:25:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Jun 2023 20:28:43 GMT
ENV GOLANG_VERSION=1.19.10
# Tue, 06 Jun 2023 20:32:46 GMT
RUN $url = 'https://dl.google.com/go/go1.19.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c749a054a5da17202113455040484893c29ebe5ab71fa89f60cdfb4561dcce8c'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Jun 2023 20:32:48 GMT
WORKDIR C:\go
# Tue, 06 Jun 2023 21:00:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 06 Jun 2023 21:00:06 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 06 Jun 2023 21:00:07 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 06 Jun 2023 21:00:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Jun 2023 21:01:16 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 06 Jun 2023 21:01:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69c8e1c8adec95ce194194fafcfc6a1e07f15344588a0b08f7f625c5a547434`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47736757cd8e844fa5669cb79caf4053a95eb6b57e09dd4ab01823f071f92f24`  
		Last Modified: Wed, 10 May 2023 01:46:45 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd4aa96423c060d9cbb5c55c535627e8c1e46ba89f752a3d601450afe81b5b8`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f8de560673af047f7136635e2e62927f8f69d11a928140de06383e86fb295`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed8138b5cc05a953f350e06a0713c2c031257b514bb362629f520d00db71fd7`  
		Last Modified: Wed, 10 May 2023 01:46:49 GMT  
		Size: 25.5 MB (25530178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a31d39859b5f50d901390aa5410b00f1637dce1a5839d12e69722fab50294`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05276aaa698fd9d43e2a1961637e16578fa84a5128237d7c2bdfe57c54fa89`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 262.2 KB (262162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145c27882aa95deb557b34ea4775c343538ab0e15df638e3ba9dba2c8b383105`  
		Last Modified: Tue, 06 Jun 2023 20:41:50 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d2b08c6f1a900f411e30837cda5535f2479950908789124b8e0816d55a2ea3`  
		Last Modified: Tue, 06 Jun 2023 20:42:22 GMT  
		Size: 157.8 MB (157784985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5738d6c2dc28bce52fe1b9b9b4334a1b8abef37c4a875452c8033efd3e019629`  
		Last Modified: Tue, 06 Jun 2023 20:41:50 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e0fa0da7d91252c25b2876e694690a91c071d00c3f53454e3d05a53ca40a1a`  
		Last Modified: Tue, 06 Jun 2023 21:04:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ff12474f51f12ca2bb1ea533024114e68145faba6b39abfb4ef12446214754`  
		Last Modified: Tue, 06 Jun 2023 21:04:57 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac0b644474175906a8e998da081458d9372cc676cfc02c4c96e549b5a91f994`  
		Last Modified: Tue, 06 Jun 2023 21:04:57 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ab42fd5113905fcea5f918cd7b973b48bd493a5639f2d08db27d7ca6cea4fd`  
		Last Modified: Tue, 06 Jun 2023 21:04:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d99b6ebc91560aeabe366aad9904cee36ba2da4aa6654e75a51646ca28e22d3`  
		Last Modified: Tue, 06 Jun 2023 21:04:57 GMT  
		Size: 1.7 MB (1682778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405c21fdaceb25058c1a46c82e31cd74abece49ba5151c28bcc3736d28b50952`  
		Last Modified: Tue, 06 Jun 2023 21:04:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
