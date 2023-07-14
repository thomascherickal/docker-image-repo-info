## `mongo:5-windowsservercore`

```console
$ docker pull mongo@sha256:8e9a01deb5cf37feb5aa822f2f9bced6dcb79227d52153b17af855bfc689f8cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `mongo:5-windowsservercore` - windows version 10.0.20348.1850; amd64

```console
$ docker pull mongo@sha256:2ac80ff59a21111afb8ff427ff788d5c85971dcfdd7f8056be24a0da9de37fa8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051064442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff9fec9cf058ddaaa9936eda8263ec2e92381f08d593259f0d9c151dce018d1e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 22:35:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 13 Jul 2023 23:05:36 GMT
ENV MONGO_VERSION=5.0.18
# Thu, 13 Jul 2023 23:05:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.18-signed.msi
# Thu, 13 Jul 2023 23:05:37 GMT
ENV MONGO_DOWNLOAD_SHA256=369e0cdc34c29290bfcc9d47569e1debad1b86010ea5e00aefd7c670717f434b
# Thu, 13 Jul 2023 23:07:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 13 Jul 2023 23:07:04 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 23:07:06 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 23:07:07 GMT
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
	-	`sha256:36a1324b166cada5486ffb8d0e180702f306c5c84aeba89efd2d8e08477ad60e`  
		Last Modified: Thu, 13 Jul 2023 23:46:42 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fabb22ebc047f61ac53e6159158353d3728d6c5598afa1c257a737f7e67815`  
		Last Modified: Thu, 13 Jul 2023 23:46:42 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60ee7bd840be2c9b75f7372e15751ad19e9c5f28799cd585b2a0d2977206242`  
		Last Modified: Thu, 13 Jul 2023 23:46:40 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185b8e802ba2fac0c3463ab0f29e7bbcc10bd25854256cbe7ba60812f7db5d98`  
		Last Modified: Thu, 13 Jul 2023 23:47:37 GMT  
		Size: 313.7 MB (313689265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28cd689919465624b85ee5a17540c986e4f9dd27f6e1252e5d2ac92039d90a4`  
		Last Modified: Thu, 13 Jul 2023 23:46:40 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9b7685857978f4269b3ccfccaba97bb07af314b4f2c0bd6140593d068e99b`  
		Last Modified: Thu, 13 Jul 2023 23:46:40 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259413b5bac24d7ddfefb0ae5d6a025444d5264ecb336b3777d4dc98b08c6aab`  
		Last Modified: Thu, 13 Jul 2023 23:46:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-windowsservercore` - windows version 10.0.17763.4645; amd64

```console
$ docker pull mongo@sha256:b45227bba4ca0d47f466483be4c28e8bed7767cc4350a7ed0b12c87f1cc6dadb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2253401843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a37b7707dd7f0aab9dd3aa225cacbc4b1c7ebfbda5a5f9f59e0464ab9fd49b6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 22:38:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 13 Jul 2023 23:07:19 GMT
ENV MONGO_VERSION=5.0.18
# Thu, 13 Jul 2023 23:07:20 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.18-signed.msi
# Thu, 13 Jul 2023 23:07:21 GMT
ENV MONGO_DOWNLOAD_SHA256=369e0cdc34c29290bfcc9d47569e1debad1b86010ea5e00aefd7c670717f434b
# Thu, 13 Jul 2023 23:09:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 13 Jul 2023 23:09:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 23:09:40 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 23:09:41 GMT
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
	-	`sha256:7317c184ba272918bfdfc8ab45a2ff974c4d58c5d0610ecb3b77d5e9c549a97d`  
		Last Modified: Thu, 13 Jul 2023 23:47:50 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a7ebc88d1fe46f7669ca5300528f72b083516df6b1f590adda0ad3af0a800c`  
		Last Modified: Thu, 13 Jul 2023 23:47:50 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af64a733c04e996751b31089acbd0ac5ab6750fe569027b255a78771b7934ed`  
		Last Modified: Thu, 13 Jul 2023 23:47:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4277341defd5838dd8a078ccc20cde4ef1077a66c71ae3f395c12d20d0add39`  
		Last Modified: Thu, 13 Jul 2023 23:48:43 GMT  
		Size: 313.7 MB (313702822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e643d307b46f9a7793614ee281fee869be1d9dd401d0c29e0e405220c25333`  
		Last Modified: Thu, 13 Jul 2023 23:47:48 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff13bd47df679d3d7c63edd00d4f84b43925d517d14e3923b3efe988001d3b8d`  
		Last Modified: Thu, 13 Jul 2023 23:47:48 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42834759d71dea94219ca49df438334488bcc8344a930bd3304431c27d226458`  
		Last Modified: Thu, 13 Jul 2023 23:47:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
