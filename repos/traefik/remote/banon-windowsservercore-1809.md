## `traefik:banon-windowsservercore-1809`

```console
$ docker pull traefik@sha256:484e4ab12cdfb1c7be97875087e9c973272beee4d346dc325bb2b6d7b342666b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:banon-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:19d30c0ce3b26fc3ef1cbd011b72de5c75ca7f38dedf06463e1f86aafedb3408
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2814326326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d50e607061a7b32e6d0ac3b4d27beddc8c995a76ef1297b925387e03e624e7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 08 Dec 2022 00:18:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.6/traefik_v2.9.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 08 Dec 2022 00:18:23 GMT
EXPOSE 80
# Thu, 08 Dec 2022 00:18:24 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Dec 2022 00:18:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8538d65fe3cfb960b6d01dd8d907de6a6f66063d0c05cdf52f4f0658d6ab0e`  
		Last Modified: Thu, 08 Dec 2022 00:19:32 GMT  
		Size: 35.7 MB (35733843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d57f1f64f20e0fe1bbaf9073780189efacd610e0e72d15890427ec3b3e714`  
		Last Modified: Thu, 08 Dec 2022 00:19:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8274a23157eecf01bc3852248ac8cfacf763a176489e430a03be4b838f4de38`  
		Last Modified: Thu, 08 Dec 2022 00:19:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f657a80dc39b16669260e73e2e16072cd23b1164d0810941fa975ca8970a200b`  
		Last Modified: Thu, 08 Dec 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
