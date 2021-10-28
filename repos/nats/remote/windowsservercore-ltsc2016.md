## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:66e5dfec5b380717e7d72eb0559430d619858fb7e561bf035f4e05d29bd2f30f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:7e87d39f63d888a8c38989beda927f43d801c6fc88dbc230a2b8b600afd2b569
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278116707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1342ba4bbfda650dd7a22cc73f3eafe211dbcdf3d88c445b13b5e1e3ed24dec6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 00:39:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:39:25 GMT
ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:45 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:17:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:17:47 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:18:48 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:20:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:20:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:20:20 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:20:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:20:21 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:2d5e5e67c70d509eb320faa6c55dd5fdc5c5440334d85dd07ea0e919299624b2`  
		Last Modified: Wed, 13 Oct 2021 00:44:15 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b125ecbbd9fcd1e607a95ad95618b22bed487633e2c3f53e74079496cbf3e7d`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d36335126bc1a01fd80e6e62c8b12b80a4ba0930c9044553d759ed416c9ad5a`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861aaad346207f6efc3d74dce720f56b81d8292a8f10b16a126d3545a67c784`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee10f08ed053b70ed8c754e81edf0e43eb621718ec915d979bc4515f6bf3614`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 347.5 KB (347462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72024e6801dae28939f9b887af08469d17db75599cdace64ba5ad1bc46105392`  
		Last Modified: Thu, 28 Oct 2021 22:21:33 GMT  
		Size: 5.0 MB (4989467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e989943b45c1112cb4df4c4b061238abebaf0125af3515e0cec1837b2bd21d`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811eabaa8cb45eb635eb3de73e9905648c98a5aaace1cfc8af9019f280ce424`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c08391a88082294bf9684ce0626a570685c8056c6e61e3f73e6763d4870ad05`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d9a660e321d771c0067346cb4c5e6807397c8be963e1c7461161d0f0e6ad`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
