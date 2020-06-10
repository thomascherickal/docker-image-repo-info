## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:168f93ffc37589489ff16a458b124925235e7342353261bbac8aaacf84e9cff3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull mongo@sha256:92da2a1d4772d0b93fc197b68d6598b900d911a2084e0c2eda1b6ec816e6c0a2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386924383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a90a68509d82192dc4f3cd1515d0842e50b5b7b604bcd15c45aca2a662980f6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:26:07 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:26:08 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:40:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:40:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:40:03 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:40:04 GMT
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
	-	`sha256:637403b20232ba07d564c2a0530b1f5b8513e13afeae1720fa945dca7a4345ce`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ddb1043b8b11997a958386f728fdd820942a38c9d43e325e22d43e7a1c209`  
		Last Modified: Wed, 10 Jun 2020 20:26:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ae9516d42c6b1c8190c4da03bc21fd92905429da8fe9c022512026413d0865`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a450568155c9a15f52f40f17ae307bb34726b6eb47ff8c1fa2a16b6a4f040`  
		Last Modified: Wed, 10 Jun 2020 20:26:57 GMT  
		Size: 93.0 MB (93002199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bb5eaf61d4fa06f97b072f70d10cf84b1ba68111389e690c2d6c39bc26ddc5`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd32776d415229410f3e7acd3749e28a532e0f5f03553a9d93021571253e3934`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333cf051585d01194811d9da3d43c32f4b55307ce87de32482f391f6158037b`  
		Last Modified: Wed, 10 Jun 2020 20:26:35 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
