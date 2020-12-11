## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:85bed3a067520da8c97d312ab21802befee7472ee9dc35df45dcc54448d8ad03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:ded61fde5f4d65506c7c25ef5601b61f7be384db7db3ebaf8b934554a35bfbf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300209802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:019b2a27930f1dbdb3cf1c358aac4842233e671468635fa07877b0fd1c0fd26e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:38:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:38:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 11 Dec 2020 19:38:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 11 Dec 2020 19:38:33 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 19:38:33 GMT
ENV LC_ALL=C.UTF-8
# Fri, 11 Dec 2020 19:38:33 GMT
ENV ROS_DISTRO=noetic
# Fri, 11 Dec 2020 19:39:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:39:40 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 11 Dec 2020 19:39:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 11 Dec 2020 19:39:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8976c0b6dafba8e29d428307d1a731a8cf6b1ebef7280ec00f1582e30d70e9bd`  
		Last Modified: Fri, 11 Dec 2020 19:48:43 GMT  
		Size: 10.9 MB (10890369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03728db810730c356cc4e6d117dbb856990d83d8b424404820b83e60d1c0a62f`  
		Last Modified: Fri, 11 Dec 2020 19:48:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c01b817549038fd01886fb541048dc802d51175b3d0280699ef1b4a2ce5826`  
		Last Modified: Fri, 11 Dec 2020 19:48:44 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229b50b83602782324ede7d94e323985fd1bb2769db16f2cbf549387fd7fe41`  
		Last Modified: Fri, 11 Dec 2020 19:49:31 GMT  
		Size: 238.9 MB (238919867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86cd2429c18dcfca36b2d9dc7c45899f54bd706f389805d0ad288196ec67a94`  
		Last Modified: Fri, 11 Dec 2020 19:48:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3af5ae05cba4b6700725717eeb2e937c33685761d1306f3987917c0cecf2188c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244180665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:074dbd295db64160e8c1b72bf0e5c62c8a4e1b87c74709c32f9cc50f753e030d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:04 GMT
ADD file:28343d2066831f0ffb2002914f158698f92b4af6dc16ac22e3d8e9c388c688bb in / 
# Tue, 17 Nov 2020 20:23:05 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 09:27:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 09:27:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 18 Nov 2020 09:27:14 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 18 Nov 2020 09:27:15 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 09:27:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 18 Nov 2020 09:27:17 GMT
ENV ROS_DISTRO=noetic
# Wed, 18 Nov 2020 09:29:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 09:29:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 18 Nov 2020 09:29:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 18 Nov 2020 09:29:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:22518ad4a7da48a5acd01946dad2fbee99e4fca910d23b78cd7e4a16c3bd1e5b`  
		Last Modified: Tue, 17 Nov 2020 20:31:35 GMT  
		Size: 49.2 MB (49179215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0016ba602c48f6ebaa4fc89ef88b2543e0081b204301c8d09c790655e635d418`  
		Last Modified: Wed, 18 Nov 2020 09:51:38 GMT  
		Size: 10.9 MB (10882463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44661561f3ffbc31e4ae03215f7cb7c0cb64819066af65f8aee0c5f103fdf7c8`  
		Last Modified: Wed, 18 Nov 2020 09:51:36 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee70efb1eaf577d44f01bec2a8ca443c1d3a74c230395810bc92fe2b35da0bb`  
		Last Modified: Wed, 18 Nov 2020 09:51:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c5b73ad0576d535dcf95aea891345972ad34120925e401d1eae2e9a7d8e52`  
		Last Modified: Wed, 18 Nov 2020 09:52:29 GMT  
		Size: 184.1 MB (184117149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82c57dce96eaa14614e982c3617dbd9a4f73085d417b220eb5f7faeb79777a9`  
		Last Modified: Wed, 18 Nov 2020 09:51:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
