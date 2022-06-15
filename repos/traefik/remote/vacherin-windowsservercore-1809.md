## `traefik:vacherin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:6050e1a959e5f7f70d9655c1c33423b4243b8330b18ec73304d7cfc006d2bf66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `traefik:vacherin-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull traefik@sha256:39a1c92106142906a1e69f743109a06104dbb8edb95b98821a6068f85e5f052a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691661835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a58ac60cb265f532de16fc533a8acf570136e1de7f6fb0c3b685623d0cff9a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:55:33 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.0-rc1/traefik_v2.8.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Jun 2022 22:55:34 GMT
EXPOSE 80
# Wed, 15 Jun 2022 22:55:35 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jun 2022 22:55:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:392089678f8c76a21765fa87bddbf80b250c43a6d2e92420bda721019dda728e`  
		Last Modified: Wed, 15 Jun 2022 22:59:44 GMT  
		Size: 28.4 MB (28376660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fb6cb782ba49713ec55a2006c9ced94da8c532a4c28fa0345faca47e36755b`  
		Last Modified: Wed, 15 Jun 2022 22:59:13 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dda7408b8eb5f0ed018ba688a91b13fe2e0965d01450af0703043a5f87281dc`  
		Last Modified: Wed, 15 Jun 2022 22:59:13 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcaea40ad950c609824906c92a711df3f64b7b589353b68bdd6a550d78a8a2b`  
		Last Modified: Wed, 15 Jun 2022 22:59:13 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
