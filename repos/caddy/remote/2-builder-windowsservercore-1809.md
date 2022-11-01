## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ee5b9081fd81e7adbf4a0c1bf8fd4f9f882e755ac9fc03b24f12c7699aa5b52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:f279c274451500e517aada07ecabddffd03b23f0b9d81791d2347e369b267a6f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2958579667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c57c677f08a022815e25e725365624f628555a00eab2b42f1830e71794c949`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:45:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:45:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:45:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:45:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:46:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:46:38 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:47:37 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:19:52 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:25:48 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:25:50 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:18:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:18:12 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:18:13 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:19:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:19:34 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a4c27e78f8821517fd551cd9e3d5f4b1e4199bdcd783b3fbda849e4995ad1`  
		Last Modified: Wed, 12 Oct 2022 13:16:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e91de5ff2103556b1048388473379f95d41247701f0911ebc7c530a861f3f5e`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52642f9e5e3a52bef8ee5677bcb62a364e07003da51f16eb28b8a4ce34fe9f7d`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26528ba698d400f5680be93457d24581b9e4e7a2399de7bb23cbd549f206613`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c89703eb31300a2a39c85ce287a6b9fe88da033828368275bdbb53c2f7704c`  
		Last Modified: Wed, 12 Oct 2022 13:16:30 GMT  
		Size: 25.4 MB (25439927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8705eaae12fa4840be2d79e376eb1b4b7b18da881acad2892b1c47336e796f46`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebda8897c2727e3b971c947385632df6f19de06da75e9f161200d43d1acf714`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 315.0 KB (315035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8667d37dce62bb077cd534d490f047b61dfe9c30023659258862cada9cbd0ba`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac8e32e89f1739964a644b8b8b5b44bbae9752f8ea1f87e93455ca36cc86a7d`  
		Last Modified: Tue, 01 Nov 2022 19:55:33 GMT  
		Size: 157.7 MB (157676844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cabbd4ff51bc72ab20efd9f4eb4ebb788679ef03c2fc9b8a72f711fe3558590`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.5 KB (1459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a7aa6766a51e2f5a5add77b40fd7eafa9d3d5049c3b4506b6b4e6dffb65cd6`  
		Last Modified: Tue, 01 Nov 2022 20:21:08 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54feb136a1e02e5d213be9750ca621c39022ff48f54c1e67daace9a82dd241f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7c0ce28f0f06a413d72723dbca806a7b025194983d436501cb04b7b2d7379`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e48594ab78eca9cfe42619a2f721de764c027be8fa22700565227c765b4ed7e`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55feb68cd00871cb13079eb862d65521274326d062594c7522edcc8f9bac23f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.6 MB (1631634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398f623f33e057b5d399473e3ee1243fef32140e9a4411c1f69a913b43acb08`  
		Last Modified: Tue, 01 Nov 2022 20:21:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
