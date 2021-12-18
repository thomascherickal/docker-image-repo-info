## `mongo:5-windowsservercore`

```console
$ docker pull mongo@sha256:6c732d5f89720aa861f3582ff19448fd400544e2c8940437b5b90ae2f35c86e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `mongo:5-windowsservercore` - windows version 10.0.20348.405; amd64

```console
$ docker pull mongo@sha256:61ce095edf1a10cc805ab5ddb76530b97361a53cd5dd0de93d897d8eca632508
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2486057262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff060b6aee32a8dc5af0bcac66de5145aad088cc2f6e96176acc1908f139b9c5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 08:07:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 08:07:57 GMT
ENV MONGO_VERSION=5.0.5
# Sat, 18 Dec 2021 08:07:58 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.5-signed.msi
# Sat, 18 Dec 2021 08:07:59 GMT
ENV MONGO_DOWNLOAD_SHA256=a791d7197849516381b3dc5b2ebb988432b95b52e347a3ce3d70d026d108886a
# Sat, 18 Dec 2021 08:09:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 08:09:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:09:36 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:09:37 GMT
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
	-	`sha256:99186b1d359df4b2c8c4e58c4871c2b0f7f142475ffffb18bed96a6de6d4240d`  
		Last Modified: Sat, 18 Dec 2021 09:06:53 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee134eabbba160b44239a1371a5297de76ed414c0bd3d005317eefeb048dfc9`  
		Last Modified: Sat, 18 Dec 2021 09:06:53 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4191b5e7f1534e3468232fd86a4125890a4b0fcf8961996b81754115db3aa9c4`  
		Last Modified: Sat, 18 Dec 2021 09:06:51 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b895affe3075b89f72f3b7454118a11802216cf1657ecd96c016b1a79a80069`  
		Last Modified: Sat, 18 Dec 2021 09:07:48 GMT  
		Size: 295.3 MB (295276128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1917e856c455140f45506260b774b02369cc3f02a13f51623be855960a1991`  
		Last Modified: Sat, 18 Dec 2021 09:06:51 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a041f329b84ccef92623f42ebc9063e3dd743e19880f1d4c20349d179758e5dc`  
		Last Modified: Sat, 18 Dec 2021 09:06:51 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f7a533f4a5dcc87f9aa66d822e412d0738f417c45e20b72afe053644970c33`  
		Last Modified: Sat, 18 Dec 2021 09:06:51 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull mongo@sha256:ab03b66e493945ef56e8a58753a16c7165d1a3e0b049f3445669e3c52c2a6c56
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (3003640307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67beafcc8debb0bbb6a4edd3af66d7555fd4888f0ad9a0ed9dbf12908b55d293`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 08:09:53 GMT
ENV MONGO_VERSION=5.0.5
# Sat, 18 Dec 2021 08:09:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.5-signed.msi
# Sat, 18 Dec 2021 08:09:55 GMT
ENV MONGO_DOWNLOAD_SHA256=a791d7197849516381b3dc5b2ebb988432b95b52e347a3ce3d70d026d108886a
# Sat, 18 Dec 2021 08:12:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 08:12:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:12:24 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:12:25 GMT
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
	-	`sha256:30e86d8cc5d7d638007d4f46887284c38c260aa8f7f897c9e33be0ebf643fc3d`  
		Last Modified: Sat, 18 Dec 2021 09:08:04 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a41ae0d046213a6456bddaef63c04cde17e326404faf2583ee4aedb0e8be4fc`  
		Last Modified: Sat, 18 Dec 2021 09:08:04 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890eb1acbec3565f478a644c9504860dd1576558ac6b1a8c8e2015317ba72416`  
		Last Modified: Sat, 18 Dec 2021 09:08:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2570c731cc6a4b6640fa9e3926b0dc2a3f223d70b679c0e334cd78ace09350`  
		Last Modified: Sat, 18 Dec 2021 09:08:57 GMT  
		Size: 295.0 MB (295025913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585d9711a8402e4ae77e4fec4694213e8e00c24f61a58b522c47041357112013`  
		Last Modified: Sat, 18 Dec 2021 09:08:02 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d9af230e33712a77bcffa99e1f63ce62decea4885299bb26540661e5929b2f`  
		Last Modified: Sat, 18 Dec 2021 09:08:02 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e45273e91eff42422f7946f4ef1c2fb913f2f8359515365a42121a8464cf72`  
		Last Modified: Sat, 18 Dec 2021 09:08:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull mongo@sha256:dc1e0e0a746355d51b918456ead65b0c79be3ff8079c5abe5557155df531807e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6574165890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fabaeef57593c53613c914f16da5a21ab483334c223dd0181771dd7922a947f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 08:12:35 GMT
ENV MONGO_VERSION=5.0.5
# Sat, 18 Dec 2021 08:12:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.5-signed.msi
# Sat, 18 Dec 2021 08:12:37 GMT
ENV MONGO_DOWNLOAD_SHA256=a791d7197849516381b3dc5b2ebb988432b95b52e347a3ce3d70d026d108886a
# Sat, 18 Dec 2021 08:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 08:15:09 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:15:10 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:15:11 GMT
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
	-	`sha256:f794b6a4e3511527ee432f9826d8c4c513d3609e9e431ebab5b3db3719b128a8`  
		Last Modified: Sat, 18 Dec 2021 09:09:14 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92c90c06db456b01aa86e6254292c16a7a7a4405c11c03270196b1b9454825c`  
		Last Modified: Sat, 18 Dec 2021 09:09:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3098383fc3df97f824b2af6a7e37c4b507f6ef5fbf0cc41c58aad7d2080d0`  
		Last Modified: Sat, 18 Dec 2021 09:09:12 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d339318b7144c3383db6dfcdf8c4be1c10fa1759f4045f7edf576875314bdf93`  
		Last Modified: Sat, 18 Dec 2021 09:14:27 GMT  
		Size: 299.4 MB (299441294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c550530f6a1130a48bff85c005030630f7d9fac99524481b9948c753a38eb15`  
		Last Modified: Sat, 18 Dec 2021 09:09:12 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0b2912a429910c0a9e5a57300ddd9c8388d64c6b056433c3cf906f1b1006fa`  
		Last Modified: Sat, 18 Dec 2021 09:09:12 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9273e0179936d4372d24a64f54fbda2084f6c348d685f86560b2957a2020202c`  
		Last Modified: Sat, 18 Dec 2021 09:09:12 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
