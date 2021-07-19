## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:d0d85cb5d8e57f4e69f2790366107adf97d1a5c3ce3ecd29e0551e75aa5c1d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `mongo:4-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull mongo@sha256:73dc6490e1159b56631bbcbd87e5cade415596dc75c26186860761cdb0ceab2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2917542756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:141ddeabfa1a67fbb2d1288f34c109ab738b9694e48f9933581127f8c1271d1a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 19 Jul 2021 17:45:01 GMT
ENV MONGO_VERSION=4.4.7
# Mon, 19 Jul 2021 17:45:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.7-signed.msi
# Mon, 19 Jul 2021 17:45:06 GMT
ENV MONGO_DOWNLOAD_SHA256=262b28c79ea8305b28be3257e3f548344998bf18891a79d8780ef2e94d70ed86
# Mon, 19 Jul 2021 17:47:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 19 Jul 2021 17:47:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 19 Jul 2021 17:47:37 GMT
EXPOSE 27017
# Mon, 19 Jul 2021 17:47:40 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91850929c78b0f578c0d6c03055dcd053dbdac894c9352bb24237c3bc806b99f`  
		Last Modified: Mon, 19 Jul 2021 18:01:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14086839fe18f943601d33b6bc77b9a91e8a9ce99d362e42b500fa3b6abd7473`  
		Last Modified: Mon, 19 Jul 2021 18:01:49 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a1324649b1f16974dd08400b73d905e77f552e9dc42cfa4d79602d7cf73e29`  
		Last Modified: Mon, 19 Jul 2021 18:01:47 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e486000e33ae22d5f25b29e6af68bac2083f21eadf60d4a95d96c1a141336f1`  
		Last Modified: Mon, 19 Jul 2021 18:02:30 GMT  
		Size: 232.1 MB (232086004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212afd44250877cdf84feaee203c30aa3b2bc5d938812d9ec61eac910889926`  
		Last Modified: Mon, 19 Jul 2021 18:01:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e647e0132d69a9cafdf88062c0014c70fe1c5d5d5f7e9768753438177d825a`  
		Last Modified: Mon, 19 Jul 2021 18:01:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb721b6ca7aaf71bf55d365d188932fdf9ae523defb3d7d551741bdc2fa2fa15`  
		Last Modified: Mon, 19 Jul 2021 18:01:46 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull mongo@sha256:7003bc9d5f83ca4830c9f76ddaba9e7cd18e3e43c01dfecc16c69037e0456863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6506097426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b101544771c0d5d17706d2de831361e5b2216bbf594ea8175ea5552e4824fa`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 19 Jul 2021 17:47:57 GMT
ENV MONGO_VERSION=4.4.7
# Mon, 19 Jul 2021 17:47:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.7-signed.msi
# Mon, 19 Jul 2021 17:48:01 GMT
ENV MONGO_DOWNLOAD_SHA256=262b28c79ea8305b28be3257e3f548344998bf18891a79d8780ef2e94d70ed86
# Mon, 19 Jul 2021 17:51:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 19 Jul 2021 17:51:04 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 19 Jul 2021 17:51:07 GMT
EXPOSE 27017
# Mon, 19 Jul 2021 17:51:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3120d909334509a18785b9a1f7abebe68511ea5306b1a3df16223b5ae80a5a9b`  
		Last Modified: Mon, 19 Jul 2021 18:02:45 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b266fbd3db8de1d39672143c95a57045a1ffc83c7d5ad86b1f617e7ba049859f`  
		Last Modified: Mon, 19 Jul 2021 18:02:46 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a77ec0351892f4b24d6ee0b5ccf7c19f99eb8f13d9021cb9fc13b6282e3d46`  
		Last Modified: Mon, 19 Jul 2021 18:02:43 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83df8c19df50deec76d3b1ed482890c5e371a6d9d72c27ac57207ce84a39a289`  
		Last Modified: Mon, 19 Jul 2021 18:07:41 GMT  
		Size: 236.5 MB (236455383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6272a039a4579ac10f9642870bc3c5643daba3f2a2c1258c892a30bf423c601a`  
		Last Modified: Mon, 19 Jul 2021 18:02:43 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaad5096a6126abea8eb37f1b68107690cbf2c49beb108d01c873b124ec61aeb`  
		Last Modified: Mon, 19 Jul 2021 18:02:43 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39ceb10c618f6e040bb9857521166831179cb815599104e9e72834aa1ed3208`  
		Last Modified: Mon, 19 Jul 2021 18:02:43 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
