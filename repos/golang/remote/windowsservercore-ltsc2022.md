## `golang:windowsservercore-ltsc2022`

```console
$ docker pull golang@sha256:c7a92beb8028dacfecd0ac8aeed4f563b10f0b743a2602162af61b0a2954161e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1366; amd64

### `golang:windowsservercore-ltsc2022` - windows version 10.0.20348.1366; amd64

```console
$ docker pull golang@sha256:18889a02577477968683b422bbab5e353c01e063fadeaec1098080a257127cb5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679709391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe65f451c0725297b1971b520438cebda06432d613e02730ea25538886e2756`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 09 Dec 2022 09:36:47 GMT
RUN Install update 10.0.20348.1366
# Tue, 13 Dec 2022 22:45:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Dec 2022 00:13:55 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Dec 2022 00:13:56 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Dec 2022 00:13:57 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Dec 2022 00:13:58 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Dec 2022 00:14:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Dec 2022 00:14:46 GMT
ENV GOPATH=C:\go
# Wed, 14 Dec 2022 00:15:18 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Jan 2023 00:00:17 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:03:31 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Jan 2023 00:03:33 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfa20ce142ecceb471dc070d9582fff942cef447b7c8ff22f2223ffe3737c99`  
		Last Modified: Tue, 13 Dec 2022 23:54:14 GMT  
		Size: 1.0 GB (1021665190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb8b9a4ec3ca516cfaa44f64e80b1e3aaecdbde870177411ff046f81f991dd2`  
		Last Modified: Tue, 13 Dec 2022 23:51:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39e949ed00a67bfedd910770b630dc901df3b74f58d6755b55714def7d6710d`  
		Last Modified: Wed, 14 Dec 2022 01:11:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eb5b41928124d94b99e548d8010c06fa5a01ddc4965df09a0a45de870fd602`  
		Last Modified: Wed, 14 Dec 2022 01:11:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf6c5652a34a0b006bbaabc715acea90b976298b71368163a4c825ca557df68`  
		Last Modified: Wed, 14 Dec 2022 01:11:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31770cf797a116c54aabbc41c4ce0a1fdd94b455881fad04c47fb8e035443a52`  
		Last Modified: Wed, 14 Dec 2022 01:11:55 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5d864bf59b78f6d1db2f91bee0c4f7959333189bb8c4a7a9c26402ac824ac3`  
		Last Modified: Wed, 14 Dec 2022 01:12:03 GMT  
		Size: 25.7 MB (25660561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318f13fe4094e65caf46f5d176223522e26763a1841252e6d76f5a68a3c816c5`  
		Last Modified: Wed, 14 Dec 2022 01:11:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7cbf5baf91a376e73bdb128ea3a0678267ed8fd1f560b300225eda3349da34`  
		Last Modified: Wed, 14 Dec 2022 01:11:53 GMT  
		Size: 514.5 KB (514472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2b4af7525729df7b5e55266503faf43ec477a8a881ddeadd2951fda23bf222`  
		Last Modified: Wed, 11 Jan 2023 00:33:43 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6617f98e78da46dbdc5e6f58ccc596c60b59df0af894a8dfc488e97e1fe714a5`  
		Last Modified: Wed, 11 Jan 2023 00:34:39 GMT  
		Size: 157.9 MB (157860086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f9a070eeb09e4593ad524c601e56d5679c0ce24a808f465fa33b5989c1b0d0`  
		Last Modified: Wed, 11 Jan 2023 00:33:43 GMT  
		Size: 1.5 KB (1540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
