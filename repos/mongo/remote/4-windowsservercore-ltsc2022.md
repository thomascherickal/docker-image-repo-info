## `mongo:4-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:1befed4a3d579a241b6146fceb481ac0a343dc1a14d49e35e440f6eb73619dba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `mongo:4-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull mongo@sha256:dd0cfd7c21bfd7cccec353ed09122187dd372d60ab74329cbdd83bed3eda8295
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480355961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d227483afc3997b1ece7635bbca46fb4b10e58fffe2eb843f58138ccf8deba1f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Wed, 11 May 2022 12:34:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 May 2022 19:24:04 GMT
ENV MONGO_VERSION=4.4.14
# Thu, 12 May 2022 19:24:05 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.14-signed.msi
# Thu, 12 May 2022 19:24:06 GMT
ENV MONGO_DOWNLOAD_SHA256=beb8d11bbf2c02142fe774cac16752281a8f0a61788d684a495337e288c63501
# Thu, 12 May 2022 19:25:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 12 May 2022 19:25:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 12 May 2022 19:25:17 GMT
EXPOSE 27017
# Thu, 12 May 2022 19:25:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:52d280e9bf32da92b07a144022b757d7e39ac8039e166551ad32f8ee416bb55f`  
		Last Modified: Wed, 11 May 2022 14:06:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb54368fac03d9454af55775d3f57143d2c9df228c0cc7528b53bc9923e4da3`  
		Last Modified: Thu, 12 May 2022 19:37:49 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62be87d152a9a28f4012057a6e264a1bae212fa26940fa3bc7b76f0a3be47a59`  
		Last Modified: Thu, 12 May 2022 19:37:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b5b4d5e48d4704baddd234802078315292d74609037031fc1e52d7e253fb51`  
		Last Modified: Thu, 12 May 2022 19:37:47 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a048c3d41cdcc1d8f695ac0bf1782ded0bc37e1082c820ab2043cdfad1e9a`  
		Last Modified: Thu, 12 May 2022 19:38:31 GMT  
		Size: 242.8 MB (242810941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7104d3452314663aba4695a2bd10bed932e361a1713585af36801f216959079c`  
		Last Modified: Thu, 12 May 2022 19:37:47 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5640e7aa966f5e97c51fce500a0d86bc9d2bb0e8f1aaca49ec1ebc97070c723b`  
		Last Modified: Thu, 12 May 2022 19:37:47 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018cd15f7cb70bdb71db5aadaffd13ec8068f2c4189ce1d4b9741ac699eacfd8`  
		Last Modified: Thu, 12 May 2022 19:37:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
