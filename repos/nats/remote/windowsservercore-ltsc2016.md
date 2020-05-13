## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:08c9781136f212ba6156cc3bb7d0371eb17053726b1ce2a851b01ba0fd721895
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull nats@sha256:9ac0a1a8b7c1d86e67b07c27da69c167bc06e4dd3d83235376b9441c2c7254dd
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5751199562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc507bd9c022cd0ed7dbbd09cfa5913d866c520bcb826bfb6132ea62ea27549`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:51:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:51:04 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:51:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:52:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:54:02 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:54:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:54:06 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:54:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:54:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356fa8d07c48624dd3553b12cafae53b1e6818e2e77c7b4ad7c5e37a6edf5f5`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d925d5330efdd0e3691f27be756f2d4bd21271b3d92a1fdbd7d0015ca751b`  
		Last Modified: Wed, 13 May 2020 14:55:21 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02c160a78fb2c0432fda99964268c0d0be0c92dd4faad28abdc2aa3e9f2f3f`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58a8e2f37803c472c8d10d3693e28446f643f41b20e716c97bb2cf561471f3c`  
		Last Modified: Wed, 13 May 2020 14:55:22 GMT  
		Size: 5.4 MB (5380611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a364666bd4bf347aa0241e06563fe518267439e92df88dd4c943475a6be316`  
		Last Modified: Wed, 13 May 2020 14:55:33 GMT  
		Size: 13.9 MB (13919327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07365ad87d191e5cdc05d203b8f0491d7c408b9cdbb94a131c53b05807f67f40`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bf5adfaf150aa00c8b9fe7bbfe96bfe97dbfee94544af1ad694e38cd7446c`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84243df3097f51931f380c65fdf517d4a61a9a052a35d3fc8847695ca727781c`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aec177c2f2c1b498277b9130ad9ff47c26a7cb4057adf463705fc2fc671029`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
