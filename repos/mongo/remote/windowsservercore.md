## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:fe738fb0d84f9a4acce3ed145a5ea5b78d69a8ec7304537931c3ad9542193b56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.469; amd64
	-	windows version 10.0.17763.2452; amd64

### `mongo:windowsservercore` - windows version 10.0.20348.469; amd64

```console
$ docker pull mongo@sha256:9a00a6623f37d2cf0f138b9b5a3d1958d2ba57e37cb4d0057d96f0db869154a9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2502977464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05399bd3aea9d9060f557a19163c6aac4c85bfd575bd561d64e16d32807160e2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 06 Jan 2022 03:56:33 GMT
RUN Install update ltsc2022-amd64
# Tue, 11 Jan 2022 19:59:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Jan 2022 19:59:42 GMT
ENV MONGO_VERSION=5.0.5
# Tue, 11 Jan 2022 19:59:43 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.5-signed.msi
# Tue, 11 Jan 2022 19:59:44 GMT
ENV MONGO_DOWNLOAD_SHA256=a791d7197849516381b3dc5b2ebb988432b95b52e347a3ce3d70d026d108886a
# Wed, 12 Jan 2022 03:40:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 03:40:22 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Jan 2022 03:40:23 GMT
EXPOSE 27017
# Wed, 12 Jan 2022 03:40:24 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b593686e27e7562a5b0696823307ffa822214cee8bd2eec1075eadad4cb9712`  
		Size: 956.0 MB (956001983 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:304b58b2bd8a968bdbcff36b25fec940dbb658b60fa8fb3695b63e3e2a4cdcff`  
		Last Modified: Wed, 12 Jan 2022 17:11:29 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749d1d680956c27db19afdf4b5920bcdd8722dd506c3fcec5f9db06860198e0b`  
		Last Modified: Wed, 12 Jan 2022 17:11:29 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7096effd5f166b3eab586e1aa21736d3e01974b5e6263ec777c0fd9aa34cd178`  
		Last Modified: Wed, 12 Jan 2022 17:11:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0474cfa2ed25d345bfbdef7755b6d77597250c34c632db2cb070959d3214fe15`  
		Last Modified: Wed, 12 Jan 2022 17:11:26 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092a0fbe35d970d35ae0efc0f0c5a30c36e0da32c65252ded3472a231589231f`  
		Last Modified: Wed, 12 Jan 2022 17:12:21 GMT  
		Size: 295.3 MB (295266491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777f885acc920989d9bef74e595f8aaf4a84a4b1c9d5597bd95b8c4671706f65`  
		Last Modified: Wed, 12 Jan 2022 17:11:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a583f1a11c9709ce9075fec11c2ddeabc4122ada37b414512c3419245b6d57`  
		Last Modified: Wed, 12 Jan 2022 17:11:26 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098059f8b984b4745509bac2671ff778518821b5c76fb6d859bce5898b0b037d`  
		Last Modified: Wed, 12 Jan 2022 17:11:26 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull mongo@sha256:ce06293818d04f3b11624454f7d6b058e5cbf12dfb9f1094ddb8b36bbdd8907d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (3007231719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:236f8afae578fe35970a968a889ff446ddb808e40e74345c05802b0845ccdd96`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 13:54:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Jan 2022 16:38:12 GMT
ENV MONGO_VERSION=5.0.5
# Wed, 12 Jan 2022 16:38:13 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.5-signed.msi
# Wed, 12 Jan 2022 16:38:14 GMT
ENV MONGO_DOWNLOAD_SHA256=a791d7197849516381b3dc5b2ebb988432b95b52e347a3ce3d70d026d108886a
# Wed, 12 Jan 2022 16:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 16:41:12 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Jan 2022 16:41:13 GMT
EXPOSE 27017
# Wed, 12 Jan 2022 16:41:14 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:537828534783cff318d36854dbda0683aef7263e437c7c669de4092e1778959c`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c8ebc4453f0055657fe47fb25819095fb1477145b6dcd99d4efa5155cdcfee`  
		Last Modified: Wed, 12 Jan 2022 17:12:43 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee19f257ccb682fd36f413462c61b626fb1b18cc0f7be6078efa7ccfec3a20c`  
		Last Modified: Wed, 12 Jan 2022 17:12:42 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00220bd2f8a21db59cd7c667523f65f886cd72c55fc70af1d3f2cf0b6ffb8c4`  
		Last Modified: Wed, 12 Jan 2022 17:12:40 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b72d327d167721d57fa6a7de6c2ebbdd116a985345076baa4ed3065a6d03e1`  
		Last Modified: Wed, 12 Jan 2022 17:17:59 GMT  
		Size: 295.0 MB (294990981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce435af465ba1e64d794e1ff8a128451dd952ac866d76bb0c37787a104815bb`  
		Last Modified: Wed, 12 Jan 2022 17:12:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9830dcd1b7844ee0ea96baf6c9d461cdae851f9b23e7ae97a9c77d77ec09d65c`  
		Last Modified: Wed, 12 Jan 2022 17:12:40 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f87ce488fbf1f021c382bfbcc297d83b0b2ba66fd9c785d3f27ed34841659b`  
		Last Modified: Wed, 12 Jan 2022 17:12:40 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
