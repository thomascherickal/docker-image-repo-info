## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8e5bb4c8c32d947b3fa0e530ecb103d4dc813be81cf27e924be9b5171dd1a8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:256d98ebfd54e7da9c594d3a17888987e08a54f31e1a902fdba6062d6475e357
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983592262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932ff705341933569835dda3a9df0a381c9efadb23aedbc990ae4c3fe927da37`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:43:34 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:43:35 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:43:36 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:43:37 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:44:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:44:11 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:44:30 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Nov 2023 02:44:31 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:46:51 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:46:53 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:36:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:36:15 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:36:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:36:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:43 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:44 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b1d4a557f047b695f94452d9707061981d7fae4239c674b332282b8291963c`  
		Last Modified: Thu, 16 Nov 2023 03:11:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45549c207f14d769cba7c36b66157ec213bbc32ce57d685d8e2c407cf3987bb`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c674717e06bf8cb25d5887393ef9568ee0ab6390966b9666808e836e9bd471d`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2227badcd9f5f2b70b3d2ffd1c18887498f413c07802bfb334e8dc7b2d2acc`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9f3b5e90a2e6028cf194e870b24a7158f875f18b81f4f9137a5db3ea1f79ac`  
		Last Modified: Thu, 16 Nov 2023 03:11:23 GMT  
		Size: 25.5 MB (25536225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7811a5416dcd19193a5b3ab9327607bf845f7ff77f95d3e20abdfb7435c32ae0`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5931209e960a94616639ea72e4d3ad9dc9cb554790ce930152c73bdc1449c034`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 266.6 KB (266600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e99ca1444cc508d00e7f114e5d0ad9c56d99298bd9767a001ab05a1735cacb4`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753e4af07bf1638babc6e18c4a455b8703dfec478e0794970b2e57d76792a281`  
		Last Modified: Thu, 16 Nov 2023 03:11:38 GMT  
		Size: 69.3 MB (69321984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ace7dc382558d5cfabba6fa5df0abb49108d5b6e7ef243a4b4ccfa7639d022`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dee0b52088af84428a19e50ee688425ccee03091d9de2d42ab608d6f4988b90`  
		Last Modified: Thu, 16 Nov 2023 05:38:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae08626268dc4e22e38977aa0284b4f4e8aa2a88d8dbf3cfe61c9ffc10292d3`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12154a346b5aa10235e1da2e2c14f346f6de03387fabad1e8b0df50ce81588e5`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33ca4e95a635026944c3bc5da0516b66036a17f0f1a41f8bc2cccfd4afd1015`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2fb80d01142c2f56374c7be06d04ac0ddebd778ee3e052d6e627969b6af7`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.7 MB (1667548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41cc79b0b9e584ff384ef15b6bd7d7f1f12e5e73e9105b3e89537f183c38d8d`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
