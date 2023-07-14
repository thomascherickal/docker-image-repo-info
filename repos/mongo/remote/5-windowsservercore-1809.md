## `mongo:5-windowsservercore-1809`

```console
$ docker pull mongo@sha256:462fec05054aeb6b686c268dbe025d2242c66488d63d12628b0345a2fc0b3cca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `mongo:5-windowsservercore-1809` - windows version 10.0.17763.4645; amd64

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
