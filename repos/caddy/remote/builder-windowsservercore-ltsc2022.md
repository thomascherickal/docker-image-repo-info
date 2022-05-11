## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:f5f71b248dea482aed03fe1e9ffdbd84e3e337044b6e4263956c9e8069ff8da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull caddy@sha256:5577ab08abcc0385dd65f73089851d37eb4cd88a29a3cd1d511c6c526221fc42
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2415395050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e125146193f9e2329bf6ce618db8d09adc336b804bec5cd23b54463959d504`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:16:59 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:17:00 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:17:01 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:17:02 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:17:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:17:52 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:18:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:18:25 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:21:20 GMT
RUN $url = 'https://dl.google.com/go/go1.18.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '41fc44109c39a98e0c3672989ac5ad205cbb5768067e099dc4fb2b75cba922cf'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:21:26 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:34:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:34:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:34:19 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:34:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb2ee3c21cb72c263da0dc4c6080f1d34c7ce3c7f24dcce76815784ec99440f`  
		Last Modified: Tue, 10 May 2022 22:52:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db422a46fd25683fe2e5990dc5db827b96c7b135679867ac162c2a318803463`  
		Last Modified: Tue, 10 May 2022 22:52:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4110a58975fa9bc64fa3a7d64804d47aa9ba813231538466dfedf4c35658cae7`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e110f1696433dc412066aa30ea4222e641d7d377d593568f539b471b865a664`  
		Last Modified: Tue, 10 May 2022 22:52:55 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aca2a7cb069b5fd7ea06af17cd99249cae08f77d945258e72108af23fb4570a`  
		Last Modified: Tue, 10 May 2022 22:53:21 GMT  
		Size: 25.7 MB (25692112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc78480e80903590627dacfc79a3c978709b8c787cc193391852c4f8bf2ffca`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f488db75670938176d831a4bc8ddd4bb629e7a61e9ce5101882db134c0d162`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 541.2 KB (541163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7e0fbd217082bd92c424bbe5de58f546b38e43068d1f7b3a1121e42ffcbac6`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d268be7c91150b1073b85f55a434b87a1602a325ad6af8f2c2896f34f83388`  
		Last Modified: Tue, 10 May 2022 22:55:29 GMT  
		Size: 149.7 MB (149697865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3786f32f80e906fe1e08346c7294bfcfaa5d640b7c8cd920c91fb3b33f8bb6e4`  
		Last Modified: Tue, 10 May 2022 22:52:53 GMT  
		Size: 1.5 KB (1536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd4f585b833fb8fb9f417326d46999e8726e1aa94e3796e9005a10daf16e12d`  
		Last Modified: Tue, 10 May 2022 23:36:48 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707272d91e9f672f1fe7a0de3ecaeefc72c1d00ee1025438e7cfb0dc74a77ee2`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90464121b8d7fd8edb1f37124b634fe69680d1b4af3a6b853417ab05e9243a0`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20695dc76bb11cb698c1e429bbcb5e3011dfd00666a09a81c2cbd4f4607b1da`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884b6dd02ff92d7127e63601c97c036dee9230f73ecfe1d2d382466b705e9836`  
		Last Modified: Tue, 10 May 2022 23:36:46 GMT  
		Size: 1.9 MB (1910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f0345f50b887c52e7c023a68e29e1332dac19143806fc334ea4d6e9a2cb0d5`  
		Last Modified: Tue, 10 May 2022 23:36:45 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
