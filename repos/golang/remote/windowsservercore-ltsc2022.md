## `golang:windowsservercore-ltsc2022`

```console
$ docker pull golang@sha256:56811870ea5e568807470c7c08c28e4d64c8069deea8b1956bff81f6358a6eb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `golang:windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull golang@sha256:46547683941fb7ee4425fb49f0abbc74fb54c49ec955eaba070d79a0a0646e17
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1560874202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc6f114c1cd91c408a97a514ac6e0a78d7b76fe3060c6e5eddc76aa31cbe3c6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 01:39:57 GMT
ENV GIT_VERSION=2.23.0
# Sat, 24 Jun 2023 01:39:58 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Sat, 24 Jun 2023 01:39:59 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Sat, 24 Jun 2023 01:40:00 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Sat, 24 Jun 2023 01:40:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 01:40:34 GMT
ENV GOPATH=C:\go
# Sat, 24 Jun 2023 01:40:55 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 01:53:07 GMT
ENV GOLANG_VERSION=1.20.5
# Sat, 24 Jun 2023 01:55:29 GMT
RUN $url = 'https://dl.google.com/go/go1.20.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c04a4ed73c3624d5b4c4f62e44a141549cc0bfd83a7492c31ca8b86b3752f077'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 01:55:31 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a725a5b1d95b19c55801da205e401134949a3ef3b2bb040c785986202ad134`  
		Last Modified: Sat, 24 Jun 2023 02:16:35 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94771fd18b203dc5bc66c78c94d318edc726e0d3622915884225783fae93b5d`  
		Last Modified: Sat, 24 Jun 2023 02:16:33 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c970e5e0e48292f70cad71999574a45005b6e3963bda38cfde70630ada11e37`  
		Last Modified: Sat, 24 Jun 2023 02:16:33 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6de2df6562966a148a26d7f00bf85d056d4d22c71ebe170634f84253f0b559`  
		Last Modified: Sat, 24 Jun 2023 02:16:33 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d888c846778cfed7da69e726b491b06cbec333bdbe711985b03844e3948608`  
		Last Modified: Sat, 24 Jun 2023 02:16:38 GMT  
		Size: 25.4 MB (25401467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ac5846332b11bb977d027d06552fe067f700a9d5a62560972a0e3c561e19be`  
		Last Modified: Sat, 24 Jun 2023 02:16:31 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0157f348cbd78f039722165c2f836f19d234498082d52f2bb0b601aca16fab`  
		Last Modified: Sat, 24 Jun 2023 02:16:31 GMT  
		Size: 264.3 KB (264272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0235a61add4a7aa7045aa27d4a97815ebd225ec0a6e814a7db2e08bd9fdabd04`  
		Last Modified: Sat, 24 Jun 2023 02:18:31 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d22d60a8242d920474d366452ef1c08363b9ac9c3c13c278e80866bb7adf2b`  
		Last Modified: Sat, 24 Jun 2023 02:18:54 GMT  
		Size: 108.9 MB (108898962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04a840fe6afe3844d4579d707ee583588027ae3b9930660ad6b876a508d5c87`  
		Last Modified: Sat, 24 Jun 2023 02:18:31 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
