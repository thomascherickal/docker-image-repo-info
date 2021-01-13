## `golang:rc-windowsservercore-ltsc2016`

```console
$ docker pull golang@sha256:9ea84907dce8399b898ba138cdcd597fdcad777fb6de8529cdb7b9d52d50f3bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `golang:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull golang@sha256:dcac782861802635da873141a43697833358faad82cb5da480938b646c59fbc6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5986039602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a23b1400b6966db1c309beb1f392a1554f91f5a71445adc0b5d95cd83df11f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:37:07 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:37:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:39:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:39:19 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:40:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Jan 2021 13:40:43 GMT
ENV GOLANG_VERSION=1.16beta1
# Wed, 13 Jan 2021 13:44:22 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16beta1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'f06e2d7f300843473527e8fdd2d496aef5ffa6507ade0ac1141934e5c6ca7d63'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:44:24 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7c74b9f7bda8494c06b61f172b711267512a7eef464aae2946fa79f14fbc6c`  
		Last Modified: Wed, 13 Jan 2021 15:10:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16980afcb11d4373e2ced6b4e81c79cdc57071c5b2d049925d8103e3b1685c0a`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b769faccdc304e663d15a124104d2aaa3ac8f722d364a8196f27a3cb7485cd`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee85b465f4b2c47a1ed4af61a17e4f6bd1f26c42b26eeba881f2a5fdf182619`  
		Last Modified: Wed, 13 Jan 2021 15:10:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a900fab54fda5407bf2c34f918f84f42c2ba78c89b79b10e5a8059a642814c5`  
		Last Modified: Wed, 13 Jan 2021 15:10:31 GMT  
		Size: 35.2 MB (35242884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4728bca9e3e0ca560fb0489af700986254ac669509fff4e8e8e208dde2bf3`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7738a5c4a381adacded290e0ed60fb37c9afa472ca097aae390199b16f444d`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 5.6 MB (5599196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0261c9acbf6a38bbf48b8ea629aa46a69d7eecca3a29e3b5a1f8d7a42776059a`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb7e9a283e1898bd3e7c5218ed4e6c6881e2a99b66ced8ca8bea57504d918e2`  
		Last Modified: Wed, 13 Jan 2021 15:13:18 GMT  
		Size: 151.3 MB (151294213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2706ebd2329fae4980e4565780ef225d63369637084ebd5b15479adc67e2069e`  
		Last Modified: Wed, 13 Jan 2021 15:10:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
