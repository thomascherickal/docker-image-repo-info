## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:bba033611034c965ca7d6847f4633a856da117d106d76544795f4dd2baeb8cf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:7647918261d11c4129e46342b5ead2bd4a7fe5890a1eabc4c8bc15117a6aafdb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815985063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8351132feba4c7211a1c6494d5aad2d2feca30b631c5c27869149ceae39308cb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:48 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:17:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:17:50 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:19:26 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:21:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:21:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:21:35 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:21:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e486f7d07050146376fe817fbaa36684d4a4c92ba71ce2493904b8e971627`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dfc4c4856991011c03cb36f66e5603195775041170086e915179ae447f12b`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1721d0ded1eec67890352a406e6b14542008bd9e4ab391d56b630212225c21`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d2310fc7f04c4bfa4f3d8c209415d3c4d2e370bcafc6783ac0cb68372df0fd`  
		Last Modified: Thu, 13 May 2021 18:23:13 GMT  
		Size: 5.7 MB (5700657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a505b878f376494baa36819bde8e2ab831b07984e236dd7ecc89ceef04ac5fd`  
		Last Modified: Thu, 13 May 2021 18:23:12 GMT  
		Size: 14.5 MB (14493751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3a5995380bec58fd2f51e5fea55c90abf06ed3fad947ccbee69af0db0728b2`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7058f8afc5efca9f3c7c6958a56aef67b654759c9b1eee80cd7ccd64dca19f29`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70901d0156f2610812331f6382df909c63e125fc2e7170237b34bd4f775feb5`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a85a17ae63e3021a02ae1cd64d1f9c0a1aa8f3c5fedc6c3251caa5c9f98974`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
