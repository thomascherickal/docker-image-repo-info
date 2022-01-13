## `golang:rc-windowsservercore`

```console
$ docker pull golang@sha256:0e47d8fa4ebf3734b471d45295dcb2944b1f5dcbb4096bc29f5474dd08baa509
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.469; amd64
	-	windows version 10.0.17763.2452; amd64

### `golang:rc-windowsservercore` - windows version 10.0.20348.469; amd64

```console
$ docker pull golang@sha256:fb2268fb6ce8acae4010997755880e5aff8b62f9ce6ba159156d97bd36b1bf81
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386191589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de57f129329bb3e548066efcd5c4477b1774850946756ea7485356c23e72bf9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 06 Jan 2022 03:56:33 GMT
RUN Install update ltsc2022-amd64
# Tue, 11 Jan 2022 18:59:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:22:31 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:22:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:22:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:22:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:23:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:23:17 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:23:37 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:23:38 GMT
ENV GOLANG_VERSION=1.18beta1
# Tue, 11 Jan 2022 23:26:49 GMT
RUN $url = 'https://dl.google.com/go/go1.18beta1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3a43ab4ec28eee6b10fd412a055724d962227f1c27a78960d6d229d741f8353d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:26:52 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b593686e27e7562a5b0696823307ffa822214cee8bd2eec1075eadad4cb9712`  
		Size: 956.0 MB (956001983 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:99e0b71ede60d3b2c5b9053bf27e47c0875590991eede49813d849cc660c7551`  
		Last Modified: Tue, 11 Jan 2022 19:32:06 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33c04b46e837d2c2d65d27c4cf6ea8cc6bc9b69b139f59939aec13286cb21d1`  
		Last Modified: Wed, 12 Jan 2022 00:33:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471cfbdc8450d61fc2679935e89cc63e93a62128657ebbff7748822fd35e11ea`  
		Last Modified: Wed, 12 Jan 2022 00:33:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7117ecfa33a6bfb5e69a464d2c63689bf85142011fadab692400e3b69b8112f1`  
		Last Modified: Wed, 12 Jan 2022 00:33:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c5e32fdff85ef6ee027f7c4c3e493cd61277c60a78ab5ed004bc7292fec2ca`  
		Last Modified: Wed, 12 Jan 2022 00:33:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5337cb4af0e43e5baa89a2ac620af93dc1cc90bd3405ef585e38c51f2bf21e`  
		Last Modified: Wed, 12 Jan 2022 00:33:29 GMT  
		Size: 25.7 MB (25726881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cba8b4a94695a9711485cb92bc0d1b020bbbe864b9c14a38924aaf3b2934526`  
		Last Modified: Wed, 12 Jan 2022 00:33:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a9d9e67464e429dc7b85b34c6f11c26495b439e99d86955e2c3aba70e8b106`  
		Last Modified: Wed, 12 Jan 2022 00:33:20 GMT  
		Size: 552.5 KB (552542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35225b2559067ec982c61576b801d4a2d269ae9e871db80a92fe936b4b2a1b55`  
		Last Modified: Wed, 12 Jan 2022 00:33:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba3e672941f7997a5f50e6ffb10a41e8c68f822cbd53d4699aefeaa985d3be4`  
		Last Modified: Wed, 12 Jan 2022 00:34:04 GMT  
		Size: 152.2 MB (152199778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cd8d91a9745f78add73507189e35541de6ded9fe45296ef9ae1bc2b0ee27e7`  
		Last Modified: Wed, 12 Jan 2022 00:33:19 GMT  
		Size: 1.5 KB (1534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull golang@sha256:fde228562aed99bf0ab11afaf1fcddc196287609e10b4b91dbb02210fd730cd6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2889947045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63cc34c3e63ae24d25eb004f5cd7352f51dd41a87a31765174ea1b1a9b5c0a8f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 05:11:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 13:12:57 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Jan 2022 13:12:59 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Jan 2022 13:13:00 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Jan 2022 13:13:01 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Jan 2022 13:14:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 13:14:34 GMT
ENV GOPATH=C:\go
# Wed, 12 Jan 2022 13:15:32 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Jan 2022 13:15:33 GMT
ENV GOLANG_VERSION=1.18beta1
# Wed, 12 Jan 2022 13:19:28 GMT
RUN $url = 'https://dl.google.com/go/go1.18beta1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3a43ab4ec28eee6b10fd412a055724d962227f1c27a78960d6d229d741f8353d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 13:19:30 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3a70d5fd54e2005efbf590b48700ed40509210354a0d8f3f18c3b444a5325896`  
		Last Modified: Wed, 12 Jan 2022 06:20:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab3a92c283c23da1114b5a193a81bc6464487c56644cd0bbb282c8006c0ffaa`  
		Last Modified: Wed, 12 Jan 2022 13:42:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1027379611971de6bc3465f90bc32c2729568caf4dfb1a06f4d6cc4ff35e99e`  
		Last Modified: Wed, 12 Jan 2022 13:42:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b47e1608cc7d7d18e98e6db8694fd18ddcc8ba3d16a703a425dae7226d8e48`  
		Last Modified: Wed, 12 Jan 2022 13:42:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c81b433ad7a26ae8b6d6fc12e05f2d425fd833e56075e1fb78fcadfab87bb2`  
		Last Modified: Wed, 12 Jan 2022 13:42:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eeae2fccea1e527dd0fa62be4cffc50ba8b29e94ec11fa0c5215f818ab8629`  
		Last Modified: Wed, 12 Jan 2022 13:42:30 GMT  
		Size: 25.4 MB (25431808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1f7bf5edc2db8a4a216d6e45e182173d1d422212d465f1ea289b8ea42bc9e9`  
		Last Modified: Wed, 12 Jan 2022 13:42:01 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfbbfd1398b65c72295f46f951a4ab9d97d5b234d1019afdd12eaa588dd478f`  
		Last Modified: Wed, 12 Jan 2022 13:42:01 GMT  
		Size: 309.2 KB (309240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e120ae46f408e7564eb1d19088e1fb55520dc820b3aba3b4dfedeeb26215ff2`  
		Last Modified: Wed, 12 Jan 2022 13:42:01 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52d29a446eeef6492040fc919fc4e95150e860c22e2770cb0bd69cdb06e3676`  
		Last Modified: Wed, 12 Jan 2022 13:44:50 GMT  
		Size: 152.0 MB (151963650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf956a8cd78baacbebf342cb28a0ad8d9a2dbda58b64e39d6d61da776357ff54`  
		Last Modified: Wed, 12 Jan 2022 13:42:01 GMT  
		Size: 1.6 KB (1583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
