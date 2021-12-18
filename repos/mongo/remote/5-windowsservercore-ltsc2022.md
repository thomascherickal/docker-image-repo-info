## `mongo:5-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:3a05fdaa293a7c95796d3c9a7ad0e5b1b496495f5be1baa27a16407ec6db6888
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.405; amd64

### `mongo:5-windowsservercore-ltsc2022` - windows version 10.0.20348.405; amd64

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
