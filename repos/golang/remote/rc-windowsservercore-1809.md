## `golang:rc-windowsservercore-1809`

```console
$ docker pull golang@sha256:92514de27afa93632ff7005ae5bcfd904692225f8350f1c555675d69c109cd14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `golang:rc-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull golang@sha256:f39bfefe8f62ccff0772c2590bddd9912aa12808c6bf6b37de5e62473a2b021f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2380550053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:964ed8381c5d9ea1c7364c845ad99f23799a26c830dd38de3a5c979407a79bee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 13:22:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Jan 2020 13:22:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Jan 2020 13:22:52 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Jan 2020 13:22:53 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Jan 2020 13:23:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Jan 2020 13:23:58 GMT
ENV GOPATH=C:\gopath
# Wed, 15 Jan 2020 13:24:21 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Feb 2020 00:28:30 GMT
ENV GOLANG_VERSION=1.14rc1
# Thu, 06 Feb 2020 00:34:08 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '4f714ebb1904b96e1a5fe551ba195d9bcef7a41706d5b34e377d0106020b3f04'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Feb 2020 00:34:10 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c34cd616875c2f9d033967e4516512eeda759d5d727381f68534f20a423fbc5`  
		Last Modified: Wed, 15 Jan 2020 14:19:45 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f8f6402962aaf689f18fb7dc48707abd1442236650fa93feafdb8a0e62b884`  
		Last Modified: Wed, 15 Jan 2020 14:19:45 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2ccd2aa22967996e2db31a32fa197fe049385493a27f6cac5d28e147dc77a1`  
		Last Modified: Wed, 15 Jan 2020 14:19:42 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4005eb5a3fe7e59daa2cf4c83ef39ebc3b67aa33c077f34727270a45d08386`  
		Last Modified: Wed, 15 Jan 2020 14:19:41 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123a2902604294d730658cf5b5098adc030395e96b276912489cd129282805d1`  
		Last Modified: Wed, 15 Jan 2020 14:19:55 GMT  
		Size: 29.6 MB (29634086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b4abbf4635cc281d4995cae6e8ea73c4f2713f902bf6d5e500134413fc88da`  
		Last Modified: Wed, 15 Jan 2020 14:19:38 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dc6850cb4055c8c383de6b662f37153a7fd9372a26c59bdd06bfb84f8220e3`  
		Last Modified: Wed, 15 Jan 2020 14:19:39 GMT  
		Size: 292.9 KB (292910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc3ebb97a1ebf45a4bee75f8e674ecfd76d28ad3230d051b5b2f366b20f8b1b`  
		Last Modified: Thu, 06 Feb 2020 00:44:25 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc934b3fc17eadfc2a7beaba0ca233ed0995678927ae30b3a8017099757d8cad`  
		Last Modified: Thu, 06 Feb 2020 00:47:41 GMT  
		Size: 133.2 MB (133202193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e719e206a5ccb9f043f806137d4fc905089f14fb24ebfdeaa1b0361c182c370`  
		Last Modified: Thu, 06 Feb 2020 00:44:25 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
