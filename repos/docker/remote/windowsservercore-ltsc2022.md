## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:86581071c1de7b05ee763fca6ed50162292701a58aaad30c1a923122ad9ac0bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:f9029f7d23d9f4b81d94e3e094a41435a0c09de68f4613d5e7c38ed885949e42
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480427300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b2d4fa77485fb961b4bc1436799322639c548bd26a069c2efd0b41e4a3f105b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 10 Jul 2023 19:15:14 GMT
ENV DOCKER_VERSION=24.0.4
# Mon, 10 Jul 2023 19:15:15 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.4.zip
# Mon, 10 Jul 2023 19:15:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 10 Jul 2023 19:15:41 GMT
ENV DOCKER_BUILDX_VERSION=0.11.1
# Mon, 10 Jul 2023 19:15:42 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.windows-amd64.exe
# Mon, 10 Jul 2023 19:15:43 GMT
ENV DOCKER_BUILDX_SHA256=ed04052b2742e0a2e45a02c87ec4f782b8c7914f56a5d3e1bb39ff9ab8687f30
# Mon, 10 Jul 2023 19:16:07 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 10 Jul 2023 19:16:08 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Mon, 10 Jul 2023 19:16:09 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Mon, 10 Jul 2023 19:16:10 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Mon, 10 Jul 2023 19:16:33 GMT
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
	-	`sha256:37fea441d423b8b9b3a4d0af0bd2489561b0c94b9eda3299b6b63ec4cb86991b`  
		Last Modified: Mon, 10 Jul 2023 19:19:06 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9436c43f779d0840378f9ad866db2303c9f90f24e295ab32c3a326492aed9244`  
		Last Modified: Mon, 10 Jul 2023 19:19:06 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015988b8107795319b47f00536effab8152972f466b1ceb70c8961baddbc08fc`  
		Last Modified: Mon, 10 Jul 2023 19:19:09 GMT  
		Size: 17.5 MB (17458530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b90aad20a238f39d9c81f37c5d23a3a664f69dea0ef914ed6c8471de327475`  
		Last Modified: Mon, 10 Jul 2023 19:19:04 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795e7edf924a05d70c74c06529c1b034638ea4fcc81505c2b2fb69e3f1131411`  
		Last Modified: Mon, 10 Jul 2023 19:19:04 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5570420c259a1cd77a0c5c1c7beecf60615324695317266248ccf08ebc9739ea`  
		Last Modified: Mon, 10 Jul 2023 19:19:04 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8579a3bc28d849f8fc9b15ae985f88b27efdbd4f26e08dc51e50b997bfff78`  
		Last Modified: Mon, 10 Jul 2023 19:19:07 GMT  
		Size: 17.9 MB (17883703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404482cda1b3e4faf9fcae2517e1a76db6519e2dfaf9a806f4d0931dab341904`  
		Last Modified: Mon, 10 Jul 2023 19:19:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce3118f20723e5ff14aefcfaa16d36d3263a90e646287da27fadae95e1a4a06`  
		Last Modified: Mon, 10 Jul 2023 19:19:02 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3f8b932ab30ca74552c3198d6f8f0f5bbf9bf8d1a618af78a2d469550c3ef9`  
		Last Modified: Mon, 10 Jul 2023 19:19:02 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e5d1a92bd3cf4b084bb1a9a358d22763fa19df27b2e383c8bd2e35bfb6af79`  
		Last Modified: Mon, 10 Jul 2023 19:19:06 GMT  
		Size: 18.4 MB (18447995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
