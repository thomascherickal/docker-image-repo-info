## `docker:windowsservercore`

```console
$ docker pull docker@sha256:f4af31b74a5253ec58671de6c2710e16a5f2ac2817548c6a7e2154049cbc3bf2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `docker:windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull docker@sha256:a9020b9c4925433869c0c958d9e53f8ad2176330779b65f82f4bf310ea4bc9ab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2737923247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ab891d90a3bc1ec92ff32071fc677c238ee44a43d6eb073003da02862bd7d8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 19:24:35 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 19:24:36 GMT
ENV DOCKER_VERSION=20.10.8
# Wed, 15 Sep 2021 19:24:37 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.8.zip
# Wed, 15 Sep 2021 19:25:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76f6f3cf73df901f0ef53d2cf3a1187cb87ff309f8b28b24c1adcc34ea9ad1`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 353.9 KB (353857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451d02c3ec1421ec5056fe967d7be6a344cb53cfd77445f76f4b50483cfae635`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5f2c36a2ae93fffd565b76d88402e7eb238d7097f5ea1c17d64a5d85d745ac`  
		Last Modified: Wed, 15 Sep 2021 19:25:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f40204892cf05231048b06e8d6fb355be34ff937c4cfe6ac6cecb768f816d1d`  
		Last Modified: Wed, 15 Sep 2021 19:26:08 GMT  
		Size: 50.9 MB (50867243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
