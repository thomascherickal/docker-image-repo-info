## `mongo:4-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:fad837c27bfcd63ef1ae4348213c3405506ecd2850c8a3ee4a195c874b30663d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `mongo:4-windowsservercore-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull mongo@sha256:23da57faba03e449c43f63181a435fabab88441e5ce619f14356995087cb996a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983568809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68fbd991c3d4c98a47d25bea05e357157fbcca75f65ef257a475a8b228779f37`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 22:35:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 13 Jul 2023 23:16:38 GMT
ENV MONGO_VERSION=4.4.22
# Thu, 13 Jul 2023 23:16:38 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.22-signed.msi
# Thu, 13 Jul 2023 23:16:39 GMT
ENV MONGO_DOWNLOAD_SHA256=95a021db597790008f2e7070fab4a7c3e0d30262f2305c615b95cb7b8afb4eed
# Thu, 13 Jul 2023 23:17:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 13 Jul 2023 23:17:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 23:17:54 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 23:17:55 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2bae42a1ce047820c1f128e4587a430377ba56a110db0d98ec3ccfbd3de58a`  
		Last Modified: Thu, 13 Jul 2023 23:23:36 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d743fd8d430eceb22ffb290bcbb359a2ff61ee787b7a09dc7e252aa3a70883b`  
		Last Modified: Thu, 13 Jul 2023 23:54:40 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a125d5b1ffaccd6f48df3f1b50e2d25e1dd6e8a91d08aa6f1387e19a97791b55`  
		Last Modified: Thu, 13 Jul 2023 23:54:40 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fd80d9d3d3c1c0a6e2ae0a8612bf3ba7702ea2035e825dd861003bc7f6c812`  
		Last Modified: Thu, 13 Jul 2023 23:54:38 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4468a8ac62828122ec8774236a1a5677e5ad9c2a11ea8a609b9016a2e55187`  
		Last Modified: Thu, 13 Jul 2023 23:55:20 GMT  
		Size: 246.2 MB (246193640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c04de418033153cda321b0e195f53487323ca06a3446369354c091d2b8c1a9`  
		Last Modified: Thu, 13 Jul 2023 23:54:38 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897dc6260b17dea7457c43f3bedbcc060d502dd5bbb1d8b834439bdfc6e002aa`  
		Last Modified: Thu, 13 Jul 2023 23:54:38 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87838e31a3689fa3e6ac4ddd70670769a217ebb81110a9908c6f707fc8d963b7`  
		Last Modified: Thu, 13 Jul 2023 23:54:39 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
