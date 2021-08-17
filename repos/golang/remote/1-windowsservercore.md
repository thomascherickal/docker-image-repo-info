## `golang:1-windowsservercore`

```console
$ docker pull golang@sha256:ac0edc8c85f1525d90cf9d8712b00b17064601dc98587309aee7745c413f71c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `golang:1-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull golang@sha256:5a21c2ef29a88259c0bd4cab37c5fa8f0de407aacfd9b924b8913dbd7ce33381
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2857181516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3f4ecf4d430e08ddcb552262b4fc54b8fcbb8ef9400a407d9df82f90e70cbe6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 12:44:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Aug 2021 12:44:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Aug 2021 12:44:58 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Aug 2021 12:45:01 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Aug 2021 12:46:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Aug 2021 12:46:38 GMT
ENV GOPATH=C:\go
# Wed, 11 Aug 2021 12:47:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 17 Aug 2021 02:15:24 GMT
ENV GOLANG_VERSION=1.17
# Tue, 17 Aug 2021 02:19:15 GMT
RUN $url = 'https://dl.google.com/go/go1.17.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2a18bd65583e221be8b9b7c2fbe3696c40f6e27c2df689bbdcc939d49651d151'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 17 Aug 2021 02:19:19 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1014a0987936e3fa4cd5e9d82f8e82b260d69af19d422f406e4ca0ca868a2c`  
		Last Modified: Wed, 11 Aug 2021 13:29:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e04f285ca5202ce380345855cc1ef257dca5d10c911e569374401b838c36c4`  
		Last Modified: Wed, 11 Aug 2021 13:29:32 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e030fd545aef8a7a910823c29f1d20459a9cadda6fb139615fc2889d11f9947`  
		Last Modified: Wed, 11 Aug 2021 13:29:32 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1e552f09bafcd7011149f53ca4fb6af5814124b3433a4fe57e214782457664`  
		Last Modified: Wed, 11 Aug 2021 13:29:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed64d631b20fa6a2ca7e09eca20fd2e38188e2c5bc403a2eb944f6287397a17`  
		Last Modified: Wed, 11 Aug 2021 13:29:38 GMT  
		Size: 25.4 MB (25449457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a878d0c3fc40265d3f68d6b133aec7f3420a961d7571859baab52b21a45fc5`  
		Last Modified: Wed, 11 Aug 2021 13:29:28 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4ac8a4869f7f108ebb1d40ba4cab2a4f2512a9d5cfc4e429b4503fae4825be`  
		Last Modified: Wed, 11 Aug 2021 13:29:28 GMT  
		Size: 321.8 KB (321821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0618a4b94c29a6c07f63a2312308e8ae8052b9c3e9f16b7f58bdffc00e91b5f8`  
		Last Modified: Tue, 17 Aug 2021 02:29:11 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71092d3782e737869101be7781727e642264a0d9777ea37f4bcb8af7cd949535`  
		Last Modified: Tue, 17 Aug 2021 02:31:52 GMT  
		Size: 145.4 MB (145400743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8d53c5e6bddcc8f48cef8855c90f51ad54d98805abeb8006d529dec35f2c4f`  
		Last Modified: Tue, 17 Aug 2021 02:29:11 GMT  
		Size: 1.6 KB (1576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull golang@sha256:b3d0829e6ae1b865b45f1cc9cd005821cda76b80bbe4fa617e514f843fbf21f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6446566161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:beae4194417afd83ef52a1f3af87d0256dab56d2a6464dbd1d92adcb94b9d3c7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 12:51:38 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Aug 2021 12:51:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Aug 2021 12:51:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Aug 2021 12:51:48 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Aug 2021 12:53:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Aug 2021 12:53:51 GMT
ENV GOPATH=C:\go
# Wed, 11 Aug 2021 12:55:27 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 17 Aug 2021 02:19:38 GMT
ENV GOLANG_VERSION=1.17
# Tue, 17 Aug 2021 02:24:20 GMT
RUN $url = 'https://dl.google.com/go/go1.17.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2a18bd65583e221be8b9b7c2fbe3696c40f6e27c2df689bbdcc939d49651d151'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 17 Aug 2021 02:24:24 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdf069d22adc9f9317381fb00edfaf147e2a08bbd9b9aa4e7668fced1fb98f7`  
		Last Modified: Wed, 11 Aug 2021 13:30:25 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fe66e8167823a0c5cbb100a89928213f61cf164cf8709d9fe899aed2983048`  
		Last Modified: Wed, 11 Aug 2021 13:30:24 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75da9fc8465c5617c2e9b3a97701f9cdfe7a723af01dc99760b253e5baccb50`  
		Last Modified: Wed, 11 Aug 2021 13:30:23 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3e058e701d1a72c8549ecca35484b40559546a5a523f18483669e7be3b724`  
		Last Modified: Wed, 11 Aug 2021 13:30:23 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368b8f9d5f23a5a86293ff894ff67bf071ab9c9a6bcc127538fb406bbd86de0d`  
		Last Modified: Wed, 11 Aug 2021 13:30:56 GMT  
		Size: 25.4 MB (25443893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce25892673b7913412a6752bf9e59770f7b6fbb617520c6d2468eb44bc660227`  
		Last Modified: Wed, 11 Aug 2021 13:30:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2d73c7ab13174923ca0891b1a659a7545e3294bde29225c8a5b69ff9bb7248`  
		Last Modified: Wed, 11 Aug 2021 13:30:21 GMT  
		Size: 312.9 KB (312924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df97c458c677aba5a6d2b7368ddfc1b31e3e8e5877ccaf9566e0791d53278849`  
		Last Modified: Tue, 17 Aug 2021 02:32:09 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f02e35bc80c918d42c28c68fa84804fc681e420b8effb40f27a068132b3ff6`  
		Last Modified: Tue, 17 Aug 2021 02:35:05 GMT  
		Size: 149.8 MB (149831814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb49e29467d986767a2ede5379f07e699cd6280218529fe700c5aad79e0a6cb`  
		Last Modified: Tue, 17 Aug 2021 02:32:09 GMT  
		Size: 1.6 KB (1576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
