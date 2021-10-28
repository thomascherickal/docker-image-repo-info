## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:f800e2895004eb8f215d1a19eda82f1d0680915ad0111eab250fdc5bc0d375bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:51a7ac5e0fd77e0d518cacc4ba8dd1ef7247cbeb90d2efc2aa36a8e2e8a18e4f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691656157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094b345fd0b9938b0e78ff8e1a41bd7a948a5d96fd0e5614e7dc9f4c4c105b0c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 00:34:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:34:11 GMT
ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:14:51 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:14:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:14:53 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:15:57 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:17:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:17:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:24 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55c74bf8af074a49872e1e0411ac5572625083d17cb1100c5cade611deeb92ff`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c196111fa2b96deb4010edf39b6c187a5308e45e859c0a062794c2fb5f3f48e`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c6b53d16e827fcca445a1d26aa91959d444f28e2137fe5fbfcf6f0e8fc54c7`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da00af251dabde3e8ca9fac5e98e48957058ae66cfc6cd227cf53306475289`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3723fb43a09376bf4c64c3a7bda1347b72d6b6d4b1c154e18966fbe654d672`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c450ca9bbda8ce4628f97b0e1ad60d3a60e9ea834594497f45d4ba31906dccae`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 358.7 KB (358737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef148399e4f9c2b7d805a4f81063d19e5d1f0af2e7cf825c953d6485930ba268`  
		Last Modified: Thu, 28 Oct 2021 22:20:56 GMT  
		Size: 5.0 MB (4965585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e2a9be13aa047556c95aa527fb1309844e9c568b6f7d47b512cc82e9898064`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.9 KB (1924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b1f93d27be52abceae707d37a2208c1754ef97d1df70376d2231249e719d2c`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980a908f4dc78616da8546ec4997c9b27ee6e032da4f9315fad2bf9965451458`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111fccb3f1e5ffbda9b83e6a4b670382b282db49b4d6cd7a30631b7a7de6c82e`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4704; amd64

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
