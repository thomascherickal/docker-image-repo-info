## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:e1bb18b4d6b5d29285df06dd3c1c50f88b9111dc27dc22332e1654f3ee3f5a06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull caddy@sha256:4a4f13fed09ca59ae5bb51476f9d1d0f1870c8550a4ab2e83a3a7d00fa142207
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1986153824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69ba82bc29d29a4c163b7e9fab68ec1308e1f0c7df9b1e096c7fc832b37cb58e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Tue, 12 Dec 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Dec 2023 23:35:08 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Dec 2023 23:35:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Dec 2023 23:35:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Dec 2023 23:35:10 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Dec 2023 23:35:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Dec 2023 23:35:47 GMT
ENV GOPATH=C:\go
# Tue, 12 Dec 2023 23:36:11 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Dec 2023 23:36:12 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 12 Dec 2023 23:38:40 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Dec 2023 23:38:41 GMT
WORKDIR C:\go
# Wed, 13 Dec 2023 02:37:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 02:37:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 13 Dec 2023 02:37:40 GMT
ENV CADDY_VERSION=v2.7.6
# Wed, 13 Dec 2023 02:37:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Dec 2023 02:38:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Dec 2023 02:38:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839fc47f6e056f9e09a214230f8b7115e69419dbc74acbbb1ad6bc0caa28862`  
		Last Modified: Tue, 12 Dec 2023 18:27:40 GMT  
		Size: 500.7 MB (500674814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c853ded9068434b9128a8016b3ae5e18f748f62801c7bb6e6092495300ec`  
		Last Modified: Wed, 13 Dec 2023 00:02:39 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf365c1e9d59a58fc8cee2522db9139b36cf02ecabe7302489a9a3667b62cea`  
		Last Modified: Wed, 13 Dec 2023 00:02:39 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dbeb610a3fa1c3f2962202c58796ff120ea20cc3ba1f2fce807cbbe2c37ab0`  
		Last Modified: Wed, 13 Dec 2023 00:02:37 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a3be8233329999132fa6e504f39c44abd589439a96846e31508037334d6d11`  
		Last Modified: Wed, 13 Dec 2023 00:02:37 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755721e8166183821011ca0acdb563f67887cfe33da36997710b182f049fbede`  
		Last Modified: Wed, 13 Dec 2023 00:02:37 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4700bd9f606505ec47d78dc66a509ca78ea2a8269a8e2b9bcf28ec33c5cbea74`  
		Last Modified: Wed, 13 Dec 2023 00:02:42 GMT  
		Size: 25.6 MB (25554973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777ab971ccee32e15de39ed82eceeb004d2d6f94af7c43ab3d6cfc1baf0abd07`  
		Last Modified: Wed, 13 Dec 2023 00:02:35 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958aa1458398ceb3a543d13279579cc48507080df3b269a5aa1a09da23b03ccf`  
		Last Modified: Wed, 13 Dec 2023 00:02:35 GMT  
		Size: 284.9 KB (284874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d369624561ac7e7cf731915f0964d62247949c50220ff13950623666d0be6677`  
		Last Modified: Wed, 13 Dec 2023 00:02:35 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a66f9cbfd2a34db803ce305db5e79aa13dbce84f3838ca16f551a83d7fa185`  
		Last Modified: Wed, 13 Dec 2023 00:02:57 GMT  
		Size: 69.3 MB (69342174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae25eae66695fd6c6163f7e78ecbd910adadaf2eb87b05f72e3aa6664d84d7a`  
		Last Modified: Wed, 13 Dec 2023 00:02:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bd9118d155d6237fe7e13dcf972ca8ea851c1a6b934808abae5e778401617d`  
		Last Modified: Wed, 13 Dec 2023 02:40:01 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a9a79eca2baf93cbb843f18acfce147dedef9278d4d1d78e35dbed565079cd`  
		Last Modified: Wed, 13 Dec 2023 02:39:59 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbc995d63f9c3efaeacfa8a0aa3fbc01dcc1c7d908188a1340d9615f57cf6a1`  
		Last Modified: Wed, 13 Dec 2023 02:39:59 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430a65e29392c4ac3c61c78279e4b342ebaf564950d5cf115782ca50d19d7b6`  
		Last Modified: Wed, 13 Dec 2023 02:39:59 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ce89df60f421a97ea4d0686cbe6f5a454701a58808b6e599604a5cec3a60d`  
		Last Modified: Wed, 13 Dec 2023 02:39:59 GMT  
		Size: 1.7 MB (1680362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa4fa3e2b0a9ba64583a0471d71a10e380ac2a137ef795d6e031cac1bc03391`  
		Last Modified: Wed, 13 Dec 2023 02:39:59 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
