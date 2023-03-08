## `golang:windowsservercore-1809`

```console
$ docker pull golang@sha256:671ddaabd0c612224815183f326ed5b4a705229efff916d03022677c932390b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `golang:windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull golang@sha256:9543cbf6c7bcdaf555292151838c81ff133c84a29610c8840dae921ff3fbc526
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2097845567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d79bbc7f27390b1c35610df8a9ebc6e1321b310f7d304e4851f71fe718a97862`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:47:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:47:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:47:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:47:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:50:19 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:51:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 08 Mar 2023 00:19:25 GMT
ENV GOLANG_VERSION=1.20.2
# Wed, 08 Mar 2023 00:24:23 GMT
RUN $url = 'https://dl.google.com/go/go1.20.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'fe439f0e438f7555a7f5f7194ddb6f4a07b0de1fa414385d19f2aeb26d9f43db'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 08 Mar 2023 00:24:24 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03ac75ee62e05ad7b8b8f97fb78a769177c49d210eedcf0a93035e9a07d0ff2`  
		Last Modified: Thu, 16 Feb 2023 00:28:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beb360c9024340aa5072ce67eab6b3cb005293938525c4f3b77c3bb03f9f501`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5051ce7a895da09ac63e7ca01ef4e30434d833dbd271107d6f96375f291752ad`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea419e1594fbbef3584b4731c356499c7b8a5616af16968e6fd693eccd92012b`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb97c6a047d2cfcb6f0ef6846e78c4d5f60212639a9d1892e2af05033c217df`  
		Last Modified: Thu, 16 Feb 2023 00:28:30 GMT  
		Size: 25.6 MB (25606151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941d25224d4bab25ba0b2304a5811b0fc2970ba6385afdbefbfec898720c3beb`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa161895f771062e6d8e8aa2e0e44c15c5affdacc8d409f6e70f1fa743a9bb1`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 335.6 KB (335550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8774f0aa960751ecf3a81fedaa15e32ddcd604d338de9dcf91753e9dbb076052`  
		Last Modified: Wed, 08 Mar 2023 00:51:54 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650f9ad8e71e3d6c1f1f9fbab90298f08aedaa9622761b936a30ae0e1488d54a`  
		Last Modified: Wed, 08 Mar 2023 00:52:31 GMT  
		Size: 108.9 MB (108934512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1247d381a1a468880872e091a4a2c38a6dc8e008ca4c01b7896a44a88a5f43a9`  
		Last Modified: Wed, 08 Mar 2023 00:51:54 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
