## `nats:windowsservercore`

```console
$ docker pull nats@sha256:2f83133d0acce8f6e25329cfa1448835465a15f6f6080d3dea01f044b04cdb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e0c232bf30691b8afe55af261d4a01f8639efc585516e1eb09940bb851eb8833
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713683278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0382d02f9daa152fcd1c45024249998399b9334f6099f446e931d98f771aef58`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 04:04:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 04:59:53 GMT
ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:16:03 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.14/nats-server-v2.9.14-windows-amd64.zip
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_SHASUM=b47ca5d88b1a74934145aba3afd6a3b0eee0e543638000cee82b468b8dfbcb3c
# Tue, 07 Feb 2023 02:16:36 GMT
RUN Set-PSDebug -Trace 2
# Tue, 07 Feb 2023 02:17:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 07 Feb 2023 02:17:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:17:47 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:17:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:17:48 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99eee4cf5f23d13a762e719b10916801f19f9df4bd7ff9b4c5cf57133b3dc04`  
		Last Modified: Thu, 12 Jan 2023 04:39:02 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda92ec365568291ec0ef873b055a8b13d2c46244c129bc4cdf81f0e43e1ec8c`  
		Last Modified: Thu, 12 Jan 2023 05:02:27 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddda27c0ef4ad351d1295efe578196d2003caa62b54a6dee81e4765decf322c9`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6375d8bcf5bfd121917c9066a7fc47758ed54929693e46c124d8b34cd701c29`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed0fe5c6e734a1bb638b4e36f3d8cea012a04915c4408581da282286dc6b9ec`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9c44c9456dd05617593616f2a49404163b5d832e2eb53dda03b1e8b59aec7`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 382.7 KB (382704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bcd7fc2e88df50e426c8b75e75d6578f5f036d2f228ed98719dea90187c5db`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 5.3 MB (5343352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9175c6ac4001ff4bc634962943cd35c9bbb984cf1b92653a90a892d15a1bd`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5172837be3b8edccf67687c538bbdc1bfb717ff392a6e6f146469c063e54c0b5`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a5a7bac5f0d37232a1b86033fb3be57356d147b1c8293d8128faf6ac70c63`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de08797cefe4c85eb6dd724a5a14d0c72406c8fce9d081ccf86b41210c6171f`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
