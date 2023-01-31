## `gazebo:libgazebo11-focal`

```console
$ docker pull gazebo@sha256:d916004c08902c33355738dcc035e49870bff98594a4d1bbf342817faaeec5b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo11-focal` - linux; amd64

```console
$ docker pull gazebo@sha256:2c445a6bb397f3f8061968548f6614efddb78269d83362ced7855aff7e8f9554
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.4 MB (610438370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6e112ac740f27532610a1ead467b9a34b3dbb5e6b1b2908de0761539f64f19`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 22:33:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 22:33:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 31 Jan 2023 22:33:41 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 31 Jan 2023 22:37:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 22:37:07 GMT
EXPOSE 11345
# Tue, 31 Jan 2023 22:37:07 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 31 Jan 2023 22:37:07 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 31 Jan 2023 22:37:07 GMT
CMD ["gzserver"]
# Tue, 31 Jan 2023 22:42:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.12.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c204f531a951b8674685b1e85469ad0e19991b9793fc97a4610ea51a750e9be4`  
		Last Modified: Tue, 31 Jan 2023 22:45:03 GMT  
		Size: 16.2 MB (16176189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799b63b16d56fa39fcb95148e4282bd57f9eeb0aadb9bd64d4d849b7664a4a8d`  
		Last Modified: Tue, 31 Jan 2023 22:45:00 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1019e74db49c9cff98efb90d242db7020363d6e5ba5c32c71f8338656879d6ee`  
		Last Modified: Tue, 31 Jan 2023 22:45:00 GMT  
		Size: 5.5 KB (5500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b1f24c41c6307f26b070787386a837f82ea0b8d7e57a8fb2ea7e9a17e57315`  
		Last Modified: Tue, 31 Jan 2023 22:45:33 GMT  
		Size: 276.0 MB (276023197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a540ebfd738ccbe9e523d1535c6ebe59e4d89810c03ff64b933f9ab943a4169`  
		Last Modified: Tue, 31 Jan 2023 22:45:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b039eeafb8ccafa1ea31636bd9184d996b983202af6354ba8cdce748a70921`  
		Last Modified: Tue, 31 Jan 2023 22:46:28 GMT  
		Size: 288.5 MB (288499430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
