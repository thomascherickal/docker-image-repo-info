## `docker:rc-windowsservercore`

```console
$ docker pull docker@sha256:fbd6ab2e893bc71e4e88046566f667fb9b0dfe771a3a1425d044553b5d1d2c5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `docker:rc-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:562c3d0b0c5bdc9cd0402b262c0ce4a4646578269a484b7dfd24603e256f7171
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826192161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe2d2d180d94ff7e47670f11b97c0aed27046565396f0d9c6b5ddb58b0ba728`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 13 May 2023 00:15:54 GMT
ENV DOCKER_VERSION=24.0.0-rc.4
# Sat, 13 May 2023 00:15:55 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-24.0.0-rc.4.zip
# Sat, 13 May 2023 00:16:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 13 May 2023 00:16:23 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Sat, 13 May 2023 00:16:24 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.windows-amd64.exe
# Sat, 13 May 2023 00:16:25 GMT
ENV DOCKER_BUILDX_SHA256=e4bb5f70d98be80421bb26b78dd71fe9184a5f94315a6712f487e9eb252ad4f1
# Sat, 13 May 2023 00:16:50 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Sat, 13 May 2023 00:16:51 GMT
ENV DOCKER_COMPOSE_VERSION=2.17.3
# Sat, 13 May 2023 00:16:51 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-windows-x86_64.exe
# Sat, 13 May 2023 00:16:52 GMT
ENV DOCKER_COMPOSE_SHA256=556cc1d373503a897ecc2def998a40b2ad1fe27ff049769eb912c7e208772e74
# Sat, 13 May 2023 00:17:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706e4e2800e9071eb58477232301ca2c6f653e33422981056024d31be8103999`  
		Last Modified: Sat, 13 May 2023 00:22:13 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25fda557e5adeb0c0be6ecd4413b77ce8964d758f236929deb14b505fc6468cd`  
		Last Modified: Sat, 13 May 2023 00:22:13 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e56435e01384c38cdb750b13c7b432240a252242269d729a451567ffeb9e00`  
		Last Modified: Sat, 13 May 2023 00:22:15 GMT  
		Size: 17.4 MB (17442733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c5e8b83c8f5a64a3229690ad0b0d8e25b5dae1b763347aaf2740c8d5d91639`  
		Last Modified: Sat, 13 May 2023 00:22:11 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3abfb6078bdc2212003210b3c895fa1ea3b882912a3c9a1e0757906a0718f0`  
		Last Modified: Sat, 13 May 2023 00:22:11 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4069ae861030999c0d6044027d0b5df002874f53b1c550d20d8dbcc3aab97368`  
		Last Modified: Sat, 13 May 2023 00:22:11 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef49a42c350e495fd97c11d7572a16e72354722f17c513105c2ed81518f2b74`  
		Last Modified: Sat, 13 May 2023 00:22:13 GMT  
		Size: 16.5 MB (16469110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052b700482db7881b8fc47cfb04db1f96cba325589e36b1e4e2b73103cfc9f00`  
		Last Modified: Sat, 13 May 2023 00:22:09 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52376875e1a84919e3ed687a549ec25a48d30c93cdc254585a93970815ab1c24`  
		Last Modified: Sat, 13 May 2023 00:22:09 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc99d829f0b8733cfe79a422ffc45946d9883a57caedcb8a8bcd15a2abe79322`  
		Last Modified: Sat, 13 May 2023 00:22:09 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826df462c2af81371bd2ade7ed34a8066b219f0e6a4777f24f79e42b126e8773`  
		Last Modified: Sat, 13 May 2023 00:22:13 GMT  
		Size: 16.8 MB (16840047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:dc423ccb272125c0a81516b4acd1abedf7a7b7c73ff45c1de2aea80676a3dffa
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123322904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b7d2640d830b5d5081ed9378e8f69b6bb40ac8ea28a13566126c5deddc60fb9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 13 May 2023 00:17:37 GMT
ENV DOCKER_VERSION=24.0.0-rc.4
# Sat, 13 May 2023 00:17:38 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-24.0.0-rc.4.zip
# Sat, 13 May 2023 00:18:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 13 May 2023 00:18:48 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Sat, 13 May 2023 00:18:48 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.windows-amd64.exe
# Sat, 13 May 2023 00:18:49 GMT
ENV DOCKER_BUILDX_SHA256=e4bb5f70d98be80421bb26b78dd71fe9184a5f94315a6712f487e9eb252ad4f1
# Sat, 13 May 2023 00:19:56 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Sat, 13 May 2023 00:19:57 GMT
ENV DOCKER_COMPOSE_VERSION=2.17.3
# Sat, 13 May 2023 00:19:57 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-windows-x86_64.exe
# Sat, 13 May 2023 00:19:58 GMT
ENV DOCKER_COMPOSE_SHA256=556cc1d373503a897ecc2def998a40b2ad1fe27ff049769eb912c7e208772e74
# Sat, 13 May 2023 00:21:06 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1464977480594472e72fd9b3b2d2c46441165edfe28b1bc371f20f2a20822f6e`  
		Last Modified: Sat, 13 May 2023 00:22:31 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7182ff8ba45c492911d2f55654a245772a264f15453593c82f1c6649ca23009`  
		Last Modified: Sat, 13 May 2023 00:22:31 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5b9ef121857df5a9d87bdeab4896000738d1385b92062ec8e4fafabc2adde9`  
		Last Modified: Sat, 13 May 2023 00:22:34 GMT  
		Size: 17.5 MB (17474368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01b0efb1b5131309148ec45dce0639eb409f70f65ff04077088c4d0b048bc19`  
		Last Modified: Sat, 13 May 2023 00:22:29 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae331680ba521c4a472cf3312cf6e48df4b7e9cc60730bc2b351101c495f35f`  
		Last Modified: Sat, 13 May 2023 00:22:29 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f85d6a57c595811f1a9c2cf06895e9a4cb66765c720f16233f4cfdf1da5043`  
		Last Modified: Sat, 13 May 2023 00:22:29 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a3021dd421d602f4d65c8934e82a0b10730448183d00a5caaa718d70dfd8c6`  
		Last Modified: Sat, 13 May 2023 00:22:31 GMT  
		Size: 16.5 MB (16489533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad594332cd5d4db41a8ae3e68cc5eab5f257a47d8a5c06d4ed403c82c3d021c`  
		Last Modified: Sat, 13 May 2023 00:22:27 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2607251220d066cc4f1d350cb9e19a7877963cd484d55d677c0079da44d1ee50`  
		Last Modified: Sat, 13 May 2023 00:22:27 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90dc96a5a853ae1bc5a9d80fd1c7029c76614f4868dc0bd09ca56ffb3a6f88b5`  
		Last Modified: Sat, 13 May 2023 00:22:27 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc73a4cb7c8f77ce7340616a9460ea22c184caca219eeb9827f778f92ef314bc`  
		Last Modified: Sat, 13 May 2023 00:22:32 GMT  
		Size: 16.9 MB (16860357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
