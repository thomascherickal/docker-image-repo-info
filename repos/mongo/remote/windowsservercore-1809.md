## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:c1b2bf4c46f7a3540451e9b11df9dbb6dfab0c373c903a7af221c98235e8c6e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull mongo@sha256:d5390190a0bf43736ec3ce61b79e6b8a3f49501b70705645d93f1c65f75a1383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2671862360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cd1543c5d140de8fda55fda73efd67ccd53690222fcc601d97d4ce4a5cb4536`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Wed, 13 Dec 2023 00:58:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2023 00:58:42 GMT
ENV MONGO_VERSION=7.0.4
# Wed, 13 Dec 2023 00:58:43 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-7.0.4-signed.msi
# Wed, 13 Dec 2023 00:58:44 GMT
ENV MONGO_DOWNLOAD_SHA256=86a9ce6ce62c9b6a3fee8739572419b59040fa25c7e07a4d1ce28894670e2a2b
# Wed, 13 Dec 2023 01:01:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2023 01:01:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2023 01:01:53 GMT
EXPOSE 27017
# Wed, 13 Dec 2023 01:01:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c910cb69fed2b0fb25386cc07fc30cdf9f1d5bbff8a0aec9f12bc1481a910225`  
		Last Modified: Wed, 13 Dec 2023 01:31:59 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40be43b866066c59d275a477ffe6cab86cfee88bb844775c07e675b6764a9900`  
		Last Modified: Wed, 13 Dec 2023 01:31:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcb2d36fa1d7d074cb9a3f21deacc68e5257b98b4e9c73391a3c63555c0a941`  
		Last Modified: Wed, 13 Dec 2023 01:31:59 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f6b4702fd3328398ff2685b0be5740a06ada0e05393651e1e93fec2c3282e0`  
		Last Modified: Wed, 13 Dec 2023 01:31:57 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd25089de2f5ef591e579acd5d86ce4d8654cc14fb6ad8a717f64231a7895a81`  
		Last Modified: Wed, 13 Dec 2023 01:33:18 GMT  
		Size: 612.1 MB (612143496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de65e956cc45649fc07de38f6791dfa1956234dcbd7907c510808ed5dfdcc37f`  
		Last Modified: Wed, 13 Dec 2023 01:31:57 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4351c0bf74fb4bc47f2efb0514c242ce2c6b8f72e5067213cb2e21ab8a35a282`  
		Last Modified: Wed, 13 Dec 2023 01:31:57 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019390280a1a15f1095c5425d3552ad980eb85515f786fb650d09a8b5fa9448f`  
		Last Modified: Wed, 13 Dec 2023 01:31:57 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
