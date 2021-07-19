## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:d5314199853bcc02c1334da8996018f0c45fd95b03c9d560f47f2065ff45423b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

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
