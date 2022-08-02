## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:8e3a01d6a2e23f24345ed5148bff04c9cd966f97bdca46dd0f92a7dc569d49af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.825; amd64
	-	windows version 10.0.17763.3165; amd64

### `mongo:windowsservercore` - windows version 10.0.20348.825; amd64

```console
$ docker pull mongo@sha256:e79f450c86c20a086b9aa1594a7653306f05a35769d789e8bfececb5b662b18d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2608683566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d4b4374ca34f78c69c71c51fc4a741a5328ce3e2bb2fced97cd4e80737c49b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Wed, 13 Jul 2022 12:42:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 02 Aug 2022 01:15:06 GMT
ENV MONGO_VERSION=5.0.10
# Tue, 02 Aug 2022 01:15:07 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.10-signed.msi
# Tue, 02 Aug 2022 01:15:08 GMT
ENV MONGO_DOWNLOAD_SHA256=5feeaf02c6a1a9125565de2e3e44a6c11d920427db31d2ef3b516e2832dcff9b
# Tue, 02 Aug 2022 01:16:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 02 Aug 2022 01:16:38 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 02 Aug 2022 01:16:39 GMT
EXPOSE 27017
# Tue, 02 Aug 2022 01:16:40 GMT
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
	-	`sha256:5297ce4fd6403a2af06d378e8e3e89d60aebd10e2d4cec98fea8e646062628cc`  
		Last Modified: Tue, 02 Aug 2022 01:23:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3495e4c8ca64350d36f43862aef3ec47e05193c467f7555572a09b57cdd3e15c`  
		Last Modified: Tue, 02 Aug 2022 01:23:59 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f84569e8efe2189c6eb5b60fda0ea0b305913e4dca4e04a42579060aec0c11`  
		Last Modified: Tue, 02 Aug 2022 01:23:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d49e80acaf280f76167ab3a9b344ecd90c30ee8f20f790134f7fddb8b2e6430`  
		Last Modified: Tue, 02 Aug 2022 01:24:53 GMT  
		Size: 308.4 MB (308442036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4641064fa25c31c49f540c543b3ed82645ddf5fcc09882e1def8a0ef9f347f01`  
		Last Modified: Tue, 02 Aug 2022 01:23:56 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9882fca01e9478bcef9324a7dcf1831c903a5d0a8e46361a3c8af24ac207d4`  
		Last Modified: Tue, 02 Aug 2022 01:23:56 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5fb1d7173df9bf96adf7e1b5b531251ad43e1607615840621155e3b2288b4`  
		Last Modified: Tue, 02 Aug 2022 01:23:56 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.17763.3165; amd64

```console
$ docker pull mongo@sha256:0082912cb385546910b8827571f4e2b732b09b05a373ba30a70c266f3ab52963
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2980256780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a03623be0394eaaea1a30b713d77e233b1cd3aff0229f56dae6ce90e147842e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 02 Aug 2022 01:16:48 GMT
ENV MONGO_VERSION=5.0.10
# Tue, 02 Aug 2022 01:16:49 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.10-signed.msi
# Tue, 02 Aug 2022 01:16:50 GMT
ENV MONGO_DOWNLOAD_SHA256=5feeaf02c6a1a9125565de2e3e44a6c11d920427db31d2ef3b516e2832dcff9b
# Tue, 02 Aug 2022 01:19:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 02 Aug 2022 01:19:08 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 02 Aug 2022 01:19:09 GMT
EXPOSE 27017
# Tue, 02 Aug 2022 01:19:10 GMT
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
	-	`sha256:855ed7871b298f532b9c6b702991cdcecffa907bc79137e32f3e894636517592`  
		Last Modified: Tue, 02 Aug 2022 01:25:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb1267b278dff66312a977aca2b58335957db7617fa2f3c360bb2a38679a1f9`  
		Last Modified: Tue, 02 Aug 2022 01:25:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b784a9e65f06ead49e1cbf0020a7433f96d2464487cdd9e231cb8377cdac8d60`  
		Last Modified: Tue, 02 Aug 2022 01:25:08 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a2ec4e7a2cb0fb513883b094075430df075560b93e6db5001ab4d325b3ca35`  
		Last Modified: Tue, 02 Aug 2022 01:26:04 GMT  
		Size: 308.2 MB (308203150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cadec584d8b55f0e28fcca575d8ff3befc112699ce69213294cfe076e24e61`  
		Last Modified: Tue, 02 Aug 2022 01:25:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd22a9e11ffd9973dde0a026eaa0e5dd23d67c1d3439fe889238f632f17704d2`  
		Last Modified: Tue, 02 Aug 2022 01:25:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff34e4a3ab8b38354f893f28ccfb9c158276aedded34518b0492b25a408c3c7a`  
		Last Modified: Tue, 02 Aug 2022 01:25:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
