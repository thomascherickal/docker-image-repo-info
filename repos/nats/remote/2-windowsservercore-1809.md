## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:2b9c20408baf29df9d8666fc894d8a5c308946331d4310ef5a82b1eed5101db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:ac025e7ac0a2786f5807888399f94d317a0636b60e8a37584569d586fb1ac146
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718991955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007419288bb7b16cd78d29d0476687df2d88011775f13b3f565c92414a214c05`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:14:46 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:14:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.3/nats-server-v2.7.3-windows-amd64.zip
# Fri, 25 Feb 2022 02:14:48 GMT
ENV NATS_SERVER_SHASUM=ddb372da68741d897006c8d4b160c7f4788603cbaacb3fa105ddf7baada04428
# Fri, 25 Feb 2022 02:15:50 GMT
RUN Set-PSDebug -Trace 2
# Fri, 25 Feb 2022 02:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 25 Feb 2022 02:17:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:17 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ed63a799d34b3a151eb2d65afc4a93d028c5308ce305f9059da19083ea4579`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa36020fa0fadcfe9ac785f1bc4cbf6e51ac336a4441d2ea628465f9f1e3832`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58aaa8ed102560150d8bd4fe887000c2789a69df5ae550a8b8058e526d01af34`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48afd20cc6576c9f831f4166f86f4cd65be8140eda5a57159bba0d62c21b1af`  
		Last Modified: Fri, 25 Feb 2022 03:15:12 GMT  
		Size: 374.3 KB (374309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb76be5e45618d5a45f4672ac8e8c8d45d10bf627dc47f3afe45c7909b223b`  
		Last Modified: Fri, 25 Feb 2022 03:15:10 GMT  
		Size: 4.9 MB (4890363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513928aafbffc4a16807de347507df4019d3096da02f3475f8731f6704a0e75d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba5e5368daffd340a50b6715a6d9d28d2f2c341d694c5d7cdae52e15e46d4d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca864d6530840f9fbdc99b6aaedcd8aa7acf319697677ca480fd220d426cb62f`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9cb037cabf38f35bdcf375e13b7790bfdc9b4e9761cd2e865cf557a7575e81`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
