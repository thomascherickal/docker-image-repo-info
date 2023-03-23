## `docker:23-windowsservercore-1809`

```console
$ docker pull docker@sha256:62338fb38b507ffaea2293eee1f5163eba14e317aa64ebbc8337dfcc20fd096f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `docker:23-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull docker@sha256:2898ec902f053ec46a5fb177d854bed9f3c859ae50efe326c090166db42eed72
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2064607957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c98df15887b7dec51110c5ad0269c8b47c4840ea80c1b66fb8c42df3e7bad64d`
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
# Thu, 23 Mar 2023 01:16:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.17.0
# Thu, 23 Mar 2023 01:16:56 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.17.0/docker-compose-windows-x86_64.exe
# Thu, 23 Mar 2023 01:16:56 GMT
ENV DOCKER_COMPOSE_SHA256=1374f42a72ac46430b4a72016d8b1428317dd81811016373518b7afa7d86cee8
# Thu, 23 Mar 2023 01:18:39 GMT
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
	-	`sha256:0c7812947a985f59929bf85915b05ed4da63a65fa8cb1815526cc65951220a26`  
		Last Modified: Thu, 23 Mar 2023 01:22:29 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0cf2fac6aa10c9e9a9cb825ea1bffb376e5fc17349d080e0086bfe7f74878e`  
		Last Modified: Thu, 23 Mar 2023 01:22:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597aafd1f813dfdea501499bbe3ad91ef51dd5afda97b481e05dcd7af024319d`  
		Last Modified: Thu, 23 Mar 2023 01:22:28 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344dcf9b4251298973dd93cc8224f4c174e4c7ea4059f5decb0bfcfeb9dd2415`  
		Last Modified: Thu, 23 Mar 2023 01:22:32 GMT  
		Size: 16.8 MB (16772598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
