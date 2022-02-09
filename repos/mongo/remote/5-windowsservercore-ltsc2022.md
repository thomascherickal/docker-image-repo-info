## `mongo:5-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:60c09f65cee189db8fffb14c0243cf5996b1a18d375450645ad4167dd5c27437
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.524; amd64

### `mongo:5-windowsservercore-ltsc2022` - windows version 10.0.20348.524; amd64

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
