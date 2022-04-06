## `gazebo:libgazebo9`

```console
$ docker pull gazebo@sha256:aa4ce32559ed2915dc533dac9fd857de43f07b5a1bd11e66814c41baa573dfa9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo9` - linux; amd64

```console
$ docker pull gazebo@sha256:ea013ab479a2c1f05cea6365040ddab815d20331d781014b783edd8f5f633d8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.7 MB (413695887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dbff45a681311891e881c0fe6d5d791570e2ffee4c8231cd51c5e1d2e68e18d`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:41:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:41:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:41:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 05 Apr 2022 23:41:56 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 05 Apr 2022 23:44:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:44:46 GMT
EXPOSE 11345
# Tue, 05 Apr 2022 23:44:46 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 05 Apr 2022 23:44:46 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 05 Apr 2022 23:44:46 GMT
CMD ["gzserver"]
# Tue, 05 Apr 2022 23:47:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo9-dev=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b732c52c0461890d4114ac1d6f5a90dc52c395a65c4bd758b0c8ec6d738eac1`  
		Last Modified: Tue, 05 Apr 2022 23:59:27 GMT  
		Size: 838.9 KB (838902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ee0349f8ecab445a2af42fa41f848d2f0c323366b404e862060a271640d13d`  
		Last Modified: Tue, 05 Apr 2022 23:59:28 GMT  
		Size: 14.7 MB (14706190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42edbaff30f55b10dcaf4867601455a75ede6ef8c86eb3ac2bcb9aa79565bf4`  
		Last Modified: Tue, 05 Apr 2022 23:59:25 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bbd609e23ed6ff073db5196922b7b66cfcfb92734e9ac03c49e00bbcdfa267`  
		Last Modified: Tue, 05 Apr 2022 23:59:25 GMT  
		Size: 5.5 KB (5461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192bd034fe54d6ec56ff7cbc51841c0e06d3d1773f42a6606971636bd3f19cd8`  
		Last Modified: Tue, 05 Apr 2022 23:59:51 GMT  
		Size: 226.2 MB (226162993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb11fa84e67e21225951f283920137efdcc341cef9d89e14a2de8990025decb`  
		Last Modified: Tue, 05 Apr 2022 23:59:25 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6357d1102872fea3d124fec62f9ccf41e0885076a3765a692094dede390a04f4`  
		Last Modified: Wed, 06 Apr 2022 00:00:27 GMT  
		Size: 145.3 MB (145271775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
