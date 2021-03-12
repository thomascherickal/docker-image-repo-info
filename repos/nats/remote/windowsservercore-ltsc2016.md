## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:fc0e60009c5d72028223e66ed67396b935dbfd43b83f7cdb41549190e57bf68b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:66126fdcc8018d2d2f9fbe281188a56efbb436849eb06ce5e2c181eeaa9b619b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816773837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad00d7822043d66e214b8523e52b7beb31d15c68c58cb98c362223663fe7d911`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:57:10 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:57:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:57:12 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:58:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 17:00:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 17:00:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 17:00:31 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 17:00:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 17:00:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58c165493987dd29c1c0acacaf9c0ff15a557060f1848ea26996b9ce21aae0`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78982f85c559dbd12ee3f51b834a0ef77c43acb0f1fff24faf9e389631b96c`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f0d273c80c1dbd9b8813a188e5920191ce2507e40d0350ee441ec34a3e9e3`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5453b687f1986b2e87d86225d728a9feb743157f8cb566b9c1d6d0ce58110e`  
		Last Modified: Wed, 10 Mar 2021 17:02:26 GMT  
		Size: 5.6 MB (5647961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ca39166547ab6aa791b61b8180813822efc34d6f57b9c72f1edacacaa8bac2`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 14.2 MB (14202739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0deae7874091de5a817595e8a5924980e12a421f9d28832257fdad32a4e3f0`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa2fd64751fb1de794b023f59afed0f96ade2d01ddf5dc5f7b58a2688b7b611`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cbeb30ccb829bb2bd06131b3cc0a0b9963ad6c19a65c8ad9f9f7cc8a2f609e`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab7b94c330f979e9c58deccfd61c87f8ab16f439585082237f3f8a83e924aa`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
