## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:bc47cc36bb8b074b83b8f38eebe614e930902febcce54ddbf1b44f128abdc0ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull mongo@sha256:a0823a941a401afe9b06dc1b790169df5a98b075ece15d826cd636fd7753f035
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2208726050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb27bb38fc93ff684e63aa1492c39a40e5800f1b5ce3bc0085ce1aa35088de5a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Thu, 16 Feb 2023 00:42:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 25 Feb 2023 00:25:17 GMT
ENV MONGO_VERSION=4.4.19
# Sat, 25 Feb 2023 00:25:18 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.19-signed.msi
# Sat, 25 Feb 2023 00:25:19 GMT
ENV MONGO_DOWNLOAD_SHA256=91e83f2fc3ddd3ab0bb170d26b89d80e4268a563deee6ce72313de5774875f08
# Sat, 25 Feb 2023 00:27:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 25 Feb 2023 00:27:44 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 25 Feb 2023 00:27:45 GMT
EXPOSE 27017
# Sat, 25 Feb 2023 00:27:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531f6c3ad9784fc2870ea5ca08c4adccd9318602ed534d822e12b8b658a7b0b6`  
		Last Modified: Thu, 16 Feb 2023 01:37:30 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357ab45889e8d146d3c5596d0e4469c8d4765532cb423f68fdce319320f54048`  
		Last Modified: Sat, 25 Feb 2023 02:24:23 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90afdd9bd1ce138ed87b320780664dee8c0ca348067a4dbfce08bec13cfa1901`  
		Last Modified: Sat, 25 Feb 2023 02:24:23 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ea7cf04f8251c936d1eab84c0d15a40ecb2ea01c2c23aaf735f0a838a754fb`  
		Last Modified: Sat, 25 Feb 2023 02:24:21 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338eff7b202d1b50afe6fa76850fa809632e72e3d385a968622c661ca3cbee12`  
		Last Modified: Sat, 25 Feb 2023 02:25:06 GMT  
		Size: 245.8 MB (245758993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6b90446d2277479fb7e51510e1bca051546699f58e30b09f62fe2b2fc8ee0e`  
		Last Modified: Sat, 25 Feb 2023 02:24:21 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d272db20a14a5cd785ad686387281b9407a19f6c6b3c2b55531d7eef2103f7f`  
		Last Modified: Sat, 25 Feb 2023 02:24:21 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b994cdf53654425bb31fd63c55460d5c66ba9c243553a93ed108bfd37ec578a`  
		Last Modified: Sat, 25 Feb 2023 02:24:21 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
