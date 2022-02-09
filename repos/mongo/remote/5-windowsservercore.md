## `mongo:5-windowsservercore`

```console
$ docker pull mongo@sha256:1bb9cf8f33a43f3a9d994ec4a4ec729de6a10cc16afed953a83be0db0eab3cc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.524; amd64
	-	windows version 10.0.17763.2565; amd64

### `mongo:5-windowsservercore` - windows version 10.0.20348.524; amd64

```console
$ docker pull mongo@sha256:2e33c72be9c2dfd405570da7c568ce40b5ff928a348c37dc77d038ed702d3900
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2518632952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4656a0a7e2a7ebb27306e0593af491f1907c749dd6cceb37f825dd042e6221`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Tue, 01 Feb 2022 02:49:40 GMT
RUN Install update ltsc2022-amd64
# Wed, 09 Feb 2022 14:56:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 16:52:33 GMT
ENV MONGO_VERSION=5.0.6
# Wed, 09 Feb 2022 16:52:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.6-signed.msi
# Wed, 09 Feb 2022 16:52:35 GMT
ENV MONGO_DOWNLOAD_SHA256=f6e2bc600b2b8b0251a9e99d84fefc43c66e45deb5793ed8e65cd12a318c76ee
# Wed, 09 Feb 2022 16:54:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Feb 2022 16:54:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Feb 2022 16:54:54 GMT
EXPOSE 27017
# Wed, 09 Feb 2022 16:54:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:898469748ff68223ab87b654b29fb366c1f4f2b7cfad7a37426346ea16db8dfa`  
		Size: 963.2 MB (963225591 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ff78097ae7bacc8d0990c9620bbe5ddc9639d4f309f097c6cdd3cc7a68e56aad`  
		Last Modified: Wed, 09 Feb 2022 16:39:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1720968c024a720137a114fface1f915ba0fd85e0492c4f3def0f09bfe86ed8`  
		Last Modified: Wed, 09 Feb 2022 17:31:41 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb8650848e898ae4b21e6c9ef08a95cb44f793d969d0c53682ea9d5b0d6c232`  
		Last Modified: Wed, 09 Feb 2022 17:31:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2cad2d5bbcf613034086611ba95509bd31a44c30ede6b2e89c18af4a30aac76`  
		Last Modified: Wed, 09 Feb 2022 17:31:38 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608f023e48193be3f253098749dfd4aaab573ce855a4ae54f1e896ec40165278`  
		Last Modified: Wed, 09 Feb 2022 17:36:58 GMT  
		Size: 303.7 MB (303698411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d57e1670d94bfce2a3d7cbc6039f4c3a0656d378b4539814336634aad541d5`  
		Last Modified: Wed, 09 Feb 2022 17:31:38 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ece5446a3ae673f58e817aa5bd340179373c2339627916fdd5cb85d5a22aff`  
		Last Modified: Wed, 09 Feb 2022 17:31:38 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd24f43a8325a63ed3a6f78a304bab36493f5a650df8b8d727999007b5acf40`  
		Last Modified: Wed, 09 Feb 2022 17:31:38 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-windowsservercore` - windows version 10.0.17763.2565; amd64

```console
$ docker pull mongo@sha256:fe6606626eff67e03aae4ff876e0aa01c6fe632da83c3459a1b8c322de6d184b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (3017197463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6897ba10a4e96c672a21cc22a603a0f4ae5f0d6c090bf37dbffd58925ad87d48`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 16:55:15 GMT
ENV MONGO_VERSION=5.0.6
# Wed, 09 Feb 2022 16:55:16 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.6-signed.msi
# Wed, 09 Feb 2022 16:55:17 GMT
ENV MONGO_DOWNLOAD_SHA256=f6e2bc600b2b8b0251a9e99d84fefc43c66e45deb5793ed8e65cd12a318c76ee
# Wed, 09 Feb 2022 16:58:12 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Feb 2022 16:58:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Feb 2022 16:58:16 GMT
EXPOSE 27017
# Wed, 09 Feb 2022 16:58:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c519ba05cc7100838acc148104c8a33bfaec5446aa2c9a10f16d6e85b11ea7fd`  
		Last Modified: Wed, 09 Feb 2022 17:37:16 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe36d1564a90d3a9bdcb5577f8f9ab60a3160122f6a73862cd76fa69c7a2d`  
		Last Modified: Wed, 09 Feb 2022 17:37:16 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360e0458d5c65d58709df9d76da6ddae568e3f109612eadbdc5b26baaa5372b5`  
		Last Modified: Wed, 09 Feb 2022 17:37:13 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b225fde6eacdc36e0ec64d139536923a38be57b7a5acca7352ccf61a5dfc52`  
		Last Modified: Wed, 09 Feb 2022 17:38:07 GMT  
		Size: 303.5 MB (303472777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9f467c6a2d07347e18eacb36da020e1392114dc0ba7fafa64ac0372812e4fe`  
		Last Modified: Wed, 09 Feb 2022 17:37:13 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142de3b921be3ef8da67ccdeda6db94ff58916785a9d4eed8a55c768b1e51c49`  
		Last Modified: Wed, 09 Feb 2022 17:37:13 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03ee4171601008010af5ae4b655173c7e1e2c5554f540be43c1d73044f44cec`  
		Last Modified: Wed, 09 Feb 2022 17:37:13 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
