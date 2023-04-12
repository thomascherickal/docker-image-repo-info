## `traefik:banon-windowsservercore-1809`

```console
$ docker pull traefik@sha256:98159a00a75874bbd128722bed10569b284254b421a8c2beb81c4e3ce54c2424
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `traefik:banon-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull traefik@sha256:98cbf00d5a641f29302e7a4755e4dd17d305d9f97debbc695185f7806d0d5528
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2107559263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c07fbcfd91407d318d7620965595e7c01922416c74f39e26b387a3f525dd03cc`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 07:13:32 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.10/traefik_v2.9.10_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 12 Apr 2023 07:13:33 GMT
EXPOSE 80
# Wed, 12 Apr 2023 07:13:34 GMT
ENTRYPOINT ["/traefik"]
# Wed, 12 Apr 2023 07:13:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.10 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359dbcd2ba39b911096f5c7e6e16eccd3f34992d30f85a09b39798629f9b513`  
		Last Modified: Wed, 12 Apr 2023 07:17:04 GMT  
		Size: 36.3 MB (36262674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3adc4f2e465650e5dfac4067f8f8510735c0905044a50118f90efa838edaf0f`  
		Last Modified: Wed, 12 Apr 2023 07:16:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade371f7c339f79b32024bda4543e08a31dbd8c205fbf430d70ae1a5e39f6008`  
		Last Modified: Wed, 12 Apr 2023 07:16:56 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5663c6bca5ff84f04a0ae58c7fff0c20b31b0436b0fb2076916931f7fe77ebb5`  
		Last Modified: Wed, 12 Apr 2023 07:16:56 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
