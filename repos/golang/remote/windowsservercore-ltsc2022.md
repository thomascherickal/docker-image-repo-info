## `golang:windowsservercore-ltsc2022`

```console
$ docker pull golang@sha256:b4e2ecfb0efbbedb99a49262f3cb6a7e571d9c9a8f915cdf51993bb7b488db70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `golang:windowsservercore-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull golang@sha256:ce3fe36da9b11704d3ada39c8a8876be05853b3041f80a7d0cd0875310cb9118
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1898159568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52e431fd1f12887d8db30ae84163c487c41a827970d0e6c7a6c9be0aa680368a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:49:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:49:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:49:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:49:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:50:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:50:33 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:51:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 01:51:03 GMT
ENV GOLANG_VERSION=1.20.3
# Wed, 12 Apr 2023 01:54:00 GMT
RUN $url = 'https://dl.google.com/go/go1.20.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '143a2837821c7dbacf7744cbb1a8421c1f48307c6fdfaeffc5f8c2f69e1b7932'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:54:02 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4eb152e8775777886c34769c9441311dc4cfa18739a77add3a28f4146876c0`  
		Last Modified: Wed, 12 Apr 2023 02:32:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178567290fd84aae46273380c8bbab148ca30148807f2152ab814a3404cf485`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd32032c86ce46fc3bd16fd2626e5ef1ad026803eb85788f8cd91806b9b8d54`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c72e3d7691a1228d8cb57c6aee1dfb1257d1f0a9ac87e1f46a51b80ca7496b1`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07645ae8480c674321c57e55fce61bb16b6c09f94b07982e8ae4730746807e61`  
		Last Modified: Wed, 12 Apr 2023 02:32:06 GMT  
		Size: 25.9 MB (25855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7114ddfb58c5199edc3cc1e070d9c70422f31bb08a24e9a22a810a95267f5dc4`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2024bc0d3314bfc3e125a3386eb0b2fda1ac02c72426efde256013cf401972`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 544.5 KB (544547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fbc75391b6206e84aa8840965a815c59032e0047705c096c0881a18592c554`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020c21195e80d5c5b273ad94394eea9353a4ecd2c84addd353cc1fdb0016cff7`  
		Last Modified: Wed, 12 Apr 2023 02:32:31 GMT  
		Size: 109.1 MB (109146275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3566358d218ff3f40128d2c7acbcab5c2c0bedacef9d9264824f21c6f683235`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 1.6 KB (1564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
