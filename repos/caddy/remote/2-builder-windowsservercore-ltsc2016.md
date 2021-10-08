## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:46edeeace8b9d8e0bed359c57f142876d74ea522aa1acbc23023964b70acab3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull caddy@sha256:e3cfac77d5fe1f76994a5f930bb3ce11940d7032346869ed40cb230c44eb58ad
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6448641763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e5218423cd8149f78d2841ce2267af636080c80e168dee2e9821e67bc5c33c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 00:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 12:29:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Sep 2021 12:29:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Sep 2021 12:29:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Sep 2021 12:29:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Sep 2021 12:31:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Sep 2021 12:31:16 GMT
ENV GOPATH=C:\go
# Wed, 15 Sep 2021 12:32:09 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 08 Oct 2021 00:21:48 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:26:18 GMT
RUN $url = 'https://dl.google.com/go/go1.17.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'fa6da0b829a66f5fab7e4e312fd6aa1b2d8f045c7ecee83b3d00f6fe5306759a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 08 Oct 2021 00:26:19 GMT
WORKDIR C:\go
# Fri, 08 Oct 2021 01:21:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 08 Oct 2021 01:21:22 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 08 Oct 2021 01:21:23 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 08 Oct 2021 01:21:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 08 Oct 2021 01:22:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 08 Oct 2021 01:22:42 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8721f004192f15fe71b8626ef3f3e34cbf2cfe1d15a63b6b544ab946162ef707`  
		Last Modified: Wed, 15 Sep 2021 01:10:18 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e53aadfbef1cc4f3dbc45317950f6ac7ebf3d2d5435f6cc133345e51b828076`  
		Last Modified: Wed, 15 Sep 2021 13:01:37 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e09fffa3b92b1b886f3bd396a99ace1c271c24920991b1eb2987bcb7bd40860`  
		Last Modified: Wed, 15 Sep 2021 13:01:33 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23d3fe9f3645327794552def0d1521a54d23445b47c8555f451c10db4fc4943`  
		Last Modified: Wed, 15 Sep 2021 13:01:33 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd5fa25aee2496a96cd80f8dbfc27e159ac29d556d3c61edcea89e99d76fa15`  
		Last Modified: Wed, 15 Sep 2021 13:01:32 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84755a39549908bfc5593b7261f1b6b6d5eba19073dcb9b135c6ab84eae0465`  
		Last Modified: Wed, 15 Sep 2021 13:01:38 GMT  
		Size: 25.4 MB (25426437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929d40ec6a00859e598e8aa73c5700faa7f06f8e0dc864a6a2da2a69f285e7c`  
		Last Modified: Wed, 15 Sep 2021 13:01:29 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4568833aa387ec42e08d96e32b67d3b0e6b0c3c75bc66a64591f2d1fbd5f244d`  
		Last Modified: Wed, 15 Sep 2021 13:01:29 GMT  
		Size: 340.1 KB (340085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d88ee737115c8f5b3ffbbeca0002ccb66bd92b6b60cf3aedb329507e38e153`  
		Last Modified: Fri, 08 Oct 2021 00:53:51 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989dc95d42425703f29871170bc98f2c6bf9c2453d89cd1d04f7e77638ef7b9a`  
		Last Modified: Fri, 08 Oct 2021 00:54:31 GMT  
		Size: 149.9 MB (149890673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed86fc5d2d8f762f1eece8066ebe8d19379c3255031db2baa40bdf17ee10eb9e`  
		Last Modified: Fri, 08 Oct 2021 00:53:51 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b373c4f49819b29c210817d94edb86905f7bedefb7de3d9092d26305b7eac256`  
		Last Modified: Fri, 08 Oct 2021 01:23:33 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457b57636ce1922275e7975eb0d68d84224e04c323f43e419c9a4c9b7528a8b1`  
		Last Modified: Fri, 08 Oct 2021 01:23:31 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5483f56cc3f19b67dfcb6a857340bfef083e5a9dffc2543a1f0ff7ae8c36264`  
		Last Modified: Fri, 08 Oct 2021 01:23:31 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb65aaa0b29133039f995b8c95d6a35becd4a7552cb4d44a754e291259600ee`  
		Last Modified: Fri, 08 Oct 2021 01:23:31 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a34422379d4d67e1781470c86d47e7bcb5e1b3b36504ca66882a36fa337f0d5`  
		Last Modified: Fri, 08 Oct 2021 01:23:31 GMT  
		Size: 1.6 MB (1638974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714e23e4dd6c7aaef30b61f361019cef0370a0a960319cfaab9d5f127da1152`  
		Last Modified: Fri, 08 Oct 2021 01:23:31 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
