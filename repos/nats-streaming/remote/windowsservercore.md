## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:ec5485694b1779cf4f4ce8a1564780d6de712def729a7d5e298851d526947b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:86325eedaef260418d499e3f4aa38efa36222bd98e04ffdea4b0d727746fb7f4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2330067385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7b45ae86062070366409305503d8b68e65e8fa8061697c8ef81f1e982dcb95`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:07:08 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:07:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:07:10 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 29 Jul 2020 23:23:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:24:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:24:39 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:24:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 29 Jul 2020 23:24:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c591c0a8170250552e7e384d3a79de15e68f382a34d1e5752c6c7ab0cbfb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1d80c963f67159f6b9cbf927c2fd4bdf00c6f73353f96b1baf98daaa6c7cb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e611a275568f5c39624077dd6209104cd19177aeced5c0b7e0f00e9e7aaa2b`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202d6df3ea1f3b2fc7051935098b72b3090d24fde9a69c97b5f103c7fc9cd862`  
		Last Modified: Wed, 29 Jul 2020 23:29:02 GMT  
		Size: 4.8 MB (4800805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a248918bc673f4346d41d4379399acb43fb4a1b069ac53e2486098f1490a27e`  
		Last Modified: Wed, 29 Jul 2020 23:29:01 GMT  
		Size: 15.1 MB (15065263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066cdde29fcbeca5770a8c97ed67775eaafbc68fa78307f8b0ac54120bf35132`  
		Last Modified: Wed, 29 Jul 2020 23:28:57 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f51cc3d1f42db8ec54c2839535304d121965fb1f5546649ab502c1867783fb`  
		Last Modified: Wed, 29 Jul 2020 23:28:57 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c06f9247e732505ce2543250bbd7a63e96ec3ac17d8990ba05ff113b1c08d`  
		Last Modified: Wed, 29 Jul 2020 23:28:57 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats-streaming@sha256:5e41d77f1cacb2aa068745e5c6e4063c60044b43a8f1f24b46c95bd82bc8c7bf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758642460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7489cee8ddc0fcba42510750637c65e5e4d9defe24d06e00bab10580debada4`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:46 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:09:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:09:48 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 29 Jul 2020 23:26:12 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:28:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:28:24 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:28:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 29 Jul 2020 23:28:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bee39dfb46c142a6dd8c7b99236cd36b36ed56346c403d7be4fb8623f9b8d5`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7de9a5c713789f72af564cdc5f28c0dba85d4b95332f815a7d0ba032170616`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba6847dae4e00016f022ecb49741fecdfb048a3cf945beed074720180415ff`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11e4ca3adc329ef1c19412ebcddb186cff619f30e894d62772b6f777124fa9b`  
		Last Modified: Wed, 29 Jul 2020 23:29:18 GMT  
		Size: 5.4 MB (5389488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3018d98e2176dfee26f60cf0c60f77183161431b01d86f1c2943f3f32669b28a`  
		Last Modified: Wed, 29 Jul 2020 23:29:21 GMT  
		Size: 15.8 MB (15781646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6728e98afe2b6c9ab8bde64249736b9ab492f2b9ac8c7d45dd4b7dadd8f06b69`  
		Last Modified: Wed, 29 Jul 2020 23:29:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98593159d8c5486ba9d33142bbf10fab23c060775080f620aa8199b6b7965736`  
		Last Modified: Wed, 29 Jul 2020 23:29:17 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f91a65067706fd35f9bd86dbfa2f21d6d7c70ccc2ddb58a3601a48405e87d75`  
		Last Modified: Wed, 29 Jul 2020 23:29:16 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
