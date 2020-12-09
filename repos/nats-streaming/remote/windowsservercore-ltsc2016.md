## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:da877310cb87d1822f44a79a76b57af2eceb3e15aa82ab406a47d32bc0de9f47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

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
