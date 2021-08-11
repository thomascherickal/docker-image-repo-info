## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:5f9e88c929ff89c3204d105008a059f9be67f540ff96b5bfec99e3b254351411
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:75b04016fe1b2f4c6a7bef238c62f6610c86ab0baed8d1031b7f061053987a27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693987543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc0c1be51519eff598c2d5cce32f011fcfe27c06a9651541cec6796f3f66a56`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 13:42:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:48:51 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:16:00 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:16:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:16:06 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:17:09 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:19:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:19:10 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c613f4c34660a122de754415a884afe6b12172ac3ce792a2e4aae831cc8b2e27`  
		Last Modified: Wed, 11 Aug 2021 16:25:11 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d8e65d39d1b09c34e0dadad1a6b7818f430fb13ce2ff8d70c549b137f9131a`  
		Last Modified: Wed, 11 Aug 2021 16:56:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48fea2e101940ffa36628a8fd4da200aa97417773d993be6df74d0bcff8dccc`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd10110cd94f48fce072addebc384215cfee9e902098952b29a44227fc4c19b`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32d77caa28f59168738bee8473e7e58d117ce711f59589f9627b0facfe620bd`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f9d42ecbcdc48ff53122318c96640c628d9f2b33df84c887b89a1b1429091e`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 351.7 KB (351714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe2bf098cd0e80bd3e81951fb0f411238d63d458bcd51ecd3427a1566fd0ffc`  
		Last Modified: Wed, 11 Aug 2021 21:24:21 GMT  
		Size: 7.6 MB (7626528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e710a2acda7795374f6c855a7d81c6156b961c06f5b0f13fd31e2d8c4952fd6`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2333773eafb1bb6c7fd6fd55fd31614ec447f3b1af48b5f63fe1ee29a4093ff2`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666623a49ff4c5032408abc00ae56261476eed8930351412760fedada9e6e136`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:c2dc8bad14a0594eb6483398e8aa5f20933884855abece46d39a9aaa5ff6c0de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283441295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4dcfbb00a058925aa22ae213359605c8892f3261a0afdd6941153ff9789f841`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 13:57:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:52:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:47 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:19:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:19:53 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:21:16 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:23:38 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:23:41 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:23:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:23:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d6d4b60a6f3b0544427c2eb9a5e27e5f6ddca0fd7632003e11331f01c4e9c6fc`  
		Last Modified: Wed, 11 Aug 2021 16:25:34 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49d3a206649779952cc6a03fdbb4e828336501708ad40c4e1a07237199e28b`  
		Last Modified: Wed, 11 Aug 2021 16:57:38 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6e2dfe14e85c8398dc3f7c7906fb1f7c777ef6d5717fe70d978ad05718ffc2`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f846ec4e42dc3dac55d428bcb2d57cab68f2b659b2cdbba1cad2800b22496145`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073e823edff403699ab0d2dff8376e1b0fb57af79842af3133c0b0c0e3c77f0`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bedf8cee66f4f7e59aee0a000c7fe523b2994d8d7f358c994942fb8b6a9ae6c`  
		Last Modified: Wed, 11 Aug 2021 21:24:57 GMT  
		Size: 338.6 KB (338573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275d8c5f6fbce1b85b62d1f70554f8ecf9d3ccdbfe54c86356703cc697b71e2b`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 12.1 MB (12125382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86e3ac00ba61bf48479b43167f3550a6c8ed7af7da7dd5c0b86441e7d8f662`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45154e30184ba145c5239532f29c91a714e1e6be10588ab43f2dfc69986775e`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254423fab1337576ad61d5fdd3942f86d494a694b38f8c0f779f9239789684b3`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
