## `mongo:5-windowsservercore-1809`

```console
$ docker pull mongo@sha256:37a3009ed11d00e8ecc7b2f362abc45de1b058e91d2036651df1d81c8bc9d341
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `mongo:5-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull mongo@sha256:165e709c03cfdb45f3718ce2f0907c3e855000bdfb79831c256159e00b9e3472
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2373699371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:607edbde0c82838e8ee50c4cc680da489100f041af759e5e9e6f8c4aaf6d3410`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Wed, 13 Dec 2023 00:58:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2023 01:14:37 GMT
ENV MONGO_VERSION=5.0.23
# Wed, 13 Dec 2023 01:14:38 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.23-signed.msi
# Wed, 13 Dec 2023 01:14:38 GMT
ENV MONGO_DOWNLOAD_SHA256=458663972f8c528dcd249e6ef21ce77aac3301a14214089b2099283b2135da37
# Wed, 13 Dec 2023 01:16:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2023 01:16:38 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2023 01:16:39 GMT
EXPOSE 27017
# Wed, 13 Dec 2023 01:16:40 GMT
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
	-	`sha256:28f0d53703b5095bc9c6a153de2045169796199d29ca463f6ac4d5fde67bb726`  
		Last Modified: Wed, 13 Dec 2023 01:43:41 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7225a55688c80e822e38b572433601a19322439a7ecfe40fa37d3fea54ea339a`  
		Last Modified: Wed, 13 Dec 2023 01:43:41 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7b0caf74fcc73d1d4f45c0fd6a002089a5d2eeb7b28d5d50a1fc19d49afbb9`  
		Last Modified: Wed, 13 Dec 2023 01:43:39 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868645c86d1d33b28d51c496bfd9c194e13bf061a8e087cc826dafd704adaf22`  
		Last Modified: Wed, 13 Dec 2023 01:44:32 GMT  
		Size: 314.0 MB (313981041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ecf1ee5ef5ff4e3e22309482be648e3f55a179951d83bfb48663a975c45912`  
		Last Modified: Wed, 13 Dec 2023 01:43:40 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24b852de0bcba20480789380be93a1804cd23710dade55708ec3e2321abd0dd`  
		Last Modified: Wed, 13 Dec 2023 01:43:39 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9dbc468efb3ccb495578850e7d3715b324ed64b6d8be3ab45b38e85ee54d69`  
		Last Modified: Wed, 13 Dec 2023 01:43:39 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
