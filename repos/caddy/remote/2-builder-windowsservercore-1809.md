## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:907bcf6ffbd9c87d579d9fd0c863633d3d5d3a4f7bbbe941849c977bcb479c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c9032910fbe59986e17e53ecbfd5ea3e2881f9620a93059d210565e8b59a25ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2198807920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb35fb2c0019120cb2f52989b07f2edcb7025e0f2c94730d2072d883a96d0e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:05:31 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:05:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:05:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:05:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:08:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:08:45 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:11:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:30:04 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:35:29 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:42:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:42:32 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:42:32 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:42:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:43:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:43:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cd8204a3a0f91264f1d80a1823c6302144beba7b949672383f79a4b0eaaaaa`  
		Last Modified: Thu, 16 Mar 2023 02:46:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9b5c8cc42aa4e27c584910b32e3dd61b08d3737c3a4bd57c718c6bdf4e918c`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d294e5fa55a2c856286550cda7d5754988031614630a73de68e7a91bb9780b1d`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae3806c822a2819e77add7db0ffb98fbf5a4db7f6b546da7836b3c5e280921`  
		Last Modified: Thu, 16 Mar 2023 02:46:18 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8496692041c620f4a5d6248542d1fbbe277a127d0c8f999f8ee24e4dd245495c`  
		Last Modified: Thu, 16 Mar 2023 02:46:27 GMT  
		Size: 25.6 MB (25579220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a76c28450756e3ff6ea6233e7b9cf00fb53673383e2b7ca14eebe7e99e29d8`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ce11a3cbfe6ecdd0116b5beb678a12cfc66ead578bf96aef94c527e0eb3ed`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 323.2 KB (323191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007aa50ce0d4dfd36bfd2d18608fce2ef6a37354603df606438b96a07124bc0f`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f5c1dcb53aa73aada7ad9d4b1bb9dc43535afd2526802db572757a4f3b1525`  
		Last Modified: Thu, 16 Mar 2023 02:50:48 GMT  
		Size: 157.8 MB (157764104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1316d76362a1808f7b882074ea5cbed1cce2892caa37cb311f38a73fdea9dcda`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c91cd00a563121fa30dbc382f5027a18ebf90cc2754e79980f37c8685c7030`  
		Last Modified: Thu, 16 Mar 2023 04:46:26 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e9290bf0d4bfd4af381743a93f904c36159f0bb345e98226221093c2adb10c`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202bbf38db2cbd0d97b70aab758abe41b4bdf86de6bbf6920ef866d23309fcb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02200a8e9b0587ea6d794a97d1478b24edc0552d50eb20ae08021c5946e976f3`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8895a312263f89855cc0e57b315b57ccef5c314eb6637732ffe3beb42297cd2`  
		Last Modified: Thu, 16 Mar 2023 04:46:25 GMT  
		Size: 1.6 MB (1614512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fcd18dab8ce707123ce4789697f284017a7694305fed4996c6cdcff9019cba`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
