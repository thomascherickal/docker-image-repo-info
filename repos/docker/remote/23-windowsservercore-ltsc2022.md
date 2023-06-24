## `docker:23-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:44dfa9177e4677f89725d802ce93ae8895351904db9d78511286dc5019e7353a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `docker:23-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:3ab469ba0244db4b24ef96eb553222a2f59cf1d3d1098ca7f0d1586a462a7889
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480265379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb69633c391fead5faa0fc9c9e1ca6b834507bbeeee8d6bba1f5a0b76b7aec61`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:37:22 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:37:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:37:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:37:51 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:37:52 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:37:53 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:38:20 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:38:21 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.0
# Sat, 24 Jun 2023 03:38:33 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.0/docker-compose-windows-x86_64.exe
# Sat, 24 Jun 2023 03:38:34 GMT
ENV DOCKER_COMPOSE_SHA256=dc6bd9c2016bbf7564959249204af044edf57ea4ff40238c5ecb4541a9d41573
# Sat, 24 Jun 2023 03:39:01 GMT
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
	-	`sha256:f2e4d934aedb3408d39924086e00ca7aaad6ba9093494927ec3193aafd92a20f`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d47816062ca7fccecb96be7bf6468c4f36ffddd3115cf4d9bf244c0379bf7c`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520b4152b36536d9d6e0fbb761f4d738b989c5b9bc20fdcb54002f3531479b5`  
		Last Modified: Sat, 24 Jun 2023 03:42:18 GMT  
		Size: 17.3 MB (17325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29907b163c6b32e00b8763615b85445316f0e6cb7cd8c84e9e27ef2d3f409a1e`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99329c21e6a062ffac537c99b986885a8362333c37717e126cb5d88df72bfca3`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ff267e35546ccc351184e91eb2272e461f812168c1c315fbc2ff57b7408600`  
		Last Modified: Sat, 24 Jun 2023 03:42:13 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6b99421718086797da2255cb6dc64b1c37da7f21897b880a0e613168d72ce5`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 17.9 MB (17867625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f4f8b85ea5f0a192f6838a9fbe5139aeeac0e942c8475f0a789a9274337235`  
		Last Modified: Sat, 24 Jun 2023 03:42:11 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e63abb1db27e786770d475189d923ac32c1bba9100eb67a5b68340995b2faa`  
		Last Modified: Sat, 24 Jun 2023 03:42:12 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a172a44e616a48aa8515eb471f07b99888430712c993310ab750ba38436e2b`  
		Last Modified: Sat, 24 Jun 2023 03:42:11 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a065bfec53c63fa47ee3b2a98128c40bbc9bd1e6c64e76012052291dfd6035`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 18.4 MB (18434918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
