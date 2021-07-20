## `traefik:brie-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0800bdc2a15e93f0683aae5bf987efaf23d801e472fe5313fc8533defc01e75d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `traefik:brie-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull traefik@sha256:045236995cdf41261a60fa3ac576c9793f3901c83ad5e08723aca2385a6893f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712513466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dcc6a0b78bd9bf639119a4f2321a083780be87427eafaccaa36ed9fba67173a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 20 Jul 2021 19:15:43 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.5.0-rc3/traefik_v2.5.0-rc3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 20 Jul 2021 19:15:46 GMT
EXPOSE 80
# Tue, 20 Jul 2021 19:15:49 GMT
ENTRYPOINT ["/traefik"]
# Tue, 20 Jul 2021 19:15:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4796c55f696739ec1ce328d3167fab87b48e4d5f09a052be043233a6a1ad5f`  
		Last Modified: Tue, 20 Jul 2021 19:17:04 GMT  
		Size: 27.1 MB (27061039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bda2e382587cb093b9bab7d0a5250c95a7180debdd090e0e931976d02939cd`  
		Last Modified: Tue, 20 Jul 2021 19:16:32 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc90f65075e51185b1a313af64e566ac0de897a4542f32f0256eabbdefc9274`  
		Last Modified: Tue, 20 Jul 2021 19:16:32 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280a84ee4e02f3017614dc94bd97f0f3f9e8ccc9fdfa04475f406ace8cd07f22`  
		Last Modified: Tue, 20 Jul 2021 19:16:32 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
