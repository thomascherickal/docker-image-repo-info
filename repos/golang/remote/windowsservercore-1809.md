## `golang:windowsservercore-1809`

```console
$ docker pull golang@sha256:51d47783786158fd4a6d5e408c62e4605c08ebd644327d309234633bcba80f2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `golang:windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull golang@sha256:a178b945ff2ed6bb449f447c3e57c6184139921486a21b7298ac5decd37faf80
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154906872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68190a6d8b4020ddbd6dd3b5650d02f54f69c4cd8208ddabf4bed71a828ddf24`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Dec 2023 23:38:53 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Dec 2023 23:38:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Dec 2023 23:38:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Dec 2023 23:38:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Dec 2023 23:40:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Dec 2023 23:40:27 GMT
ENV GOPATH=C:\go
# Tue, 12 Dec 2023 23:41:35 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Dec 2023 23:41:36 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 12 Dec 2023 23:44:50 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Dec 2023 23:44:52 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c57683b4a629f3325c8517d99f497d4ffbcd0e70354e70a95d983a275bfe398`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95bef40c25d2abc3a12986675189e7152f6197fdc5a17343bdee3f0bc2e95a8`  
		Last Modified: Wed, 13 Dec 2023 00:04:14 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b043d50fbb4f0d8961fe3a95130f520d57cfe7e6e85b15cd4f9f14a01364f7ee`  
		Last Modified: Wed, 13 Dec 2023 00:04:14 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55867ab446b5d5e34f9e6d414898b9a0b31051afc81b28ace1ce47e27d9e24ee`  
		Last Modified: Wed, 13 Dec 2023 00:04:14 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10285db29cf842d22a49b00cb66fbbfe20e7d4e72a0d3e393d58824190f6835b`  
		Last Modified: Wed, 13 Dec 2023 00:04:19 GMT  
		Size: 25.6 MB (25558777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3037ad7a881ee540014f48a43aa3a857c479d9cefb413ce61a914c943901890b`  
		Last Modified: Wed, 13 Dec 2023 00:04:12 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788faab53b378465ec447dde1961338c1349487d1152856c0524e2f6a503ec70`  
		Last Modified: Wed, 13 Dec 2023 00:04:12 GMT  
		Size: 282.5 KB (282534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc4b3ad2cc8f1d1b0630df92c06f374f5b420ee099e35053c1cd6e24e4d2db7`  
		Last Modified: Wed, 13 Dec 2023 00:04:12 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b1064571111ad923855b0f83eb719752d01921d346a48cc45627432cfab098`  
		Last Modified: Wed, 13 Dec 2023 00:04:34 GMT  
		Size: 69.3 MB (69345663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51105d12d66b535f3229f3dc981d3d3cb0c830f862093c39cc191360020d3b2e`  
		Last Modified: Wed, 13 Dec 2023 00:04:11 GMT  
		Size: 1.6 KB (1574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
