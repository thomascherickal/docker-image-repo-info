## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:5016a9ee6f22300f4699ec2ba33c105b273e55c4b6931dcdbe8a7326d9dc037a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:e288b33447f0b01c2ee0954c57e574b43ce9ed4b56cbd813eca3cb1df8d9f766
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1572061864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c236dcd08d81ed31367d57c62c7e77e2421092030cd5365c6a225b0ad121c6b5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 02:57:40 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 02:57:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 02:58:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 02:58:23 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 02:58:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:16:17 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:19:43 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:19:45 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:34:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:20:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:47 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:21:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:21:22 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fc8728d9c7bf65edf893fd902f8b1bd780f93623858960c9db79e39922b169`  
		Last Modified: Thu, 12 Jan 2023 03:47:24 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7935a4c648078e79f67a11bcd5908e251110dd6c5a4ee49a607f332dd25af9`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257f8b122044547f89f00f58661b25aca97c92f3831e7aaa11975639b6e35d4`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95acaa75c1852ba1320c5db382b01f587badb615b6746b59be27eedcf96ab667`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5201ba65043fa621c187729f18aecf4c549cdfa12cd6d8cab7a901d893f3a8a8`  
		Last Modified: Thu, 12 Jan 2023 03:47:29 GMT  
		Size: 25.7 MB (25702230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a317a349bca5ab28ba7c1ce039928a56390f7e7a8d7ddec07efcc1c9883e5d`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850296b8fbb853a6eb6341f7484cd4bc622e9f679f12c4123eddf08b7f398fb`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 554.2 KB (554212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80b3d62f45a345eaac7caba0cdc514011cc61ea8f9d7d7b82d1bd4f8f3dbea4`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320dc1bc3ac081a72fbca97a699b20068d92c70b3caaec8ca53036ab37509933`  
		Last Modified: Thu, 12 Jan 2023 03:51:58 GMT  
		Size: 157.9 MB (157885976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230636fcbea662dc69129c73285f4376c0b83a3222e8d438ec859d14ee1201b8`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e22afffddeddb0a4127481e5016946bd3f35379291c6bb1e3b85e92e7acef`  
		Last Modified: Thu, 12 Jan 2023 05:37:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aaa30213dc8e6b5906114a862d8398ac157fd2f8c835767a058069f180a181`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b39a2446c556432e7503cc419fe42c4d14ff3fc744cf6d475136c5058bc18d6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ea60403f6819d31f67d7dc2d230def090cb6366c7cd272d99d8d06aac019d`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5970b711fddee53f278567276c42d2b169c5286a5133ba48ce3a599b253b37ab`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.9 MB (1871861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1270e653c78ffbadd8ab6379e16db4c45c20fb148d294ec9654f1d13367fea6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
