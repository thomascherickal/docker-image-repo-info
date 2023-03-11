## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:67c955c184896942b6e88e02e4af0317efba8ef9066d543fd09cb3fb8607ccf2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `docker:20-windowsservercore` - windows version 10.0.20348.1547; amd64

```console
$ docker pull docker@sha256:6a3da5cc3e29150067a1deddf0273ae6499491c2be5fff6f2d6dd99a36aa1c48
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1768910711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68892c2220ec64e924a988bb749da04bd85ce693305a7f1c52845279bb06cf58`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:33:13 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 02:37:56 GMT
ENV DOCKER_VERSION=20.10.23
# Thu, 16 Feb 2023 02:37:57 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Thu, 16 Feb 2023 02:38:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 11 Mar 2023 01:20:09 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Sat, 11 Mar 2023 01:20:10 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.windows-amd64.exe
# Sat, 11 Mar 2023 01:20:11 GMT
ENV DOCKER_BUILDX_SHA256=e4bb5f70d98be80421bb26b78dd71fe9184a5f94315a6712f487e9eb252ad4f1
# Sat, 11 Mar 2023 01:20:47 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Sat, 11 Mar 2023 01:20:47 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Sat, 11 Mar 2023 01:20:48 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-windows-x86_64.exe
# Sat, 11 Mar 2023 01:20:49 GMT
ENV DOCKER_COMPOSE_SHA256=a35d1188e796dbda914ddb9677059c654b445aa2921066e0b556ca9906bb603c
# Sat, 11 Mar 2023 01:21:18 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e31c0ce3f337b044901163fed3eab931c5230b0243d3265fb3aa74a4d5a2aa6`  
		Last Modified: Thu, 16 Feb 2023 02:40:50 GMT  
		Size: 769.3 KB (769272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37000251b28c80b932b3966a757f238990dd0606d478d8de8cccb1d802ec715`  
		Last Modified: Thu, 16 Feb 2023 02:41:21 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f9bb19df9823688a18314d31ef7b8dace8b26e828c29f902f388073292c7ee`  
		Last Modified: Thu, 16 Feb 2023 02:41:21 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6e72881b95eb9b53a07b0a42327076108754c7e0c89547c51a0c821550082`  
		Last Modified: Thu, 16 Feb 2023 02:41:31 GMT  
		Size: 56.0 MB (55968992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fd2dd333714581c7c78c24eb627fe5c46a2bc49fdda266b0e2f776c2fbdd1b`  
		Last Modified: Sat, 11 Mar 2023 01:25:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae82ba6f6ba841c9418f00e68065e187b55b27cc17bfdae9f746fbcd791d03b`  
		Last Modified: Sat, 11 Mar 2023 01:25:31 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd25a55c44aea31bf3f5198360e89a4952df84a64bea433a910f43929ac76c5c`  
		Last Modified: Sat, 11 Mar 2023 01:25:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c27220b84872ddd23ee5999650aceaac373533ca0854a5b50bc50d9f92ded2f`  
		Last Modified: Sat, 11 Mar 2023 01:25:31 GMT  
		Size: 16.7 MB (16736167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc1c47ff039bf26836d07c2726f7ea6073d0cd97ce2e530ce0590a2979ea47e`  
		Last Modified: Sat, 11 Mar 2023 01:25:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6d244535534ca293f46bf58860f22dd80862820c4961b920d21320ea35d8df`  
		Last Modified: Sat, 11 Mar 2023 01:25:26 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc36cddff6496665b67be076912e626299d92218eeae4155714967a165851f85`  
		Last Modified: Sat, 11 Mar 2023 01:25:26 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8233db51d8f27483c785e50c75bc3d34ae188d01573e84cbe046797034ed89d6`  
		Last Modified: Sat, 11 Mar 2023 01:25:31 GMT  
		Size: 16.1 MB (16077236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-windowsservercore` - windows version 10.0.17763.4010; amd64

```console
$ docker pull docker@sha256:f9ef6e6b115aec84da8b808b21614850866d6a21406444bae8c61a724545c4ea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051576352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:611355a5907f1a4e4c9341ba9614873a2af7bb0404933565a582f3a9a76b8c7e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:35:24 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 02:38:43 GMT
ENV DOCKER_VERSION=20.10.23
# Thu, 16 Feb 2023 02:38:44 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Thu, 16 Feb 2023 02:40:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 11 Mar 2023 01:21:36 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Sat, 11 Mar 2023 01:21:37 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.windows-amd64.exe
# Sat, 11 Mar 2023 01:21:38 GMT
ENV DOCKER_BUILDX_SHA256=e4bb5f70d98be80421bb26b78dd71fe9184a5f94315a6712f487e9eb252ad4f1
# Sat, 11 Mar 2023 01:22:48 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Sat, 11 Mar 2023 01:22:49 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Sat, 11 Mar 2023 01:22:50 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-windows-x86_64.exe
# Sat, 11 Mar 2023 01:22:50 GMT
ENV DOCKER_COMPOSE_SHA256=a35d1188e796dbda914ddb9677059c654b445aa2921066e0b556ca9906bb603c
# Sat, 11 Mar 2023 01:24:05 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fec720058b47d0684c0cd4510fc0ecbd46e9190c17f7c384e1910dace8de10`  
		Last Modified: Thu, 16 Feb 2023 02:41:06 GMT  
		Size: 512.2 KB (512156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d0b4bbc1480a317988f088f1dde1ea8db127278dc02abee34914efec310919`  
		Last Modified: Thu, 16 Feb 2023 02:41:41 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34394b061f1fb129f4945bdd6b34b289924c9362c4566c3b5dcba92523e9c334`  
		Last Modified: Thu, 16 Feb 2023 02:41:41 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f9c27a974e711d0fe130afe51966a55008d5db57e075d7cb1f6cd044c3caf6`  
		Last Modified: Thu, 16 Feb 2023 02:41:51 GMT  
		Size: 55.7 MB (55742637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0422fd48b44b823751896f06e193ff087b6e742471379e95828ec135844aaa24`  
		Last Modified: Sat, 11 Mar 2023 01:25:49 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26317f2081ac354e3d452ec62a0b8e45be907848d72afec7aefbac2d9013987`  
		Last Modified: Sat, 11 Mar 2023 01:25:48 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd3f38268010c14aeb90119ad7880cb40ebe04428f802c199649159e8aeccba`  
		Last Modified: Sat, 11 Mar 2023 01:25:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c8f5ed7b4ee9e58e05074460938d58a17306bc612125fafa73291db7db450e`  
		Last Modified: Sat, 11 Mar 2023 01:25:49 GMT  
		Size: 16.5 MB (16515071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd47f0bf337a9b8993a9dda2e68c73f29f15d8b6097032e6aaae441489ac345`  
		Last Modified: Sat, 11 Mar 2023 01:25:44 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4c7da557db12513122a48c4833f8f4b136ba220c0caaed5a4a233b2c02317f`  
		Last Modified: Sat, 11 Mar 2023 01:25:44 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c816d661fed34c69e6de245310ea2709ecd4935c94f39474604b29b0f42de9`  
		Last Modified: Sat, 11 Mar 2023 01:25:44 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff15f4f8396a41e73c2f04222153603c04133646b57e21ef42c2bb72a923264`  
		Last Modified: Sat, 11 Mar 2023 01:25:48 GMT  
		Size: 15.8 MB (15835977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
