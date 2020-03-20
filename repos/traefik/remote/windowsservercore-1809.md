## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:4aee458ca67f38c594327c15417266a1de3c2c0b7da10adfc52a9d3281e71226
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull traefik@sha256:3b931df7ee834cd3981b0feed94aa43c270f61cd9b77fe55a521f2b752f53f51
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2289603149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b29a74a7f7c2b1610fac17b8e9a47ce49630ce32c1470e065db828d23d08f1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 19 Mar 2020 23:41:52 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.8/traefik_v2.1.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 19 Mar 2020 23:41:56 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:41:58 GMT
ENTRYPOINT ["/traefik"]
# Thu, 19 Mar 2020 23:41:59 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa08490fed3660037a1b158752b8fe631ad840b0f2907c5fc2485a9e14e43ea3`  
		Last Modified: Thu, 19 Mar 2020 23:42:51 GMT  
		Size: 24.3 MB (24262030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97399e32101679e0af4842e21af256551e26a9ee7a8d9eca1324c30fbf93a627`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142ff7dfc7b934a74d26c9bf367751fab4187d03eb3a4d53a682baf74371f93d`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695d512369d35885c9793f1d4824dae683f03a4f251b460b87c4c52790df131`  
		Last Modified: Thu, 19 Mar 2020 23:42:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
