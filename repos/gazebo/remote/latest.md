## `gazebo:latest`

```console
$ docker pull gazebo@sha256:98f767e129018b36537c741b16ac29f941c20d38aa01dd0c703f394c6ebd827a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:latest` - linux; amd64

```console
$ docker pull gazebo@sha256:a7fb204920a8c47f40d79ca44e0a1bbf7ac5a6db4e3c288e15dc404c77572a15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.5 MB (610530817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0d69441e73d69797787c5f10d82e567cac3666632d67ea550c398f11b474349`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 02:08:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 02:08:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 02:08:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 02 Dec 2023 02:08:59 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 02 Dec 2023 02:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.14.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 02:13:58 GMT
EXPOSE 11345
# Sat, 02 Dec 2023 02:13:59 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 02 Dec 2023 02:13:59 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 02 Dec 2023 02:13:59 GMT
CMD ["gzserver"]
# Sat, 02 Dec 2023 02:20:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.14.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc1327734170da8c4ae4171fb4248189d0691d6b4a3f01b09239c3e34688651`  
		Last Modified: Sat, 02 Dec 2023 02:20:57 GMT  
		Size: 1.2 MB (1198788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84dd867ca9b97ffec894f23529995ae3df71466b32e7078d8fada607b01d09cf`  
		Last Modified: Sat, 02 Dec 2023 02:20:57 GMT  
		Size: 16.2 MB (16161063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240d02b73937d779dc47b94e4706bdd00946df208a9407a9f1a7eab05d039ca7`  
		Last Modified: Sat, 02 Dec 2023 02:20:54 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16c6e1aed79b417d12a0de26e989d0d51f91917bd091bae2311f0dbcc6bf964`  
		Last Modified: Sat, 02 Dec 2023 02:20:54 GMT  
		Size: 5.5 KB (5501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab2d8196f5d9e94e1b05625b3249595258c6d308ecfa0d46fd33a373d8de6a6`  
		Last Modified: Sat, 02 Dec 2023 02:21:25 GMT  
		Size: 276.1 MB (276065228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cd787e92a814371065e781202ca1d68950e01d33ab54770e740326d2ffac01`  
		Last Modified: Sat, 02 Dec 2023 02:20:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e90fd725f7fa95b47abbc510ae0af9d6ccd7794ca908a12c83a5aabd1df8881`  
		Last Modified: Sat, 02 Dec 2023 02:22:16 GMT  
		Size: 288.5 MB (288514581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
