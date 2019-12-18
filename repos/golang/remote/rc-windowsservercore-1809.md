## `golang:rc-windowsservercore-1809`

```console
$ docker pull golang@sha256:5aabddeb3e00bc7d251d4938ae95017cdae4919d37f726ddc49329c72a085d07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.678; amd64

### `golang:rc-windowsservercore-1809` - windows version 10.0.17763.678; amd64

```console
$ docker pull golang@sha256:0497b044181e63412b7de365f8b524746a9df11613aca9cbc3b10580a845a7f0
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2319454700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb22e9f8dc0fd73e610b464401290926b1bc8a6bf16c5ba6050642ed9c9f4aa1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Aug 2019 16:30:23 GMT
RUN Install update 1809-amd64
# Tue, 13 Aug 2019 23:19:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Aug 2019 23:19:22 GMT
ENV GIT_VERSION=2.11.1
# Tue, 13 Aug 2019 23:19:23 GMT
ENV GIT_TAG=v2.11.1.windows.1
# Tue, 13 Aug 2019 23:19:24 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.11.1.windows.1/MinGit-2.11.1-64-bit.zip
# Tue, 13 Aug 2019 23:19:26 GMT
ENV GIT_DOWNLOAD_SHA256=668d16a799dd721ed126cc91bed49eb2c072ba1b25b50048280a4e2c5ed56e59
# Tue, 13 Aug 2019 23:20:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 		Write-Host 'Complete.';
# Tue, 13 Aug 2019 23:20:40 GMT
ENV GOPATH=C:\gopath
# Tue, 13 Aug 2019 23:21:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 29 Aug 2019 21:40:52 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:46:30 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ed34ad4b9594ab0d19b2fed9b07ea56c573279f46041b3c40a17c39a35bf285c'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Thu, 29 Aug 2019 21:46:32 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e7a74de96ddd92684be53d574a43478c79c354fd328bf65d1efd9c4fb6bf29f4`  
		Last Modified: Fri, 09 Aug 2019 17:25:39 GMT  
		Size: 626.1 MB (626095226 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49e8b556e9f23d14a64e75a20243fad37f4429d9a29d8cb9fb084196bac2de5d`  
		Last Modified: Wed, 14 Aug 2019 01:09:25 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a7bfcc225796a3792d6eaefeffbd2c6c261d56dcfdb10bca22a1cbd128d6cb`  
		Last Modified: Wed, 14 Aug 2019 01:09:25 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7207398804693630e8b05adb375451974c6b7c5f1d5825feb471d6f5620582`  
		Last Modified: Wed, 14 Aug 2019 01:09:23 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b2d9de546f619698e8ea94803ab9a2d94a0699bceace7938dac83ef0e99437`  
		Last Modified: Wed, 14 Aug 2019 01:09:22 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8db49b48f004e4768a4b9edd3d965990a1353a69b6325b83730d88f716c2bf`  
		Last Modified: Wed, 14 Aug 2019 01:09:22 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54004d7266ffbe75a23db50e689668d2373fc034f971f659f455f167979e7e8`  
		Last Modified: Wed, 14 Aug 2019 01:09:33 GMT  
		Size: 28.8 MB (28804746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacf9c73615357841b65e8e81ef3d273a8920e6695e4684fca0c74345b64e12b`  
		Last Modified: Wed, 14 Aug 2019 01:09:18 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9531ff8d766637ed4fc53fa834505f51621208c436eb2abf12113f8ee9cc87bc`  
		Last Modified: Wed, 14 Aug 2019 01:09:19 GMT  
		Size: 294.5 KB (294524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b380245310403f664b8fc37500e9521036198caf42f6149b553eab06759a5f0`  
		Last Modified: Thu, 29 Aug 2019 22:04:29 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cd884ea7ab852e67dfe14b127919d9eb96d4a9af711c9e11f933cf516a159d`  
		Last Modified: Thu, 29 Aug 2019 22:06:03 GMT  
		Size: 129.6 MB (129565166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093485e90233883847c0dc917d8ae8db37c17c4bd0719d11b88ac3b6e9a8a542`  
		Last Modified: Thu, 29 Aug 2019 22:04:29 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
