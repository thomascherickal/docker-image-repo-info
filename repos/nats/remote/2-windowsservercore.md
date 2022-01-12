## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:24e44e15d62a911e94d6ff5b7e22accfe329f699b42ade9ebb1a5caa3197f373
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2452; amd64
	-	windows version 10.0.14393.4886; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:7f3bfcdbda90968d69223b48664ee1ec937a82bce7365c82135785fe353ba699
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2717536770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4622435affd612664c15aa4fd83b1e45ba56de92d3c7e6dd3dd924adf28111bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 13:54:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Jan 2022 15:10:29 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:10:30 GMT
ENV NATS_SERVER=2.6.6
# Wed, 12 Jan 2022 15:10:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Wed, 12 Jan 2022 15:10:33 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Wed, 12 Jan 2022 15:11:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 15:13:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 15:13:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:27 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:537828534783cff318d36854dbda0683aef7263e437c7c669de4092e1778959c`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576e7772519d67febb0ceb94d8f22531ea99f0c60c36e67a4f5a497c384f5e0`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf1f761c394ef0da3c3fef1865f52e977d392f3f0b6c0575c3d1341da6cd7e9`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e647346313038e022d4394703013d0963bc45ad0782bcf984166dd279d475c5d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb56fc761a44bdcdde0f2cfaa2a75932b2ac8fe3c78177727284b0f58037fb0`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5797262702f20651c9e1f79f4fbfbe22a260dc9bb7408bf5820eb186b3063f4d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 338.2 KB (338250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cad06e122fd976b54af5acb5a3ba1d1299d61be733e7c2eadeb185aca82942`  
		Last Modified: Wed, 12 Jan 2022 15:14:31 GMT  
		Size: 5.0 MB (4954480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cf217b75c847a9ef63c4cc6093d9aa9c783f67b2c999fb7b23249e80b6e6c`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1f92fb92be2d3b29fc1f42015a4d47bb112ae53db5fab9fa63f432838b7747`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099a82c04f8e6eee73daaccc93d0ad74009ffb4c94eb7d9c8a6a52b4e6bdf2fd`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507bd2ef766612deffd70102b577c1242165b07a8464313f8454713360560c86`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats@sha256:e476d11dde611fc9b39eb6a45798c2e503fa1bfa4ece59509826bfaed6a4cbe1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283541821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084594550a22f2aa624e5b2e740a29366a6846c2e1f194854e6e32270f5f0edb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:57:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Jan 2022 19:57:40 GMT
ENV NATS_DOCKERIZED=1
# Tue, 11 Jan 2022 21:15:53 GMT
ENV NATS_SERVER=2.6.6
# Tue, 11 Jan 2022 21:15:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Tue, 11 Jan 2022 21:15:56 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Tue, 11 Jan 2022 21:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:18:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:18:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 11 Jan 2022 21:18:26 GMT
EXPOSE 4222 6222 8222
# Tue, 11 Jan 2022 21:18:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 11 Jan 2022 21:18:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25aec0a6b64c784bf7521344203ee5def4d38eedfdd68f4b452d3250b5b9ddcf`  
		Last Modified: Tue, 11 Jan 2022 21:19:46 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fffdd310a93f98578e45ffbf8e22c031b37efefcc042f21d2a63c2a77c4ee3`  
		Last Modified: Tue, 11 Jan 2022 21:19:45 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15052497c858a1a8b4a8159d05850fbf43551aad161e61ae0fd6880c46eb4556`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080911a4b1ac40e1f062d68ed70319860e88ecb9abec2aef41d0bc3bae89098d`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e79cea19a92f33c59acbcc8f501e9acdb5985bbad5b03ccd1190848ae1b4cf1`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0544e04ecd7b6afc6366924310fd892736faf1983ea2ee9e40efd31a0ec502`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 337.0 KB (337010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8906d4ca25b04680081cc6af81b8eec86a9756abb72e21ed2785f82372ba7c58`  
		Last Modified: Tue, 11 Jan 2022 21:19:43 GMT  
		Size: 5.0 MB (4988964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a01b43c4c8c06f528a3080b9f4d396d196ff851a603ac22c9ce560c3d5b082`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 2.0 KB (1973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156e4bebcfed633295afa0f9dacd6146736cb7de973581f01931fdf6d5f5ae`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ee9fcf4be90533587d2a54238465fc8f6bad0744784041f675b2e97a93bb9`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e44c694323da6f62bebd7b52b659731c89b1e15c15e5c345ec43e24cba28f7`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
