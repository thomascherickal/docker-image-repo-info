## `docker:windowsservercore`

```console
$ docker pull docker@sha256:9fd6220c95c38a6961bdb8ac3f8a7e51a526f90729a7f1c2698f8483c4db3a1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1607; amd64
	-	windows version 10.0.17763.4131; amd64

### `docker:windowsservercore` - windows version 10.0.20348.1607; amd64

```console
$ docker pull docker@sha256:e99c397ebd8872c9ab32cf170796a097bd6495b6cec42cabd0b6d4b70f7d30fe
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1766064235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e0cc96f89f42f9030ae0713768c5a554c908f2dd967cf8309793eecb65c2f6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:48:27 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 04:48:28 GMT
ENV DOCKER_VERSION=23.0.1
# Thu, 16 Mar 2023 04:48:29 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Thu, 16 Mar 2023 04:49:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 04:49:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Thu, 16 Mar 2023 04:49:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.windows-amd64.exe
# Thu, 16 Mar 2023 04:49:10 GMT
ENV DOCKER_BUILDX_SHA256=e4bb5f70d98be80421bb26b78dd71fe9184a5f94315a6712f487e9eb252ad4f1
# Thu, 16 Mar 2023 04:49:47 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 27 Mar 2023 22:15:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.17.2
# Mon, 27 Mar 2023 22:15:29 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.17.2/docker-compose-windows-x86_64.exe
# Mon, 27 Mar 2023 22:15:30 GMT
ENV DOCKER_COMPOSE_SHA256=0869cfe9d799d511e4eaf87029ed08ea256e7000f312023c062d7ddcadc385db
# Mon, 27 Mar 2023 22:16:04 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8618e746130a44a38c8238602d9bcd946d80bd2d8378a6a88b481e06dbb717`  
		Last Modified: Thu, 16 Mar 2023 05:04:57 GMT  
		Size: 733.4 KB (733414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062bc738477402769a7c91526d78e79eb1bea43110a2ebb60fca4d6dc4dc496b`  
		Last Modified: Thu, 16 Mar 2023 05:04:56 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07883eef61a34739d4fd0910b4263a7e81dc90430191b85e951901ce8260231`  
		Last Modified: Thu, 16 Mar 2023 05:04:56 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5900f43a367928830694dc14cba97d65135f4edd98dd5b0a0cd8340ed9ee70`  
		Last Modified: Thu, 16 Mar 2023 05:04:59 GMT  
		Size: 17.6 MB (17565544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e79086220f31b5b3467958be34eb2e74ed4394cc1cdc759145bdf2ba31ebd4`  
		Last Modified: Thu, 16 Mar 2023 05:04:54 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc1445696a2a44f3dedb3b3b2f53ac6818ddcddb74e3fe80cadec5d6ebbb48d`  
		Last Modified: Thu, 16 Mar 2023 05:04:54 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b7b8e006d746d52dce97ed705cc437ea4b6c3daa624ee9cca1219a721a3c43`  
		Last Modified: Thu, 16 Mar 2023 05:04:53 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c6fc05fb186b25c3416c92ac4ab87aebcc357fe4d5470f6123108fc9f7eefc`  
		Last Modified: Thu, 16 Mar 2023 05:04:54 GMT  
		Size: 16.7 MB (16711853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856c885bf3b4fb4baad526b96d12001e8df5f537f564aa154d6375b4d3a54ab2`  
		Last Modified: Mon, 27 Mar 2023 23:16:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a6e627aa6c962bc34e3b2545cc653f35d55f37f645252c854d2288405e8e28`  
		Last Modified: Mon, 27 Mar 2023 23:16:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700183fcfcc742358d53eab2904ca6311f92bf834fa373b2a45197b4cd5bb56e`  
		Last Modified: Mon, 27 Mar 2023 23:16:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3512d5212b8e18dfe9fa9f50f76ec896d22b533180e24053ea0fb3af440a351c`  
		Last Modified: Mon, 27 Mar 2023 23:16:08 GMT  
		Size: 17.1 MB (17100567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.4131; amd64

```console
$ docker pull docker@sha256:47ec696fdfc3730ad47e8052e4516030cf69648ef7844ca3bb74387333ce4f9f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2064716914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:505bdb534a073f8eb5ffbca8846ea603394de3a2d3e8a42693af25ca2c84d40c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:51:57 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 04:51:57 GMT
ENV DOCKER_VERSION=23.0.1
# Thu, 16 Mar 2023 04:51:58 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Thu, 16 Mar 2023 04:53:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 04:53:26 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Thu, 16 Mar 2023 04:53:27 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.windows-amd64.exe
# Thu, 16 Mar 2023 04:53:28 GMT
ENV DOCKER_BUILDX_SHA256=e4bb5f70d98be80421bb26b78dd71fe9184a5f94315a6712f487e9eb252ad4f1
# Thu, 16 Mar 2023 04:54:59 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 27 Mar 2023 22:16:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.17.2
# Mon, 27 Mar 2023 22:16:14 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.17.2/docker-compose-windows-x86_64.exe
# Mon, 27 Mar 2023 22:16:15 GMT
ENV DOCKER_COMPOSE_SHA256=0869cfe9d799d511e4eaf87029ed08ea256e7000f312023c062d7ddcadc385db
# Mon, 27 Mar 2023 22:17:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
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
	-	`sha256:e82a1257835f94345167154714886a4d51ef66180e08e94b575d6b92e636cfbd`  
		Last Modified: Thu, 16 Mar 2023 05:05:31 GMT  
		Size: 478.7 KB (478744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8945827ee90e8cbb75f52a45e7b5a1693ef854f802a7b8ae0d7d742831301241`  
		Last Modified: Thu, 16 Mar 2023 05:05:31 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00244b98c13b17eb532950bf224849293229bc41103d1ae919169da46217599d`  
		Last Modified: Thu, 16 Mar 2023 05:05:30 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c277980333ab9741a23330c533cc83f86ac0abb32a36a5747991b61ac6cb1b`  
		Last Modified: Thu, 16 Mar 2023 05:05:34 GMT  
		Size: 17.3 MB (17342835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06d6b59a5ff92409e4eabbad5852ea5cb585041f5977a726a13755c054b56b4`  
		Last Modified: Thu, 16 Mar 2023 05:05:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aeb94e5427b3267a91cd4b8c9271541041c9dc3d2e95b2aa52d9d55b7881ec`  
		Last Modified: Thu, 16 Mar 2023 05:05:23 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8d8a8289ec4dc10b4f54fdf23f9ef3c941960bde7a4c6fa14edccae39c2777`  
		Last Modified: Thu, 16 Mar 2023 05:05:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3b595928c23657a2974ca62cf18f536a9556c29f2c481f0d0a32d4c468799d`  
		Last Modified: Thu, 16 Mar 2023 05:05:22 GMT  
		Size: 16.5 MB (16492086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab09bd6d39925a9158b1a32e3fca556490ea48db27188236bf34158b06c94ea`  
		Last Modified: Mon, 27 Mar 2023 23:16:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16672b69f9cf42840daba022526671098e7501d979af6e339391bb9d26fc5e65`  
		Last Modified: Mon, 27 Mar 2023 23:16:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64483ec8696be2048c4b7c2d3ae984dbf64a01748ddce540a47ecadd5ec7c9c`  
		Last Modified: Mon, 27 Mar 2023 23:16:22 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc75b13eb67b3a8847faec274aadc92a9ea2b49f6931a5a213d01498f0a4a7c8`  
		Last Modified: Mon, 27 Mar 2023 23:16:26 GMT  
		Size: 16.9 MB (16881554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
