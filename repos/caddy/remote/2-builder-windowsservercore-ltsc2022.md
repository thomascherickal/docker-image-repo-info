## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:39520901129debe71fc3b671250e73c438c85ee3435b24c8c8c5bc6293f05800
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:6e35c0ddda3afe05cb015c908260022b09ae192d81ad72f3bf1e32c70d7cb243
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2659936170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265570f6cf9dffda304fb3a6712c85940e0f8d23ef6d8ffbfd8e1ebdd6d89d85`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:40:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:40:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:40:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:40:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:41:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:41:26 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:41:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:15:18 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:35 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:19:38 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:19:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:19:43 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:19:45 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:19:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:20:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:20:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8b589252b90e37349f39b9d4495646791b4050d7cd218336fcc4624b0ebe2`  
		Last Modified: Wed, 12 Oct 2022 13:15:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811ef63d5261b55ee6b499dbc7fcd1ed13386326466fb81a0801abbcbcb75d3f`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816740cd643a7a4e72aa527cd033d0c95686c9725ff70dac3260b44dce508e73`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e30c8b316e75d786cfd91f97b9fae4c89fb00f3fce0619eb4e66bc3165521`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a0d37b81c920d4b783c0b2cfad656a4b8733960ba3afd4e0a1f39f202f948`  
		Last Modified: Wed, 12 Oct 2022 13:15:32 GMT  
		Size: 25.7 MB (25689345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b699f53b56e90279b0bb8ce4434f9b68bbc28fa30756476e22c7ef3dc869e24a`  
		Last Modified: Wed, 12 Oct 2022 13:15:21 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fcf632f60c89dd981a8a7fa084e738f55129b1786fd9a9e9f5ab8aa1e02d82`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 526.5 KB (526519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8b0d888223c93af8f0c84ad35156f79df9b0d9ae107f61ded320d2a4fed5f3`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49602de12fff655f45d03b1befdd7e56321771c65ed690492e4092da51046bb3`  
		Last Modified: Tue, 01 Nov 2022 19:54:22 GMT  
		Size: 157.8 MB (157838831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cb5ede4eaf1f86f7c0957639a8b53a0c6740df6fa395d3d286e32bff6b9195`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d0ae347408d32205a9ca4c0628e814833984ac8c0fbfb6c6687b9c94a733aa`  
		Last Modified: Tue, 01 Nov 2022 20:21:30 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453489637085324b6412fd9d83cc639d7a9f9135fb5db5dec214462b3293c98f`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc23fcabe43926f14c7d7e786e9175c87fe573e41fc0158bdc02cfc08fb567`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528f2dc5e38ba5bad570845252c13446ea9637f9c7a80590c93c28886ab79803`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd45b40a0e40f3a52f9a7e2e1cf3cf3b0501ca3f8d637ef46596ee30a9193264`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.8 MB (1837122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bd243dcf25ec803b906e53fa263b2803735773f0227c1c4bac5d52654bb8c6`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
