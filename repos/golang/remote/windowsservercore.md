## `golang:windowsservercore`

```console
$ docker pull golang@sha256:fc890eb62c36a4b99bee690c7912b21f1ee66071e3a97afb76b9db1ce443d8e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.469; amd64
	-	windows version 10.0.17763.2451; amd64
	-	windows version 10.0.14393.4886; amd64

### `golang:windowsservercore` - windows version 10.0.20348.469; amd64

```console
$ docker pull golang@sha256:197db40b76cce7e70d59e59cc567896395730c6491e7b3da5d1f4c22efa72404
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2379603452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79cbf44ca2d6b524c24bfafa8b9834f0d6037d50e52e097518edefe18dd286d0`
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
# Tue, 11 Jan 2022 23:49:46 GMT
ENV GOLANG_VERSION=1.17.6
# Tue, 11 Jan 2022 23:52:59 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:53:01 GMT
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
	-	`sha256:af591c468e014307dc43a97e00c818b3b7acbc7b27de278bf1faf17358860197`  
		Last Modified: Wed, 12 Jan 2022 00:37:41 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6469e64bcf49daee32dea37f8fa94244f9c13ba65b454049a73b3b5b8d8ea7`  
		Last Modified: Wed, 12 Jan 2022 00:38:15 GMT  
		Size: 145.6 MB (145611623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fafff45c869bf51b7c84d028496992e3d30eac68bff6280e7fa754a14d0cba6`  
		Last Modified: Wed, 12 Jan 2022 00:37:41 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:windowsservercore` - windows version 10.0.17763.2451; amd64

```console
$ docker pull golang@sha256:49f4b487ec8699ef797a83375c2d74877ba7d5ebd71beaccdfe42883845442ed
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2882771823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb289631534e10918f5b31171d45fc0fbe365c62189f74dab81e9e919b0c6d18`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 05:42:07 GMT
RUN Install update 1809-amd64
# Tue, 11 Jan 2022 18:28:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:27:04 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:27:05 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:27:06 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:27:08 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:28:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:28:42 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:29:44 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:53:14 GMT
ENV GOLANG_VERSION=1.17.6
# Tue, 11 Jan 2022 23:57:11 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:57:13 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ca87ac6c02d88482e9b4bf7c5b3be47ddaa1940332b4730a0b1384b4efb987cf`  
		Size: 993.3 MB (993251600 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d817badb08ee5a6edbd47efdaa8f9393db0c59d351be8a78deda5364ab70de7f`  
		Last Modified: Tue, 11 Jan 2022 18:34:27 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ada63dc008195485ae0731db2565b5d623934b26e48de5197425cfa9b37298a`  
		Last Modified: Wed, 12 Jan 2022 00:34:24 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777a82a5a181c521a5d0d54281a6011f091128b428de56f1efd201fa18e19e6a`  
		Last Modified: Wed, 12 Jan 2022 00:34:20 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74c867ed128cf0441faadf742a89c31cfe803cb2f6aa235f15daeea8fa5cb3b`  
		Last Modified: Wed, 12 Jan 2022 00:34:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f76926e34db152771b6ae59ed3a8c561d62cce2b71e201b69c8ba9a4aa19647`  
		Last Modified: Wed, 12 Jan 2022 00:34:20 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6896a1446766e2ce228c178cc69b20534f0911ef8c079151df9e169580ffb8ce`  
		Last Modified: Wed, 12 Jan 2022 00:34:27 GMT  
		Size: 25.5 MB (25456669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4224f2695e4dbf558987c0b621e53e7f2cf4294979cf39b6554f0dfdc873e1`  
		Last Modified: Wed, 12 Jan 2022 00:34:17 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420bb11f89959035c209b18ab6383726d2cf0e3922197c3aa6fb0f83afa7afb5`  
		Last Modified: Wed, 12 Jan 2022 00:34:17 GMT  
		Size: 327.2 KB (327186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a620f246a3066bd6bcd9cf40ff5f4ba41391a48e47475fd5a8643629c7d9b2`  
		Last Modified: Wed, 12 Jan 2022 00:38:32 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad1e3f7b1410bbf68944ee3336da8b54aa5676d1f39be718cda0e4af79a4522`  
		Last Modified: Wed, 12 Jan 2022 00:39:10 GMT  
		Size: 145.4 MB (145391945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e852d631dc9c7c39bc584e89d1cad82f0dce37a31f34e6ffd14a06011a83cbf`  
		Last Modified: Wed, 12 Jan 2022 00:38:32 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:windowsservercore` - windows version 10.0.14393.4886; amd64

```console
$ docker pull golang@sha256:6f0754f78696154649226d43f7e5b15549ed17dcb1ebb1b0280bd27e9f3116e6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6453808037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce978954ec9498e578ee29e9d6fcd065bb578f441f6b3fd1ed501b33e80c39a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:14:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:34:03 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:34:05 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:34:06 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:34:07 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:35:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:35:42 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:36:45 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:57:30 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 12 Jan 2022 00:01:53 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 00:01:55 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b5116c05ddf6ecb5a348f7628e3f3264afbb9909d86798316dbaff4a0e991a2`  
		Last Modified: Tue, 11 Jan 2022 19:35:13 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2caa59a1aaa1c092020bbca2ed4bb1396365f4d9d04ddbbd111ee689414c97a`  
		Last Modified: Wed, 12 Jan 2022 00:35:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9fe19533bf1afd7f80fd9cf407f00011eff59836d40dcceb1896e75ea99bf5`  
		Last Modified: Wed, 12 Jan 2022 00:35:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40700bafb918466fc1727b2e59ec5eb21d347affb09989cc72ac6db12220b882`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3180faaeb4219e7d41bb57faeebe12d142e8e246bac5ab81c8ef38499116de13`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6189cfcbd5a7447e171b486da44213e8ff4721ecbf15998668c0b32e6fb06aaa`  
		Last Modified: Wed, 12 Jan 2022 00:35:18 GMT  
		Size: 25.4 MB (25440280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4766ed70813b67e83228fa314c288fe9a1998bb85cbbd29f2a4b0518e49a7c15`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8f2e04b601edd119e847cbb2468052ab4681cd44bf4e9bbdf9b6c3f792d0ae`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 306.6 KB (306585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef103850c637e1ce1f8d175e0c4b5c7d6c2a3a29d2b8ad15bed8eab49be3dde0`  
		Last Modified: Wed, 12 Jan 2022 00:39:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1f406ac407910a0724e1fbad6ed8772a277ce69316a98a2defcebb5320504`  
		Last Modified: Wed, 12 Jan 2022 00:40:03 GMT  
		Size: 149.8 MB (149846909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdefe1352ad86026fe87510dd97f9a9acdbb5a700fc6a8aea2bd6eaa3194bd6`  
		Last Modified: Wed, 12 Jan 2022 00:39:28 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
