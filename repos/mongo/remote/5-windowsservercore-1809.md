## `mongo:5-windowsservercore-1809`

```console
$ docker pull mongo@sha256:b4424a1674d60d818a8ce41cf194d0809dac1ceaa4c094731bcc5503614f5daf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `mongo:5-windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull mongo@sha256:fcbf54c5f3a05f7658e17b06b40811704deba1ab525443ebd1b8bcc7bf69620e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3091477531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5469fa7a4c8e889fa10355124b696df6f943071979d339b1b9f89594e49490b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 01:42:55 GMT
ENV MONGO_VERSION=5.0.14
# Wed, 14 Dec 2022 01:42:56 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.14-signed.msi
# Wed, 14 Dec 2022 01:42:57 GMT
ENV MONGO_DOWNLOAD_SHA256=d67e360f14dd4f1516d322d85c9c9aed3ff0bcf5e08b50ea9e60f64ee4817720
# Wed, 14 Dec 2022 01:46:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 14 Dec 2022 01:46:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Dec 2022 01:47:00 GMT
EXPOSE 27017
# Wed, 14 Dec 2022 01:47:02 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c64af9e3f1b8a4046298bcfd1ced73fe6963154bae2f51795b5f8cdbc439229`  
		Last Modified: Wed, 14 Dec 2022 02:22:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f78c8719cdd594545c56c991663d368ff6e643c5a1fa32e6e8a8d574527df43`  
		Last Modified: Wed, 14 Dec 2022 02:22:05 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1259ca867cccccd50c0f053b97edd8fa6af75fe89cf07f6355a06f4fca703b5`  
		Last Modified: Wed, 14 Dec 2022 02:22:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e03e9b10b425985523191edafe1d8b876c056bc183de3ae024b0f1004e5867c`  
		Last Modified: Wed, 14 Dec 2022 02:23:23 GMT  
		Size: 310.8 MB (310770718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc09f8f2453180d82ccfa47d17acaf64f7a8203b1657420903a2697024a28b1f`  
		Last Modified: Wed, 14 Dec 2022 02:22:03 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e254c643edab7b246d7714118fdc1b6c85f0268f7b810a807092d96813b13443`  
		Last Modified: Wed, 14 Dec 2022 02:22:03 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0688e67920112ec4bbf82edc8f260d951314808ab1f967c08e1340c967b507c1`  
		Last Modified: Wed, 14 Dec 2022 02:22:03 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
