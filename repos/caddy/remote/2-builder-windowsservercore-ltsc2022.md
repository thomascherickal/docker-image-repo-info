## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:52c38c8373f27a366c68033cbcf38908183bcbfb1d15c77f0a6184de5297ca81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull caddy@sha256:87c2a0e1e436b5923868300dbaff15ff3fcaf238585c26dfc3ddae194dd3e091
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1873786914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c148ed76f4ea520961157a29cf0a754ffe1c3dc3429a81c99129988b92f4e2c4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 13 Jul 2023 20:29:19 GMT
ENV GIT_VERSION=2.23.0
# Thu, 13 Jul 2023 20:29:20 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 13 Jul 2023 20:29:21 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 13 Jul 2023 20:29:21 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 13 Jul 2023 20:30:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 13 Jul 2023 20:30:03 GMT
ENV GOPATH=C:\go
# Thu, 13 Jul 2023 20:30:22 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Aug 2023 21:35:14 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 01 Aug 2023 21:37:37 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Aug 2023 21:37:39 GMT
WORKDIR C:\go
# Tue, 01 Aug 2023 22:23:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Aug 2023 22:23:56 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 01 Aug 2023 22:23:56 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 01 Aug 2023 22:23:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Aug 2023 22:24:20 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Aug 2023 22:24:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ab322251f8c00d29baecc140e08d269c37b32475902e7a2822076226f616fa`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a968ab3b5ad50a23776f7dd7e039322644cac504ae091a0b0cd2e1b88fbb7e69`  
		Last Modified: Thu, 13 Jul 2023 21:07:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ba07cbbe0cde4ed464b5564160e204ded4877d3a1e5cf5fa3e155d5c0c3500`  
		Last Modified: Thu, 13 Jul 2023 21:07:34 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22efbf516ade60254b7399cfd7c01ac615e7d0c3745272b9636c39ba1b16c6e9`  
		Last Modified: Thu, 13 Jul 2023 21:07:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195ef065fa8b0419c3b6dc860031273f7cb1e3adab37c0a55458d916644f7f32`  
		Last Modified: Thu, 13 Jul 2023 21:07:40 GMT  
		Size: 25.5 MB (25535727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792bc8f98993f23c77f2a5ab339752f8bed1c5769eff7a72bd01f84cae18d978`  
		Last Modified: Thu, 13 Jul 2023 21:07:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ee2ce3d2ac713b0419f7347636dffe3f3d8639e4f3476fc6cf2f233ed3392b`  
		Last Modified: Thu, 13 Jul 2023 21:07:32 GMT  
		Size: 263.2 KB (263191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326ef3ff4b4f0b55d50275b360cf494cf23752c258adb2116098f5e5a3199fa5`  
		Last Modified: Tue, 01 Aug 2023 22:00:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b097dfbd4dafff76dab0b850bb2b043b71c920e96c26552d47f479821c9617`  
		Last Modified: Tue, 01 Aug 2023 22:00:48 GMT  
		Size: 108.9 MB (108930621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13679ff7ad3316b11d9df991a057252d1ac7662138189bc9c290725e4eef2066`  
		Last Modified: Tue, 01 Aug 2023 22:00:25 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b59d6e268c1969e97464b079d6a48a68a9c847224617e027ae77bb6348e9673`  
		Last Modified: Tue, 01 Aug 2023 22:27:24 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a16b5dbf63e48eeaf90e250d730c598c6d2599f4f07d6b17f0be5b7fbe3b01`  
		Last Modified: Tue, 01 Aug 2023 22:27:22 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145f07830bda851ba97c81f04bc775e9b211348968b542f358329f1c4ec091ee`  
		Last Modified: Tue, 01 Aug 2023 22:27:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f77e84a5fa1eb345ea688b6a087df7739622ab35627ea13e8fb5eb3c8afad5b`  
		Last Modified: Tue, 01 Aug 2023 22:27:22 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3a54610a48ab0ca6469abdeb79462f9b5ac292bdec8e5468fd140a0ea7b028`  
		Last Modified: Tue, 01 Aug 2023 22:27:23 GMT  
		Size: 1.7 MB (1674036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946a17eec28aeb0e9cd83868d49e966ff0881b0121ca3ddce4ef21d505b5dbcd`  
		Last Modified: Tue, 01 Aug 2023 22:27:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
