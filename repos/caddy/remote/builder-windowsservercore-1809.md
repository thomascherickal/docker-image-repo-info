## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:80ca8f74f642d7218cc111d5ea59115a305c4cd6030325cb4c4a7fad93d4c5a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull caddy@sha256:9ccfa9fc4fc4236cf295417a18c7d16b0a79495b916cd1b95c231e18daed3423
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674256754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e7531282f56b1596b6475bd16a7058aaa9dc1e6884e7902f556e23b3eccf951`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 22:21:43 GMT
ENV GIT_VERSION=2.23.0
# Tue, 10 May 2022 22:21:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 10 May 2022 22:21:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 10 May 2022 22:21:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 10 May 2022 22:23:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:23:36 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:24:28 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 10 May 2022 22:40:47 GMT
ENV GOLANG_VERSION=1.17.10
# Tue, 10 May 2022 22:44:40 GMT
RUN $url = 'https://dl.google.com/go/go1.17.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba9198a29fa5c4f322212d21569e8507165c3b34e1ed1f1f9cf6dfb71ddcdeb2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 10 May 2022 22:44:47 GMT
WORKDIR C:\go
# Tue, 10 May 2022 23:33:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 May 2022 23:33:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:33:04 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:33:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:34:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 10 May 2022 23:34:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01012ab52f3f9693dd4b85e6e19a0b2659b4f869d6b5b5d2ea62afe84c9037c`  
		Last Modified: Tue, 10 May 2022 22:55:50 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988abb6e02c6ab2eb0330641b6378c4e110c132c761de086dfc1629462491e90`  
		Last Modified: Tue, 10 May 2022 22:55:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b62ac07a4cd6e0fd762f7f6e904be7b001affa78e8fbfeb8ca017a6f643d62c`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e235721feec6368d5a652fd467681dffe74326d42da4bed8e43f777bc39c47`  
		Last Modified: Tue, 10 May 2022 22:55:47 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195b6f87245387233358bc8fcc2679a23d9aa46cd4bfef94ac49284694c5c42`  
		Last Modified: Tue, 10 May 2022 22:56:13 GMT  
		Size: 25.6 MB (25580295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cfe0249f2fac54d31ea467ce63bdc69e4504b726a87d969fb1b42ab2ab3853`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c97dcc9056ac36ad6120d94049a937f5366e71fda7c478ff3462d542cc0645`  
		Last Modified: Tue, 10 May 2022 22:55:45 GMT  
		Size: 322.0 KB (321981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4753086b1ed8db6655e0993e3f676d7f71455415cce16cd5593b330f9a89b3a`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66134c7f83737bd3064ea2c3dce37ea0157cde99b46bbf80744100fd7f18a0aa`  
		Last Modified: Tue, 10 May 2022 23:07:31 GMT  
		Size: 142.6 MB (142588622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0697a4af489e787e5def466bbf9614e20bf5b1cea211f3a8f8ce2f0b5a10a3f`  
		Last Modified: Tue, 10 May 2022 23:05:04 GMT  
		Size: 1.6 KB (1566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c242b44aab0e82a2f6bf16213c350b73347e55ad15ecafa05877414e1327e96b`  
		Last Modified: Tue, 10 May 2022 23:36:29 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223dbf32ed9ac3b13af8e1196395df286392aa610ec5ba0bf809061dbf84a5cb`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a255b634df668adc897872554f8b720fdd5e6f4a9c47db0bbc489d25a0aaa66e`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18292f9995b50f39e6e8ef4cfa31d2913132bef8804b56e260a907b205cd18`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a524248b6a67f943614b53e6a0825bd107c0b90796733fccfe1184d013a45`  
		Last Modified: Tue, 10 May 2022 23:36:28 GMT  
		Size: 1.7 MB (1691907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4398dd61eb69a257d8e25ec572462f611d347efd5e30a944117a652f47314944`  
		Last Modified: Tue, 10 May 2022 23:36:26 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
