## `golang:windowsservercore-ltsc2022`

```console
$ docker pull golang@sha256:3ddd0bb87f3e56448b52e0ea1f4e8de90b36c99ff7a12289c6556c031353d925
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `golang:windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull golang@sha256:73928fdf1ebf6f1cbafdb983b32bdcfc67988f3336c790eb6f118d51bd982c51
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1814300147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ff93afbe1e2d12f1417bf146720525c3300be3d365574dd254299e3598f747`
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
# Wed, 15 Feb 2023 23:44:04 GMT
ENV GOLANG_VERSION=1.20.1
# Wed, 15 Feb 2023 23:47:17 GMT
RUN $url = 'https://dl.google.com/go/go1.20.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b493969196a6de8d9762d09f5bc5ae7a3e5814b0cfbf9cc26838c2bc1314f9c'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:47:18 GMT
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
	-	`sha256:a6db8675ff95fd87e8e89cc433742cf3d84da3917fbcaf40d2c038236cc248a5`  
		Last Modified: Thu, 16 Feb 2023 00:26:39 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847d86f8685399a8848f96788ce5f6671aa844f7bb99177c182388bd1ef30a14`  
		Last Modified: Thu, 16 Feb 2023 00:27:26 GMT  
		Size: 108.5 MB (108517926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8ee04b3c1c64de4bb6c0d08867c46adec1a405e58d2c8e435a744ef620a95a`  
		Last Modified: Thu, 16 Feb 2023 00:26:39 GMT  
		Size: 1.6 KB (1564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
