## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:24ef5942230ae96a43fa09cb0d1c4c987b02bb1fe5ece0090f368cc503504e25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `mongo:4-windowsservercore` - windows version 10.0.20348.405; amd64

```console
$ docker pull mongo@sha256:27aa8f568cc5c1eee7558ee0a5eacbeb7617d778e4d1eb8e0c2b2de5f09344b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2425478573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231ebe8a0899724654e55759155cc1252a4ca17a1c8f69d68d6036a367da57a0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 08:07:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 30 Dec 2021 19:16:35 GMT
ENV MONGO_VERSION=4.4.11
# Thu, 30 Dec 2021 19:16:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.11-signed.msi
# Thu, 30 Dec 2021 19:16:37 GMT
ENV MONGO_DOWNLOAD_SHA256=40b6f28996f80e4c1922c6e4b61cec0bc16f72cb2f35cb997e64a3a6b6f95074
# Thu, 30 Dec 2021 19:18:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 30 Dec 2021 19:18:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 30 Dec 2021 19:18:46 GMT
EXPOSE 27017
# Thu, 30 Dec 2021 19:18:47 GMT
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
	-	`sha256:e40a7c1cc51d0900b3e94594c09f103bbd9ee55d6fcdb2c64866a7ae6de2a500`  
		Last Modified: Thu, 30 Dec 2021 19:32:15 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1b88e2e0a7b7cfeb4241f9848005f6e4aee8bda854eb4da7b34fb25ac3eb2`  
		Last Modified: Thu, 30 Dec 2021 19:32:15 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58641560e2c37ae3cd49dd061f472dd46f5884ed9492ae3daeaa7e3ce561f050`  
		Last Modified: Thu, 30 Dec 2021 19:32:12 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd03d20be44aa0b57e956d8886dda694023ad20703ff0819dc83ae7054cf36ff`  
		Last Modified: Thu, 30 Dec 2021 19:36:12 GMT  
		Size: 234.7 MB (234697203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbb78ba2b5851ffc0713de07198c16352be53f2a4e9a9c230c86d52d49430bb`  
		Last Modified: Thu, 30 Dec 2021 19:32:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236521806d691ae93485dfbd64bc7150a5943be9444c1a5bc7312b6e644e1aeb`  
		Last Modified: Thu, 30 Dec 2021 19:32:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0962feb380e6893dd8a8bd99b4a605daa6bca00af99ac75d1829228a082a07`  
		Last Modified: Thu, 30 Dec 2021 19:32:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull mongo@sha256:91187fbb011faa505b71b943e01ec0083fa3f8bf0dc59113b1b8a79b25bb6e71
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2943091621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53979306b0aebbec2e345f3ffb6863bbdd5a66c2ab91f0dd92472eebddafc104`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 30 Dec 2021 19:19:01 GMT
ENV MONGO_VERSION=4.4.11
# Thu, 30 Dec 2021 19:19:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.11-signed.msi
# Thu, 30 Dec 2021 19:19:04 GMT
ENV MONGO_DOWNLOAD_SHA256=40b6f28996f80e4c1922c6e4b61cec0bc16f72cb2f35cb997e64a3a6b6f95074
# Thu, 30 Dec 2021 19:21:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 30 Dec 2021 19:21:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 30 Dec 2021 19:22:01 GMT
EXPOSE 27017
# Thu, 30 Dec 2021 19:22:02 GMT
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
	-	`sha256:2e467430b7b5b8ef19782fb4228a5d6532d70874d633a67168b8b2175f456121`  
		Last Modified: Thu, 30 Dec 2021 19:36:28 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbef78f6b5b5c7f794965946b3ab4be6ad83346c1c0ecb4bc1cf0366b24b44c`  
		Last Modified: Thu, 30 Dec 2021 19:36:27 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8df198cabca36e3c10ee9560564fd1d09219415dce3a037160022ce2d096b9`  
		Last Modified: Thu, 30 Dec 2021 19:36:25 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c74fce9aa44aa81034bb5b8d1eabad02008f804174f602a22d53fc57fb01fa8`  
		Last Modified: Thu, 30 Dec 2021 19:37:08 GMT  
		Size: 234.5 MB (234477221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0665ead594505d72dff8fd2155f726652d680b2ab6a0637eaa3d1d4f3a1cfaf`  
		Last Modified: Thu, 30 Dec 2021 19:36:25 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e573dd0930d86888cc990caac3e3d439637b53b2857b7388c38cb2062a6f3a1f`  
		Last Modified: Thu, 30 Dec 2021 19:36:25 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310d93fa584bdeb22b4296590b9fe4f0a5fee456aebf66cf39099c453126a491`  
		Last Modified: Thu, 30 Dec 2021 19:36:25 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull mongo@sha256:2ec88f24901757e056f203e47f6e11f269404de9624b4d3ec59d4d8547e2ebae
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6513592168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc045655fd55c4fdb7dd18a346bc66aa0581ed0d5bec50fc6ffdcdbeb76378d0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 30 Dec 2021 19:22:14 GMT
ENV MONGO_VERSION=4.4.11
# Thu, 30 Dec 2021 19:22:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.11-signed.msi
# Thu, 30 Dec 2021 19:22:17 GMT
ENV MONGO_DOWNLOAD_SHA256=40b6f28996f80e4c1922c6e4b61cec0bc16f72cb2f35cb997e64a3a6b6f95074
# Thu, 30 Dec 2021 19:25:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 30 Dec 2021 19:25:26 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 30 Dec 2021 19:25:27 GMT
EXPOSE 27017
# Thu, 30 Dec 2021 19:25:29 GMT
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
	-	`sha256:ffcf107a7880db1af7913afdf5332bd7994fa4947fee917756fca6a300bcdac1`  
		Last Modified: Thu, 30 Dec 2021 19:37:23 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2452862863d72f89eeb3df3535838d2519f1b5eaf77fdba6aa3a127c4729d057`  
		Last Modified: Thu, 30 Dec 2021 19:37:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be50e90940b286fa9726e99c23c7319e8e9b6587aa32dc1341093347816fd3af`  
		Last Modified: Thu, 30 Dec 2021 19:37:20 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bda93bc05c8c4df4ec9d23d404fd0d1d903f77b364684b0bc8de5f1c7c15a0`  
		Last Modified: Thu, 30 Dec 2021 19:41:27 GMT  
		Size: 238.9 MB (238867713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8341d7b3372ab731d6459a27056a4e3c42a32914ac0f69ed31f07061cc3bd7`  
		Last Modified: Thu, 30 Dec 2021 19:37:20 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddc428ecee9709877106821abb9860a5dc3b928aa77513e93fcf9a49049f140`  
		Last Modified: Thu, 30 Dec 2021 19:37:20 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d427d925cf54df6d116a13f6f6283702176c7716e90630238d4c0e6bfc1bd89`  
		Last Modified: Thu, 30 Dec 2021 19:37:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
