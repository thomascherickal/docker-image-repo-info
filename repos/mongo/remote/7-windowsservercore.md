## `mongo:7-windowsservercore`

```console
$ docker pull mongo@sha256:c61436fb16a166f75e2a40a93266ef45686539392b3d2e167eb9f07e35c2b28d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1970; amd64
	-	windows version 10.0.17763.4851; amd64

### `mongo:7-windowsservercore` - windows version 10.0.20348.1970; amd64

```console
$ docker pull mongo@sha256:dc6f698ec71f53c4281831c3c3f36d58a8e4222af3f6475fa43aa8caae6a6e41
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2450041340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d13114064afbb61e5b6ba2ab1332891d07d88250ab1c01f71cd26cd5f9390ba`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 03:53:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 03:53:58 GMT
ENV MONGO_VERSION=7.0.1
# Wed, 13 Sep 2023 03:53:58 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-7.0.1-signed.msi
# Wed, 13 Sep 2023 03:53:59 GMT
ENV MONGO_DOWNLOAD_SHA256=bcdcdc445e53106f6c596304061529c055cda6f23cc06fe8adcc7f7c41c64d99
# Wed, 13 Sep 2023 03:56:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 03:56:20 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Sep 2023 03:56:21 GMT
EXPOSE 27017
# Wed, 13 Sep 2023 03:56:21 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f19fc66ee381d7fb9811b24aea9ed1dff8ef483bc0e019d3c24c09fb8fbecd`  
		Last Modified: Wed, 13 Sep 2023 04:35:02 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0029ad3474e3d7133b3d70f7639476d0fc94ae22ba2fda09467c653ee4636b`  
		Last Modified: Wed, 13 Sep 2023 04:35:02 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a900b49f75a7a7279a5ee8cb0c70202bf65cfeec06cb76fe3e0fee52d2df318`  
		Last Modified: Wed, 13 Sep 2023 04:35:02 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf108ce64c000eca6779d5792da89c7d518f61a4af402122221bee0364ec3d2a`  
		Last Modified: Wed, 13 Sep 2023 04:35:00 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ad51db2978b895017222f859851c377cd9d13382bdbd57258d036314acde21`  
		Last Modified: Wed, 13 Sep 2023 04:36:26 GMT  
		Size: 612.8 MB (612757388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65fcb8ed0c7a40dc12933450886cee77436ca95a98580799980184c629e62fb`  
		Last Modified: Wed, 13 Sep 2023 04:35:00 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bad7e6a670987202a4b0476cacf539f12acede747d85bdf88fffa8dcaa3a506`  
		Last Modified: Wed, 13 Sep 2023 04:35:00 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd300a4d02ae9f89b1f9a0e5530c431d957ded0a87e675b8a6c71a0dc15681`  
		Last Modified: Wed, 13 Sep 2023 04:35:00 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:7-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull mongo@sha256:aa3bea14a403635b210df5381dd1ce7b5a1cc993521beebda3a03634c5ee6609
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2629144057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9beadbd700fd6a9a077eccccedefca451b634ed86ba5b0ad3ab3abca04d52698`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 03:56:42 GMT
ENV MONGO_VERSION=7.0.1
# Wed, 13 Sep 2023 03:56:43 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-7.0.1-signed.msi
# Wed, 13 Sep 2023 03:56:44 GMT
ENV MONGO_DOWNLOAD_SHA256=bcdcdc445e53106f6c596304061529c055cda6f23cc06fe8adcc7f7c41c64d99
# Wed, 13 Sep 2023 04:00:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 04:00:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Sep 2023 04:00:08 GMT
EXPOSE 27017
# Wed, 13 Sep 2023 04:00:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f4a6f2a7858242d9ca188c91efdcfc9ed8d2fe0c65896f57bf2569e07acafd`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccdc772231461649c4cc3125c785b7139a75e7660c54d12028fb4a0c6155c8e`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de315aa6301a93362366a1d06f2583d13fc43b4025601f478c094103cd6de599`  
		Last Modified: Wed, 13 Sep 2023 04:36:43 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3e7d2eb8ea6807138b76053119ef04d9e9aa562080e674f02d74b3e057b277`  
		Last Modified: Wed, 13 Sep 2023 04:38:00 GMT  
		Size: 612.8 MB (612804383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fc5245a35e897b8c60223b51b8e517c5f817380908195aece91aa8bf8f7100`  
		Last Modified: Wed, 13 Sep 2023 04:36:43 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb10459f8c8e98a96b3335074bdb2945cac012a2e43a927c19f2a496ae8451dd`  
		Last Modified: Wed, 13 Sep 2023 04:36:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801fb60f6f0c1ea225dfb7dbc779903f9838162beb4694139e5ee19b32288605`  
		Last Modified: Wed, 13 Sep 2023 04:36:43 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
