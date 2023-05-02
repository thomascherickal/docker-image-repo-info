## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:868cd5f9e043c258a54e53976f26cc52ca12bfb46872bed07a6e1bf54615a83a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:95b0abac9a901a46cf4efc5f05cac202b732eca2531d527b148039cc7dfd7584
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2256629977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69d8bfe5f5975fac3c2bbdab8a34e5f77de58727f526b86bd4a9bd26eefc815f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:54:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:54:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:54:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:54:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:56:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:56:40 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:57:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 02 May 2023 18:50:57 GMT
ENV GOLANG_VERSION=1.19.9
# Tue, 02 May 2023 18:54:17 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 02 May 2023 18:54:19 GMT
WORKDIR C:\go
# Tue, 02 May 2023 19:21:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 02 May 2023 19:21:36 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 02 May 2023 19:21:37 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 02 May 2023 19:21:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 02 May 2023 19:22:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 02 May 2023 19:22:52 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a6de00b28bac0666d00c5a680ca62116074e664878553846026da5c3116e14`  
		Last Modified: Wed, 12 Apr 2023 02:32:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefb03e237e07e11ef0bcedf393cddb3fea112dbf95771c2a8fd09138f5fa331`  
		Last Modified: Wed, 12 Apr 2023 02:32:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ef0a611281437670a551a9d388018ca6583c5f934b5f26514f7cdd8d1a8771`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e751ae5812845616a66f9446726d4aba077b086487190ab0cf05ddd245b9c8`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d802cb7e5f3a9b618e9765e831db7ae04a9097f456a4cf70b15706bbb289a5`  
		Last Modified: Wed, 12 Apr 2023 02:32:55 GMT  
		Size: 25.6 MB (25604110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30278f60b48b729152d141e9b3a5e94c8ed1d95059849d727e1dafd7331f1bbc`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0812ea54b5317c55bbbec51b566520e84db2b58e2b8d86f92fd75ab23d0694`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 332.4 KB (332356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbd158a37945a999be084049f01bf6028d17280d3344a7387fbcb7283c4e65f`  
		Last Modified: Tue, 02 May 2023 19:03:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5eb0bb6cfc6cebc9c358ea44562744158c8c3cd6563982bea5ac9e1ad4c95c9`  
		Last Modified: Tue, 02 May 2023 19:03:55 GMT  
		Size: 157.8 MB (157756250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3b8947fdb09228b2574ae5a5b7f07089576fedfa428977aae9a9b7813d0669`  
		Last Modified: Tue, 02 May 2023 19:03:18 GMT  
		Size: 1.6 KB (1573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14feeb31d1d50b1b26475950472a67a004b81eceb4a18b01c880029cdba01faf`  
		Last Modified: Tue, 02 May 2023 19:24:10 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492e31e1dad0cbd86a0a59c34296777ab141af8e770059ed39b86119a73d9d1b`  
		Last Modified: Tue, 02 May 2023 19:24:08 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f13c5b134c4f98d3d23d35578505a8f52574c59027c01df0aab2a8e3fd5c8a6`  
		Last Modified: Tue, 02 May 2023 19:24:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade778d704f5521a21ad2137fa452f8cc58fa0a98e5f794c754791b8c34544f2`  
		Last Modified: Tue, 02 May 2023 19:24:07 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a6edb62e0d355d31426fc0c144c7ee9fd31be0ee95300057b7546e87759ade`  
		Last Modified: Tue, 02 May 2023 19:24:08 GMT  
		Size: 1.6 MB (1627466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f816444f7a8fee8708cae5a6db25873fa5d460cc818028826b72afc02d36d32`  
		Last Modified: Tue, 02 May 2023 19:24:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
