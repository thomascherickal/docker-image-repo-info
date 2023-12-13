## `mongo:6-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:b5f2c9ad5e6010baa07643ed15025fc1f74f89d4e542fb0f18f5ad74056c523e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `mongo:6-windowsservercore-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull mongo@sha256:ec2937f63d1a3c4211565985ccd5c389d4ac8f1a0aa5d5809a8350bad25cb9bf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2407858782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:649d3b3211999dcc38a6016a3ec7efba7d483f021a41ac14970c6c618137f89e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Wed, 13 Dec 2023 00:55:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2023 01:05:06 GMT
ENV MONGO_VERSION=6.0.12
# Wed, 13 Dec 2023 01:05:06 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-6.0.12-signed.msi
# Wed, 13 Dec 2023 01:05:07 GMT
ENV MONGO_DOWNLOAD_SHA256=126024e5292da3470eb119d798d11862ce1f0472836bce7d3210dcb522b80aa3
# Wed, 13 Dec 2023 01:07:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2023 01:07:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2023 01:07:12 GMT
EXPOSE 27017
# Wed, 13 Dec 2023 01:07:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839fc47f6e056f9e09a214230f8b7115e69419dbc74acbbb1ad6bc0caa28862`  
		Last Modified: Tue, 12 Dec 2023 18:27:40 GMT  
		Size: 500.7 MB (500674814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b375e2cf70a6193773bc43a5e86e2cdc8eabcdadf1d60aeed9bf6665ef6f33`  
		Last Modified: Wed, 13 Dec 2023 01:30:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a66735c882fe450fdb600b8fb107f2eb2cfc4e9d9b66ad8a9ee68acfa53e5ae`  
		Last Modified: Wed, 13 Dec 2023 01:36:42 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44a8cb1254395e493afbba1d54a60b161df0cf255b7269b0e078ff342e614a0`  
		Last Modified: Wed, 13 Dec 2023 01:36:42 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db25e67cda9e67e14e6af02bf4fe53447dcebb6ada9f497421126ac8c4080b69`  
		Last Modified: Wed, 13 Dec 2023 01:36:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c4bd7e807d0108eb00e0d4f8fe605c6cc09d035219721689c39d8dbc84837a`  
		Last Modified: Wed, 13 Dec 2023 01:37:58 GMT  
		Size: 518.6 MB (518575403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0fd76671eb2d85a0fa7ff2e6318358dd9e5d90111d4d68c183b03f79d628d4`  
		Last Modified: Wed, 13 Dec 2023 01:36:40 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c71328ccf4cb4b0bb87d918f700850a671bdac41008cf7d6c662697dc065c8`  
		Last Modified: Wed, 13 Dec 2023 01:36:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ac3e389290814599098b980b38742eb787cbd0c0610100e0c57f134c7b9d41`  
		Last Modified: Wed, 13 Dec 2023 01:36:40 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
