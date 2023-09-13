## `mongo:5-windowsservercore`

```console
$ docker pull mongo@sha256:10fa07acc79a9b917969b38329bcf1913190684106f8c5d63d020183cb2214d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1970; amd64
	-	windows version 10.0.17763.4851; amd64

### `mongo:5-windowsservercore` - windows version 10.0.20348.1970; amd64

```console
$ docker pull mongo@sha256:ab4170aedb46b84d838861816da8c26ebf7d8a485d62e059696f139b6988d92f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2150776930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8793120d28c01817f298de81c2a65900080cd25d37770a61774ffd4032b02f72`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 03:53:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 04:22:57 GMT
ENV MONGO_VERSION=5.0.20
# Wed, 13 Sep 2023 04:22:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.20-signed.msi
# Wed, 13 Sep 2023 04:22:58 GMT
ENV MONGO_DOWNLOAD_SHA256=0d4aab3972b834d3d75a7c0348c4d788418b485633615cebc96d876c4c48c43b
# Wed, 13 Sep 2023 04:24:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 04:24:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Sep 2023 04:24:20 GMT
EXPOSE 27017
# Wed, 13 Sep 2023 04:24:21 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f19fc66ee381d7fb9811b24aea9ed1dff8ef483bc0e019d3c24c09fb8fbecd`  
		Last Modified: Wed, 13 Sep 2023 04:35:02 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d4f917ab010d7955ce43a8312a6eadb03f070326017eaa7dbd7487bce1da9`  
		Last Modified: Wed, 13 Sep 2023 04:56:16 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c70002fe3ce8f92916db7d98022bac5cfbf6fae9fc1f461dd4911d8bad22129`  
		Last Modified: Wed, 13 Sep 2023 04:56:16 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10673a136e47e72daa9b073a59fc823413450d767ad3ca2e79e9c4805a8ca91`  
		Last Modified: Wed, 13 Sep 2023 04:56:14 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831b85e64ed0c0c5a0ac4f1c9afaf59714e2e88c0d0a6f34d2b3e48b9b3aff45`  
		Last Modified: Wed, 13 Sep 2023 04:57:05 GMT  
		Size: 313.5 MB (313493480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dacea95c665b4120c57e64e67546ada1b6ac6e8102b7da05af16a5f3d56c84fd`  
		Last Modified: Wed, 13 Sep 2023 04:56:14 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f73158e377197421a11b0b519d6c84bc11817de66f4f4e4f0b0ede80c99c30`  
		Last Modified: Wed, 13 Sep 2023 04:56:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9e37443a16b2e9977c0ee4b83d3d91964c8ceabd6f42df511ce93671dfc175`  
		Last Modified: Wed, 13 Sep 2023 04:56:14 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull mongo@sha256:04040eff9b2b5e00ba8f12eb24cd2148f9517cb38fd3cc2676da1ab378b06286
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2329857390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b42558a7305d6ef07f927c78b7a36e1f82e4db640d8261f3dd4126a1b3067ed5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 04:24:40 GMT
ENV MONGO_VERSION=5.0.20
# Wed, 13 Sep 2023 04:24:41 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.20-signed.msi
# Wed, 13 Sep 2023 04:24:41 GMT
ENV MONGO_DOWNLOAD_SHA256=0d4aab3972b834d3d75a7c0348c4d788418b485633615cebc96d876c4c48c43b
# Wed, 13 Sep 2023 04:26:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 04:26:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Sep 2023 04:26:40 GMT
EXPOSE 27017
# Wed, 13 Sep 2023 04:26:41 GMT
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
	-	`sha256:99f4701a95882ca9ed303a53a2e1a8808bd813c43fddd3307d8cdda9b38c4411`  
		Last Modified: Wed, 13 Sep 2023 04:57:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539a05ea266189ed64b7e611617a7d2aa58d9dbd6450d15b1947161f0100aa17`  
		Last Modified: Wed, 13 Sep 2023 04:57:19 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa5f51d1c1310ba77d3686286e26c0311c0d1916f7025ea6c5de59edab0d82`  
		Last Modified: Wed, 13 Sep 2023 04:57:17 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d067f6b976e653216c565c61a32eb4ad43238151e61babf14287e4a91fa26`  
		Last Modified: Wed, 13 Sep 2023 04:58:07 GMT  
		Size: 313.5 MB (313517904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067d5a7f27c48777378d57400e2a31224282620c660181e53c720195d0971b3a`  
		Last Modified: Wed, 13 Sep 2023 04:57:17 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee84ed91b2e50244d0b52500d3b77441134495baf17bcd51bb15fcf77e15eac9`  
		Last Modified: Wed, 13 Sep 2023 04:57:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15832c7f04cbc6c16ea9316216f72cb0556b742c8e867bc7e785f337373aa200`  
		Last Modified: Wed, 13 Sep 2023 04:57:17 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
