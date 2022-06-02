## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:953ce09aa0ed7974eb4ab361ccbd6a032165a4b42f6012e9edcac1ac253bb7ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull mongo@sha256:f5314a98f9b2abf45c5d0e66109dc7d5132f19a0ef707608a14f37fa419c07c7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2811380540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731fd22444d0d651b0bda4a2a858f2d132df3d3dd2c1418cbeff4775ba841b30`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Wed, 11 May 2022 12:42:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 02 Jun 2022 18:29:47 GMT
ENV MONGO_VERSION=5.0.9
# Thu, 02 Jun 2022 18:29:49 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.9-signed.msi
# Thu, 02 Jun 2022 18:29:49 GMT
ENV MONGO_DOWNLOAD_SHA256=0e8032c352253173e9d1683ac7b39c79a4eaed0682e8c0655ca0b3ebd6b11d74
# Thu, 02 Jun 2022 18:31:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 02 Jun 2022 18:31:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 02 Jun 2022 18:31:57 GMT
EXPOSE 27017
# Thu, 02 Jun 2022 18:31:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b34adcbd607b6c175a7c7a819fecbbfd53899678f53f169f2b4504070ec6b0ab`  
		Last Modified: Wed, 11 May 2022 14:07:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25af2be13e0b425b1ab63d2f9bb381390bcfc2596383b2e16713ebf2a1fd30be`  
		Last Modified: Thu, 02 Jun 2022 18:42:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd685396f479c961130078fa61a9b0641d89ecdf9a1de4f4bf7b59b7ea45e2f9`  
		Last Modified: Thu, 02 Jun 2022 18:42:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092e8c3b76716c39e2e0918bcd60337757f72fa9be1e5b4089edb012fedb6934`  
		Last Modified: Thu, 02 Jun 2022 18:42:43 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b5892d41d9f4320bd09865818751271bc1e6cf894c51faf1eb9cb64c12f35f`  
		Last Modified: Thu, 02 Jun 2022 18:48:13 GMT  
		Size: 307.3 MB (307314841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f1dcc78a9ea8b74096eb4e5a145c0a7ad9e8c620f421251aab48f9bc72443e`  
		Last Modified: Thu, 02 Jun 2022 18:42:43 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e56b378fc81a6f3f26351d7a96b07ee8b81eddff5c2b4a245569fbd30ec9dc3`  
		Last Modified: Thu, 02 Jun 2022 18:42:43 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a89ed2188e369be934d0616b7f79ccb18750405d0e822e459bcf048881ecd5`  
		Last Modified: Thu, 02 Jun 2022 18:42:43 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
