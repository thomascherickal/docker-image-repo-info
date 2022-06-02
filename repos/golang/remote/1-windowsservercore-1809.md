## `golang:1-windowsservercore-1809`

```console
$ docker pull golang@sha256:c4e20b291c54f6501a033406bfd4b652881bf69ac0c1371e8c401c6f690c71b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `golang:1-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull golang@sha256:487ef9eb0ee6853bb2a0c7f5319773e232bf240c4247202ae9cf3f6610073587
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679546290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c506c8075604a5318c731c6af4834b84581a9bfbb97f57c8d96b96707f224961`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:21:43 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:21:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:21:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:21:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:23:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:23:36 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:24:28 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 01 Jun 2022 23:19:02 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 23:23:07 GMT
RUN $url = 'https://dl.google.com/go/go1.18.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '9c46023f3ad0300fcfd1e62f2b6c2dfd9667b1f2f5c7a720b14b792af831f071'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 01 Jun 2022 23:23:13 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01012ab52f3f9693dd4b85e6e19a0b2659b4f869d6b5b5d2ea62afe84c9037c`  
		Last Modified: Tue, 10 May 2022 22:55:50 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988abb6e02c6ab2eb0330641b6378c4e110c132c761de086dfc1629462491e90`  
		Last Modified: Tue, 10 May 2022 22:55:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b62ac07a4cd6e0fd762f7f6e904be7b001affa78e8fbfeb8ca017a6f643d62c`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e235721feec6368d5a652fd467681dffe74326d42da4bed8e43f777bc39c47`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195b6f87245387233358bc8fcc2679a23d9aa46cd4bfef94ac49284694c5c42`  
		Last Modified: Tue, 10 May 2022 22:56:13 GMT  
		Size: 25.6 MB (25580295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cfe0249f2fac54d31ea467ce63bdc69e4504b726a87d969fb1b42ab2ab3853`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c97dcc9056ac36ad6120d94049a937f5366e71fda7c478ff3462d542cc0645`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 322.0 KB (321981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dc288e337b76fda8623680f18337c4b78ccbee9f0ce3a7430a6b55b6b20c73`  
		Last Modified: Wed, 01 Jun 2022 23:46:47 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e69e97f763f508105fe5912b6a5354711d4cfece559b9a0ca1c37b92514ba3`  
		Last Modified: Wed, 01 Jun 2022 23:47:23 GMT  
		Size: 149.6 MB (149576688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cee23a66a74df107597da974f1279d6b695571734e483317347644833a6273`  
		Last Modified: Wed, 01 Jun 2022 23:46:47 GMT  
		Size: 1.5 KB (1532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
