## `golang:1-windowsservercore-1809`

```console
$ docker pull golang@sha256:8d62482bde5b804a1e0e04ac2f60b91a45070213ded09a2fd0a3448a00d991a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `golang:1-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull golang@sha256:b0e2dbba43e24ea610059784b9822bdbabef65c2f77a9404240ef3b350fe31b5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509014744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94dec8bb9a8e35c1570ab7d534a2692375abbbd348edc1cbdbd8f225094f8132`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 03:21:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Aug 2020 03:21:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Aug 2020 03:21:03 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Aug 2020 03:21:04 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Aug 2020 03:22:19 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 03:22:20 GMT
ENV GOPATH=C:\gopath
# Wed, 12 Aug 2020 03:22:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Aug 2020 03:22:42 GMT
ENV GOLANG_VERSION=1.15
# Tue, 01 Sep 2020 00:21:57 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'dc491314dff5b87ad50bf1cf56715de8f8c54489be30f3e19239bc2ad1af25e3'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Sep 2020 00:22:00 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf9a89c3c77e3691ad21e944e050d0f707af4beccb5d0e6320c06a87ddbc8c`  
		Last Modified: Wed, 12 Aug 2020 03:39:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0d146795e491f61f0b626ef03d38388471a63b670048b8c448bd4dc5a7f646`  
		Last Modified: Wed, 12 Aug 2020 03:39:30 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e961ddbe3bac93f578dd1dff989cbafe17af1dd2990775cbedd26a925cb681`  
		Last Modified: Wed, 12 Aug 2020 03:39:31 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0882ddbf133ed474230ca699b21fe43a313120fdc105bbfa9499266cc4e29769`  
		Last Modified: Wed, 12 Aug 2020 03:39:29 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3479a311bf6fe991ffc5cc38be99ab660b0f84d2581a0dcd51c4dd69c7b8a48c`  
		Last Modified: Wed, 12 Aug 2020 03:39:37 GMT  
		Size: 34.2 MB (34235512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1762bbf84da632ba41d69e12e39ddfdddb007189e5b3b8ebe9b6f39737c39819`  
		Last Modified: Wed, 12 Aug 2020 03:39:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94125dc057700b2f1fb9b7ba07b1f6471c131d5e91b6732581994259f7f2775`  
		Last Modified: Wed, 12 Aug 2020 03:39:25 GMT  
		Size: 303.7 KB (303696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae119fc49ba49b85c298a9884d09e57937d851e70794215b335e8119f08d7fc`  
		Last Modified: Wed, 12 Aug 2020 03:39:25 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a32d8e269da96a407ff8652e4248b1f4af6ef716277d20694db76cd580d8af9`  
		Last Modified: Tue, 01 Sep 2020 00:34:47 GMT  
		Size: 138.6 MB (138599257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ca1c3761dde214db9d5944d50a47eac08a21feb0ead02cd0745dc9945dd4bb`  
		Last Modified: Tue, 01 Sep 2020 00:34:19 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
