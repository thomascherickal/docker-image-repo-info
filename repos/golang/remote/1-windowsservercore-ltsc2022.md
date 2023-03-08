## `golang:1-windowsservercore-ltsc2022`

```console
$ docker pull golang@sha256:440278cd863c4a347209ab77784fcf12959fef2ed4abedecbc3d6bee5e09c90e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `golang:1-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull golang@sha256:e22db6cbe34a6012abdc4b59791f00ea0c1671bd607935db65f44ba84428d543
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1814920640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a469c90cc42978cd5f9ff010de36333abfab61e277af0543f54b52076b2c69a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:42:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:42:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:42:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:42:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:43:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:43:28 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:44:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 08 Mar 2023 00:15:24 GMT
ENV GOLANG_VERSION=1.20.2
# Wed, 08 Mar 2023 00:19:02 GMT
RUN $url = 'https://dl.google.com/go/go1.20.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'fe439f0e438f7555a7f5f7194ddb6f4a07b0de1fa414385d19f2aeb26d9f43db'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 08 Mar 2023 00:19:04 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048a86b3278e59b840ad06b4cf5f5888ce1068d503522a95eb470d5126ed69a`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b07973952171f91c05aade363f3e6c9a2e84548f33eaa3c8e48632460e61f8`  
		Last Modified: Thu, 16 Feb 2023 00:26:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a95dff10905572b5f9177959a5a9f60a9364e1dd627ed52e34ec4bee3fb3069`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267caf437f5a3d92235ab7b8d55b2c812744f166725151ba701aef9d682c6e9`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a959ece2e33bce3f35c5c0adb01a3426c92111b309c15f8cc31200ebcf899`  
		Last Modified: Thu, 16 Feb 2023 00:26:54 GMT  
		Size: 25.9 MB (25852811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065416c07c5d80f7a085e0e84237051d7050a71103cc9d7fb6d5ef57725dc4c6`  
		Last Modified: Thu, 16 Feb 2023 00:26:39 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07015cae66c7ebb6b0adce2dfe424313b228bb703ac3e900deebe74ae961bb49`  
		Last Modified: Thu, 16 Feb 2023 00:26:40 GMT  
		Size: 571.7 KB (571672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bf0160f9904c7c766dd9d1a809407a6cc6d7f888d595d3e6fc1bc2da3af2ed`  
		Last Modified: Wed, 08 Mar 2023 00:51:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11113e604e7c49a742407d6b5cc80e00a7d8e1995ac4fdf09409a51ab237e3d`  
		Last Modified: Wed, 08 Mar 2023 00:51:39 GMT  
		Size: 109.1 MB (109138391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c93a85f2974733a41d8cd826539a1deb329a8fb8fc090df912699a38efd01f`  
		Last Modified: Wed, 08 Mar 2023 00:51:02 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
