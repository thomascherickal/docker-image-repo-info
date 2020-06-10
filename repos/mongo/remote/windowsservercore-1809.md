## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:a2557c1e77031161eb1a8e02a1272ee02834e1b13a4fac614015f1d8e363df01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:425ecf5dd6f35766a92f49ecb2ca4411ea6976534a07155ac9edef481e725aec
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752061282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ed7dd4d09745f84d50a5aa670fedb6c133809bdf70e31ca312a2949ac1fd21`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 19:32:44 GMT
ENV MONGO_VERSION=4.2.7
# Wed, 10 Jun 2020 19:32:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.7-signed.msi
# Wed, 10 Jun 2020 19:32:45 GMT
ENV MONGO_DOWNLOAD_SHA256=d085db55ea34452617e73a5d7ad80fbc4b9eaf75990e49080a7c3ced13fbb42c
# Wed, 10 Jun 2020 19:51:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 19:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 19:51:59 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 19:52:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf06d0ea6b59b7ed927cfc2d1015230e9e95bda7bfc80f297878880b126162f4`  
		Last Modified: Wed, 10 Jun 2020 20:30:08 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4730881db54360d7cd92c5af46fb536dfff33659c5d6d69bd8db3c71a2844f32`  
		Last Modified: Wed, 10 Jun 2020 20:30:08 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7070782e951460b20909be58236b6757425812caba69bb700708ccaab90f3b5b`  
		Last Modified: Wed, 10 Jun 2020 20:30:05 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a5f955fe6870efc8b0bb32dec11b13d4031de342cd63852174bf47dfb5088f`  
		Last Modified: Wed, 10 Jun 2020 20:38:15 GMT  
		Size: 458.1 MB (458139029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a023862b17e1578235588291fb7ccc64c972f970a06f7c32cbd9a1f385b27ea`  
		Last Modified: Wed, 10 Jun 2020 20:30:05 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc99a6b2c7c66bfa89c6e33309fc65283b7a034316c3d5371f30e81688bea067`  
		Last Modified: Wed, 10 Jun 2020 20:30:05 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3101ed2271ecfed7b4a66770e3490b7c15bdaa8a3d54b067e0c64fb651915a`  
		Last Modified: Wed, 10 Jun 2020 20:30:06 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
