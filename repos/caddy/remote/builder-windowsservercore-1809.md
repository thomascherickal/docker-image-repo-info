## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4860fe163f2de790e463ce7028ef13969dbeecb0f45308f3d12328e85f987def
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull caddy@sha256:b61326682d1d6676e9624dba0b04a073246d32f8a77a61cb9e9d2c9e8519a6a3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2886655071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea8778f89343219e1d75244f6734d26e3164bd65c85c9b72d2f71e46aa54441`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 13:09:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Feb 2022 13:42:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Feb 2022 13:42:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Feb 2022 13:42:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Feb 2022 13:42:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Feb 2022 13:43:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Feb 2022 13:43:41 GMT
ENV GOPATH=C:\go
# Wed, 09 Feb 2022 13:44:39 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 11 Feb 2022 01:19:17 GMT
ENV GOLANG_VERSION=1.17.7
# Fri, 11 Feb 2022 01:23:16 GMT
RUN $url = 'https://dl.google.com/go/go1.17.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1b648165d62a2f5399f3c42c7e59de9f4aa457212c4ea763e1b650546fac72e2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 11 Feb 2022 01:23:18 GMT
WORKDIR C:\go
# Fri, 11 Feb 2022 02:18:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 11 Feb 2022 02:18:20 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 11 Feb 2022 02:18:21 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 11 Feb 2022 02:18:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Feb 2022 02:19:17 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 11 Feb 2022 02:19:18 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f0c1566a9285d9465334dc923e9d6fd93a51b3ef6cb8497efcacbcf64e3b93fc`  
		Last Modified: Wed, 09 Feb 2022 13:26:13 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b56caecef9c44ed58d2621ffb6f87f797b532c81f1271d9c339222462523eb2`  
		Last Modified: Wed, 09 Feb 2022 14:31:28 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3ed0a076d58c949f5debdbc3616b6ccd008426c62635ab387836344123e2a6`  
		Last Modified: Wed, 09 Feb 2022 14:31:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25f9584c1aa90dae36704d6bef0e59e72002fcb13e8a4618f64c9b13479c0df`  
		Last Modified: Wed, 09 Feb 2022 14:31:26 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4fbc7cf0f85fc63860f052f76bfb4429eca8b878abce79a25bfdc30f9e9f5`  
		Last Modified: Wed, 09 Feb 2022 14:31:26 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c325dc9f1660ea537aae55b89be63d336762d5a3a02e929d52940586fb0f677e`  
		Last Modified: Wed, 09 Feb 2022 14:31:31 GMT  
		Size: 25.4 MB (25448246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f3aabaa2a9bf80e2a7f417dba559f6b34e640c21b138dce099328406c8903`  
		Last Modified: Wed, 09 Feb 2022 14:31:23 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e61367d26baed9e16a8d5310c520ae3429d5cc7956569f325cd9de01f33604`  
		Last Modified: Wed, 09 Feb 2022 14:31:24 GMT  
		Size: 317.3 KB (317319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eb9abc560e8d857685b3b0131c733bdbb5f3c79e93fe7e9163e443736c2f51`  
		Last Modified: Fri, 11 Feb 2022 01:47:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffb0b96d90540c5fe04bec7c3803e767fc06c03da00c569b92ec1abeb2db503`  
		Last Modified: Fri, 11 Feb 2022 01:47:34 GMT  
		Size: 145.5 MB (145485006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c16363a908ee64151cd232d466b723e3edac978f1c7693db3dcbed09694d76`  
		Last Modified: Fri, 11 Feb 2022 01:47:01 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edee74e5c93cc1579fcf04a44c9ebc4410d86ac14b5f6e606d4f8bd660a1399`  
		Last Modified: Fri, 11 Feb 2022 02:20:06 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eee5ead478b943535e2bbe67a756df790b5a29564ad2f1162d3529495421da4`  
		Last Modified: Fri, 11 Feb 2022 02:20:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85326812722a5684f628d60dc9b8588818d6e5a7742467f5bd3254d1b71f6551`  
		Last Modified: Fri, 11 Feb 2022 02:20:04 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b834a18e319d23bb598514ecd566bcb781b0e2399e7e44bc020337937fcd8e90`  
		Last Modified: Fri, 11 Feb 2022 02:20:04 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e81b5d61dec4ab5538b351b1573b88407a2462f2bff4a15dc964854ec824d37`  
		Last Modified: Fri, 11 Feb 2022 02:20:04 GMT  
		Size: 1.7 MB (1671502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32ab8f24a99ab88153713bf4dbb41115793864929887641d1933f06c15c4ac5`  
		Last Modified: Fri, 11 Feb 2022 02:20:03 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
