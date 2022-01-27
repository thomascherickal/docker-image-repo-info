## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:89b3dac80f3f9c2cfa6a51201d66a6ce07cc824ab9c160cc9529794802ddcd61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:72af0e06b32a67c1a6bfa9204d4f2c702aed93b21813fae661fdfffdf554b680
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2886236941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f985de62284201d13a9b844cf326330406053348fdd15ae97730c4daa3b6b3ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 15:09:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 26 Jan 2022 15:09:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 26 Jan 2022 15:09:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 26 Jan 2022 15:09:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 26 Jan 2022 15:11:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:11:29 GMT
ENV GOPATH=C:\go
# Wed, 26 Jan 2022 15:12:29 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 26 Jan 2022 15:29:08 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 26 Jan 2022 15:33:30 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:33:32 GMT
WORKDIR C:\go
# Wed, 26 Jan 2022 21:02:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:02:42 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 26 Jan 2022 21:02:43 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:02:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 26 Jan 2022 21:03:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 26 Jan 2022 21:03:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e066feb335981c422e18ec3e99d79f1c5be6b43ca35ab0430187cde79a8ba19`  
		Last Modified: Wed, 26 Jan 2022 16:03:50 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98ce4c8c854279fe1e91c71aa96b5228b24e217162fdc7508fa1ffed2d93f3e`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff64477d4a2364cc1faf09a8f6ca0359be8089d74617888efc97fc1ec2ec925`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730c3ddd3a11e217b2bc0dd3198cefbc720787b51b86f921a046fb40be043a7`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f86077710bb19cc328ec7f872e5557f814c2d3be829a2c1975471547f3adc7`  
		Last Modified: Wed, 26 Jan 2022 16:04:30 GMT  
		Size: 25.5 MB (25472102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01031350b313b8d7dc8b649f435561b95b072ded45bcb1e12d170b2d802406c1`  
		Last Modified: Wed, 26 Jan 2022 16:03:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8558cedae20f4e01a76f91a8787b6ffec7812eb6b0013980e19c208f3e7b0cf`  
		Last Modified: Wed, 26 Jan 2022 16:03:45 GMT  
		Size: 335.0 KB (335017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7f568a047da2280936ebaab2fd0479b3a6a5e9afa603fa8eba6f3fa1cc96d2`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db36d4d0813c6743a4407bdba7a0be0025b10f8cbedde63043409911b556d56`  
		Last Modified: Wed, 26 Jan 2022 16:16:20 GMT  
		Size: 145.4 MB (145423291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f910516d12aa2decb0589c60b2bc4f4400ff2edac20fd2377ab1ed892a5b6c65`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbdb95dd3db1da9bfe68bf24ccb98e47681fc4cfa8ab474ce4efc25aff2ab07`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a65566fe525e381f5639a47cd2c97196e907894f6c10762ff3cae32fa1cdd3b`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863595908562193e85b1287222d90951da4cf1f7a075b4820e9da7b8d1b9a4da`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00292f0ba4bd525f47671337689f4d11e1ee966d077007a37eaae7fc0eda5bb`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003cfef2605574ce4be63540f97caab8b329406d8c890067541e16081d8c4f6`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.7 MB (1667078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21146e014bbacf566bd713a4d1a891e05e7f8da85f2cae49232335f811cb7f8`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
