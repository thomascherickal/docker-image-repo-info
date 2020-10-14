## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:da571ef250c5edb0bc827882ed50510f5544c83ca042f377ca757dd2bdfe13e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats@sha256:c6745b513657e4cd88add91d5190cd2f436a8656601772df6a93d127cf2dadd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760744682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06be644c4b30a273fa9e9ac950062191f85c180f626cecf6304d4b11dd0c2a02`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:38 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:26:39 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:26:39 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:27:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:29:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:29:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:29:43 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:29:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:29:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a67950e40a28ee038ef7352f74395d34b51ad95977986eb94b4fc675a66b732`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adb0de29d8a18a8f87a6be459adb01ad061744c01626323900842810994d9bd`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5759300f31d593f3bafb4b58d462d6980bbafe93c00b2e26f3f7a5009f6183`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d724370e6153197bcd6fcb34163f448999f5086b5b76b726419e2ba8756fab`  
		Last Modified: Wed, 14 Oct 2020 16:31:38 GMT  
		Size: 5.4 MB (5422970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d6803e1700049865bde5e42a043a685787ef6952b6d294169e31a1e7ad0825`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 14.0 MB (13959179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8052312cc55beca318ec095742d503a659b78b71a6a8f711932998a7d312052`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac373a9054384aece98f8f7964feb2bc8f8c2c13e692c156e775d6fc4b202927`  
		Last Modified: Wed, 14 Oct 2020 16:31:33 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d0a2418aea8509bca4632465c04f864b847472a8da8938186f8f4f22ecb6c`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b32d70dd6bf96bf57929e861e1ef3ce7d6c9e6037332d4858e8cd4e76f6fba`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
