## `mongo:5-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:100d6776e64f0b48090f4097c9c0472f20bacd30dd7c88e92b2eb4335dbcaa09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `mongo:5-windowsservercore-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull mongo@sha256:2ac80ff59a21111afb8ff427ff788d5c85971dcfdd7f8056be24a0da9de37fa8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051064442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff9fec9cf058ddaaa9936eda8263ec2e92381f08d593259f0d9c151dce018d1e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 22:35:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 13 Jul 2023 23:05:36 GMT
ENV MONGO_VERSION=5.0.18
# Thu, 13 Jul 2023 23:05:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.18-signed.msi
# Thu, 13 Jul 2023 23:05:37 GMT
ENV MONGO_DOWNLOAD_SHA256=369e0cdc34c29290bfcc9d47569e1debad1b86010ea5e00aefd7c670717f434b
# Thu, 13 Jul 2023 23:07:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 13 Jul 2023 23:07:04 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 23:07:06 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 23:07:07 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2bae42a1ce047820c1f128e4587a430377ba56a110db0d98ec3ccfbd3de58a`  
		Last Modified: Thu, 13 Jul 2023 23:23:36 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a1324b166cada5486ffb8d0e180702f306c5c84aeba89efd2d8e08477ad60e`  
		Last Modified: Thu, 13 Jul 2023 23:46:42 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fabb22ebc047f61ac53e6159158353d3728d6c5598afa1c257a737f7e67815`  
		Last Modified: Thu, 13 Jul 2023 23:46:42 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60ee7bd840be2c9b75f7372e15751ad19e9c5f28799cd585b2a0d2977206242`  
		Last Modified: Thu, 13 Jul 2023 23:46:40 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185b8e802ba2fac0c3463ab0f29e7bbcc10bd25854256cbe7ba60812f7db5d98`  
		Last Modified: Thu, 13 Jul 2023 23:47:37 GMT  
		Size: 313.7 MB (313689265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28cd689919465624b85ee5a17540c986e4f9dd27f6e1252e5d2ac92039d90a4`  
		Last Modified: Thu, 13 Jul 2023 23:46:40 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9b7685857978f4269b3ccfccaba97bb07af314b4f2c0bd6140593d068e99b`  
		Last Modified: Thu, 13 Jul 2023 23:46:40 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259413b5bac24d7ddfefb0ae5d6a025444d5264ecb336b3777d4dc98b08c6aab`  
		Last Modified: Thu, 13 Jul 2023 23:46:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
