## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:f3ea4c55909d3b260e1d6a640115c42ebc240f0c6287bb0e355a0021698ca24e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:553ab1ce45bd46319b5725c4ea4de6b7dcc7f134a9b55e714e4cff3071a28f27
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489015393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db786d738e72eab560c58d9dbbd7cc94652b6b709df212c481bfd1ebe0e6122`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:15:17 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:15:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:15:19 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:15:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:17:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:17:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:14 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:15 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eacc1557a5f598517d44067ac8b634ea5d5e69d42a1617106f9917729a8c379`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa7e8f9ba961758d5a71af29a4a19cf6ca923af4448ae8a6277e1377d51f530`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4079551a9fca404ec9047c7636afa519b4f3c0ce24ffba49c9d4503bb4b4fc1c`  
		Last Modified: Fri, 21 May 2021 01:22:10 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbead1c591568fa5311d9717df9a03bcbc282c2e69bca75ce29d267124440de7`  
		Last Modified: Fri, 21 May 2021 01:22:12 GMT  
		Size: 5.1 MB (5121053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379f226586f2c06e7a584a154bff396271b8bdeea8bb4aa2e8037d6026df831`  
		Last Modified: Fri, 21 May 2021 01:22:19 GMT  
		Size: 9.4 MB (9391861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5225325bfc14a5f9df997fb0fc74c89153de81b9b13ba8bc4cd5f540978d4c`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ab2c552e1b6e47aab0a8ea18011e429db83e3011e396d73a0c5b32b20996ba`  
		Last Modified: Fri, 21 May 2021 01:22:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026cdaadb4db8cdde5c7cea375f57180c5d516d136932d10fd7c44e364a54c31`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db123c2d63b10aa6d21dd4071dfe6a32635e695067a54beb2a94a6a09297c24`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
