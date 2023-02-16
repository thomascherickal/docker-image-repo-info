## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:b8df44f1eef6d9b70f14030214ec5993321d52d10efa2e6a3b6723d7395e9112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `mongo:4-windowsservercore` - windows version 10.0.20348.1547; amd64

```console
$ docker pull mongo@sha256:18a47804425ba94af89ddc53c9a5ca270d2f1d381c0c7d4df0d2684143b4d79d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1925055076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef8a0bca16981d47591f2ea5ef534d3d9aa408da6d1cdb774d42c233388578b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Thu, 16 Feb 2023 00:38:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Feb 2023 01:10:31 GMT
ENV MONGO_VERSION=4.4.18
# Thu, 16 Feb 2023 01:10:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.18-signed.msi
# Thu, 16 Feb 2023 01:10:33 GMT
ENV MONGO_DOWNLOAD_SHA256=e647d6432ceaf4949bd989e10bad5cd10788f87c41ac2fc054a6e6122503fc64
# Thu, 16 Feb 2023 01:12:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 01:12:42 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Feb 2023 01:12:43 GMT
EXPOSE 27017
# Thu, 16 Feb 2023 01:12:44 GMT
CMD ["mongod" "--bind_ip_all"]
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
	-	`sha256:028996d5eeb6d70e4f35b4acb3bafeee3f326bb40438911de597cad432ffdbc1`  
		Last Modified: Thu, 16 Feb 2023 01:35:55 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78495744982e7f2837f6e73122ec00dce8aadb4da29077bea2323fa043847f67`  
		Last Modified: Thu, 16 Feb 2023 01:50:19 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4a184d7a1031150770242a6b8a27bd2e2602bb00063d6035f86b0a0d0fd54b`  
		Last Modified: Thu, 16 Feb 2023 01:50:19 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74facc7cc6f60480825d820f3171c28e57ed862b9038b792f276c6d30224b0fb`  
		Last Modified: Thu, 16 Feb 2023 01:50:18 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46f64c22cd85f875ecdec566ac0de932443e9cd7227e01e8d5aa3255e52a7f7`  
		Last Modified: Thu, 16 Feb 2023 01:51:02 GMT  
		Size: 245.7 MB (245698894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d435a726a37c8ccc3d47334da397927bb9fa72cc98ef38a8a13d9eea03be18`  
		Last Modified: Thu, 16 Feb 2023 01:50:17 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4f131fb16f346208eafbc22894b692d4580cea3ad5919300d53e35c8f98036`  
		Last Modified: Thu, 16 Feb 2023 01:50:17 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad88b36c7152b9106b35d936a0bf3389a63701ce42ae2d06138ea1f4d7c4ba0a`  
		Last Modified: Thu, 16 Feb 2023 01:50:17 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.4010; amd64

```console
$ docker pull mongo@sha256:e47e8232b4114a83c80add505509cb9e0cd015dd56d91fc2f909733119ca5029
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2208468596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc90165c6207af498065740f4f91fc8d59dc59c58ecadc97c241a3e4dc20e113`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Thu, 16 Feb 2023 00:42:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Feb 2023 01:13:08 GMT
ENV MONGO_VERSION=4.4.18
# Thu, 16 Feb 2023 01:13:09 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.18-signed.msi
# Thu, 16 Feb 2023 01:13:10 GMT
ENV MONGO_DOWNLOAD_SHA256=e647d6432ceaf4949bd989e10bad5cd10788f87c41ac2fc054a6e6122503fc64
# Thu, 16 Feb 2023 01:16:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 01:16:21 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Feb 2023 01:16:22 GMT
EXPOSE 27017
# Thu, 16 Feb 2023 01:16:23 GMT
CMD ["mongod" "--bind_ip_all"]
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
	-	`sha256:531f6c3ad9784fc2870ea5ca08c4adccd9318602ed534d822e12b8b658a7b0b6`  
		Last Modified: Thu, 16 Feb 2023 01:37:30 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd25bf144ead231f1123c024a794d09ee3e763d6f8d3cde07300cc315f39642a`  
		Last Modified: Thu, 16 Feb 2023 01:51:14 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f90a2cfdb78e6c90c5cba7a6056907217db0d732e425783f2d2b4ceb30f85`  
		Last Modified: Thu, 16 Feb 2023 01:51:14 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb01bdba2979f502c9a6000684c679884112f4fe736ea1ad0fdf6a5e87cd1e6`  
		Last Modified: Thu, 16 Feb 2023 01:51:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e19877ed1686424d5af0a8ce10e2e5f77926f0d5522a59e82ea99a0d6147c6`  
		Last Modified: Thu, 16 Feb 2023 01:51:57 GMT  
		Size: 245.5 MB (245500868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29730b869b6b2525cce78162664e5551d3ceacae68cb7f01b412869d82750899`  
		Last Modified: Thu, 16 Feb 2023 01:51:12 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bb095d3bc2bf9449df361cbaf51669aa764a5b50d0ebeceae5463fb9b41198`  
		Last Modified: Thu, 16 Feb 2023 01:51:12 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae61edc11dc5f58cffdd136d973aaadb042ac31cb193b0408ddd3874bb71f50`  
		Last Modified: Thu, 16 Feb 2023 01:51:12 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
