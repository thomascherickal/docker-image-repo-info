## `mongo:5-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:d8d50dee2fb021dafed59578d63d75674a4889e912711ec2f04676c256d9365f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1366; amd64

### `mongo:5-windowsservercore-ltsc2022` - windows version 10.0.20348.1366; amd64

```console
$ docker pull mongo@sha256:836fbad647e65d93679419e46c15df6e15c430f7d2d63a789ae37fcd1b889949
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2806625307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0f98f2a72e45a3306a0e90121d8cfc0531c729dd33884944abb722f85155077`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 09 Dec 2022 09:36:47 GMT
RUN Install update 10.0.20348.1366
# Wed, 14 Dec 2022 01:25:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 01:40:10 GMT
ENV MONGO_VERSION=5.0.14
# Wed, 14 Dec 2022 01:40:11 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.14-signed.msi
# Wed, 14 Dec 2022 01:40:12 GMT
ENV MONGO_DOWNLOAD_SHA256=d67e360f14dd4f1516d322d85c9c9aed3ff0bcf5e08b50ea9e60f64ee4817720
# Wed, 14 Dec 2022 01:42:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 14 Dec 2022 01:42:42 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Dec 2022 01:42:43 GMT
EXPOSE 27017
# Wed, 14 Dec 2022 01:42:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfa20ce142ecceb471dc070d9582fff942cef447b7c8ff22f2223ffe3737c99`  
		Last Modified: Tue, 13 Dec 2022 23:54:14 GMT  
		Size: 1.0 GB (1021665190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8089cb1a16f1eb694714863a5048821ebd084d4fc95740d2ca48fb1089820f`  
		Last Modified: Wed, 14 Dec 2022 02:12:39 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074c43d023e5fc61492e8841751ae876d65850bfe4d29bf4f532c6d122aaefa5`  
		Last Modified: Wed, 14 Dec 2022 02:20:29 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beeeb59692126a9c7717f9b094bd9a9f86c6feb92cdeb05159f727cdfc32086f`  
		Last Modified: Wed, 14 Dec 2022 02:20:29 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841eb37adfc9d3c673ba70d00318503f86ed5aa2b370573d40b699b159a42b67`  
		Last Modified: Wed, 14 Dec 2022 02:20:26 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214cfabe4f2336895f31345f96f001242e381602785be5a0a5c8189fcebbcd48`  
		Last Modified: Wed, 14 Dec 2022 02:21:51 GMT  
		Size: 311.0 MB (310952575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfbb60c15ae525f4ef219f57d83ad6cfabe63ade27a87a4d0a5bfcb46c042a2`  
		Last Modified: Wed, 14 Dec 2022 02:20:26 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b8c3ac2bc35651fd82275db2b049cca26c37d9280d09a6e0b06829f9cc91b`  
		Last Modified: Wed, 14 Dec 2022 02:20:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9555a6a1d79d9a385ed60d8bb29f35c5de8f01e4d2f69464d027a1f37a9f4ef0`  
		Last Modified: Wed, 14 Dec 2022 02:20:26 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
