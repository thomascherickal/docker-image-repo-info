## `gazebo:libgazebo9`

```console
$ docker pull gazebo@sha256:6c1922d778493ea7bf1b7cdc87677fb7703348c07e0fa657052c1aa1d9b7b46f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo9` - linux; amd64

```console
$ docker pull gazebo@sha256:3f93b06aa674b8600dfb828feeb128aa92d1cbf83833724b19abeef656127354
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.8 MB (413822096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7774774c12d1586491b0b79fb3e8f4236b90166f29e97852e5970d2cb6d903e0`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:16:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 22:23:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 22:23:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 31 Jan 2023 22:23:42 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 31 Jan 2023 22:26:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 22:26:59 GMT
EXPOSE 11345
# Tue, 31 Jan 2023 22:26:59 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 31 Jan 2023 22:26:59 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 31 Jan 2023 22:26:59 GMT
CMD ["gzserver"]
# Tue, 31 Jan 2023 22:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo9-dev=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703b06e751e0680eec7a303ffd99a0b6d283044ef8ce1df7aa4f2659738335e`  
		Last Modified: Tue, 31 Jan 2023 20:06:30 GMT  
		Size: 819.0 KB (818957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f00d6665c90db0e4381bb217148ad56fdc75dbff0badd71c6be39e332a2080b`  
		Last Modified: Tue, 31 Jan 2023 22:42:36 GMT  
		Size: 14.7 MB (14711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeff9821033b3e28e6908bfcf7bfd22dceb0772bd9c5225cf0e7f0d252b205a`  
		Last Modified: Tue, 31 Jan 2023 22:42:33 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410c96625d6f0dda084d9d88b90802285121ad66b7c9afdaadfd01ceb058a7bf`  
		Last Modified: Tue, 31 Jan 2023 22:42:34 GMT  
		Size: 5.5 KB (5458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6791092f0bf70394abb38db7eddff689ee2ef9ccc519271eddf2758a5200ebe`  
		Last Modified: Tue, 31 Jan 2023 22:43:01 GMT  
		Size: 226.2 MB (226206756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e501f20a2b368172752d82b86643bca320a79da5527bb9b85f935b131369a1`  
		Last Modified: Tue, 31 Jan 2023 22:42:34 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9715d1b8143ecd1a05516c5ec8dcb714ad2efd85257cd0275209b5ba18896ee`  
		Last Modified: Tue, 31 Jan 2023 22:43:34 GMT  
		Size: 145.4 MB (145366552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
