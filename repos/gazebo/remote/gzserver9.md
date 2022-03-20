## `gazebo:gzserver9`

```console
$ docker pull gazebo@sha256:96983b6917b12ef3943c86ac707e074223a8c2158265c6f301aaddd71cc3f8e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver9` - linux; amd64

```console
$ docker pull gazebo@sha256:9f3a6a90806e52877d6ac44dc92f5e287fbb3d4fc128c070207a417fc64fee72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.4 MB (268423902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba2c88dc88f68ae2ada1c58d74eb457ed2e15e46b1575abe4648fa130daf8ed`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:07:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:50:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:51:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 19 Mar 2022 22:51:08 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 19 Mar 2022 22:53:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 22:53:52 GMT
EXPOSE 11345
# Sat, 19 Mar 2022 22:53:52 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 19 Mar 2022 22:53:52 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 19 Mar 2022 22:53:52 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed186fe30ca85957e7e878753de089d2e8a5010dea43d74e99fb9771929b361`  
		Last Modified: Fri, 18 Mar 2022 09:59:31 GMT  
		Size: 839.0 KB (838975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a80e5c5d6c29949b7e2820fb10ec17dbbce79e0eb8d801154146c76d49b736`  
		Last Modified: Sat, 19 Mar 2022 22:58:15 GMT  
		Size: 14.7 MB (14706225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e65f49de8156f0b8fc422c9f7f5693076ac6e3d476db0b9b22a78cfa49dd5d`  
		Last Modified: Sat, 19 Mar 2022 22:58:11 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf23135115a943a3d07749707e65f5192a7b531cb01c139b051a388a62c0edd3`  
		Last Modified: Sat, 19 Mar 2022 22:58:11 GMT  
		Size: 5.5 KB (5462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63936adb2b2e16e13a7b7646edda5c8f54018391465293cb40b248c2e72ffcd`  
		Last Modified: Sat, 19 Mar 2022 22:58:38 GMT  
		Size: 226.2 MB (226162977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbd1e77752220c1f41de08e78d29e91ce464bd79c5296ef740bc1fa2a6fc220`  
		Last Modified: Sat, 19 Mar 2022 22:58:11 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
