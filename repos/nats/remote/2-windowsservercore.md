## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:01e61321ee0c2a556640c7b04f8aaf24a2e46524bdec3c3b451c81dd170d0825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:9d7b29f769b82966a826e9eebcbff7022824cb343278b2c9dd87014b310f6bc2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2683024603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db44bc7e8ad93293de37107a4b87601bb8241a7d0762deac86c4a40d5ef262f0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 13:44:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Aug 2022 15:27:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:27:51 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 15:27:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 10 Aug 2022 15:27:53 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 10 Aug 2022 15:28:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Aug 2022 15:30:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Aug 2022 15:30:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:08 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da71148bcd96afa7027d6172acee93aad6002bfbe87cadf468260667c09b3a89`  
		Last Modified: Wed, 10 Aug 2022 15:05:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dc1c1069568772f0068cef343e37284e5f5e488dbfc15e037d95bce032d917`  
		Last Modified: Wed, 10 Aug 2022 15:30:56 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890750ec51eb48085268f820e86c5b7ff873ff61875ed2b5df77150e4f667aff`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da392874ede7ff085d580701bc4800047c2c07531b8dfb625241622eaba1995c`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a137a2c60ae08a2536eb110f4f21b9c80f33a03ab2d732da15f5f3de36c588`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf94feb41446a9b0f0b35e7d386675c5b6256a8123327795d03d29f60b9400`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 340.8 KB (340788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab22594d9c79ecf05870151796e0c4df02facc4a9c10e99fcbea268fcbe9886`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 5.0 MB (4957679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143ae888a3c2d7c0f27e7935a85c8a25ef108bb2421c597eea07c8283cf18cbd`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16fcb36242a120d1667323616c739921e5e2ccd627ea85b09d12df62368dc62`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478c487cdfd4835865c12e472c096f810ceb98ae9fa4d8a77c2080b01e22f095`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2414c1290a3b460fc321c6c8630ddd4386a1f7192c489baca687f6ce4bd010e`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
