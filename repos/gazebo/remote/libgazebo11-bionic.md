## `gazebo:libgazebo11-bionic`

```console
$ docker pull gazebo@sha256:1dfc5ff149e1b584cc4cec442d70fba7db920f91291a6fb842d42a87b5930faa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:6109d85fad78f4f4ffa691f000b5f1b8ed818a106127dbc54d0e6130659ccdaa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **547.0 MB (547024971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a1734b55d6f4a93e04f35687c024723d3b7cec7eb143de470be8e192d55123`
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
# Tue, 05 Apr 2022 23:48:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:48:20 GMT
EXPOSE 11345
# Tue, 05 Apr 2022 23:48:20 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 05 Apr 2022 23:48:20 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 05 Apr 2022 23:48:20 GMT
CMD ["gzserver"]
# Tue, 05 Apr 2022 23:50:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.10.2-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:2c431d7c11177733ff15c30100ae180f474d88c34cb00b3f8c79fe5da7dabe57`  
		Last Modified: Wed, 06 Apr 2022 00:01:04 GMT  
		Size: 235.5 MB (235459835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73492b40f3c76e106ff9afdf84d52cc787052f35e079ea144e0ab403a625a5b`  
		Last Modified: Wed, 06 Apr 2022 00:00:36 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13753af572b95750547203eaf266b02918b7d18615e63353aa37152ea7d3daea`  
		Last Modified: Wed, 06 Apr 2022 00:01:49 GMT  
		Size: 269.3 MB (269304017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
