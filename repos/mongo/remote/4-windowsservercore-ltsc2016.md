## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:a36d7ecbdc4c624df511498438403025f5626e307093623c939e431f515fbba0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull mongo@sha256:c0324035c885d8a6803b728da74987e5b8caec2a8c06776cb381eb572667c941
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6506445822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a057314eafb562d70c604203f66b6d3d3c386fa1e7f434beae7f6f68e8d3eb8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 00:39:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 16 Oct 2021 00:18:06 GMT
ENV MONGO_VERSION=4.4.10
# Sat, 16 Oct 2021 00:18:07 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.10-signed.msi
# Sat, 16 Oct 2021 00:18:08 GMT
ENV MONGO_DOWNLOAD_SHA256=b48fbc7ba392f505a89af03301ed8f3f99b35c6ee8f3c9595cfebacf26ba68ee
# Sat, 16 Oct 2021 00:20:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 16 Oct 2021 00:20:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 16 Oct 2021 00:20:09 GMT
EXPOSE 27017
# Sat, 16 Oct 2021 00:20:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d3c52a3fe41298469bd9ca8471cd22a349f75bf82b049e968c97dd7cbf538b9`  
		Last Modified: Wed, 13 Oct 2021 00:44:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8359b72697a6127fcf97513f37601616a2ff9e7cb0c5ab62fa868657d966e31`  
		Last Modified: Sat, 16 Oct 2021 00:23:48 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5933c69966a3d17e81f5524fbd2d52250ba5a5b7d67609e8068197edf90cc38a`  
		Last Modified: Sat, 16 Oct 2021 00:23:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca7cd5836a6074160dd472704ff0111bc4f47fecd523ddbe9e7ac81abe60165`  
		Last Modified: Sat, 16 Oct 2021 00:23:46 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b83b59f2bda9e99287bbe3d24bb6920091d5cb2c58e659e6d2c1f4ef20dfb`  
		Last Modified: Sat, 16 Oct 2021 00:24:31 GMT  
		Size: 233.7 MB (233669376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405e36e5c70101ec861f61601a3bdfa596e29304e389594d73eec70ae729af9a`  
		Last Modified: Sat, 16 Oct 2021 00:23:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4020c95a869d7e7ab286398be46ccd4c02fb77d170cecd43b63e9f371c2b0d1`  
		Last Modified: Sat, 16 Oct 2021 00:23:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdab31a96006dab2681e55dc2ed204d1604bd6ade7cb3b2edf6511fbba8d1189`  
		Last Modified: Sat, 16 Oct 2021 00:23:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
