## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:4121b3254b9e520fb13fe01c60e2a06aef50a48d6bfa47c96b8c3b1d8a0674b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:3f18f0540591a191146d319beaa54fd3e4e9e04e149a7a417ae2c1de45d125c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679277996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99559015cf04f0c211803b1feba4d9e791ce826d1ffdbbfa80aea0ab980fc9f5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:42:11 GMT
ENV MONGO_VERSION=4.4.3
# Tue, 09 Feb 2021 20:42:11 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Tue, 09 Feb 2021 20:42:12 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Tue, 09 Feb 2021 20:44:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:44:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:44:08 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:44:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a4a33f1f276e776a3b431358f3364f1419734ee0bd3a2d6f9d259643033a4c`  
		Last Modified: Tue, 09 Feb 2021 21:14:59 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaab413ea8419163db0151aae262b7ac8cdf7ca0713c1605aa8d68b65d716bb`  
		Last Modified: Tue, 09 Feb 2021 21:14:58 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6776006f32be140fc37c053fa193fc556d84c8289ea5e09c5314813a092377`  
		Last Modified: Tue, 09 Feb 2021 21:14:56 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924eb14e95fcb6eacf76c5c1c514d00d40a775d6ae7c194ce09d8d0d24c2444c`  
		Last Modified: Tue, 09 Feb 2021 21:19:16 GMT  
		Size: 240.0 MB (240001428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16021235707b8310a74fa8275ef7631f2dc30f79c1d6b3d68b51a6ca7cf64ffc`  
		Last Modified: Tue, 09 Feb 2021 21:14:56 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac72e712ff6055a56c7d9684535277fa2a3c4439f6b1a1549f1fdc99dc084d1d`  
		Last Modified: Tue, 09 Feb 2021 21:14:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06969c192bec93baea3a0074593a5ddae36de1c1b5669e72a424946a4a3a7c11`  
		Last Modified: Tue, 09 Feb 2021 21:14:56 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
