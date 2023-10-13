## `nats:windowsservercore`

```console
$ docker pull nats@sha256:36def1f4c1d5a7a2038f81e533bb5dd5ddaf79e195b2083651de412b8a09e3ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b96058f0abbf858d83160210231c7c2a0bed54c8fcda52342133dfc9f0ad258a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037938189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:876c267b5fecf8ba8da6cfc10f1952395f0aa829d899d6a6f789b46423d6cf74`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:15:06 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:15:07 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.3/nats-server-v2.10.3-windows-amd64.zip
# Fri, 13 Oct 2023 20:15:08 GMT
ENV NATS_SERVER_SHASUM=4c1d9537562134450e2332dc1561d1ab64beb45fc82e01bc89b9403e3f6d680f
# Fri, 13 Oct 2023 20:16:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:17:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:17:55 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:17:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:17:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf2c59764edeb5a9eb73e90ad90f0df91e731dac208e75bb8d3045985a35b46`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f059f74917a94519977101cdcd91e6eca57a387d5d53147d5b96fa722552e0`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fb62c7bf71d873fbed15e0344a8f6976b86f16d41276ab009108e9b918a855`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad74f3edaa649c29cd7ad4508d28d0e25979664c3a3198452019a82661e026`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 454.6 KB (454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c7895231c0ab196b12f1327f4487a221bbd9d87e0011eb693d7d2bd2a206e`  
		Last Modified: Fri, 13 Oct 2023 20:21:53 GMT  
		Size: 5.9 MB (5879724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc539d58ea38523dd5da406ce195e9af73cc0b40a406cdad13ce87eb641d8308`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34090a57ba21eb445112261cc5e97b649674a537ea643c543eb7d5d6a3ba4c`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072215f5155480305c6d5df8627c9b86f41581c8e2cd3d6a5d31288f6b4b414`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36d40fb089c2f6b3e8ab73302ca5e82c97115acc8c4497d931c6ca9c39cc2b3`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
