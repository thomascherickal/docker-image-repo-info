## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:bdae2ba436141537c4af7221b03d9c814a9c695a22ae43b8c14c226b13ec2963
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull mongo@sha256:bbd6097c5eb0230e4cc612d5beff810f2e02663f02f796fc8b2619eba343ee97
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6570757584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe13c6537be8fe5fe8046484d19bf0bfc43155c4c64dbf8635efd250f326c8b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 14:32:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 19:11:30 GMT
ENV MONGO_VERSION=5.0.3
# Wed, 10 Nov 2021 19:11:31 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.3-signed.msi
# Wed, 10 Nov 2021 19:11:32 GMT
ENV MONGO_DOWNLOAD_SHA256=ed1cc2eee23f4fb9cc7f70867e29d7c9a1e1af1d9b4aa917d247a4921c4ffd7e
# Wed, 10 Nov 2021 19:13:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 19:13:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Nov 2021 19:13:57 GMT
EXPOSE 27017
# Wed, 10 Nov 2021 19:13:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6f303e73635c7923a8c64f8938e7ba4c10210fd15a6ce63aa8a62d5a8ea8c0a`  
		Last Modified: Wed, 10 Nov 2021 16:21:33 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969c93faa9ae58d6c3bb99426286ddd8c42002211bdcc3c87b5dcdd262f59150`  
		Last Modified: Wed, 10 Nov 2021 19:39:51 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e76b1015c45cbef1a1b7333fc1243f8672ff468afc5561ca26e894daf2c0fe`  
		Last Modified: Wed, 10 Nov 2021 19:39:51 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65dcac25ca8e7c3f930e80cd66762e28e1c4c91db4f84f3beffb25c5af59e79b`  
		Last Modified: Wed, 10 Nov 2021 19:39:49 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da155e1bbbb7d9dfaf14f6c5df8e7d11f40c9aa7e206df93dba40a6f266562`  
		Last Modified: Wed, 10 Nov 2021 19:40:38 GMT  
		Size: 297.7 MB (297656872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793194e2fc283ef65036106164f87c6441c4352d09768fb8348c64168fd4d9a8`  
		Last Modified: Wed, 10 Nov 2021 19:39:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2405472076ce8fe8d1a1abe2ec11f382621aed815f48c5effc8026e36d0cd7ae`  
		Last Modified: Wed, 10 Nov 2021 19:39:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd43b07778911c5c6edb3aa14a26dfe7e46a69d305fc8bb62788ef338ba983b`  
		Last Modified: Wed, 10 Nov 2021 19:39:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
