## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4eed6304aa3dcd2487f2458eb28c35a51333b31ee8a245989fd6a72ab7d0ada6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:4e109ae3674f6c6f89624f5f567f95f999f5b0df6caf154d5c5dfd726f87dbdd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888960382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c3d30744a48b86ec57d491e6e151bf73a6f2032aa729c64190d1aef1a4e519e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 02:34:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Apr 2022 02:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Apr 2022 02:34:13 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Apr 2022 02:34:22 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Apr 2022 02:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:37:05 GMT
ENV GOPATH=C:\go
# Wed, 13 Apr 2022 02:38:54 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 02:55:20 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:02:03 GMT
RUN $url = 'https://dl.google.com/go/go1.17.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '82752c3313cc6c1e1b5d73743a3ec569b09a14246fc2cb0824cf30f9f42a6005'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 03:02:09 GMT
WORKDIR C:\go
# Wed, 13 Apr 2022 04:41:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:41:11 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 04:41:12 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:41:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 04:42:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Apr 2022 04:42:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9b761254212cd472f566f902a9830a91c33e94d06fb02a0192e29fe447bf98`  
		Last Modified: Wed, 13 Apr 2022 03:15:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210c142bbabba5cac6b3d06dc265578eafda02e9f54b2b955129652065abba5`  
		Last Modified: Wed, 13 Apr 2022 03:15:05 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24b5fea0cadfc385f0501b3cd52647d69ba5dd030f05bc637848ed7298ed45e`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1490fa326c6ac4254cc7e87bd773641c1a74d6d68ef0ee562e1296aa6e5ba09`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5425f63a29b9eb9b5bbbf135d080f8b1d2415a665b41591175a49f41da70d`  
		Last Modified: Wed, 13 Apr 2022 03:15:23 GMT  
		Size: 25.5 MB (25453409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf5f939642f2aaa6426ec58683c461b2fc27f9b92ed53ceea3d53e5f5b8d18d`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ec6181c5a38a1257f1181b0b390b0fa168627daeb103a617f04cf11c9666`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 328.4 KB (328368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6a29e70c078bf2fc470013ea504caa6d82ef66cd3af18be02f62f0d134dff6`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a058a0e83dbc0674b085ab0d0151f94531062126dc4b1f43b0084df40fb62`  
		Last Modified: Wed, 13 Apr 2022 03:21:14 GMT  
		Size: 145.6 MB (145578329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9b48a173bb3f29a006a2592b0bd8c63b07c7323137db4862e9a98fdde16b0`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.5 KB (1520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49552906c9650efac10c4f00d5c31cebf6f940a05f00b03588df052cff5966c5`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c413ca6d8afb37ed0141a7d70605c26e6e41e5eff4bc87310dfc61a4401c2efb`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b4bcf4a2711e0b5cb2da5cb559b24909aa338f368d3707abf4c6864460db2e`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78562e4c0ea533a4cf051d0b9bc839623424c2f916a5ede43fb15f0716caa9e5`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e585753aa23f898a3a13160e144661683e6a6e158380f4c959ce67481d1d2c`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.7 MB (1661442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a64286d73ce8637abf3f1f6f9610e0336567c77c2c3595d2afc4491ebc3ca`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
