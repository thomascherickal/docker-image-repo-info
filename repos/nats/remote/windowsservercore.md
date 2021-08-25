## `nats:windowsservercore`

```console
$ docker pull nats@sha256:a306b6fed9ddc40af4f29308e35543bac76b4a8912f864c07af9b4e8e0b77ca0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:6ccc9955cf40adb8ea2b253b9c6f23ec93119c186698e5ed532d40e6200d614e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691299672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a412cc016f80e4dadbe3a3dc5c2cb6a64665b0e6822a6da3cbb43db4b69bfe4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:05:31 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:06:19 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:07:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:07:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:36 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:07:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce301f5f5d39ac4e8d9bcfbc328bd5b19ba33be4296e36dfaf38b97e237916cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd17b61217b895023497478b1741228ad7221f8c66e6112fad1b40bacc1ce5d`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94970df4678e54913d95980d02d9ff71d30d50a6723c96ec2a2c337d5ec94cc3`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca036463e9405a39d3eecaf7c6d1460f43db9a3fb3a3a8ce3fa2a79129d9859`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 372.2 KB (372161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3001228d4034679deb65e7813f9dad7e0bc52fa0888e3d8aabda79d824feca6`  
		Last Modified: Wed, 25 Aug 2021 16:10:59 GMT  
		Size: 4.9 MB (4916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece4ad52d4d5186da25b2c5ee6ee1dece7dfa1006619a8c8dd61f03203bfb572`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bb136a83c4336ce77e23e25557549ed19968dd767ba7b9d2cc1e844eb6ba5f`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81fc52dc0eca24c32caca4700eda8838cb051b275a5522341356faa175af5f4`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997d37eb36b34583172efc2d68231049fdbe4e1566a53766ab1dd9aeac733a6`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:5f695f38c757cde6d2289cdba59daf5cedbed071bcd3b928c22b955fd45572a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276233135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907eb440adcedcaa19bd8bda99341412fe2a823e1a7d3077d43d16c276523a2b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:08:07 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:08:08 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:08:09 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:08:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:10:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:10:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:10:17 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:10:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:10:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9a660f8d67a5c8b9457024d09e515ec58c8139030455fad6d652311b6efe4`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03452b1283e873ff333ca54ed6173a3903c0ee3a0d275877acbe830baba2300e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d20a02f5d333ae12d83abd2efbb61180409c8fc087bbfae23a15333093bfd`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6996d861cc65b368ae3430040a02f90e24442c11c36ba92e60ca871ea2ea2e4e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 337.3 KB (337279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a3283ad2e2971b500f94eddc08246fe108cd32ace09dc8d975000b95a7ef6`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 4.9 MB (4917237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee3ec74d5606f197fc248615bc3f601b7ead0dfeec128858be0db44a480d5c2`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eee0b51f0797517ba761ef6dbba5511ca115f27a7fed19265c2547da9697b`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec6d361ef3b2338bd83a5d1f88667ceef00c4882ba2b9f425305114c0093802`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac609389baf550f0bab83b6b5bc067bf62486e9bc22d12b12c9d0866fbacb48`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
