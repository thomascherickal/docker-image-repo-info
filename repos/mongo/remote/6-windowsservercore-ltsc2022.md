## `mongo:6-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:ef426e7967c90c1e3851adf82973a902c5e58b0cd611a18dc64d0dca6793f321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1006; amd64

### `mongo:6-windowsservercore-ltsc2022` - windows version 10.0.20348.1006; amd64

```console
$ docker pull mongo@sha256:37e53cf9fa8ba23daafca167272dab0373c9526b5074ff938c307abec49608d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2857462878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0759b8fd6b1467dbde4f980845c89b17cb4f80699fc15e819ce46bd7364eb18a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 13:31:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 18:11:11 GMT
ENV MONGO_VERSION=6.0.1
# Wed, 14 Sep 2022 18:11:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-6.0.1-signed.msi
# Wed, 14 Sep 2022 18:11:13 GMT
ENV MONGO_DOWNLOAD_SHA256=999b39df67a77eda3198f8412dc159b0cd8aa6677b901a0cf287921884306ac3
# Wed, 14 Sep 2022 18:13:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 18:13:08 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Sep 2022 18:13:09 GMT
EXPOSE 27017
# Wed, 14 Sep 2022 18:13:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a16438b2cffe7980c606769d49003f7f1c4d27549445f824511a81834513616a`  
		Last Modified: Wed, 14 Sep 2022 18:58:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42056ad640d8d7c2493a6678000376a5ab8f23647b2d3d671a9b0e3b771a562b`  
		Last Modified: Wed, 14 Sep 2022 18:58:47 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dddc6f555305340d9c516485111fe36a788f6ca32cf390a80cbd5c208be7c9d`  
		Last Modified: Wed, 14 Sep 2022 18:58:48 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb15f702434eea314d2632b8ec7c8f048618a787ace68f869aaa718a2ffddee`  
		Last Modified: Wed, 14 Sep 2022 18:58:45 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6f425ed5435e62305abdc8461925a35c4072691f3e92729fa313a290544505`  
		Last Modified: Wed, 14 Sep 2022 19:00:05 GMT  
		Size: 510.5 MB (510503448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22032f41e64570ba7bc81f11cbde982dce6d4f744ebf18d8a8144766b883ccbd`  
		Last Modified: Wed, 14 Sep 2022 18:58:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a574e2d2128265a569688bfeae3010298bc5a47953da896bc62b3b185df422f5`  
		Last Modified: Wed, 14 Sep 2022 18:58:45 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54b383a371438ea44132b8a9e1dcbe070e3866d31e45afd7cdc06963f90a4f5`  
		Last Modified: Wed, 14 Sep 2022 18:58:45 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
