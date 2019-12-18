## `golang:rc-windowsservercore-1809`

```console
$ docker pull golang@sha256:d295f628e024d1f480b90782c8c74806bd3a6a342ece9614aefccd205ff7c6cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `golang:rc-windowsservercore-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull golang@sha256:b866cd34212167102835b9dd5858e8562b932fca20ed4f78fd8d55d0cb917457
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2379190589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:516eb1d29c27204cfeddb85bf9b817d1cd9f03d4f6726dc063b14ed130ce84fe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Tue, 10 Dec 2019 21:34:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 13:34:08 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Dec 2019 13:34:09 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Dec 2019 13:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Dec 2019 13:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Dec 2019 14:05:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 14:05:36 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Dec 2019 14:05:59 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 18 Dec 2019 02:17:22 GMT
ENV GOLANG_VERSION=1.14beta1
# Wed, 18 Dec 2019 02:23:06 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'daa07bea59ae0a11f8b5898f6f6f5b781ded4ee3c627400c857fc91ce5af5045'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 02:23:07 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e147f14e0d6a9cbd5261162dea8f3aac7a34db5d9f6a587a9aac6b88722a2da4`  
		Last Modified: Tue, 10 Dec 2019 22:07:34 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af04e5d2b105e542e6e35206984acde93bb7a05561558d5a68f4fe03a778781e`  
		Last Modified: Wed, 11 Dec 2019 14:39:54 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bfa557c5a2cdcf513aacd1331305f25ac3bc238a197b565a30e804041bcaaf`  
		Last Modified: Wed, 11 Dec 2019 14:39:52 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9225ac8c8af277dc04a83e5f427d1f786a5379ffeceefcb0a642804a1900a9b`  
		Last Modified: Wed, 11 Dec 2019 14:39:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5242d39c53cd757a2da7e1000dcfb3088458cbd7b9bae77856922ba0e0d3cfb`  
		Last Modified: Wed, 11 Dec 2019 14:39:52 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c56e66099f600dc40be5c6cefd6a108baa3aad0e55436bb71bbce49ecfa38`  
		Last Modified: Wed, 11 Dec 2019 14:40:04 GMT  
		Size: 29.7 MB (29668246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d207701eb729d7c7ed930fccce6a64828e8daef2b47d253498e0a7f1d769e176`  
		Last Modified: Wed, 11 Dec 2019 14:39:48 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f457a79e6f154e969cf9a5c28d049ca14572cfe51a231f795fb99fa1b40af1`  
		Last Modified: Wed, 11 Dec 2019 14:39:49 GMT  
		Size: 319.4 KB (319420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d893ded76110cf92f1c4d8091954ac2834cad20299b335b5a661bd5df731eb27`  
		Last Modified: Wed, 18 Dec 2019 02:34:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903c7ddb83e7472af89f7740f9bd8b28f434d5b6cb90bf5dd84e4df2d89f2705`  
		Last Modified: Wed, 18 Dec 2019 02:35:50 GMT  
		Size: 132.9 MB (132889980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5749c39dfe23e4d5c1ceaae796c8f7e521e95f26ac5b071484b26c9613f142c4`  
		Last Modified: Wed, 18 Dec 2019 02:34:12 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
