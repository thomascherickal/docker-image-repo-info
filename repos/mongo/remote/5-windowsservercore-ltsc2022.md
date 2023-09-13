## `mongo:5-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:0e55750211c8834c4796ec718d3766ff01b67c896beee34ded84e7da1cb5bb5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `mongo:5-windowsservercore-ltsc2022` - windows version 10.0.20348.1970; amd64

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
