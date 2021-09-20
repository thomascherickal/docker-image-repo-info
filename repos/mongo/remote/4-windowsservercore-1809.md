## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:6ecb0a0bde026a7525ce6c93d9f40525cfe9f3da598cc727097914bf4f61308c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull mongo@sha256:d620a4ecf9f242ef42e9c7ddfd4f7aad8cb231bceb75f8dbcca1a776eba47e2a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2919081688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5633770451f2fb83dd8e89c1baaa82be0459e2731f6c27535fbcd1d2d2006b39`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 20 Sep 2021 22:19:51 GMT
ENV MONGO_VERSION=4.4.9
# Mon, 20 Sep 2021 22:19:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.9-signed.msi
# Mon, 20 Sep 2021 22:19:53 GMT
ENV MONGO_DOWNLOAD_SHA256=aa2eef8fbf94a91428da1ec9cd61acd7e44612e2ae35ae616aefe0a8f93cf282
# Mon, 20 Sep 2021 22:21:48 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 20 Sep 2021 22:21:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 20 Sep 2021 22:21:51 GMT
EXPOSE 27017
# Mon, 20 Sep 2021 22:21:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31cef213761bff76f1a4027487e4185b67a5fa3a8ff854b598a867c6a9b3364b`  
		Last Modified: Mon, 20 Sep 2021 22:44:18 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933f061d3eceb83250199275c5110be2b6bb250a672607f17a740a2a10abd3ab`  
		Last Modified: Mon, 20 Sep 2021 22:44:19 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1b4304e935f5186a12bcda1e26c2c76fb604ffc8e479abff2a6449a8e5e416`  
		Last Modified: Mon, 20 Sep 2021 22:44:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d6da60c8f475ee54a180f018be40246941a32b994119a55dbbe2e710d54829`  
		Last Modified: Mon, 20 Sep 2021 22:44:55 GMT  
		Size: 232.4 MB (232373997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e426f185114d43faa0e436af16b6414184a531b9887075e0f1469de82332b326`  
		Last Modified: Mon, 20 Sep 2021 22:44:16 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0837a2663efd6de58c9d565d10fe060667fc3abc4e605dd25ea13cad46440892`  
		Last Modified: Mon, 20 Sep 2021 22:44:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e811d4ecf9e736b78b78bcd5c184fddb4c52f72ac302d825b4709b2d1713c8`  
		Last Modified: Mon, 20 Sep 2021 22:44:16 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
