## `gazebo:gzserver11`

```console
$ docker pull gazebo@sha256:e4f09de0559c0a22d7c4c97d0c115e4c1bbac2cb395e49916cf589e9f2e1032d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11` - linux; amd64

```console
$ docker pull gazebo@sha256:d1bee56269c490c2d6f517eddfccec274f2b3e40b72869748327a0fbfa722ebf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321938940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a81fd800592312552ab6aa935278011de17a9ffc9892f3f992aef1b76479f1e`
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
