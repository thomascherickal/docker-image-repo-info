## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:bc53fd4f3c8c41cedca5e96eef4e332448d0e81701e549ea8307d9d9b3ed49bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:57d5184c67e7ffdcc336120392dd9ea88dda6b1e9dd7b64ac696413dfb43d4cb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2392182292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e34fa08d33dac0beea657140566bb92dfda1c443d2a73c7f162ce1b7090f97`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:24:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 03 Nov 2020 00:18:03 GMT
ENV NATS_SERVER=2.1.9
# Tue, 03 Nov 2020 00:18:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Tue, 03 Nov 2020 00:18:05 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Tue, 03 Nov 2020 00:18:35 GMT
RUN Set-PSDebug -Trace 2
# Tue, 03 Nov 2020 00:19:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 03 Nov 2020 00:19:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 03 Nov 2020 00:19:44 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:19:45 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 03 Nov 2020 00:19:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad001e4fbf5cfc7ed201221adacaa53c349e1df3803ec7e47dadb618535d55ab`  
		Last Modified: Wed, 14 Oct 2020 16:30:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a2af87fd33c68c6533923c647759616b3077c1840f5567e460da2748a0f371`  
		Last Modified: Tue, 03 Nov 2020 00:23:47 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ce5e4542999cf9f6d8d7d2dba56cc2039373ce5cdf3780368c2114da0c1149`  
		Last Modified: Tue, 03 Nov 2020 00:23:48 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85345f4503b10e646a64434605b9f55e6afb0bff479b20784e22848d8f12208`  
		Last Modified: Tue, 03 Nov 2020 00:23:47 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb46738109d9434cb2f2f0896119814e5bc46572e8bb932e5cf5aa8bfc466da1`  
		Last Modified: Tue, 03 Nov 2020 00:23:47 GMT  
		Size: 4.8 MB (4841876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eb712ac0a1a1c35352a7dd76105d3b9825f07d8624f5466b265c2d9c583fca`  
		Last Modified: Tue, 03 Nov 2020 00:23:58 GMT  
		Size: 13.2 MB (13239457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af06ba9ee11c3749011a69251193bd540f0665a49f9d61996b33b5e5e4aa2fc8`  
		Last Modified: Tue, 03 Nov 2020 00:23:43 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbda7d22d66e27b2f85513282318e637161a3b5bd02893fe0f10a0ddb05d884f`  
		Last Modified: Tue, 03 Nov 2020 00:23:44 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be43e86601421a995400699fc1d92667899b1d9e1d483c6d9552bc90a1ca6f6`  
		Last Modified: Tue, 03 Nov 2020 00:23:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31096e00a73ce7d918f9598ae3a8b0e2fbf0f2d24521c1ad8e7f8c95165d6c4`  
		Last Modified: Tue, 03 Nov 2020 00:23:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
