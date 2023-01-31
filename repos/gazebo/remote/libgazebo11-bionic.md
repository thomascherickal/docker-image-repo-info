## `gazebo:libgazebo11-bionic`

```console
$ docker pull gazebo@sha256:4077a547edbc3b00ab6831df74231348e2d8f1242e2378e5975d7c83c98eace1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:ea08104266dbece6ac0e0038f2724c029239ade815173b9443c99154386f6d22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **547.3 MB (547303284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ffffd27072cac3426220e60a3759dd677da0f3f21e2569e2872202baade634`
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
# Tue, 31 Jan 2023 22:30:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 22:30:48 GMT
EXPOSE 11345
# Tue, 31 Jan 2023 22:30:48 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 31 Jan 2023 22:30:48 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 31 Jan 2023 22:30:48 GMT
CMD ["gzserver"]
# Tue, 31 Jan 2023 22:33:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.12.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:54002f4c0eea58f535bc2f451fd5a9509b204fc8a710ddfdcf0b77278818a4c6`  
		Last Modified: Tue, 31 Jan 2023 22:44:11 GMT  
		Size: 235.6 MB (235581180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a7e168245076e9a521c71698cd6d9712a38865fd208a1b0e01bbd2247755c3`  
		Last Modified: Tue, 31 Jan 2023 22:43:43 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10623ba02324847a603be93c95e271ab7a9eb71ccfbf27cec6b41e975ebbef4`  
		Last Modified: Tue, 31 Jan 2023 22:44:54 GMT  
		Size: 269.5 MB (269473314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
