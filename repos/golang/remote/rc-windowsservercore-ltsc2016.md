## `golang:rc-windowsservercore-ltsc2016`

```console
$ docker pull golang@sha256:5646ea3d98a01a6d6699c51e781a119813372e38bca624c52a9babf4739025f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `golang:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull golang@sha256:2ecc96f2a4f37ba01456de42d1965426e54e2b3b961d9a2b2ac1400278ead343
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5900842386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3f3c321332a73016b524b3acfaec9bf5b25d39ff32913c078f7cf83220d4a1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 13:24:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Dec 2019 13:24:19 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Dec 2019 13:24:20 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Dec 2019 13:24:21 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Dec 2019 13:25:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 13:25:57 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Dec 2019 13:27:07 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 18 Dec 2019 02:10:16 GMT
ENV GOLANG_VERSION=1.14beta1
# Wed, 18 Dec 2019 02:17:07 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'daa07bea59ae0a11f8b5898f6f6f5b781ded4ee3c627400c857fc91ce5af5045'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 02:17:09 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3950a365ed21df7c5fc18af8b2147b5e63405629fea5a0ac991e8b82c2125f4e`  
		Last Modified: Wed, 11 Dec 2019 14:37:31 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f5739c346c42e45481f6abde958aaba0f6bf3a4f9c48289094f27b3361047d`  
		Last Modified: Wed, 11 Dec 2019 14:37:28 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6b396f1ce59257b7cef357370a5558ca4ba777270c1a28899df9612eb27adc`  
		Last Modified: Wed, 11 Dec 2019 14:37:26 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cce0af848e7c1522aa44d86b83ee44cb66d456a43edbd249a94418e43278b6`  
		Last Modified: Wed, 11 Dec 2019 14:37:26 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a49e787d145d51033130cfc379eda9fac5672649dbe9de44457d5231568304a`  
		Last Modified: Wed, 11 Dec 2019 14:37:41 GMT  
		Size: 30.5 MB (30462349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f180f53ab92b4c0d4b9731490d0390bbb70114064244ca352a6f20f9a859b1e8`  
		Last Modified: Wed, 11 Dec 2019 14:37:23 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0151a3d149c0a1af3e6800a5d696cab934d1b96840b6bd58b799f83b8b956f`  
		Last Modified: Wed, 11 Dec 2019 14:37:25 GMT  
		Size: 5.3 MB (5321723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c3491bbbe9ba62ce7529dbc8e96bcaac4c3a1fc22d31b1789431121a1fdae0`  
		Last Modified: Wed, 18 Dec 2019 02:31:57 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191cb96569364986e755328eba6381693910cb98aa7bb32dfe53e23e402847e`  
		Last Modified: Wed, 18 Dec 2019 02:33:36 GMT  
		Size: 142.3 MB (142344795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7860ec20ba728b503dae5a8543be1e0507cf6bc6ba8686a5145cc33357af5a23`  
		Last Modified: Wed, 18 Dec 2019 02:31:57 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
