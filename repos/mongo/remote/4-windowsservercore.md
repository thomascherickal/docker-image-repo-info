## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:d92aab026d49032525faa7dbd53e4adea2c6e82fbc283a75f79d9dbc7a7018af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.825; amd64
	-	windows version 10.0.17763.3165; amd64

### `mongo:4-windowsservercore` - windows version 10.0.20348.825; amd64

```console
$ docker pull mongo@sha256:1ded5ed093f4723f51e0ce6efb7515979363a3757d0bdfabe3a165310200d5d8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2543670609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a53610586989bd3bd39d588d12f0a744f1f7ed2b58c8a41cf43c86f0514e477`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Wed, 13 Jul 2022 12:42:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 16:31:11 GMT
ENV MONGO_VERSION=4.4.15
# Wed, 13 Jul 2022 16:31:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.15-signed.msi
# Wed, 13 Jul 2022 16:31:13 GMT
ENV MONGO_DOWNLOAD_SHA256=cac59647e791ef572d2706c82ed3d5e8fdb2c93e0680a3d18a8a831e7ee35a36
# Wed, 13 Jul 2022 16:32:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Jul 2022 16:32:29 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Jul 2022 16:32:30 GMT
EXPOSE 27017
# Wed, 13 Jul 2022 16:32:31 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a596a8bd7e59e41c674f92ccf4bda0ac985c9143ed67987de02e069f2fbf87de`  
		Last Modified: Wed, 13 Jul 2022 14:16:39 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3e930fc7d0c4cc33528de8211fe7d5d3b600ff1342019c4b502297f3937c4e`  
		Last Modified: Wed, 13 Jul 2022 16:55:14 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476640975d1a3232cb9fffa202af71c4d117d349b24b62250f23c0b23bb17a8d`  
		Last Modified: Wed, 13 Jul 2022 16:55:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f09c95f7e605bdbae54e1f7b20c804387f2b69ff5c1efcd75424c36a8b3d70`  
		Last Modified: Wed, 13 Jul 2022 16:55:12 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34289804cb85d38152dbeb4f6ca704c0fe1c864ff326535d7732f69d8c177c8b`  
		Last Modified: Wed, 13 Jul 2022 16:55:54 GMT  
		Size: 243.4 MB (243429107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6ace596f62f8a24f3dc8bf0341bb62e55caf263d10df8389e6f17ff699869`  
		Last Modified: Wed, 13 Jul 2022 16:55:11 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a579c53898d9a00864ffdc06aeebd7fd2bbc2cca1f7ac514602eec3b4915118`  
		Last Modified: Wed, 13 Jul 2022 16:55:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24e2d38a5793a5e98900d3fd2d1198b75c58211797b046afc59abcce21f67f`  
		Last Modified: Wed, 13 Jul 2022 16:55:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.3165; amd64

```console
$ docker pull mongo@sha256:c94c2dc58f18959aae1292805adce411d65bb332e2c2f77c3fe1e131a00cda80
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2915215737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae65d969d356c7c6a994671e8164e267dae2c7f44f54984f4c30f84a48b3aa5d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 16:32:38 GMT
ENV MONGO_VERSION=4.4.15
# Wed, 13 Jul 2022 16:32:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.15-signed.msi
# Wed, 13 Jul 2022 16:32:40 GMT
ENV MONGO_DOWNLOAD_SHA256=cac59647e791ef572d2706c82ed3d5e8fdb2c93e0680a3d18a8a831e7ee35a36
# Wed, 13 Jul 2022 16:34:48 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Jul 2022 16:34:49 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Jul 2022 16:34:50 GMT
EXPOSE 27017
# Wed, 13 Jul 2022 16:34:51 GMT
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
	-	`sha256:ddb19f70690ca3a7e2bd5bfd8226b0bc4a06c8b4fa09a66aa6285e72124a1166`  
		Last Modified: Wed, 13 Jul 2022 16:56:10 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf776110eb467f0627ae7ca1bed00d0fbe4a541816e15f3ac69a0e0658f8e515`  
		Last Modified: Wed, 13 Jul 2022 16:56:10 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65659b8a3ba5bcbbd84ab7660001efb52dacc544292dd94e45ee5525bc9d4673`  
		Last Modified: Wed, 13 Jul 2022 16:56:08 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa860208369136a991b5c9f88b46b8b9908b0d8cdebaea4dc1015d9b7844d`  
		Last Modified: Wed, 13 Jul 2022 16:56:49 GMT  
		Size: 243.2 MB (243162152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcb2e52d179b7c9068d930b7ab52d77fc14c7e0f164b3a4622aef66a4acc3ae`  
		Last Modified: Wed, 13 Jul 2022 16:56:07 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee36f0273b36718ffa7bc84870cb1e2e79e815679d0490537fc7f9591530971`  
		Last Modified: Wed, 13 Jul 2022 16:56:07 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c841a61362bf21ed716b11f738b5acab2e9eb8abd76041163e4869d42f28d54`  
		Last Modified: Wed, 13 Jul 2022 16:56:08 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
