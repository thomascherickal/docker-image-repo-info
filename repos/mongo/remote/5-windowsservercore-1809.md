## `mongo:5-windowsservercore-1809`

```console
$ docker pull mongo@sha256:4bb1b0546f4fb5130121b32268f514371fb2be17cc0f70bdba01261e31d93f39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `mongo:5-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull mongo@sha256:0082912cb385546910b8827571f4e2b732b09b05a373ba30a70c266f3ab52963
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2980256780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a03623be0394eaaea1a30b713d77e233b1cd3aff0229f56dae6ce90e147842e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 02 Aug 2022 01:16:48 GMT
ENV MONGO_VERSION=5.0.10
# Tue, 02 Aug 2022 01:16:49 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.10-signed.msi
# Tue, 02 Aug 2022 01:16:50 GMT
ENV MONGO_DOWNLOAD_SHA256=5feeaf02c6a1a9125565de2e3e44a6c11d920427db31d2ef3b516e2832dcff9b
# Tue, 02 Aug 2022 01:19:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 02 Aug 2022 01:19:08 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 02 Aug 2022 01:19:09 GMT
EXPOSE 27017
# Tue, 02 Aug 2022 01:19:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49b5d162039eae4fe1f7d6cc0d4b3be061cabb5d1d89950262e1b010e7ed67bb`  
		Last Modified: Wed, 13 Jul 2022 14:16:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855ed7871b298f532b9c6b702991cdcecffa907bc79137e32f3e894636517592`  
		Last Modified: Tue, 02 Aug 2022 01:25:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb1267b278dff66312a977aca2b58335957db7617fa2f3c360bb2a38679a1f9`  
		Last Modified: Tue, 02 Aug 2022 01:25:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b784a9e65f06ead49e1cbf0020a7433f96d2464487cdd9e231cb8377cdac8d60`  
		Last Modified: Tue, 02 Aug 2022 01:25:08 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a2ec4e7a2cb0fb513883b094075430df075560b93e6db5001ab4d325b3ca35`  
		Last Modified: Tue, 02 Aug 2022 01:26:04 GMT  
		Size: 308.2 MB (308203150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cadec584d8b55f0e28fcca575d8ff3befc112699ce69213294cfe076e24e61`  
		Last Modified: Tue, 02 Aug 2022 01:25:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd22a9e11ffd9973dde0a026eaa0e5dd23d67c1d3439fe889238f632f17704d2`  
		Last Modified: Tue, 02 Aug 2022 01:25:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff34e4a3ab8b38354f893f28ccfb9c158276aedded34518b0492b25a408c3c7a`  
		Last Modified: Tue, 02 Aug 2022 01:25:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
