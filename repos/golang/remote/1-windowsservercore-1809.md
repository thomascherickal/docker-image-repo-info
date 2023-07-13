## `golang:1-windowsservercore-1809`

```console
$ docker pull golang@sha256:c7c3dd56bcf9381a255b8de966d7f9303144bb833afb80b11aa2504ffddc6aac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `golang:1-windowsservercore-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull golang@sha256:61c69dc167ab6f4dd9e8bdd8da837885a40ab4c551067f9b1507fbf7f6e8422c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2074331520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce8bcb102e7bee37f8aad79eacfaad1e4f99b14fdc9055e8279ae2b39a46203b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 13 Jul 2023 20:32:49 GMT
ENV GIT_VERSION=2.23.0
# Thu, 13 Jul 2023 20:32:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 13 Jul 2023 20:32:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 13 Jul 2023 20:32:52 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 13 Jul 2023 20:34:19 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 13 Jul 2023 20:34:20 GMT
ENV GOPATH=C:\go
# Thu, 13 Jul 2023 20:35:18 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 13 Jul 2023 20:46:31 GMT
ENV GOLANG_VERSION=1.20.6
# Thu, 13 Jul 2023 20:49:44 GMT
RUN $url = 'https://dl.google.com/go/go1.20.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b67dd7f2b4589701e53c98e348e1b4d9a7c3536dc316941172b2f0b60ae4ce5f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 13 Jul 2023 20:49:46 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e45ab66f9ac94fc8ae1502d608bfafe55474826433492ded72aec621e806135`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec77006091819bb389d795fbc65cfaa9816b1ec1d290fa69d7463deca96f34`  
		Last Modified: Thu, 13 Jul 2023 21:08:49 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644e3d07488adc4a8ad4814e56aa81e6fca904355063f428ffb268295652ffe2`  
		Last Modified: Thu, 13 Jul 2023 21:08:49 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd32009b5917604a82cfb40d9544473ce70effdf77f88e2789da38c728bf558`  
		Last Modified: Thu, 13 Jul 2023 21:08:49 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a4965a15372d2b5cedfe4d4430099e41e99422d4cca3691a98cbec84eecbac`  
		Last Modified: Thu, 13 Jul 2023 21:08:55 GMT  
		Size: 25.5 MB (25539036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae3b26bb532e185a0466f153372175d53da071a98b81698629642ad9beaa7f6`  
		Last Modified: Thu, 13 Jul 2023 21:08:47 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c849e84b956dfd8d9b126adc28c0df4e277eb9af511f64babd04a6a14726333a`  
		Last Modified: Thu, 13 Jul 2023 21:08:47 GMT  
		Size: 199.7 KB (199676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d198b69a7b771e6e7cc3c2928c066c7c49f8eb71db9d8f3043e32d897a241d75`  
		Last Modified: Thu, 13 Jul 2023 21:11:43 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f89412f9862f88684a4772ad20d2b5904ec11ed0d9658426202e912d1c9bfb6`  
		Last Modified: Thu, 13 Jul 2023 21:12:07 GMT  
		Size: 108.9 MB (108892705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d81636262b66c585f8cd69b8d112b622ae8a77d442e29739b92c1c0dc24eeaf`  
		Last Modified: Thu, 13 Jul 2023 21:11:43 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
