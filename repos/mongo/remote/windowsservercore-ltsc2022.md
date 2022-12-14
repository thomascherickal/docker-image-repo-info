## `mongo:windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:f898250b61cd33a23646ab1b83242b5b0f1c0c8f71b53ab6d52e748b273b7df6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1366; amd64

### `mongo:windowsservercore-ltsc2022` - windows version 10.0.20348.1366; amd64

```console
$ docker pull mongo@sha256:a19506653bd46d63ce3824ae2924d6c122e4f659dfa4adf55357003534b36f48
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (3008915450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2c1a12b60661f202b13e3e66c896a5f475209bcbe52f5313593e863fb25ae7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 09 Dec 2022 09:36:47 GMT
RUN Install update 10.0.20348.1366
# Wed, 14 Dec 2022 01:25:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 01:25:55 GMT
ENV MONGO_VERSION=6.0.3
# Wed, 14 Dec 2022 01:25:56 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-6.0.3-signed.msi
# Wed, 14 Dec 2022 01:25:57 GMT
ENV MONGO_DOWNLOAD_SHA256=6557ae0360747d348aefdf30d1360f577804c446579c2012e0b04e5ec2489c49
# Wed, 14 Dec 2022 01:29:24 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 14 Dec 2022 01:29:26 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Dec 2022 01:29:27 GMT
EXPOSE 27017
# Wed, 14 Dec 2022 01:29:28 GMT
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
	-	`sha256:c9159dee34db9650725d16f561f4c4872f13cae60b4f3b1ae02c4287729d1939`  
		Last Modified: Wed, 14 Dec 2022 02:12:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b4cd04942aeb01b53830a5b65f00b43f1eb77012b741eb73a3ca687e83da7c`  
		Last Modified: Wed, 14 Dec 2022 02:12:39 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac86cb7dd79cead605633ede6c5e8737ff6169e6eb5de57ae4157760f41c61e`  
		Last Modified: Wed, 14 Dec 2022 02:12:36 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2321d9a65550355ae68241a144ca700c84c2035b3b8cdfebe259a52649d19dd7`  
		Last Modified: Wed, 14 Dec 2022 02:14:05 GMT  
		Size: 513.2 MB (513242677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99adab971b2f968a2fadaf1a1e4ac68fc4a9a6ab4c537e903377d85acd7d2f8e`  
		Last Modified: Wed, 14 Dec 2022 02:12:36 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861a13ab2f7b6f1d34e86a147f3571059251b92ff3360f914c4a8c480580907a`  
		Last Modified: Wed, 14 Dec 2022 02:12:36 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4d3c10f424434f3e7b4f55a45df2e89c7467b3fdfbf1f5bc5654fa2231e624`  
		Last Modified: Wed, 14 Dec 2022 02:12:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
