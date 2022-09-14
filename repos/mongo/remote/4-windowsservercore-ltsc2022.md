## `mongo:4-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:647e0e646836f6c535e23932ca227368d5044c9e520ccc2243d6612cbae33a16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1006; amd64

### `mongo:4-windowsservercore-ltsc2022` - windows version 10.0.20348.1006; amd64

```console
$ docker pull mongo@sha256:ea000dd779fc4ad5186c1e55504447731b7e3e9d788594362a8f29ddb5a7f1f1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2591219015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed6246659011b4df5a4ae8a09023396606adde375034b16a10999a9d376ec648`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 13:31:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 18:31:14 GMT
ENV MONGO_VERSION=4.4.16
# Wed, 14 Sep 2022 18:31:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.16-signed.msi
# Wed, 14 Sep 2022 18:31:16 GMT
ENV MONGO_DOWNLOAD_SHA256=0b6606a06c438c09777807e7637031e3efc2347bd9c60432b1be4a33f1f59045
# Wed, 14 Sep 2022 18:32:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 18:32:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Sep 2022 18:32:35 GMT
EXPOSE 27017
# Wed, 14 Sep 2022 18:32:36 GMT
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
	-	`sha256:9489453e05e862607355c418219af63c525762d8b9fb3cb3be0b5a4972a857b4`  
		Last Modified: Wed, 14 Sep 2022 19:13:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac21072ceadf5ecf9061514c6c47564df61f42dbdfb576abcbb083268197fd1`  
		Last Modified: Wed, 14 Sep 2022 19:13:25 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b5ab0c3cae4ddb0bb654d2c89ddeea013a9c35f67d9ad29e8610283fec7d6f`  
		Last Modified: Wed, 14 Sep 2022 19:13:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb9c49187e84d46c7fceef3a27722f8b0a8b3520d05bb16ff8fc1d82a7018c0`  
		Last Modified: Wed, 14 Sep 2022 19:14:10 GMT  
		Size: 244.3 MB (244259850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81663e953bc4d0e8de93ce9e4c0dc08998133bdd9a2998923243ecf4ba46d062`  
		Last Modified: Wed, 14 Sep 2022 19:13:22 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda46afbf8bcaf38bec296a7112ae654190ca1d08a3785617213509b5ce65a6e`  
		Last Modified: Wed, 14 Sep 2022 19:13:22 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8235db0c6ffdc98974298c4287c6d6eb7d7fbbfe3162d80794713a3d65afbe`  
		Last Modified: Wed, 14 Sep 2022 19:13:22 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
