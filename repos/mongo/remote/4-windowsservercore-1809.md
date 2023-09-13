## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:e9ed35195ad4b931cff92687aa096c66672ebc3988fae4fad4a6c76f6317facd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull mongo@sha256:24f62a70fc98db78a80e60da0aa7970f4f06ac291864efb8e6fcec2f73665a20
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2262562680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:237d811e2bf4c7b25c60ce4123ffa6d2d1df29f3434a9bd1e5e97bae13bdd669`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 04:29:59 GMT
ENV MONGO_VERSION=4.4.24
# Wed, 13 Sep 2023 04:30:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.24-signed.msi
# Wed, 13 Sep 2023 04:30:01 GMT
ENV MONGO_DOWNLOAD_SHA256=9f9b32cb6e34d2fa0e2843526c7192eac5a07b28f1300455aeb988e33bf9a714
# Wed, 13 Sep 2023 04:31:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 04:31:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Sep 2023 04:31:57 GMT
EXPOSE 27017
# Wed, 13 Sep 2023 04:31:57 GMT
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
	-	`sha256:74b771d55fd09c440ca07736b35d8c4064b4ea4e9f574e921798a9ca4d068e57`  
		Last Modified: Wed, 13 Sep 2023 05:01:18 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fef83e53851f2fd958791d7328a1ef438dd97a585b39c12bc9527109295e649`  
		Last Modified: Wed, 13 Sep 2023 05:01:18 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb82ec6dd8d985ee4c9daf1b2b7f9015b78aea876a385a3b7895c2ac539f136`  
		Last Modified: Wed, 13 Sep 2023 05:01:16 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1cee33605918d4728ae68e293ac70be269bf8862cec5e6bc01f4441b86787c`  
		Last Modified: Wed, 13 Sep 2023 05:01:54 GMT  
		Size: 246.2 MB (246222949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040402dea97512d2e5dfee2718a1569988f7758ddf9a308e73ac29fe5040faa1`  
		Last Modified: Wed, 13 Sep 2023 05:01:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1599867c637fc0231842080b16f5969f53a7e3957b1d11c66d10577adf0e45`  
		Last Modified: Wed, 13 Sep 2023 05:01:16 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1194f8c9a8445b1135b1f61f6000f25a8943cf1eeab8b42d02c756c0f028043a`  
		Last Modified: Wed, 13 Sep 2023 05:01:16 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
