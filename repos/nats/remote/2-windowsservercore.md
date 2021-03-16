## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:20cf55d646dc015d67cf875917303b92617df0171995ba47d6b618e4e529ac0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:6d99e95fff4ff767ab455c72aa0361e2607d0e869cd0ebc03108d6ebe754a0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480270595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb19c744ee00d943aca95c0fa139702f823a1d2a6c29284a88efbc92dff715`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:15:09 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:15:11 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:15:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:16:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:16:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:16:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c501e38cf1bef759506cac477656d1525304d314d1a87272b2e5a0d9340ec`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3a3e3973ec4905795d6f69337230ae1a3ffa39b5e67e3218240c9d81767f30`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9182aecd18e9366e616d956594c87a9ec12af89cdb5174b5e44491595b993f44`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f873dc755700e152b9e36bdf8e52acd3c0b3f89834258861ec7b63cad2f83e`  
		Last Modified: Mon, 15 Mar 2021 20:21:56 GMT  
		Size: 5.1 MB (5065010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b58dffd304059fbf01e8f232cae78694b01f59492227e635b13f4146e5398de`  
		Last Modified: Mon, 15 Mar 2021 20:21:51 GMT  
		Size: 13.7 MB (13658048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1636b7b5c5e6f053527b20437d39447a1784781d3096d989e47565502c2a24`  
		Last Modified: Mon, 15 Mar 2021 20:21:48 GMT  
		Size: 2.0 KB (1955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec3c66b0dc873dd0d4229a873a8159b0f5cede6052128b2801276a929425d83`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a4f11cb5d2d425ca56aa82fb6143e429ff6b4a1fdce2c446c0cd47c21f8c`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f5314021a971f3e889e272e828fecd71afa4737daaac51ff38997e799940d2`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:dff89ffda8b40b781df892c7c718b15a74e1b36f494dbf2ad90e7452ecc62ff2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817000223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c590e9cb4ced34c77d451c8a89d263bb88a3e585734a8fb8b5b6e757282d49a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:26 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:17:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:18:51 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:20:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:20:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:20:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd615c71b4eb4a71c45a379e363133bbb592ced1d774829054c1bcbf02c424`  
		Last Modified: Mon, 15 Mar 2021 20:22:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de2ae9457cb71c5bb1e8bdb53c2b939780bb3464988803dca8de78d26e6466`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d31805eb5a4d29293c5e38dfdeded0848951ded5074473f16379814ad721dfa`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821fcfe740d7a4d72ebce808af7aab6d489ed0ebb05a3267af44b6ecdd077cf`  
		Last Modified: Mon, 15 Mar 2021 20:22:41 GMT  
		Size: 5.7 MB (5657003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5450f7da02165757aac5e164ed5942b0d00029e6640e4381b387e0e385928f0b`  
		Last Modified: Mon, 15 Mar 2021 20:22:36 GMT  
		Size: 14.4 MB (14419153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcc2db76c93f9eb235e225a970ef65b1af8da4bff671559ed6c69083ebe489`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52e6deb4edd19df80782ba9567175f929679b82d28178ecb8abe5d9148a429d`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b683bc157b68668fb555d38ed7784efab9518ab6d38c3021ffdebac80a849a`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2f56628b687521cdb1e451f56f34abe807cb72da1a00c1c16c00e82adf9702`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
