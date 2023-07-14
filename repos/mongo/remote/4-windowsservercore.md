## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:336b6390a7fc7521df6bb18731f80d0c9fb003d41dcc26f13eea1fc99cfd8451
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `mongo:4-windowsservercore` - windows version 10.0.20348.1850; amd64

```console
$ docker pull mongo@sha256:23da57faba03e449c43f63181a435fabab88441e5ce619f14356995087cb996a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983568809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68fbd991c3d4c98a47d25bea05e357157fbcca75f65ef257a475a8b228779f37`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 22:35:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 13 Jul 2023 23:16:38 GMT
ENV MONGO_VERSION=4.4.22
# Thu, 13 Jul 2023 23:16:38 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.22-signed.msi
# Thu, 13 Jul 2023 23:16:39 GMT
ENV MONGO_DOWNLOAD_SHA256=95a021db597790008f2e7070fab4a7c3e0d30262f2305c615b95cb7b8afb4eed
# Thu, 13 Jul 2023 23:17:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 13 Jul 2023 23:17:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 23:17:54 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 23:17:55 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2bae42a1ce047820c1f128e4587a430377ba56a110db0d98ec3ccfbd3de58a`  
		Last Modified: Thu, 13 Jul 2023 23:23:36 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d743fd8d430eceb22ffb290bcbb359a2ff61ee787b7a09dc7e252aa3a70883b`  
		Last Modified: Thu, 13 Jul 2023 23:54:40 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a125d5b1ffaccd6f48df3f1b50e2d25e1dd6e8a91d08aa6f1387e19a97791b55`  
		Last Modified: Thu, 13 Jul 2023 23:54:40 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fd80d9d3d3c1c0a6e2ae0a8612bf3ba7702ea2035e825dd861003bc7f6c812`  
		Last Modified: Thu, 13 Jul 2023 23:54:38 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4468a8ac62828122ec8774236a1a5677e5ad9c2a11ea8a609b9016a2e55187`  
		Last Modified: Thu, 13 Jul 2023 23:55:20 GMT  
		Size: 246.2 MB (246193640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c04de418033153cda321b0e195f53487323ca06a3446369354c091d2b8c1a9`  
		Last Modified: Thu, 13 Jul 2023 23:54:38 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897dc6260b17dea7457c43f3bedbcc060d502dd5bbb1d8b834439bdfc6e002aa`  
		Last Modified: Thu, 13 Jul 2023 23:54:38 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87838e31a3689fa3e6ac4ddd70670769a217ebb81110a9908c6f707fc8d963b7`  
		Last Modified: Thu, 13 Jul 2023 23:54:39 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.4645; amd64

```console
$ docker pull mongo@sha256:f8a5b0c41cf1bb52bb62f8c13d3ae54e4932c30d968384d60cb2e254c1278b55
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2185914290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a795115e367a68e714db1282f92cf617af2e8273133d361cf3d09509fd368d2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 22:38:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 13 Jul 2023 23:18:05 GMT
ENV MONGO_VERSION=4.4.22
# Thu, 13 Jul 2023 23:18:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.22-signed.msi
# Thu, 13 Jul 2023 23:18:07 GMT
ENV MONGO_DOWNLOAD_SHA256=95a021db597790008f2e7070fab4a7c3e0d30262f2305c615b95cb7b8afb4eed
# Thu, 13 Jul 2023 23:20:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 13 Jul 2023 23:20:08 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 23:20:09 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 23:20:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b452db6d50a62b6e0e8dadb19715cfcf62cf73e54b5d3bac96621c1093673c`  
		Last Modified: Thu, 13 Jul 2023 23:25:18 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804c87b2d64ef611fb6cfe62be79a8941aa9cac7d2c60ec4a28aa1f2d1d56279`  
		Last Modified: Thu, 13 Jul 2023 23:55:34 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2041b4955b343de2dc24e52d5d8fb625b774e7b8f19039d8408ff87a91cae86`  
		Last Modified: Thu, 13 Jul 2023 23:55:33 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a63da99f9031b22e3294968d56c01eb27b1abe3ba0b65f9a0449ca339effb7`  
		Last Modified: Thu, 13 Jul 2023 23:55:31 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bfc0757f68d428bc76d409d531490672ca729de09e0791bf24f2937111603c`  
		Last Modified: Thu, 13 Jul 2023 23:56:14 GMT  
		Size: 246.2 MB (246215315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5610680044fb8d8f27ac5466fe62eda3a50f246b14b51cab39bb481978758b09`  
		Last Modified: Thu, 13 Jul 2023 23:55:31 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d11e702098e582d478d5623f5070fc430cbf3c63594895b26d085369573a474`  
		Last Modified: Thu, 13 Jul 2023 23:55:31 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eeca32f93b02bd1b5e951034ca4aa989004fe38d78301f7073f3b9b1118660`  
		Last Modified: Thu, 13 Jul 2023 23:55:31 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
