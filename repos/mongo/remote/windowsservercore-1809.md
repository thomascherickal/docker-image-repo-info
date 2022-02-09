## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:9d0792c73fd68c0bcbf23c28251716684050a9a4503b104165b15d6134500df8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull mongo@sha256:fe6606626eff67e03aae4ff876e0aa01c6fe632da83c3459a1b8c322de6d184b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (3017197463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6897ba10a4e96c672a21cc22a603a0f4ae5f0d6c090bf37dbffd58925ad87d48`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 16:55:15 GMT
ENV MONGO_VERSION=5.0.6
# Wed, 09 Feb 2022 16:55:16 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.6-signed.msi
# Wed, 09 Feb 2022 16:55:17 GMT
ENV MONGO_DOWNLOAD_SHA256=f6e2bc600b2b8b0251a9e99d84fefc43c66e45deb5793ed8e65cd12a318c76ee
# Wed, 09 Feb 2022 16:58:12 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Feb 2022 16:58:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Feb 2022 16:58:16 GMT
EXPOSE 27017
# Wed, 09 Feb 2022 16:58:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c519ba05cc7100838acc148104c8a33bfaec5446aa2c9a10f16d6e85b11ea7fd`  
		Last Modified: Wed, 09 Feb 2022 17:37:16 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe36d1564a90d3a9bdcb5577f8f9ab60a3160122f6a73862cd76fa69c7a2d`  
		Last Modified: Wed, 09 Feb 2022 17:37:16 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360e0458d5c65d58709df9d76da6ddae568e3f109612eadbdc5b26baaa5372b5`  
		Last Modified: Wed, 09 Feb 2022 17:37:13 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b225fde6eacdc36e0ec64d139536923a38be57b7a5acca7352ccf61a5dfc52`  
		Last Modified: Wed, 09 Feb 2022 17:38:07 GMT  
		Size: 303.5 MB (303472777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9f467c6a2d07347e18eacb36da020e1392114dc0ba7fafa64ac0372812e4fe`  
		Last Modified: Wed, 09 Feb 2022 17:37:13 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142de3b921be3ef8da67ccdeda6db94ff58916785a9d4eed8a55c768b1e51c49`  
		Last Modified: Wed, 09 Feb 2022 17:37:13 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03ee4171601008010af5ae4b655173c7e1e2c5554f540be43c1d73044f44cec`  
		Last Modified: Wed, 09 Feb 2022 17:37:13 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
