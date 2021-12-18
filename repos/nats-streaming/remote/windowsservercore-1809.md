## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:e8717b1af9495be0396d6b91c3b9be076fc62c4d5c27222d253340050d8e70bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:420220a9afa15857377173cc8f141ae0373a42f666d9d133fcf747088a6d87a0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2716755888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e34c0986c57d10e61a41f5d9d253df4fb832be016255f195afb5b747924e636d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:32:10 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 07:59:49 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 07:59:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 07:59:51 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:00:48 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:02:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:02:35 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:36 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d22d2238b031d3f13bcd6c144e80f8f8402332b8ee8e53cc54b7912c3ac808cb`  
		Last Modified: Sat, 18 Dec 2021 03:59:34 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c5f7f5394b88876960b5ac27980fb2e22584cf50ecde4d9537e88ddbf849c3`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4330e24c7d8e5e42a117873554d01f36a0dc5de956de58eb98bc343f3b7053`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85e10ba361bd6036ce996ef1fc18a56eae46bfe2f2a3aa167c91a9910e44b1e`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73619ef7215a1f395f4b26e9d2c8f3163b1eadc526a4b86834c34d2d210bbbb5`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f06960fbd4efa8dc36c8d215c51aa6c8e6adadb62e05f799bc7770a768385`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 365.8 KB (365782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b13efc00f53324e98bc4459fd1a2e6c14d2dbb3ddce59ac2d39a8d2976ead8d`  
		Last Modified: Sat, 18 Dec 2021 08:06:22 GMT  
		Size: 7.8 MB (7774250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbd74dd7052b02b86f232c8f3bc9d759fd4f2a1f81fcf4748927895a03331c`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9da21c0ea9106d6386e5f731911254e0aad700297c81ecb6b7cbc2b22a81e36`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2561dd2bec68b686d5c3e5494fffeb0a77f681864f74eb9fed80413145fbeca2`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
