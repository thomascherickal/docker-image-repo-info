## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:91b561ad0ebb161ab053796f75c267b493cbec18e4afcd5106e28c0286b4e864
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull mongo@sha256:b535ac763925729c9a50fa413c0fdb040caa9ea746273518617388ec0daebc2e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2979214856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71637d731d3717083b8015c2317354bd6567bdb2b193f2b1a9dfdd8356e4f55d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 16:25:56 GMT
ENV MONGO_VERSION=5.0.9
# Wed, 13 Jul 2022 16:25:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.9-signed.msi
# Wed, 13 Jul 2022 16:25:58 GMT
ENV MONGO_DOWNLOAD_SHA256=0e8032c352253173e9d1683ac7b39c79a4eaed0682e8c0655ca0b3ebd6b11d74
# Wed, 13 Jul 2022 16:28:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Jul 2022 16:28:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Jul 2022 16:28:06 GMT
EXPOSE 27017
# Wed, 13 Jul 2022 16:28:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49b5d162039eae4fe1f7d6cc0d4b3be061cabb5d1d89950262e1b010e7ed67bb`  
		Last Modified: Wed, 13 Jul 2022 14:16:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b17baa80703fd2cfbd6f4e7e10be78a69221d1025e16d1f4375b1dddeacd6b`  
		Last Modified: Wed, 13 Jul 2022 16:51:47 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d13642013f3d708bd3b2261f90748746c0d686189184c510e1b501817e8d660`  
		Last Modified: Wed, 13 Jul 2022 16:51:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e28e740eaac933026f973b42eda3c0daed17e3d7b55c2ea20f52ba3975f594c`  
		Last Modified: Wed, 13 Jul 2022 16:51:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ea0064b332e4f55d50911e55b6d76739dab5cd94abfcaa7a6d56fb6ffe7948`  
		Last Modified: Wed, 13 Jul 2022 16:52:37 GMT  
		Size: 307.2 MB (307161238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3cb00338d9f07b7cfed1e42c8c92ef8f647c44cad043b39ea833e9686997f9`  
		Last Modified: Wed, 13 Jul 2022 16:51:44 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31388ea3f0af124b5f8e7f83ce2f97ba6e78ae978ae13411d099e40b29a010d9`  
		Last Modified: Wed, 13 Jul 2022 16:51:44 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e7b4106f3c99bce7206f76765f990f0b20e72c3c1fcfa6f86b2d22f85e8511`  
		Last Modified: Wed, 13 Jul 2022 16:51:44 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
