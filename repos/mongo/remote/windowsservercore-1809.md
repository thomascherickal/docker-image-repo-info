## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:404b3eae63d02d3c6a2760ed238db20e488cc94b243d25a3a6e8ca3c3b5c5c71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull mongo@sha256:b8a4306a7efd06901a64e98873724be32114052175c8103f3c29cf120822e20b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3092322485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9135c23aa74903f69ddb4bc719f8e797b7cb6c46ca6f96051a0c4506b1b8d855`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 14:18:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 23:17:45 GMT
ENV MONGO_VERSION=4.4.1
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.1-signed.msi
# Wed, 11 Nov 2020 23:17:46 GMT
ENV MONGO_DOWNLOAD_SHA256=acc93c7d8b8c3c8994940bdf2640215a5d3114ca7838be3cfc2d5887e170eaf7
# Wed, 11 Nov 2020 23:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 23:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 23:41:32 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 23:41:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e03cd29396986910a2aaaf968e93bebcaf4b0101821290e0560b401893615ccf`  
		Last Modified: Wed, 11 Nov 2020 16:53:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3782a1fe88b06a9b62d3eb916d4468eb354dacc4e2521319c058b9b43ca43`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a3485eb54bd2655ec1decccd1d37039c1ccc675b140430cf04a45dd9976b1`  
		Last Modified: Thu, 12 Nov 2020 00:37:15 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01d21dd9eba6f79dd8c14fe853a17d4f042da315a2fc11fd14b0baed8c5ae1`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80032f8c0b7a1597680b4d5e81e5e52bdf2a857e799570ba239a1dd4632d28ad`  
		Last Modified: Thu, 12 Nov 2020 00:50:50 GMT  
		Size: 704.3 MB (704285218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae731d2e21a6f2463e2cf0b4cb9b27f934e819512db205f9c9047eb9fa212d`  
		Last Modified: Thu, 12 Nov 2020 00:37:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5c75b9fdf84fa236b47bf0f5f45a095b6c2556af532009f78950d59237f525`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99b6006cd455c86a04f5e9e7ed7c73fb01e1c9eedf5d9bb4297ee2ad9499b94`  
		Last Modified: Thu, 12 Nov 2020 00:37:12 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
