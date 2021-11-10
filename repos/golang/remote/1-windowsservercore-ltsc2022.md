## `golang:1-windowsservercore-ltsc2022`

```console
$ docker pull golang@sha256:5bb35522eda2705e84043a13a817946afd34311dd17a097cc3bf69a9785c5c64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.350; amd64

### `golang:1-windowsservercore-ltsc2022` - windows version 10.0.20348.350; amd64

```console
$ docker pull golang@sha256:d5d7b007ed5d9192c31fa886e8d1b623fb403d9e92754ce111cdf7a94973cb71
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2356474935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0705fdf32d7a8325f361132ddc3821a79f00ff8d96cbe762061ddeb51dc85002`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 03 Nov 2021 08:36:33 GMT
RUN Install update ltsc2022-amd64
# Wed, 10 Nov 2021 01:38:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:22:31 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:22:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:22:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:22:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:23:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:23:19 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:23:38 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Nov 2021 13:23:39 GMT
ENV GOLANG_VERSION=1.17.3
# Wed, 10 Nov 2021 13:26:03 GMT
RUN $url = 'https://dl.google.com/go/go1.17.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e78684b955742e215926204afc6ed62b9d165b509e25a687d62902516f08726b'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:26:06 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0eb404f1860fa8786ad09d1d9fe9fd580115f83cd38623bc4eb0c46abdaa0a3`  
		Size: 932.9 MB (932907933 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:27ded59d7006d9d7bffa7c253cd04a900a5d6b0d47b84d0edd624d12fd64cdc9`  
		Last Modified: Wed, 10 Nov 2021 02:07:39 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c8da5c86a468b2fe50c22d34ead6ad8eb01aa1b5b262eec65394923a5a2513`  
		Last Modified: Wed, 10 Nov 2021 14:04:18 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876dcf96238934dec5cc9605bc9bac3b621dad6917d7e8d59890b06ba0a7a6c3`  
		Last Modified: Wed, 10 Nov 2021 14:04:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fe8c8e41f94d3ec1b119db49f9aa03dbe93c1123648a9d1f8b9129dc0b8123`  
		Last Modified: Wed, 10 Nov 2021 14:04:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e606198baaa9997fc0b098964d0e241e017f14b348901d7a4f064b8447ce010e`  
		Last Modified: Wed, 10 Nov 2021 14:04:13 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d3b55e1d50fff3c37e9db90767f2611d6f8130797d9308d00e27f32bd47713`  
		Last Modified: Wed, 10 Nov 2021 14:04:20 GMT  
		Size: 25.7 MB (25697981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e37b08ca8c6e334587bd0b8b2643d610737ee07765f4c620752a3c121014768`  
		Last Modified: Wed, 10 Nov 2021 14:04:10 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82fe85265b4235639078385a55bc05727cd6d92234a6b7ad134852118530a7b`  
		Last Modified: Wed, 10 Nov 2021 14:04:11 GMT  
		Size: 551.5 KB (551510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9061109c0866dbdea9de30e1c652c678a075da8f6d4b56a54dd65acd98de34ad`  
		Last Modified: Wed, 10 Nov 2021 14:04:10 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1e90eaa484891e81d567be578e3e613fad3d633c4929f2027c1a09f63824d2`  
		Last Modified: Wed, 10 Nov 2021 14:04:45 GMT  
		Size: 145.6 MB (145607063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c38f779bb92450b4eb797cb84181ccb3e5cd7833b415081687cea714989e0b`  
		Last Modified: Wed, 10 Nov 2021 14:04:10 GMT  
		Size: 1.5 KB (1495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
