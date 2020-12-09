## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:78cddd38d3c26f2a74454532132969b5fbc9fbff9cc8708cf338c1b33a80c17b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:7a8ab0956821d178ef84f6f10c399d44005ca86dd75378d41a5980979ed24409
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2411449594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146757e90d9c2df66c7933b807c71d62de612813d33a32f15c8d7fdd710ddae`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:36:04 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:02:20 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:02:21 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:02:22 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:02:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:04:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:04:10 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9257be76bd37cad15d45905ec5910266409794a9dbd8a0428174f8b2f352a`  
		Last Modified: Wed, 09 Dec 2020 17:42:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36644685392e418bf32ab96db81c8f6a861b913256c244637d9d3ee45098a9cb`  
		Last Modified: Wed, 09 Dec 2020 23:08:22 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9469bed00eb5f6a5b7c050a1aaee856134ec78bab6076cc793e26dc52ec71fa`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9d451908e3e8ec10448e052cf25767a282312e49e29d2a0b42652cf217e28`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870e3bb830bd8ad9b84a928d2b858be730dcdba8016206ee4aeda623d98754b3`  
		Last Modified: Wed, 09 Dec 2020 23:08:20 GMT  
		Size: 4.8 MB (4843348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d24c0a2fc2b3ecd1b0467794ae95667a29e1bd550bf2bf9c455499839253bc`  
		Last Modified: Wed, 09 Dec 2020 23:08:23 GMT  
		Size: 15.7 MB (15722612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09371bf015245c95ce8d5db6b8d7f90fc6d8527f83101535c8c6af719b628e79`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff8db511e98efbde9cbbf6ecd2d9bd2b73565c7c4e0d24dddeb6edfa2a1875`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13217bf3886546791bd6c26ab23636f9bc595fd80abf1e7d6ab6f10f8613cdee`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull nats-streaming@sha256:33a909f6239f294532f68e91f94655aa881f2c8701293c9963e4b1c85b1a1a52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5790922042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e094a16d960a68e3691347bc7923c1f94b7db31dedb2ef74b9d87436170384`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:38:10 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:27 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:04:28 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:04:28 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:05:39 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:07:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:07:45 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:07:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:07:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d972336c8bcee0026c76e8f199cef405112a70aeef9917f07d2859f15162c1`  
		Last Modified: Wed, 09 Dec 2020 17:42:56 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4f52064be159ebf6d7d967a842e39ae04b53dcf15dd8b582a77af431f81df7`  
		Last Modified: Wed, 09 Dec 2020 23:09:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d1ecc24d286c8499d1698affa71481762f11bb3d4fdd9d35763dcbe94e9e9a`  
		Last Modified: Wed, 09 Dec 2020 23:09:00 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649366889ec5703d27a79142f0331f2a462858d6d6ee2a7c1bd8e426bece4236`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916349c9d6afe29e7418ee0e8f0454bb37038070600eaef872fb7356c1147d0`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 5.5 MB (5528923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e032e6db488d413de3f4681555d2b57bb4472c3b16ed16a5c07f2e921f1ed`  
		Last Modified: Wed, 09 Dec 2020 23:09:01 GMT  
		Size: 16.5 MB (16540005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5c8ab334a9fbf340bbb2d213d16e91599eee98aafa72f7f8fbb6d4d147b27`  
		Last Modified: Wed, 09 Dec 2020 23:08:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db5c24070ad330bcb0f078a2325aba107a3a8615fc004248d02e8e828fa8ce`  
		Last Modified: Wed, 09 Dec 2020 23:08:58 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21108015f9c4f2ee78087806b4ca0582f2618489ed4899b07b6290d743b8ef3d`  
		Last Modified: Wed, 09 Dec 2020 23:08:57 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
