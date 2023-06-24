## `docker:windowsservercore`

```console
$ docker pull docker@sha256:021f215b63dd231dc093cd7437f9fc896527bc0d467f829e1ec10d4f9455396f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `docker:windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:ebc80c06160be1357f432cabfc6251d968359fb27421bb2b6917de209d4e4ad6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480375746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee25ec0480e76f3e3c66f672eb5766c95a35aae602da7897c040651aaa45c4e2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:33:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:33:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:34:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:34:05 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:34:06 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:34:07 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:34:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:34:35 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.0
# Sat, 24 Jun 2023 03:34:36 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.0/docker-compose-windows-x86_64.exe
# Sat, 24 Jun 2023 03:34:37 GMT
ENV DOCKER_COMPOSE_SHA256=dc6bd9c2016bbf7564959249204af044edf57ea4ff40238c5ecb4541a9d41573
# Sat, 24 Jun 2023 03:35:02 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9422c57cfa4958bc0481159cf6f3ea51c62e434b415bd37af5122a927dad44e5`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3038159acbdccb213594b93376d485aeeb899ddecb260c15c35876de1a826205`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de76d8841c57bd71ac348e6e5adafd8c4bb7b220dba2990cfb45212e8c02ec51`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 17.4 MB (17435791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601d2c848cc34db3244fd32712379ae9207438e92e8b1bfc93158f40c450b05f`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2546289e6eaf1c79435f5ebc3913d3400b9e48f9865fbac9a4f64a9631e16c`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7be502d4e9bbbfde8c8e153a1b773402566c1780fe74fc0ebd74481ab156a59`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a421c1544ba646557911d25deeb82872547032eda17bffad452d2d66dbe4714`  
		Last Modified: Sat, 24 Jun 2023 03:41:34 GMT  
		Size: 17.9 MB (17867701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce91003ebf51f269f36c1466ff682074b9d5f0cc0f959c9e2e6109eb6a03796`  
		Last Modified: Sat, 24 Jun 2023 03:41:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15344fe4571c8c0612c5ba8a9510f8664d321dcdf55d26f6ca07c4e4452880df`  
		Last Modified: Sat, 24 Jun 2023 03:41:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7708db62637ac83391cea38aae6332a3670cbdb14010c0ca3b8c1e88ff5818c`  
		Last Modified: Sat, 24 Jun 2023 03:41:29 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923f0e43e96d8547dd9bdf6fabb90d588557c5c92893990d374d1e3dfdc6fb89`  
		Last Modified: Sat, 24 Jun 2023 03:41:34 GMT  
		Size: 18.4 MB (18434502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:460d09b2f3a5109cd7532bcc085fe0a7f4f76485ea010d9ed89e2963d889eea4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704765604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9dced64a03914ac14f64f7bbe7e6754351eb2f4f6370c7dd19cb4947281e4af`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:35:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:35:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:36:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:36:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:36:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:36:10 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:36:41 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:36:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.0
# Sat, 24 Jun 2023 03:36:42 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.0/docker-compose-windows-x86_64.exe
# Sat, 24 Jun 2023 03:36:43 GMT
ENV DOCKER_COMPOSE_SHA256=dc6bd9c2016bbf7564959249204af044edf57ea4ff40238c5ecb4541a9d41573
# Sat, 24 Jun 2023 03:37:14 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed839336f22dd57d3537286fd2cb28bb3fc0572198a3b9bd727227ee4cbdf055`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce643c4303a7b93be26b0dd0216711bedc40974b948aa175e501ebfd967e8da`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc026cb3268fba4d3f45b15b22d85c45b0833d7e6f03faf3f1adb1f7750eb889`  
		Last Modified: Sat, 24 Jun 2023 03:41:57 GMT  
		Size: 17.4 MB (17427965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ada76c0fbca30898687db44782375adfd8511d9f5fe79eb1df4524e36cb3b`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a336a464a58681af94fdcfb3fbc461c2ac77b4bd2d6ec0c339fbae654521420`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f6fe82d1e4f989c122320481c6c3473632cffcc634f225106e7c73585db1c7`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6f83ed64356628e46ae865b628bc2568b3e8679ec35b1c6211d4c49ee99d80`  
		Last Modified: Sat, 24 Jun 2023 03:41:55 GMT  
		Size: 17.9 MB (17857203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ceef668a9f9d710bf676c93031943411eb376c7555b3641ff1eff4e3762a163`  
		Last Modified: Sat, 24 Jun 2023 03:41:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb16a8ed2372b28b1ce0a965169faaa225ad10239717c408ff2fa64f22da784`  
		Last Modified: Sat, 24 Jun 2023 03:41:50 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a0125beb539dadae7968839eb480ba29c3b2684daed1f4b92205c96de03723`  
		Last Modified: Sat, 24 Jun 2023 03:41:50 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7046c9169102383c51093b0139de9b03483313b54e12fe2ca0807ce4b60efe40`  
		Last Modified: Sat, 24 Jun 2023 03:41:55 GMT  
		Size: 18.4 MB (18425797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
