## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:f5022549bc80a9db2612765446cab1bfd7a1be26e723a61158bc4b0c031f5fec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:836eedb3e349b1f2b43a2a8a1075a7c75daec9d12da9a688fbf0e0ccc6f5f900
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2019348725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cd0dd10b5e08978a6e679dbfbbc002970ff7ae24add62a49afe725523436b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 02:59:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Mar 2023 04:05:12 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:09:46 GMT
ENV NATS_SERVER=2.9.15
# Thu, 16 Mar 2023 04:09:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Thu, 16 Mar 2023 04:09:48 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Thu, 16 Mar 2023 04:10:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Mar 2023 04:12:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Mar 2023 04:12:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:12:51 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:12:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:12:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474eedda733dad347e4baad9fb9f3d700b58e5788f7453d1979cebb167746b32`  
		Last Modified: Thu, 16 Mar 2023 03:44:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c46bc18b88e816c6caaf34206ccb18a5b7f6665a73ae9a4678525d49fcb1f2`  
		Last Modified: Thu, 16 Mar 2023 09:07:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a68e4291e27c96744fec7ab4710e923e5b1e40c9f3c6a2e92b8739a3d31b5`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3459f257cce40d5f7ebac46302e2139fb4d25193d8d5cfead8e487c752e1b2d3`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6975473a2f80a1aefa9af46e42f89a933991476f79d5e5a2da8e146697cffe44`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be22253a34963956a4b34689b662e68bd6064ddf0b8aed7177c361264681e439`  
		Last Modified: Thu, 16 Mar 2023 09:07:25 GMT  
		Size: 474.3 KB (474294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec188877326c722f291ad8e0486acf0351224348d1a7d5d69d2f46dd2b34d6b`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 5.4 MB (5352102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaf0234efde44a2b0e27f3aad8cc98edda5e6d51bdfc76348701cfdbd1b4182`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6235fe1716486135953312ee3d91de53d571a34c36eb3af9ab08e7457ea13a3`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2ba63ea546de8e882e02776ea30e2b71555c06d83d435809a377b1e02a664f`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfddbc298f640d6da169c875464a1fe1c426dbe0c2564f3bbf7ddbc3cee8a`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
