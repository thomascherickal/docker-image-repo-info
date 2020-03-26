## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:7a1741b8902fee16a0b0b552d35553541739a449f3ab2e6c8fc0a734b0c45c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull mongo@sha256:87b85e0a0f75fd5bb80386235ae745fb0bb26c9495afb518f286a315516a4be8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720903345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5dc99b035be504c15cf68c8df72864a684d0893a89169f0d275494b53ff8bb8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 26 Mar 2020 19:29:53 GMT
ENV MONGO_VERSION=4.2.5
# Thu, 26 Mar 2020 19:29:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Thu, 26 Mar 2020 19:29:55 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Thu, 26 Mar 2020 19:48:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 26 Mar 2020 19:48:49 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 26 Mar 2020 19:48:50 GMT
EXPOSE 27017
# Thu, 26 Mar 2020 19:48:52 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d663840c734a93752b6337d2409d194921fe04e8708ba7807ef8d08a3a3236`  
		Last Modified: Thu, 26 Mar 2020 19:50:19 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b80b62ed743e8e87f2ea7affc7fcf9c1fc623770fccca2773984c5eb0fbad9`  
		Last Modified: Thu, 26 Mar 2020 19:50:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b2b393d41959bcf72ed74472bfc20c8e2db75a968385f423d3796e6f7e1bc8`  
		Last Modified: Thu, 26 Mar 2020 19:50:17 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c020cbb663a5f3faf907127d8425bca5672fbd5ee0cdaaa3bdd3db1d51e9906`  
		Last Modified: Thu, 26 Mar 2020 19:51:48 GMT  
		Size: 455.6 MB (455559027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489b16fdcbfded3da27ae54b57f523ae63737750b7adcf59662d676c25afcde1`  
		Last Modified: Thu, 26 Mar 2020 19:50:17 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f075d012de8605d94e95a0f25d73cf060218efc3feebb6b63268ca1dae077f6`  
		Last Modified: Thu, 26 Mar 2020 19:50:17 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b0af806780fe08a684198f0f768d6b1881fffad0ea769dc343f8e692bd36e8`  
		Last Modified: Thu, 26 Mar 2020 19:50:17 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
