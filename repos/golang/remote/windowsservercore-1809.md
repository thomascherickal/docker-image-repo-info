## `golang:windowsservercore-1809`

```console
$ docker pull golang@sha256:c062a0f3fe1c6933cd89254239cba236ff37d6ce568b5854704392c5b29cfea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `golang:windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull golang@sha256:b0e80fae0befb86cf3d585f6f6dd4069340651d729f9019f766d4fcd56f20018
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2608853320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad283465532165f764806aaed447d99eeb933500c8127ff1625a3e845dccf8b3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:32:54 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:32:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:34:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:34:01 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:34:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Jan 2021 13:47:32 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 13 Jan 2021 13:50:15 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:50:17 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad72ac4b6931b207a545d6d62fda35143222f3144778d4338ba25345066dce83`  
		Last Modified: Wed, 13 Jan 2021 15:07:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa315e63f98a74b6d8eaa632289849e8ec86de24cc05b5a05e0f5e60fef47ca1`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32646dc4c31ba7b4756ec7a55372b0b826608da90c73a1b0e70be1ec400e5cd9`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e012143f550ba0c16a6368ae3695a74a56b153468e98d9c463221448e557b`  
		Last Modified: Wed, 13 Jan 2021 15:07:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de36418fb6d968516c8374e5baf49e2bce6bbab4a107753c235e67c36187e16`  
		Last Modified: Wed, 13 Jan 2021 15:07:25 GMT  
		Size: 34.5 MB (34452685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349aa2cb74f5d5cc343c42d6ba9fec62a6885cedcc0f07995fa77e3f68c6ac75`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384ca1dabb9f23cb13f29f907b3a436e7676da86a825631d876e4a204898b47`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 300.8 KB (300786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d2e467ff941e29cd3a8cdb0706b227a1475b3c0d048a45ecda6820adac910d`  
		Last Modified: Wed, 13 Jan 2021 15:14:27 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3537629bf7b43c4d30c002c5a0dc0e2ec5e3d828cf7ef088f88f2663abf50205`  
		Last Modified: Wed, 13 Jan 2021 15:14:57 GMT  
		Size: 138.3 MB (138318432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff0d78dc7ca0efc7677698accfc5f2599714e1a53cecb7eee760cef28131d8`  
		Last Modified: Wed, 13 Jan 2021 15:14:28 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
