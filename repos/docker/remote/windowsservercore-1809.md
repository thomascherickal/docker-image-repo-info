## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:c60157fce4fa3276653e172382be58c88cdd047293e2ccab58d68c842892cf4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull docker@sha256:dcc3ec866812ef6805a048087bb4a9205bb06b7c407e13281b995673651967b9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2122590252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f2822c695a2818eb732aecb5bb5bda744b307e6611f531aa34ae9eb60bafbb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:25:51 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 18 Apr 2023 00:16:44 GMT
ENV DOCKER_VERSION=23.0.4
# Tue, 18 Apr 2023 00:16:44 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.4.zip
# Tue, 18 Apr 2023 00:17:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 18 Apr 2023 00:18:00 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Tue, 18 Apr 2023 00:18:01 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.windows-amd64.exe
# Tue, 18 Apr 2023 00:18:01 GMT
ENV DOCKER_BUILDX_SHA256=e4bb5f70d98be80421bb26b78dd71fe9184a5f94315a6712f487e9eb252ad4f1
# Tue, 18 Apr 2023 00:19:19 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 18 Apr 2023 00:19:20 GMT
ENV DOCKER_COMPOSE_VERSION=2.17.2
# Tue, 18 Apr 2023 00:19:21 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.17.2/docker-compose-windows-x86_64.exe
# Tue, 18 Apr 2023 00:19:22 GMT
ENV DOCKER_COMPOSE_SHA256=0869cfe9d799d511e4eaf87029ed08ea256e7000f312023c062d7ddcadc385db
# Tue, 18 Apr 2023 00:20:35 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f180306e9d61cdf6a72f401f1f32a79e350f22b096e8dd7910d6afe20e3e23e9`  
		Last Modified: Wed, 12 Apr 2023 04:07:41 GMT  
		Size: 500.1 KB (500143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b928a08d5396441d12513b010e0563a20aa7cbb8a70c8679eecf8086e5d687a8`  
		Last Modified: Tue, 18 Apr 2023 00:21:51 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9073a0296ef428b991b431b31a876f7c079fa8ddbf85b68ac6516096c43b4f81`  
		Last Modified: Tue, 18 Apr 2023 00:21:51 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7816ad40cca28c0a6ad4471edfdbd7519e6c7fdc546885fb22abe956a15be12b`  
		Last Modified: Tue, 18 Apr 2023 00:21:54 GMT  
		Size: 17.4 MB (17392664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbb925bd9e68d4c69e225d68df3cbb6a4c096aaa7a27a056b4703147ca2853b`  
		Last Modified: Tue, 18 Apr 2023 00:21:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064e9792d4371c1e5fd8e0dbef0059e9ec14cb56dc5b4faca3dc1d8ee1eea594`  
		Last Modified: Tue, 18 Apr 2023 00:21:49 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb83adf02396cbf5bfb050455a6f0ae25cea66d81b48e8b6355244001316a904`  
		Last Modified: Tue, 18 Apr 2023 00:21:49 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92549bc5dcf75d7b4411375dd37b5dfe979a7538be155cc09b7308a24e8d346`  
		Last Modified: Tue, 18 Apr 2023 00:21:51 GMT  
		Size: 16.5 MB (16513922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dc10ee48658f51b4c174d6630d0033ed0733bc795b7647ce21a461b6e017e5`  
		Last Modified: Tue, 18 Apr 2023 00:21:47 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c138959207683244a8682ffe26541e52630e9643af2e294af58521a42fdf303`  
		Last Modified: Tue, 18 Apr 2023 00:21:47 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b769b70109dcc5e77def78ae909b98c6c7944bf3f2b290424e84cbc0a289cf8`  
		Last Modified: Tue, 18 Apr 2023 00:21:47 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0a6e4b6e6772e01e5f5b642b2b2fc6612ce3ed1c1e84447aff60169abc89fe`  
		Last Modified: Tue, 18 Apr 2023 00:21:51 GMT  
		Size: 16.9 MB (16879578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
