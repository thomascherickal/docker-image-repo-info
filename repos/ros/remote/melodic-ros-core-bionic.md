## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:a3b125e1c3878c6b9a9a1fffeeb501440fc8aa95b9fe55e4747857190c2720e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:e63efc8d3dcc12b35471b985ae23584e5f60842f5a91cd2adbdf8b9794e597c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291981786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e529341f61d8acdd4d6a5ee0b19a927dca4ccddc8ff3b18c0a26f4e914a1c18e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:56:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:43:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:44:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 04:44:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 04:44:01 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 04:44:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 04:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:47:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 04:47:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 04:47:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45265e2e7c48feafb38d0b16636d20d32043625dc345459a4518d1d7a29dae6`  
		Last Modified: Fri, 09 Dec 2022 02:14:58 GMT  
		Size: 820.1 KB (820060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b699a755bf153866a23ed8b002a67bfa13848daef2a2a20271b3a60b773a21f`  
		Last Modified: Fri, 09 Dec 2022 05:32:06 GMT  
		Size: 4.9 MB (4877466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37933e70036afa5f68c964920f75d5fe39ba984d38ebe7770057b2a34b7a00f9`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2e60c7740e7e1bfec9c209f6caa06ccc4a6551c996ab69e6f5c1ff461713d`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c9e1d09bba71766986ae6d6f90e24f70b356f807ae63a99ca29f082dd7bcd2`  
		Last Modified: Fri, 09 Dec 2022 05:32:40 GMT  
		Size: 259.6 MB (259570951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bdadb07060e567a2ee23d3f32ea8a446f72688e5c5bb41529772f673b19a84`  
		Last Modified: Fri, 09 Dec 2022 05:32:05 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:5c912d5c5ba14503727abe4ad8027257d321d59b78fd4eca576f9ffaea9e8deb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266247531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d74b49e7f558f88a94a3d8e4940d4e66a40c3139700cce81c1206f67a574ed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:55:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 01:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 01:55:59 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:00:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:00:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:00:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ab6a3ae2c4cb8cc88f2f67c7c5d8184197045fee6f572400f2c04beb49194`  
		Last Modified: Fri, 09 Dec 2022 02:26:20 GMT  
		Size: 820.1 KB (820119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7d65111cb5a3475a8facd7f917c0b13fba32ed3570eadd1ce71053b5523694`  
		Last Modified: Fri, 09 Dec 2022 02:26:19 GMT  
		Size: 4.1 MB (4088517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e82cbb05378b82635152f7aa029757dd51cc28c6ec7eed07739ed4fcd73b0`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17193e3a9e3b6541a582be00109b22f1b2e82120aa95b4240117e37626c4b57`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfe93a9e028c602e8b91af7d9e87182cd0f54f12a3d83af90e4783652a96d43`  
		Last Modified: Fri, 09 Dec 2022 02:26:59 GMT  
		Size: 239.0 MB (239031841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ff685ed8d822c2c0d8df320d574841fdadb694cc7ce39f044a079392141782`  
		Last Modified: Fri, 09 Dec 2022 02:26:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4761e3a78091f3a3b115082988e372ace4f03ae30b7d2d81650f85ec3bc0a8fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281558508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779f48d9a3dd10268a4144638379699a2ae7d0eddb22efdd72b7f4cb1a0108e1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:43 GMT
ADD file:eb8b2914800b2ed866666fbff73c8234f4ac2a5ef01743d6fea0984230c2f464 in / 
# Fri, 09 Dec 2022 01:46:44 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:30:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:30:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 09 Dec 2022 02:30:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LANG=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 09 Dec 2022 02:30:27 GMT
ENV ROS_DISTRO=melodic
# Fri, 09 Dec 2022 02:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:34:34 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 09 Dec 2022 02:34:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 09 Dec 2022 02:34:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:87acad9590b042ceb59687d498c396e9344cf2e381923fecd299555966b14975`  
		Last Modified: Fri, 09 Dec 2022 01:47:46 GMT  
		Size: 23.7 MB (23734135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e110f90dd1bba4514a38610a8039d10fb965153c646cbdcc25e91d7990e944cf`  
		Last Modified: Fri, 09 Dec 2022 03:20:57 GMT  
		Size: 820.0 KB (819953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa421c1eeb6c5699681d3f12f6e9f5234e4ca92d6b3f56bef738bc783551dc19`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 4.5 MB (4460459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e9746700d724bc14303e9dc3b2aa940d786297f633be20289c04478615808f`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efba5c3d42c8e98a599b71910369cbee203810449325cd9c332377b995ff89d1`  
		Last Modified: Fri, 09 Dec 2022 03:20:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b629070abb5a845b61064c328d86cebcb97cd0b3f7756927b021577c1ddd09`  
		Last Modified: Fri, 09 Dec 2022 03:21:29 GMT  
		Size: 252.5 MB (252542114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6edea557a18140384a3ef4aae9de2cbb07dba0c00b8695597f9d6694fa04b4`  
		Last Modified: Fri, 09 Dec 2022 03:20:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
