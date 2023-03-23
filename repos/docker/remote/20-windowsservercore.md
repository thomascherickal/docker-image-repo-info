## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:ecf4f9e2cd010c6fa68fb43da79be275e47a252a67b5fafdacdbbb2f2c843a1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1607; amd64
	-	windows version 10.0.17763.4131; amd64

### `docker:20-windowsservercore` - windows version 10.0.20348.1607; amd64

```console
$ docker pull docker@sha256:14be4a7efe98f56433d46e8bf48ca3e04cb99c32735d613359fb87588a3b3117
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1804327037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1e60f5ea22bb67b4af9f5464b363b1787a2b42368ac54e79c58f892b468d668`
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
# Thu, 16 Mar 2023 04:56:41 GMT
ENV DOCKER_VERSION=20.10.23
# Thu, 16 Mar 2023 04:56:42 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Thu, 16 Mar 2023 04:57:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 04:57:29 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Thu, 16 Mar 2023 04:57:30 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.windows-amd64.exe
# Thu, 16 Mar 2023 04:57:32 GMT
ENV DOCKER_BUILDX_SHA256=e4bb5f70d98be80421bb26b78dd71fe9184a5f94315a6712f487e9eb252ad4f1
# Thu, 16 Mar 2023 04:58:19 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Thu, 23 Mar 2023 01:18:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.17.0
# Thu, 23 Mar 2023 01:18:58 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.17.0/docker-compose-windows-x86_64.exe
# Thu, 23 Mar 2023 01:18:59 GMT
ENV DOCKER_COMPOSE_SHA256=1374f42a72ac46430b4a72016d8b1428317dd81811016373518b7afa7d86cee8
# Thu, 23 Mar 2023 01:19:36 GMT
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
	-	`sha256:2d1dcd7ff62e8f9e0a17ffbbff0e8d7339c26437a170d56f77c9583bdfd391bd`  
		Last Modified: Thu, 16 Mar 2023 05:05:57 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3980cc096c68060dc316171fdd5b1dfd1966fc246444329fb15dffd719912785`  
		Last Modified: Thu, 16 Mar 2023 05:05:57 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3be3a71c80a098a3a64a9f905e71da918009c1819e7e5f9670e276101f76c6`  
		Last Modified: Thu, 16 Mar 2023 05:06:08 GMT  
		Size: 55.9 MB (55938215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95cf757689fca9e470351e13a554725455975b6d13d577c878b1b87e8ffa1b0`  
		Last Modified: Thu, 16 Mar 2023 05:05:55 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a527313acf61cbdeaee03fe67a68d132320893286c149d7e9dc5bc6111ee8c8`  
		Last Modified: Thu, 16 Mar 2023 05:05:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507adf21bfdf4a9d3a815a748d57be08d9e94caff06302dd2986aaad56a6bc9c`  
		Last Modified: Thu, 16 Mar 2023 05:05:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743ee42a8e48f98077b951767219e5eeb856f992815680ba333052715e7b65f0`  
		Last Modified: Thu, 16 Mar 2023 05:05:55 GMT  
		Size: 16.7 MB (16711996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef855580df5065d9837f9707b57a032d6b628d0d68d270f0ec7435ad5a0c8c31`  
		Last Modified: Thu, 23 Mar 2023 01:22:52 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536f7b28639b267939c078a4ca0b78044e4e60e0329637ccf5ade25565409c70`  
		Last Modified: Thu, 23 Mar 2023 01:22:52 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded3a01e73141bc9a9bb65661e4e16d4bd66af04cc30a89a316fe64db9c135a4`  
		Last Modified: Thu, 23 Mar 2023 01:22:52 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c40fa97bad9ca21ee3c3f712e299f30e16aca11ed8f15b42dc390428142138`  
		Last Modified: Thu, 23 Mar 2023 01:22:57 GMT  
		Size: 17.0 MB (16990637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-windowsservercore` - windows version 10.0.17763.4131; amd64

```console
$ docker pull docker@sha256:dece1f701d55d3a735720c0e86e22b0bb7759fff21e8537a5798c55993ee6023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2102984722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a0f1f2b55bf04208d749132e8bf97d1ff79bdc4d22265d40f59402fff5fb54`
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
# Thu, 16 Mar 2023 04:59:11 GMT
ENV DOCKER_VERSION=20.10.23
# Thu, 16 Mar 2023 04:59:12 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Thu, 16 Mar 2023 05:00:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 05:00:46 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Thu, 16 Mar 2023 05:00:47 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.windows-amd64.exe
# Thu, 16 Mar 2023 05:00:48 GMT
ENV DOCKER_BUILDX_SHA256=e4bb5f70d98be80421bb26b78dd71fe9184a5f94315a6712f487e9eb252ad4f1
# Thu, 16 Mar 2023 05:02:19 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Thu, 23 Mar 2023 01:19:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.17.0
# Thu, 23 Mar 2023 01:19:51 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.17.0/docker-compose-windows-x86_64.exe
# Thu, 23 Mar 2023 01:19:53 GMT
ENV DOCKER_COMPOSE_SHA256=1374f42a72ac46430b4a72016d8b1428317dd81811016373518b7afa7d86cee8
# Thu, 23 Mar 2023 01:21:15 GMT
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
	-	`sha256:4187d93a0dea223ecae3e6d8f92d14a705f8f228aeb1b18e4bd4ffd442b7c1dc`  
		Last Modified: Thu, 16 Mar 2023 05:06:28 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77d4bfc27625f3c07731da8936b5518c04d1aa517f428f49f738a3bf6e4f3ab`  
		Last Modified: Thu, 16 Mar 2023 05:06:28 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430451525b3d288c5911ea3aa5a2e06670232aa92dccc1627202238546e04795`  
		Last Modified: Thu, 16 Mar 2023 05:06:39 GMT  
		Size: 55.7 MB (55720911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a46b8a89a32bd0606adc5869fcdc0197842bc190c1e63cc1f72c1506d68b14`  
		Last Modified: Thu, 16 Mar 2023 05:06:26 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cee513ab20a2978c8635e230fdf699eb05025402e046113f0754345e5bf296`  
		Last Modified: Thu, 16 Mar 2023 05:06:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d6226b1566226d2b1731fb2d5f140050d01f677dfead0141753f765c14a6b`  
		Last Modified: Thu, 16 Mar 2023 05:06:26 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601db99d3728ef4bfdefe4a55e9b505c587eaa698af102bd21f218f809777ad6`  
		Last Modified: Thu, 16 Mar 2023 05:06:26 GMT  
		Size: 16.5 MB (16491494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517c9a96778c7b6e792d1a7046092f457685d218d67dea256a47963247a51097`  
		Last Modified: Thu, 23 Mar 2023 01:23:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cb77753d4e0059a59bedbc3e4a1bbcefbde4a191eba635b259b19ad6248abf`  
		Last Modified: Thu, 23 Mar 2023 01:23:13 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600ee29b59323da05a8a8078ef62261ed64b542716f66d42793badec860dbc19`  
		Last Modified: Thu, 23 Mar 2023 01:23:13 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228b5cfcb090ef0e662ceb3dc1b3132ce1c4ce3f2b7f3fe062e546bb9f21e771`  
		Last Modified: Thu, 23 Mar 2023 01:23:16 GMT  
		Size: 16.8 MB (16771987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
