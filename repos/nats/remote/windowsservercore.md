## `nats:windowsservercore`

```console
$ docker pull nats@sha256:6a5048505a376ddee83a546a4c677bd2c62eaf943530ea64bc946e77b092500c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:df85f652123fd850bc088bf1796ad63e262c83117ef33c913c2324c329e83281
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001923911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba49e1850a02235e7b24a350ba3483aa40adb3e25011cf8af425be0f74d9bb21`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Thu, 10 Aug 2023 01:11:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 10 Aug 2023 02:32:08 GMT
ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:32:09 GMT
ENV NATS_SERVER=2.9.21
# Thu, 10 Aug 2023 02:32:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.21/nats-server-v2.9.21-windows-amd64.zip
# Thu, 10 Aug 2023 02:32:11 GMT
ENV NATS_SERVER_SHASUM=43df40bcf81e819e3467a31c548643439d4200486f3032c61ae4b134243f8796
# Thu, 10 Aug 2023 02:33:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 10 Aug 2023 02:34:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 10 Aug 2023 02:34:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:44 GMT
EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5180b8f5f7c2303ba89717cfa778a2173921ca7efdc058cfd6ed951c6d5ca3`  
		Last Modified: Thu, 10 Aug 2023 01:57:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fed0c598ca0ae763bd83f045a0c9262bf153a47e508b736992d196e2fb47dea`  
		Last Modified: Thu, 10 Aug 2023 02:35:22 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8065a1cb0e804bbb19260f95fcb2ee724ea73de1da4df8e9744f6498cec33d62`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5638bc45d3356ae277d06dab7b839bf52e16bc50a37408b0de976cebfcd1ab`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc44a5e39ba10538d5f0af74a7c7c00bb731116d9f5f8f19b9469e2464baf901`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98483cb493b32b2587f35850b72b5beb7a5354034943519da2056a8b88a51036`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 242.8 KB (242767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678609a7e25485895fffda9b5eea9f940ffc5e5e34155de64f2933803428c0e`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 5.7 MB (5712861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b6362b379d0e5ed852e577058ae198521bd47c70a6654e5bdd24a5fbc7f326`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79936c5c24a0ca205db9a615d4c0113a2e3093ae64cdabc9a8b1fa930327830c`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca71b03ad3cfece28d778d224d9c61ca3dbea97dc6761af0d411ddb0275f965d`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484f29887b314709fa52867baf4fc140ec7488361c38d1811854c07d682c1451`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
