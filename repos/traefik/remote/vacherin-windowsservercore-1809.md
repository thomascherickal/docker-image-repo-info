## `traefik:vacherin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0452c0b7d3b50f73e9eb3fe14d6aea1e711f6893e551b120297714a56ff87497
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `traefik:vacherin-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull traefik@sha256:2b8833b7f478aaea0660b13d76008d9c443d2ca9ede8260a66ddf77ec0dced93
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691946058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d9c077b951799d1719407d6ccf0a6090d7e4d83443cd12c0caf9f434bc9b14`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 27 Jun 2022 18:17:18 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.0-rc2/traefik_v2.8.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 27 Jun 2022 18:17:19 GMT
EXPOSE 80
# Mon, 27 Jun 2022 18:17:20 GMT
ENTRYPOINT ["/traefik"]
# Mon, 27 Jun 2022 18:17:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0627793c2162afa6503cffbc5b8ba07a3595e6afbd36adbce6d742441eedfe14`  
		Last Modified: Mon, 27 Jun 2022 18:19:33 GMT  
		Size: 28.7 MB (28660585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626e3c272bba114d389797970221df5c5d727a4e344654e1051e1b06b0103758`  
		Last Modified: Mon, 27 Jun 2022 18:19:26 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a99af0b984050234a2f65ab1dc7fce35c19bd14abd01a715c1843c2c31fcd7f`  
		Last Modified: Mon, 27 Jun 2022 18:19:26 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea9164ac6cfca8b4cc1e060af7e958fe125cae7beafb2cadbe2ad1698b2e167`  
		Last Modified: Mon, 27 Jun 2022 18:19:26 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
