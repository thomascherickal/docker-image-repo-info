## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:d9aaa295d957ae1661bcd4b25998267be43ca348c0f1bf4b7b25e73aaa878aa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `mongo:4-windowsservercore` - windows version 10.0.20348.405; amd64

```console
$ docker pull mongo@sha256:941585fe7dc06034c0b355278009f4877028d376ad3875a7a5a66b6f7b87790c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2424752668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cffefe57d5459675bf983b140c3e9eb7ef2103064414d31c08fc3703105c017`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 08:07:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 08:26:35 GMT
ENV MONGO_VERSION=4.4.10
# Sat, 18 Dec 2021 08:26:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.10-signed.msi
# Sat, 18 Dec 2021 08:26:37 GMT
ENV MONGO_DOWNLOAD_SHA256=b48fbc7ba392f505a89af03301ed8f3f99b35c6ee8f3c9595cfebacf26ba68ee
# Sat, 18 Dec 2021 08:28:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 08:28:05 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:28:06 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:28:07 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c1de582c6c9c68cde1be202b853d6f5b2dae10020d41c1402bdaede850c77e8`  
		Last Modified: Sat, 18 Dec 2021 09:06:53 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a35400f16b1c1d2ec44136d5cd0a276eb696075ffc251d3b0b61f0f27d4df88`  
		Last Modified: Sat, 18 Dec 2021 09:35:53 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f70f5407fa5ebb6fdff2234f7411de16209ca1005ccfcdd980bdac3ff2b1f2`  
		Last Modified: Sat, 18 Dec 2021 09:35:53 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d73875f12700065e04022c122dc2208b6512a9aab029bb0225c7a29ae970691`  
		Last Modified: Sat, 18 Dec 2021 09:35:51 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff95a4bf9f3ed793eb4fdd29c2a2c263efc7f2cad1f8034d7381d2ed8defc2f6`  
		Last Modified: Sat, 18 Dec 2021 09:36:35 GMT  
		Size: 234.0 MB (233971299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b84c36c75430453925b40e83a5e70571ac04de9be4c13da37312e362eb66ece`  
		Last Modified: Sat, 18 Dec 2021 09:35:51 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4dcdea530c2a003656291263f05bb1a8f399512b82013897694fb2d0336a31`  
		Last Modified: Sat, 18 Dec 2021 09:35:51 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2418b63f99a7ae60bd15ce1fb94d3ca61fc7742f5002230edbf063979a0b1ad`  
		Last Modified: Sat, 18 Dec 2021 09:35:51 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull mongo@sha256:e9c8c8567abc20442162a36f963a467e1390c366bf1ff8194610f6fd9244f8b4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2942357242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5e868cd1be264b11124a097a79a86846fe1021059c34240c54460ce0e0a789c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 08:28:18 GMT
ENV MONGO_VERSION=4.4.10
# Sat, 18 Dec 2021 08:28:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.10-signed.msi
# Sat, 18 Dec 2021 08:28:20 GMT
ENV MONGO_DOWNLOAD_SHA256=b48fbc7ba392f505a89af03301ed8f3f99b35c6ee8f3c9595cfebacf26ba68ee
# Sat, 18 Dec 2021 08:30:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 08:30:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:30:42 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:30:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d22d2238b031d3f13bcd6c144e80f8f8402332b8ee8e53cc54b7912c3ac808cb`  
		Last Modified: Sat, 18 Dec 2021 03:59:34 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42502f871d0345eb2f08ae91e195496a2cc17a3e94689838f42de80a7bd0443`  
		Last Modified: Sat, 18 Dec 2021 09:36:50 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d63d10c58f620696828e656563f3e4da1f04809a5d3ae87d94a430391cc903b`  
		Last Modified: Sat, 18 Dec 2021 09:36:50 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170733aaef4d8887f617335bbefbcaf2da71ddc03e0c0e2eea5387b82ad5b2d6`  
		Last Modified: Sat, 18 Dec 2021 09:36:48 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b537d228dfc418e8facc15e07f2b95c5c9a0d26cf6a956a156fadc55453a6718`  
		Last Modified: Sat, 18 Dec 2021 09:37:32 GMT  
		Size: 233.7 MB (233742794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ea4a20dbc04960242a758c5e87bdf8c44a7e2c90a0b55daa55041b8e756610`  
		Last Modified: Sat, 18 Dec 2021 09:36:48 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b603c32aafcb2a60374228f94e41ab86bf9c0d565b19c079332d0afc6d3c8c`  
		Last Modified: Sat, 18 Dec 2021 09:36:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27480d3e8a689a755685949fb0ab351bb8636216693210fbb2fb24c761d028e0`  
		Last Modified: Sat, 18 Dec 2021 09:36:48 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull mongo@sha256:70b3b385fde4a911ca34f470eb1649e8ee87143fc5353412e8d1016a7fd48700
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6508384497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfd5969045afa80cc59a7033a0dc306f960dc90a6902e2df9529a98dee6272b6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 08:31:00 GMT
ENV MONGO_VERSION=4.4.10
# Sat, 18 Dec 2021 08:31:01 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.10-signed.msi
# Sat, 18 Dec 2021 08:31:02 GMT
ENV MONGO_DOWNLOAD_SHA256=b48fbc7ba392f505a89af03301ed8f3f99b35c6ee8f3c9595cfebacf26ba68ee
# Sat, 18 Dec 2021 08:33:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 08:33:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:33:18 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:33:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6bffd19db3f71ba2031bea25a529c67034869e7e1bbf9e2431d5ee747bd6d6d`  
		Last Modified: Sat, 18 Dec 2021 04:00:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c6174b9ffa12f2f64f1094ac05392a4664374da300eacabadbed47a9c440e4`  
		Last Modified: Sat, 18 Dec 2021 09:37:47 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758897b605c126c182ca4dd30588487e6264646c8445d29041862b2034f4cbed`  
		Last Modified: Sat, 18 Dec 2021 09:37:47 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fa575e00334b4eaa9f3086ccd22332ca62340874a7dbe846edc9fe8ad6eb21`  
		Last Modified: Sat, 18 Dec 2021 09:37:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590397f9ff8c82a5de437427d07a6ec2c6a3119801569c5b32938e257e7bf633`  
		Last Modified: Sat, 18 Dec 2021 09:42:03 GMT  
		Size: 233.7 MB (233659943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7426a56ad6a704f1c4ab3ec834a5b4b2860da65aa806529dcc12a83f887536`  
		Last Modified: Sat, 18 Dec 2021 09:37:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359ba05af637fa9447644451ef97a1f1dc22170857f529d2ac59683ba06303e5`  
		Last Modified: Sat, 18 Dec 2021 09:37:45 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e4fa854744ef197af3df688116aeb52a4a5d82b7151da02681bc030b7bb690`  
		Last Modified: Sat, 18 Dec 2021 09:37:45 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
