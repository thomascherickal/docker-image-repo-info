## `gazebo:libgazebo11`

```console
$ docker pull gazebo@sha256:51bee1c9852eedf74c4c9309c1f19268593e31fbd308b3b176c577d4bb5be458
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo11` - linux; amd64

```console
$ docker pull gazebo@sha256:87be20f401a041593225c3d3150d7b545c7e9e84e1867eb9050b25bdb5c3c9b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.4 MB (610428914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78472cf2e273ca87c6ab9f99cc5b9cbd7e0b694a0816e77cbc990e8c71ae1683`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 16:23:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 16:23:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 25 Oct 2022 16:23:49 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 25 Oct 2022 16:27:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 16:27:16 GMT
EXPOSE 11345
# Tue, 25 Oct 2022 16:27:16 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 25 Oct 2022 16:27:16 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 25 Oct 2022 16:27:16 GMT
CMD ["gzserver"]
# Tue, 25 Oct 2022 16:31:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.12.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778f2ed9e43ab2f34b8effd97c264f823bf07e53e2094517b3eedd682a4d37ba`  
		Last Modified: Wed, 26 Oct 2022 16:37:48 GMT  
		Size: 16.2 MB (16181419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4e046ed5d8aed26b3cc2a362aebf04e5c2c644381b15b85e0a14d880b9129b`  
		Last Modified: Wed, 26 Oct 2022 16:37:44 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba1ebdedae980f6556e1d105203aa8d49331eb679c22e26cf1b2561a9fd80d6`  
		Last Modified: Wed, 26 Oct 2022 16:37:45 GMT  
		Size: 5.5 KB (5501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7b2d158870abdadd00adc989a44ff0024d595958682932eb8f188a5ea5a24f`  
		Last Modified: Wed, 26 Oct 2022 16:38:25 GMT  
		Size: 276.0 MB (276022576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf5583419a61e41bd432eff6ce52ed4a721946e46fbc30632bd9af9b8d1368a`  
		Last Modified: Wed, 26 Oct 2022 16:37:44 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d11fad89781b7f46b69f4efcc6c65fefc6ce6156a170c0b06b002f5caf6508`  
		Last Modified: Wed, 26 Oct 2022 16:39:47 GMT  
		Size: 288.5 MB (288476074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
