## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9cfea454a5d6b43341f213ae8515bf3ccf36487967fc16fad686bd3bed667681
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

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
