<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ros`

-	[`ros:foxy`](#rosfoxy)
-	[`ros:foxy-ros-base`](#rosfoxy-ros-base)
-	[`ros:foxy-ros-base-focal`](#rosfoxy-ros-base-focal)
-	[`ros:foxy-ros-core`](#rosfoxy-ros-core)
-	[`ros:foxy-ros-core-focal`](#rosfoxy-ros-core-focal)
-	[`ros:foxy-ros1-bridge`](#rosfoxy-ros1-bridge)
-	[`ros:foxy-ros1-bridge-focal`](#rosfoxy-ros1-bridge-focal)
-	[`ros:galactic`](#rosgalactic)
-	[`ros:galactic-ros-base`](#rosgalactic-ros-base)
-	[`ros:galactic-ros-base-focal`](#rosgalactic-ros-base-focal)
-	[`ros:galactic-ros-core`](#rosgalactic-ros-core)
-	[`ros:galactic-ros-core-focal`](#rosgalactic-ros-core-focal)
-	[`ros:galactic-ros1-bridge`](#rosgalactic-ros1-bridge)
-	[`ros:galactic-ros1-bridge-focal`](#rosgalactic-ros1-bridge-focal)
-	[`ros:latest`](#roslatest)
-	[`ros:melodic`](#rosmelodic)
-	[`ros:melodic-perception`](#rosmelodic-perception)
-	[`ros:melodic-perception-bionic`](#rosmelodic-perception-bionic)
-	[`ros:melodic-robot`](#rosmelodic-robot)
-	[`ros:melodic-robot-bionic`](#rosmelodic-robot-bionic)
-	[`ros:melodic-ros-base`](#rosmelodic-ros-base)
-	[`ros:melodic-ros-base-bionic`](#rosmelodic-ros-base-bionic)
-	[`ros:melodic-ros-core`](#rosmelodic-ros-core)
-	[`ros:melodic-ros-core-bionic`](#rosmelodic-ros-core-bionic)
-	[`ros:noetic`](#rosnoetic)
-	[`ros:noetic-perception`](#rosnoetic-perception)
-	[`ros:noetic-perception-buster`](#rosnoetic-perception-buster)
-	[`ros:noetic-perception-focal`](#rosnoetic-perception-focal)
-	[`ros:noetic-robot`](#rosnoetic-robot)
-	[`ros:noetic-robot-buster`](#rosnoetic-robot-buster)
-	[`ros:noetic-robot-focal`](#rosnoetic-robot-focal)
-	[`ros:noetic-ros-base`](#rosnoetic-ros-base)
-	[`ros:noetic-ros-base-buster`](#rosnoetic-ros-base-buster)
-	[`ros:noetic-ros-base-focal`](#rosnoetic-ros-base-focal)
-	[`ros:noetic-ros-core`](#rosnoetic-ros-core)
-	[`ros:noetic-ros-core-buster`](#rosnoetic-ros-core-buster)
-	[`ros:noetic-ros-core-focal`](#rosnoetic-ros-core-focal)
-	[`ros:rolling`](#rosrolling)
-	[`ros:rolling-ros-base`](#rosrolling-ros-base)
-	[`ros:rolling-ros-base-focal`](#rosrolling-ros-base-focal)
-	[`ros:rolling-ros-core`](#rosrolling-ros-core)
-	[`ros:rolling-ros-core-focal`](#rosrolling-ros-core-focal)
-	[`ros:rolling-ros1-bridge`](#rosrolling-ros1-bridge)
-	[`ros:rolling-ros1-bridge-focal`](#rosrolling-ros1-bridge-focal)

## `ros:foxy`

```console
$ docker pull ros@sha256:7df70a68e8d6963b1e9c87eb4a8bb83987fb50f4ffc5f975a46e2562d8364a03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:2698d8c16d0ed15fbfdbf4a20e453898e2666b63b13dff040dc02d4bb4aac27f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.7 MB (236661450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95c9583cf6d6337f2faf2152edfa50d373b62bcc61607abdc49b1cb27c1327c3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 06:15:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:16:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:16:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:16:01 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:16:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:16:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:16:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 06:16:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a11bd747cd1c0f05aaf05f86b0b071e211e24fee36a2d1eba6287b56c3d495`  
		Last Modified: Fri, 01 Oct 2021 06:27:34 GMT  
		Size: 120.0 MB (119979073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048f14944693ffe48c11da0fab1a89302596d8549c164cbe52e259248057d6e4`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef60063893f6152f6d112c4e75ec931e39cfd94ccbec4dc7259b62f52162cc10`  
		Last Modified: Fri, 01 Oct 2021 06:27:54 GMT  
		Size: 70.8 MB (70844886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e04a47d5f112afff24a90ea8c4cde578be5ca1d6f55b453ca1ccc424451769e`  
		Last Modified: Fri, 01 Oct 2021 06:27:43 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfee6dd2516d9b2bcb3f166d23a07676af3a89c474295b071d2e522487bccb6`  
		Last Modified: Fri, 01 Oct 2021 06:27:43 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5954ec391e927d2012041b8cf4cc36623a8e9f5e5a3e07d3848803c74e6967a6`  
		Last Modified: Fri, 01 Oct 2021 06:27:45 GMT  
		Size: 10.3 MB (10288760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:31d63d88187a2b64f48d06510ece9c247b5cd1ec8f5b2d4cbab7f4dc37679ed7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212760655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb27d3c45f06609d31f288e9fd8d465a62944b0bc2504e1686e8e2537194be7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 04:10:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:11:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:11:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:11:01 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:11:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:11:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:11:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 04:11:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d02714a0c044608ab1f7859767d58d255098ee9cebea2c7c5fab4ff70a31b6c`  
		Last Modified: Fri, 01 Oct 2021 04:24:27 GMT  
		Size: 104.2 MB (104153975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f55c77ae30f9470c54c6ec75c59610b1c692ac602c8d71470e9ced72ae29481`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13085cdbcffdd38531e9a60254d6729a5b0a267c586ee7f0472f27d23a1d307`  
		Last Modified: Fri, 01 Oct 2021 04:24:50 GMT  
		Size: 65.2 MB (65182848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb2811f8bc8e43b7bb19d1f1ff90e57d038989ad87a6c7b9427d908e8f7cd6`  
		Last Modified: Fri, 01 Oct 2021 04:24:40 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492e203009a6a167685712ebfb95726988183e06532dbec90f2ef8840e699e22`  
		Last Modified: Fri, 01 Oct 2021 04:24:39 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea6f51c2e6dcd600f529f77d8bf0dbc012628721de2acf0f203d57ba93ab1b3`  
		Last Modified: Fri, 01 Oct 2021 04:24:41 GMT  
		Size: 9.3 MB (9305836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:7df70a68e8d6963b1e9c87eb4a8bb83987fb50f4ffc5f975a46e2562d8364a03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:2698d8c16d0ed15fbfdbf4a20e453898e2666b63b13dff040dc02d4bb4aac27f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.7 MB (236661450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95c9583cf6d6337f2faf2152edfa50d373b62bcc61607abdc49b1cb27c1327c3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 06:15:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:16:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:16:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:16:01 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:16:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:16:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:16:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 06:16:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a11bd747cd1c0f05aaf05f86b0b071e211e24fee36a2d1eba6287b56c3d495`  
		Last Modified: Fri, 01 Oct 2021 06:27:34 GMT  
		Size: 120.0 MB (119979073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048f14944693ffe48c11da0fab1a89302596d8549c164cbe52e259248057d6e4`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef60063893f6152f6d112c4e75ec931e39cfd94ccbec4dc7259b62f52162cc10`  
		Last Modified: Fri, 01 Oct 2021 06:27:54 GMT  
		Size: 70.8 MB (70844886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e04a47d5f112afff24a90ea8c4cde578be5ca1d6f55b453ca1ccc424451769e`  
		Last Modified: Fri, 01 Oct 2021 06:27:43 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfee6dd2516d9b2bcb3f166d23a07676af3a89c474295b071d2e522487bccb6`  
		Last Modified: Fri, 01 Oct 2021 06:27:43 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5954ec391e927d2012041b8cf4cc36623a8e9f5e5a3e07d3848803c74e6967a6`  
		Last Modified: Fri, 01 Oct 2021 06:27:45 GMT  
		Size: 10.3 MB (10288760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:31d63d88187a2b64f48d06510ece9c247b5cd1ec8f5b2d4cbab7f4dc37679ed7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212760655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb27d3c45f06609d31f288e9fd8d465a62944b0bc2504e1686e8e2537194be7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 04:10:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:11:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:11:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:11:01 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:11:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:11:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:11:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 04:11:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d02714a0c044608ab1f7859767d58d255098ee9cebea2c7c5fab4ff70a31b6c`  
		Last Modified: Fri, 01 Oct 2021 04:24:27 GMT  
		Size: 104.2 MB (104153975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f55c77ae30f9470c54c6ec75c59610b1c692ac602c8d71470e9ced72ae29481`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13085cdbcffdd38531e9a60254d6729a5b0a267c586ee7f0472f27d23a1d307`  
		Last Modified: Fri, 01 Oct 2021 04:24:50 GMT  
		Size: 65.2 MB (65182848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb2811f8bc8e43b7bb19d1f1ff90e57d038989ad87a6c7b9427d908e8f7cd6`  
		Last Modified: Fri, 01 Oct 2021 04:24:40 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492e203009a6a167685712ebfb95726988183e06532dbec90f2ef8840e699e22`  
		Last Modified: Fri, 01 Oct 2021 04:24:39 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea6f51c2e6dcd600f529f77d8bf0dbc012628721de2acf0f203d57ba93ab1b3`  
		Last Modified: Fri, 01 Oct 2021 04:24:41 GMT  
		Size: 9.3 MB (9305836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:7df70a68e8d6963b1e9c87eb4a8bb83987fb50f4ffc5f975a46e2562d8364a03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:2698d8c16d0ed15fbfdbf4a20e453898e2666b63b13dff040dc02d4bb4aac27f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.7 MB (236661450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95c9583cf6d6337f2faf2152edfa50d373b62bcc61607abdc49b1cb27c1327c3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 06:15:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:16:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:16:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:16:01 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:16:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:16:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:16:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 06:16:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a11bd747cd1c0f05aaf05f86b0b071e211e24fee36a2d1eba6287b56c3d495`  
		Last Modified: Fri, 01 Oct 2021 06:27:34 GMT  
		Size: 120.0 MB (119979073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048f14944693ffe48c11da0fab1a89302596d8549c164cbe52e259248057d6e4`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef60063893f6152f6d112c4e75ec931e39cfd94ccbec4dc7259b62f52162cc10`  
		Last Modified: Fri, 01 Oct 2021 06:27:54 GMT  
		Size: 70.8 MB (70844886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e04a47d5f112afff24a90ea8c4cde578be5ca1d6f55b453ca1ccc424451769e`  
		Last Modified: Fri, 01 Oct 2021 06:27:43 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfee6dd2516d9b2bcb3f166d23a07676af3a89c474295b071d2e522487bccb6`  
		Last Modified: Fri, 01 Oct 2021 06:27:43 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5954ec391e927d2012041b8cf4cc36623a8e9f5e5a3e07d3848803c74e6967a6`  
		Last Modified: Fri, 01 Oct 2021 06:27:45 GMT  
		Size: 10.3 MB (10288760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:31d63d88187a2b64f48d06510ece9c247b5cd1ec8f5b2d4cbab7f4dc37679ed7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212760655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb27d3c45f06609d31f288e9fd8d465a62944b0bc2504e1686e8e2537194be7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 04:10:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:11:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:11:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:11:01 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:11:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:11:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:11:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 04:11:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d02714a0c044608ab1f7859767d58d255098ee9cebea2c7c5fab4ff70a31b6c`  
		Last Modified: Fri, 01 Oct 2021 04:24:27 GMT  
		Size: 104.2 MB (104153975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f55c77ae30f9470c54c6ec75c59610b1c692ac602c8d71470e9ced72ae29481`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13085cdbcffdd38531e9a60254d6729a5b0a267c586ee7f0472f27d23a1d307`  
		Last Modified: Fri, 01 Oct 2021 04:24:50 GMT  
		Size: 65.2 MB (65182848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb2811f8bc8e43b7bb19d1f1ff90e57d038989ad87a6c7b9427d908e8f7cd6`  
		Last Modified: Fri, 01 Oct 2021 04:24:40 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492e203009a6a167685712ebfb95726988183e06532dbec90f2ef8840e699e22`  
		Last Modified: Fri, 01 Oct 2021 04:24:39 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea6f51c2e6dcd600f529f77d8bf0dbc012628721de2acf0f203d57ba93ab1b3`  
		Last Modified: Fri, 01 Oct 2021 04:24:41 GMT  
		Size: 9.3 MB (9305836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:8e9098074e85331503dc6644d6158203df77a60776f1328d83ee6901c49aea6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:971b28b6d4e0595f615c6362188b66f003e9e17571cc24798ed7a41ff5d1b2bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155281145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:127b322a603b2a42aea08bdef92c8ce5d6b3f93292788ab143c7a981031d011c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 06:15:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:16:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:16:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:16:01 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a11bd747cd1c0f05aaf05f86b0b071e211e24fee36a2d1eba6287b56c3d495`  
		Last Modified: Fri, 01 Oct 2021 06:27:34 GMT  
		Size: 120.0 MB (119979073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048f14944693ffe48c11da0fab1a89302596d8549c164cbe52e259248057d6e4`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f03c5cfea7fbbec6ac09aaee15eb8c0b436bdc364a0b4eb9732593e6ed040dd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138025307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5969317ce1a30737f8e0e460aa31d369a062d4f2cdf3528755cabc468f301c2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 04:10:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:11:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:11:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:11:01 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d02714a0c044608ab1f7859767d58d255098ee9cebea2c7c5fab4ff70a31b6c`  
		Last Modified: Fri, 01 Oct 2021 04:24:27 GMT  
		Size: 104.2 MB (104153975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f55c77ae30f9470c54c6ec75c59610b1c692ac602c8d71470e9ced72ae29481`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:8e9098074e85331503dc6644d6158203df77a60776f1328d83ee6901c49aea6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:971b28b6d4e0595f615c6362188b66f003e9e17571cc24798ed7a41ff5d1b2bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155281145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:127b322a603b2a42aea08bdef92c8ce5d6b3f93292788ab143c7a981031d011c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 06:15:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:16:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:16:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:16:01 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a11bd747cd1c0f05aaf05f86b0b071e211e24fee36a2d1eba6287b56c3d495`  
		Last Modified: Fri, 01 Oct 2021 06:27:34 GMT  
		Size: 120.0 MB (119979073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048f14944693ffe48c11da0fab1a89302596d8549c164cbe52e259248057d6e4`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f03c5cfea7fbbec6ac09aaee15eb8c0b436bdc364a0b4eb9732593e6ed040dd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138025307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5969317ce1a30737f8e0e460aa31d369a062d4f2cdf3528755cabc468f301c2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 04:10:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:11:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:11:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:11:01 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d02714a0c044608ab1f7859767d58d255098ee9cebea2c7c5fab4ff70a31b6c`  
		Last Modified: Fri, 01 Oct 2021 04:24:27 GMT  
		Size: 104.2 MB (104153975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f55c77ae30f9470c54c6ec75c59610b1c692ac602c8d71470e9ced72ae29481`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:cab0bb769bd317f011dc12d3facdca69f1fba414b2a7f3ae200641097bc09529
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:8f88647e50c42f9547aed07e6221d36c940d3eafa5ab5af8c2a9d145988e8f40
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.5 MB (345516519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:894b70088b436277c4539f27a1d07ec70a49f0a5117ad7e582e04f26c65bca40`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:36:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:37:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:51:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 04:51:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 04:51:14 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Aug 2021 04:52:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:52:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 04:52:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:52:14 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:52:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:52:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:52:56 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 04:53:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:53:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 04:53:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:53:26 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 04:53:26 GMT
ENV ROS2_DISTRO=foxy
# Tue, 31 Aug 2021 04:53:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:54:08 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a41ae3b013398d2c13b5bceb3338e9582560c6d0ffd908463d766628be0a9c`  
		Last Modified: Tue, 31 Aug 2021 05:02:39 GMT  
		Size: 1.2 MB (1182916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8296a87df0b7498eeb5c80b365dfd866191372bea87427717ea787d78a5a7`  
		Last Modified: Tue, 31 Aug 2021 05:02:37 GMT  
		Size: 5.5 MB (5547451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f6733b55cc5feea2d4ee150c8dea08c02292286df2ded324ce1cce11cafe5e`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a37fcb7b853af691c37b315d95d9c1f6192ce41615e3588a9a36e174207371`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df88af5f8567a6f2cbdc3288e39989bafc21e16e19c1d0b21ec421155ba9d237`  
		Last Modified: Tue, 31 Aug 2021 05:05:42 GMT  
		Size: 120.0 MB (119973947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5d11ffe6ed85c308c8f7f83eb6779e2f81b2ce6c1328f73073878bc370843a`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee662a194237d1061dfbe6700abce9590c93e1d7c9fdc2c8030642fe89c07a`  
		Last Modified: Tue, 31 Aug 2021 05:06:03 GMT  
		Size: 70.8 MB (70844284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bba301f8377dd61e4e0a5652dea9356c35c590a01f73b857f8f9ee364e8a7`  
		Last Modified: Tue, 31 Aug 2021 05:05:53 GMT  
		Size: 240.5 KB (240536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e54ad7e3a8e61b43a65537755c95964771958deaa3af31dfd1a3b366ceeb99`  
		Last Modified: Tue, 31 Aug 2021 05:05:53 GMT  
		Size: 2.0 KB (2032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f52ad208f27349b733c344754e7d5177833503ac3b8823c6416f1dba05b5707`  
		Last Modified: Tue, 31 Aug 2021 05:05:55 GMT  
		Size: 10.3 MB (10283858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768b198d04340eb2ebf05156bc4b5f86c6a05d3360700100c75a80dd9976da47`  
		Last Modified: Tue, 31 Aug 2021 05:06:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36cb26c992a114bd50224b9eea9b3fabef4528c8ac1b1491b05d4d6a1886ea9`  
		Last Modified: Tue, 31 Aug 2021 05:06:22 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3e679549c9b0594b5dc1323db3cde02472a4fa2cc4dbcfad2f3925034f8e62`  
		Last Modified: Tue, 31 Aug 2021 05:06:36 GMT  
		Size: 76.1 MB (76133180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec1e759c05a811f810316f756889904a777305840694dbce8d41616fffb2e66`  
		Last Modified: Tue, 31 Aug 2021 05:06:28 GMT  
		Size: 32.7 MB (32735199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c41e2713c687f7c56f2f408e1063cd8756038afc615615f4238b2c28aa2667`  
		Last Modified: Tue, 31 Aug 2021 05:06:22 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c8524cea13cd0d60ab079d11f926b595139ae0f1b8a6ca8e78fc386fd4683ecc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (314037710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23ba52270226f4808eb5db842151fb54102254f2f869045e283b3d00cba56c0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:35:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 02:40:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 02:40:15 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Aug 2021 02:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:56 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 02:40:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 02:40:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:41:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 02:41:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 02:41:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 02:42:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:42:02 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 02:42:02 GMT
ENV ROS2_DISTRO=foxy
# Tue, 31 Aug 2021 02:42:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:42:43 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b869ca97320a7af4e9ce7c382543a1b04a7005c70779507cbb85ace89adde42e`  
		Last Modified: Tue, 31 Aug 2021 02:52:34 GMT  
		Size: 1.2 MB (1183579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c7b498b8e70b033b401f685710eb46ada1aab199891dfe061488eb0ba40831`  
		Last Modified: Tue, 31 Aug 2021 02:52:32 GMT  
		Size: 5.5 MB (5512786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153e16b4767757045ca5abd59a845a7b7cbc2916b1d1a63d930661eec9fc232b`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e90d25ecd370ffb201a02739df5a10f437fb2d2c95060875411cf40d5d0e12`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac2567afd7f21270eaf5dac9596df45b6dda0b77d64188744a7081a5f346b5`  
		Last Modified: Tue, 31 Aug 2021 02:55:58 GMT  
		Size: 104.2 MB (104162618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e0daf045c79605e6b79149e30817a2a6a12ee94bd746d4ddbf97b159b86d9f`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053652fdf77cf09c2d5f748e1392a941b0a2640722c2e70d661cb0f79ed668cf`  
		Last Modified: Tue, 31 Aug 2021 02:56:20 GMT  
		Size: 65.2 MB (65183560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aedc85ca67006659dbfc2b17452494645c1f0e417864446282ae6f592dc634e`  
		Last Modified: Tue, 31 Aug 2021 02:56:10 GMT  
		Size: 240.5 KB (240543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf81879f4a40b97c2359dafad0f780449e33d1663620a7c84e6edc1d195e3e4`  
		Last Modified: Tue, 31 Aug 2021 02:56:09 GMT  
		Size: 2.0 KB (2024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68fc5fc59c2a35f0a91dba364f8820a1bdf634a40ffa0598d351cb20b4af65a`  
		Last Modified: Tue, 31 Aug 2021 02:56:11 GMT  
		Size: 9.3 MB (9298963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd3283cc3a3d0b05c08fbf8f9dd92a0d58882e3d3f4b30ad40605ca33f18330`  
		Last Modified: Tue, 31 Aug 2021 02:56:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3042d28ddb6bf62c8b0e1e54bc0d10a513a2f5c9b3a1f4202288198c324738d`  
		Last Modified: Tue, 31 Aug 2021 02:56:39 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c80802dfb985bc5e968ed325b0300ccc446bdd9de54b7af679333b9ebc11c74`  
		Last Modified: Tue, 31 Aug 2021 02:56:55 GMT  
		Size: 76.2 MB (76167513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d418353022c19184ddb5003057db95c611277d1f1bf4d789fab26eea7b08d5`  
		Last Modified: Tue, 31 Aug 2021 02:56:44 GMT  
		Size: 25.1 MB (25109980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1457cde4b44826bb5c7364ac964c0eea2aa3fb528fc1a5a935aec01b6be8bcf`  
		Last Modified: Tue, 31 Aug 2021 02:56:39 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:cab0bb769bd317f011dc12d3facdca69f1fba414b2a7f3ae200641097bc09529
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:8f88647e50c42f9547aed07e6221d36c940d3eafa5ab5af8c2a9d145988e8f40
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.5 MB (345516519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:894b70088b436277c4539f27a1d07ec70a49f0a5117ad7e582e04f26c65bca40`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:36:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:37:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:51:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 04:51:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 04:51:14 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Aug 2021 04:52:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:52:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 04:52:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:52:14 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:52:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:52:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:52:56 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 04:53:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:53:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 04:53:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:53:26 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 04:53:26 GMT
ENV ROS2_DISTRO=foxy
# Tue, 31 Aug 2021 04:53:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:54:08 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a41ae3b013398d2c13b5bceb3338e9582560c6d0ffd908463d766628be0a9c`  
		Last Modified: Tue, 31 Aug 2021 05:02:39 GMT  
		Size: 1.2 MB (1182916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8296a87df0b7498eeb5c80b365dfd866191372bea87427717ea787d78a5a7`  
		Last Modified: Tue, 31 Aug 2021 05:02:37 GMT  
		Size: 5.5 MB (5547451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f6733b55cc5feea2d4ee150c8dea08c02292286df2ded324ce1cce11cafe5e`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a37fcb7b853af691c37b315d95d9c1f6192ce41615e3588a9a36e174207371`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df88af5f8567a6f2cbdc3288e39989bafc21e16e19c1d0b21ec421155ba9d237`  
		Last Modified: Tue, 31 Aug 2021 05:05:42 GMT  
		Size: 120.0 MB (119973947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5d11ffe6ed85c308c8f7f83eb6779e2f81b2ce6c1328f73073878bc370843a`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ee662a194237d1061dfbe6700abce9590c93e1d7c9fdc2c8030642fe89c07a`  
		Last Modified: Tue, 31 Aug 2021 05:06:03 GMT  
		Size: 70.8 MB (70844284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bba301f8377dd61e4e0a5652dea9356c35c590a01f73b857f8f9ee364e8a7`  
		Last Modified: Tue, 31 Aug 2021 05:05:53 GMT  
		Size: 240.5 KB (240536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e54ad7e3a8e61b43a65537755c95964771958deaa3af31dfd1a3b366ceeb99`  
		Last Modified: Tue, 31 Aug 2021 05:05:53 GMT  
		Size: 2.0 KB (2032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f52ad208f27349b733c344754e7d5177833503ac3b8823c6416f1dba05b5707`  
		Last Modified: Tue, 31 Aug 2021 05:05:55 GMT  
		Size: 10.3 MB (10283858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768b198d04340eb2ebf05156bc4b5f86c6a05d3360700100c75a80dd9976da47`  
		Last Modified: Tue, 31 Aug 2021 05:06:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36cb26c992a114bd50224b9eea9b3fabef4528c8ac1b1491b05d4d6a1886ea9`  
		Last Modified: Tue, 31 Aug 2021 05:06:22 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3e679549c9b0594b5dc1323db3cde02472a4fa2cc4dbcfad2f3925034f8e62`  
		Last Modified: Tue, 31 Aug 2021 05:06:36 GMT  
		Size: 76.1 MB (76133180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec1e759c05a811f810316f756889904a777305840694dbce8d41616fffb2e66`  
		Last Modified: Tue, 31 Aug 2021 05:06:28 GMT  
		Size: 32.7 MB (32735199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c41e2713c687f7c56f2f408e1063cd8756038afc615615f4238b2c28aa2667`  
		Last Modified: Tue, 31 Aug 2021 05:06:22 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c8524cea13cd0d60ab079d11f926b595139ae0f1b8a6ca8e78fc386fd4683ecc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (314037710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23ba52270226f4808eb5db842151fb54102254f2f869045e283b3d00cba56c0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:35:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 02:40:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 02:40:15 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Aug 2021 02:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:56 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 02:40:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 02:40:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:41:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 02:41:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 02:41:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 02:42:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:42:02 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 02:42:02 GMT
ENV ROS2_DISTRO=foxy
# Tue, 31 Aug 2021 02:42:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:42:43 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b869ca97320a7af4e9ce7c382543a1b04a7005c70779507cbb85ace89adde42e`  
		Last Modified: Tue, 31 Aug 2021 02:52:34 GMT  
		Size: 1.2 MB (1183579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c7b498b8e70b033b401f685710eb46ada1aab199891dfe061488eb0ba40831`  
		Last Modified: Tue, 31 Aug 2021 02:52:32 GMT  
		Size: 5.5 MB (5512786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153e16b4767757045ca5abd59a845a7b7cbc2916b1d1a63d930661eec9fc232b`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e90d25ecd370ffb201a02739df5a10f437fb2d2c95060875411cf40d5d0e12`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac2567afd7f21270eaf5dac9596df45b6dda0b77d64188744a7081a5f346b5`  
		Last Modified: Tue, 31 Aug 2021 02:55:58 GMT  
		Size: 104.2 MB (104162618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e0daf045c79605e6b79149e30817a2a6a12ee94bd746d4ddbf97b159b86d9f`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053652fdf77cf09c2d5f748e1392a941b0a2640722c2e70d661cb0f79ed668cf`  
		Last Modified: Tue, 31 Aug 2021 02:56:20 GMT  
		Size: 65.2 MB (65183560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aedc85ca67006659dbfc2b17452494645c1f0e417864446282ae6f592dc634e`  
		Last Modified: Tue, 31 Aug 2021 02:56:10 GMT  
		Size: 240.5 KB (240543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf81879f4a40b97c2359dafad0f780449e33d1663620a7c84e6edc1d195e3e4`  
		Last Modified: Tue, 31 Aug 2021 02:56:09 GMT  
		Size: 2.0 KB (2024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68fc5fc59c2a35f0a91dba364f8820a1bdf634a40ffa0598d351cb20b4af65a`  
		Last Modified: Tue, 31 Aug 2021 02:56:11 GMT  
		Size: 9.3 MB (9298963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd3283cc3a3d0b05c08fbf8f9dd92a0d58882e3d3f4b30ad40605ca33f18330`  
		Last Modified: Tue, 31 Aug 2021 02:56:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3042d28ddb6bf62c8b0e1e54bc0d10a513a2f5c9b3a1f4202288198c324738d`  
		Last Modified: Tue, 31 Aug 2021 02:56:39 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c80802dfb985bc5e968ed325b0300ccc446bdd9de54b7af679333b9ebc11c74`  
		Last Modified: Tue, 31 Aug 2021 02:56:55 GMT  
		Size: 76.2 MB (76167513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d418353022c19184ddb5003057db95c611277d1f1bf4d789fab26eea7b08d5`  
		Last Modified: Tue, 31 Aug 2021 02:56:44 GMT  
		Size: 25.1 MB (25109980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1457cde4b44826bb5c7364ac964c0eea2aa3fb528fc1a5a935aec01b6be8bcf`  
		Last Modified: Tue, 31 Aug 2021 02:56:39 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:2d92486cfb3ed94398eecca3d5c4f216575de4dea5cca38fd12ac90336fa636b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:9648d0d7c95527560f0c41900d1e6b3017f328b8e0402f4e4c494762a577342c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232087757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db669bad6bdfd484e6ccb224c0f8bb78bde84b0c8d743f5d5958264074133972`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:17:26 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 06:18:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:18:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:18:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:18:13 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:18:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:18:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:18:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 06:18:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9822a4f6cce53e502f5d2f90766f69c34822c58ef403536e917a5764f0da7c1`  
		Last Modified: Fri, 01 Oct 2021 06:28:28 GMT  
		Size: 103.6 MB (103627341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851399abce02bb2417f097f4b9e221270de786a2e80c2dc8fcbcfb1cb020ba9a`  
		Last Modified: Fri, 01 Oct 2021 06:28:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81845ac1fa58515b9795aeefc552c8a929f48198138cb17f53148898b37db19e`  
		Last Modified: Fri, 01 Oct 2021 06:28:48 GMT  
		Size: 70.8 MB (70797034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83a67c347309cd372427e3d88709d763e70bd64603af459c3e065606f6b0d17`  
		Last Modified: Fri, 01 Oct 2021 06:28:38 GMT  
		Size: 249.8 KB (249784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e77d775d64408c5f419496bdf6e2ee24eacebeaecb4d36500bee1674f36fc8b`  
		Last Modified: Fri, 01 Oct 2021 06:28:37 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18f89042f2ee52694a46d3e2f87640f9e83749213cc8a4fc0572ee0b3ae3837`  
		Last Modified: Fri, 01 Oct 2021 06:28:41 GMT  
		Size: 22.1 MB (22109474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f0e90ba0022309fe9329fab449ae8db5fdabb6bb12193d8afa44463e4187dd0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220717384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27fec039201ed58727d4d8d24c313fd9555fb766694c66d9872c6d671371d69f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:12:32 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 04:13:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:13:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:13:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:13:15 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:13:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:13:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:13:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 04:14:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54decf9b73cbac297a45e39fb0f0a1737a8362434870dc3738d10beb0a2889d`  
		Last Modified: Fri, 01 Oct 2021 04:25:29 GMT  
		Size: 100.0 MB (100019555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5222af82eed2e3ce5f12efb7bf53fe5a36cd902d1aad23496451e2e5b7008cb`  
		Last Modified: Fri, 01 Oct 2021 04:25:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1f8d464e088a93212124cc454a911291a90ebc0ceda7bb008739d2119535f7`  
		Last Modified: Fri, 01 Oct 2021 04:25:51 GMT  
		Size: 65.1 MB (65138949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4301f82170ff301ec6d7a6d31f6ef80b4501f39487513306f4f62791138a5f1`  
		Last Modified: Fri, 01 Oct 2021 04:25:41 GMT  
		Size: 249.8 KB (249786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47eff13df5f05b0c2b5cb0dc41452eb70f262a0d7c7015a119a3e9a2ca88fea8`  
		Last Modified: Fri, 01 Oct 2021 04:25:41 GMT  
		Size: 2.0 KB (2017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe2fb84e643657d9e97cf57c6b4e045801fc7253d8f9a9b93e9494e73073487`  
		Last Modified: Fri, 01 Oct 2021 04:25:44 GMT  
		Size: 21.4 MB (21435746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:2d92486cfb3ed94398eecca3d5c4f216575de4dea5cca38fd12ac90336fa636b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:9648d0d7c95527560f0c41900d1e6b3017f328b8e0402f4e4c494762a577342c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232087757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db669bad6bdfd484e6ccb224c0f8bb78bde84b0c8d743f5d5958264074133972`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:17:26 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 06:18:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:18:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:18:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:18:13 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:18:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:18:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:18:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 06:18:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9822a4f6cce53e502f5d2f90766f69c34822c58ef403536e917a5764f0da7c1`  
		Last Modified: Fri, 01 Oct 2021 06:28:28 GMT  
		Size: 103.6 MB (103627341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851399abce02bb2417f097f4b9e221270de786a2e80c2dc8fcbcfb1cb020ba9a`  
		Last Modified: Fri, 01 Oct 2021 06:28:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81845ac1fa58515b9795aeefc552c8a929f48198138cb17f53148898b37db19e`  
		Last Modified: Fri, 01 Oct 2021 06:28:48 GMT  
		Size: 70.8 MB (70797034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83a67c347309cd372427e3d88709d763e70bd64603af459c3e065606f6b0d17`  
		Last Modified: Fri, 01 Oct 2021 06:28:38 GMT  
		Size: 249.8 KB (249784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e77d775d64408c5f419496bdf6e2ee24eacebeaecb4d36500bee1674f36fc8b`  
		Last Modified: Fri, 01 Oct 2021 06:28:37 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18f89042f2ee52694a46d3e2f87640f9e83749213cc8a4fc0572ee0b3ae3837`  
		Last Modified: Fri, 01 Oct 2021 06:28:41 GMT  
		Size: 22.1 MB (22109474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f0e90ba0022309fe9329fab449ae8db5fdabb6bb12193d8afa44463e4187dd0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220717384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27fec039201ed58727d4d8d24c313fd9555fb766694c66d9872c6d671371d69f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:12:32 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 04:13:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:13:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:13:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:13:15 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:13:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:13:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:13:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 04:14:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54decf9b73cbac297a45e39fb0f0a1737a8362434870dc3738d10beb0a2889d`  
		Last Modified: Fri, 01 Oct 2021 04:25:29 GMT  
		Size: 100.0 MB (100019555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5222af82eed2e3ce5f12efb7bf53fe5a36cd902d1aad23496451e2e5b7008cb`  
		Last Modified: Fri, 01 Oct 2021 04:25:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1f8d464e088a93212124cc454a911291a90ebc0ceda7bb008739d2119535f7`  
		Last Modified: Fri, 01 Oct 2021 04:25:51 GMT  
		Size: 65.1 MB (65138949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4301f82170ff301ec6d7a6d31f6ef80b4501f39487513306f4f62791138a5f1`  
		Last Modified: Fri, 01 Oct 2021 04:25:41 GMT  
		Size: 249.8 KB (249786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47eff13df5f05b0c2b5cb0dc41452eb70f262a0d7c7015a119a3e9a2ca88fea8`  
		Last Modified: Fri, 01 Oct 2021 04:25:41 GMT  
		Size: 2.0 KB (2017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe2fb84e643657d9e97cf57c6b4e045801fc7253d8f9a9b93e9494e73073487`  
		Last Modified: Fri, 01 Oct 2021 04:25:44 GMT  
		Size: 21.4 MB (21435746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:2d92486cfb3ed94398eecca3d5c4f216575de4dea5cca38fd12ac90336fa636b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:9648d0d7c95527560f0c41900d1e6b3017f328b8e0402f4e4c494762a577342c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232087757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db669bad6bdfd484e6ccb224c0f8bb78bde84b0c8d743f5d5958264074133972`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:17:26 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 06:18:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:18:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:18:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:18:13 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:18:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:18:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:18:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 06:18:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9822a4f6cce53e502f5d2f90766f69c34822c58ef403536e917a5764f0da7c1`  
		Last Modified: Fri, 01 Oct 2021 06:28:28 GMT  
		Size: 103.6 MB (103627341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851399abce02bb2417f097f4b9e221270de786a2e80c2dc8fcbcfb1cb020ba9a`  
		Last Modified: Fri, 01 Oct 2021 06:28:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81845ac1fa58515b9795aeefc552c8a929f48198138cb17f53148898b37db19e`  
		Last Modified: Fri, 01 Oct 2021 06:28:48 GMT  
		Size: 70.8 MB (70797034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83a67c347309cd372427e3d88709d763e70bd64603af459c3e065606f6b0d17`  
		Last Modified: Fri, 01 Oct 2021 06:28:38 GMT  
		Size: 249.8 KB (249784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e77d775d64408c5f419496bdf6e2ee24eacebeaecb4d36500bee1674f36fc8b`  
		Last Modified: Fri, 01 Oct 2021 06:28:37 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18f89042f2ee52694a46d3e2f87640f9e83749213cc8a4fc0572ee0b3ae3837`  
		Last Modified: Fri, 01 Oct 2021 06:28:41 GMT  
		Size: 22.1 MB (22109474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f0e90ba0022309fe9329fab449ae8db5fdabb6bb12193d8afa44463e4187dd0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220717384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27fec039201ed58727d4d8d24c313fd9555fb766694c66d9872c6d671371d69f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:12:32 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 04:13:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:13:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:13:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:13:15 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:13:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:13:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:13:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 04:14:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54decf9b73cbac297a45e39fb0f0a1737a8362434870dc3738d10beb0a2889d`  
		Last Modified: Fri, 01 Oct 2021 04:25:29 GMT  
		Size: 100.0 MB (100019555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5222af82eed2e3ce5f12efb7bf53fe5a36cd902d1aad23496451e2e5b7008cb`  
		Last Modified: Fri, 01 Oct 2021 04:25:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1f8d464e088a93212124cc454a911291a90ebc0ceda7bb008739d2119535f7`  
		Last Modified: Fri, 01 Oct 2021 04:25:51 GMT  
		Size: 65.1 MB (65138949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4301f82170ff301ec6d7a6d31f6ef80b4501f39487513306f4f62791138a5f1`  
		Last Modified: Fri, 01 Oct 2021 04:25:41 GMT  
		Size: 249.8 KB (249786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47eff13df5f05b0c2b5cb0dc41452eb70f262a0d7c7015a119a3e9a2ca88fea8`  
		Last Modified: Fri, 01 Oct 2021 04:25:41 GMT  
		Size: 2.0 KB (2017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe2fb84e643657d9e97cf57c6b4e045801fc7253d8f9a9b93e9494e73073487`  
		Last Modified: Fri, 01 Oct 2021 04:25:44 GMT  
		Size: 21.4 MB (21435746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:4e2809cdcc7af59431e0d7a2078e94b2441812ea8b6f905c7e27e143f2689241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:ca6d08f25fc4045ab6badd6401e4f48b41df0392c18b75acd63e10a611ecae48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138929413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459837a92d8240e96cdcdfa7a775c3e626fc7703324ae049861a215467f2b863`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:17:26 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 06:18:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:18:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:18:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:18:13 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9822a4f6cce53e502f5d2f90766f69c34822c58ef403536e917a5764f0da7c1`  
		Last Modified: Fri, 01 Oct 2021 06:28:28 GMT  
		Size: 103.6 MB (103627341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851399abce02bb2417f097f4b9e221270de786a2e80c2dc8fcbcfb1cb020ba9a`  
		Last Modified: Fri, 01 Oct 2021 06:28:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3b0fdd8bf86851bd4da361bfb1d9b5fdb989f169b1a756366a7952bde75ae273
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133890886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea9506a9ae0089fae05bac2076051fb643004efc0d0f3af33486b90af02baba`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:12:32 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 04:13:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:13:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:13:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:13:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54decf9b73cbac297a45e39fb0f0a1737a8362434870dc3738d10beb0a2889d`  
		Last Modified: Fri, 01 Oct 2021 04:25:29 GMT  
		Size: 100.0 MB (100019555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5222af82eed2e3ce5f12efb7bf53fe5a36cd902d1aad23496451e2e5b7008cb`  
		Last Modified: Fri, 01 Oct 2021 04:25:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:4e2809cdcc7af59431e0d7a2078e94b2441812ea8b6f905c7e27e143f2689241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:ca6d08f25fc4045ab6badd6401e4f48b41df0392c18b75acd63e10a611ecae48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138929413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459837a92d8240e96cdcdfa7a775c3e626fc7703324ae049861a215467f2b863`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:17:26 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 06:18:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:18:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:18:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:18:13 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9822a4f6cce53e502f5d2f90766f69c34822c58ef403536e917a5764f0da7c1`  
		Last Modified: Fri, 01 Oct 2021 06:28:28 GMT  
		Size: 103.6 MB (103627341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851399abce02bb2417f097f4b9e221270de786a2e80c2dc8fcbcfb1cb020ba9a`  
		Last Modified: Fri, 01 Oct 2021 06:28:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3b0fdd8bf86851bd4da361bfb1d9b5fdb989f169b1a756366a7952bde75ae273
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133890886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea9506a9ae0089fae05bac2076051fb643004efc0d0f3af33486b90af02baba`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:12:32 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 04:13:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:13:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:13:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:13:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54decf9b73cbac297a45e39fb0f0a1737a8362434870dc3738d10beb0a2889d`  
		Last Modified: Fri, 01 Oct 2021 04:25:29 GMT  
		Size: 100.0 MB (100019555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5222af82eed2e3ce5f12efb7bf53fe5a36cd902d1aad23496451e2e5b7008cb`  
		Last Modified: Fri, 01 Oct 2021 04:25:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:adacb9799830b22fe8a6a5650a7c81a36fa0a2c7a1aa34472ddef67c52039aef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:d89be531d646c8e82d7dfbb3ca7dfd7f9335363994b55614101f722813881d39
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326880801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7812a078c618dd4dcfb36b221e873d5a670deb26c8dfb961eb3075a916ba42`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:36:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:37:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:51:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 04:51:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 04:54:18 GMT
ENV ROS_DISTRO=galactic
# Tue, 31 Aug 2021 04:55:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:55:02 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 04:55:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:55:03 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:55:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:55:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:55:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 04:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:56:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 04:56:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:56:07 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 04:56:08 GMT
ENV ROS2_DISTRO=galactic
# Tue, 31 Aug 2021 04:56:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:56:43 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a41ae3b013398d2c13b5bceb3338e9582560c6d0ffd908463d766628be0a9c`  
		Last Modified: Tue, 31 Aug 2021 05:02:39 GMT  
		Size: 1.2 MB (1182916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8296a87df0b7498eeb5c80b365dfd866191372bea87427717ea787d78a5a7`  
		Last Modified: Tue, 31 Aug 2021 05:02:37 GMT  
		Size: 5.5 MB (5547451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f6733b55cc5feea2d4ee150c8dea08c02292286df2ded324ce1cce11cafe5e`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a37fcb7b853af691c37b315d95d9c1f6192ce41615e3588a9a36e174207371`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efb944408b964105643d544dff0dc733eb8d44ed1de5b8b96a59fce413301b7`  
		Last Modified: Tue, 31 Aug 2021 05:07:04 GMT  
		Size: 103.6 MB (103635163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6430b8a0fe47d0895611bc815af1176487e40d10ecfa0c664b5cf278eb64329`  
		Last Modified: Tue, 31 Aug 2021 05:06:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d291c6bb9e0790320805a2525a26a3e2641c8af6c9a2e31b471fe3d65a00fd2a`  
		Last Modified: Tue, 31 Aug 2021 05:07:26 GMT  
		Size: 70.8 MB (70797909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55bf8bc67c6b36b8c4779cf9095d44baac5dca1f0e681df5d871b5dd1d7598`  
		Last Modified: Tue, 31 Aug 2021 05:07:16 GMT  
		Size: 245.0 KB (245018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2db00f36100999ddf906185f71203edcc71ced81d7357356cb674401a7a135`  
		Last Modified: Tue, 31 Aug 2021 05:07:16 GMT  
		Size: 2.0 KB (2024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1236b10237bb3e0a0bdbbcfc0be50417bcd7a0d003f5d31eac0eb12b146896b9`  
		Last Modified: Tue, 31 Aug 2021 05:07:23 GMT  
		Size: 22.1 MB (22108557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8e0df54953596c16dc36daeb3691b791b14cf9e04ba8734e31828a7285895c`  
		Last Modified: Tue, 31 Aug 2021 05:07:40 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a29bf8f81bb48cbcc321ad02c8677d5151e2076c4cc4fb2410f5e7cc1a5459`  
		Last Modified: Tue, 31 Aug 2021 05:07:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc32a80cea910fa49d27fa3ef8a06747f16e654d59a78d348e5f4dacb8b4bfc`  
		Last Modified: Tue, 31 Aug 2021 05:07:54 GMT  
		Size: 78.4 MB (78425289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e88331304f4b116379d4fea65bfc04f8077c27c230c5906925931be4d08d841`  
		Last Modified: Tue, 31 Aug 2021 05:07:43 GMT  
		Size: 16.4 MB (16363360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9597f00570c0fc4a2a273dbbd44d6c1647c1751d05a36bc3a1ae474ae37ad87`  
		Last Modified: Tue, 31 Aug 2021 05:07:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ee3aaa53b5dd9b2f6c0676fdb499beb43d3aa6eb5e7def7a7594da50b85f135c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.0 MB (314996851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9498f260b5eed9c2e2bdae18ec2ac543e03c00e6e934a013f8e6b3f148abe78`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:35:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 02:40:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 02:42:53 GMT
ENV ROS_DISTRO=galactic
# Tue, 31 Aug 2021 02:43:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:43:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 02:43:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 02:43:33 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:44:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:44:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 02:44:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 02:44:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:44:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 02:44:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:44:46 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 02:44:46 GMT
ENV ROS2_DISTRO=galactic
# Tue, 31 Aug 2021 02:45:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:45:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:45:21 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b869ca97320a7af4e9ce7c382543a1b04a7005c70779507cbb85ace89adde42e`  
		Last Modified: Tue, 31 Aug 2021 02:52:34 GMT  
		Size: 1.2 MB (1183579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c7b498b8e70b033b401f685710eb46ada1aab199891dfe061488eb0ba40831`  
		Last Modified: Tue, 31 Aug 2021 02:52:32 GMT  
		Size: 5.5 MB (5512786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153e16b4767757045ca5abd59a845a7b7cbc2916b1d1a63d930661eec9fc232b`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e90d25ecd370ffb201a02739df5a10f437fb2d2c95060875411cf40d5d0e12`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d77fc4622ebe94f4dbfef84290640d2b0a8cb645e806937cae119da66e0a32c`  
		Last Modified: Tue, 31 Aug 2021 02:57:26 GMT  
		Size: 100.0 MB (100037845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a1ce4ccd8df8c236b714872e85748b5011a9c784f1308d3e8b7cde6d55cdcf`  
		Last Modified: Tue, 31 Aug 2021 02:57:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f71bfc8c301186b7c6a5b38b04e91f5b5a52d664b2f8270051b08e762181c`  
		Last Modified: Tue, 31 Aug 2021 02:57:48 GMT  
		Size: 65.1 MB (65138271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44554f0d6a1dfdf9fb1da0b542b9e1bcbbecca7421118b2a705e78f5b956b609`  
		Last Modified: Tue, 31 Aug 2021 02:57:38 GMT  
		Size: 245.0 KB (245012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217cf8322ac9a1b82365a9710371636864d32637d22bd1d637b2bb97c4ddd306`  
		Last Modified: Tue, 31 Aug 2021 02:57:38 GMT  
		Size: 2.0 KB (2016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120720b5aa2190a67c0c60941709cb411d04a7bc7e208f954115857ef0529410`  
		Last Modified: Tue, 31 Aug 2021 02:57:41 GMT  
		Size: 21.4 MB (21435306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000b79fc3753c17e268692b74af07168e20ef832f41c2b6d51aa4ebdc9b0b584`  
		Last Modified: Tue, 31 Aug 2021 02:58:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcfa3302fc9ef900d7b52b011d213d5500e493f37186bf49394b21ab8667ad9`  
		Last Modified: Tue, 31 Aug 2021 02:58:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267cbfb8468f5b8c83aa8a80301a114a9cfbf2fa9ceecbfbc4199761e9d3a022`  
		Last Modified: Tue, 31 Aug 2021 02:58:21 GMT  
		Size: 78.4 MB (78375726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d60cd931079f2558a9451c7b49abf36df676a1d533d65e6a646fe8b96549293`  
		Last Modified: Tue, 31 Aug 2021 02:58:07 GMT  
		Size: 15.9 MB (15890170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9e59276ccde1a327278f910f28b22a92d0e79cfa1b7b11a53e064f99baab37`  
		Last Modified: Tue, 31 Aug 2021 02:58:04 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:adacb9799830b22fe8a6a5650a7c81a36fa0a2c7a1aa34472ddef67c52039aef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:d89be531d646c8e82d7dfbb3ca7dfd7f9335363994b55614101f722813881d39
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326880801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7812a078c618dd4dcfb36b221e873d5a670deb26c8dfb961eb3075a916ba42`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:36:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:37:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:51:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 04:51:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 04:54:18 GMT
ENV ROS_DISTRO=galactic
# Tue, 31 Aug 2021 04:55:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:55:02 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 04:55:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:55:03 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:55:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:55:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:55:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 04:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:56:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 04:56:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:56:07 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 04:56:08 GMT
ENV ROS2_DISTRO=galactic
# Tue, 31 Aug 2021 04:56:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:56:43 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a41ae3b013398d2c13b5bceb3338e9582560c6d0ffd908463d766628be0a9c`  
		Last Modified: Tue, 31 Aug 2021 05:02:39 GMT  
		Size: 1.2 MB (1182916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8296a87df0b7498eeb5c80b365dfd866191372bea87427717ea787d78a5a7`  
		Last Modified: Tue, 31 Aug 2021 05:02:37 GMT  
		Size: 5.5 MB (5547451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f6733b55cc5feea2d4ee150c8dea08c02292286df2ded324ce1cce11cafe5e`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a37fcb7b853af691c37b315d95d9c1f6192ce41615e3588a9a36e174207371`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efb944408b964105643d544dff0dc733eb8d44ed1de5b8b96a59fce413301b7`  
		Last Modified: Tue, 31 Aug 2021 05:07:04 GMT  
		Size: 103.6 MB (103635163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6430b8a0fe47d0895611bc815af1176487e40d10ecfa0c664b5cf278eb64329`  
		Last Modified: Tue, 31 Aug 2021 05:06:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d291c6bb9e0790320805a2525a26a3e2641c8af6c9a2e31b471fe3d65a00fd2a`  
		Last Modified: Tue, 31 Aug 2021 05:07:26 GMT  
		Size: 70.8 MB (70797909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55bf8bc67c6b36b8c4779cf9095d44baac5dca1f0e681df5d871b5dd1d7598`  
		Last Modified: Tue, 31 Aug 2021 05:07:16 GMT  
		Size: 245.0 KB (245018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2db00f36100999ddf906185f71203edcc71ced81d7357356cb674401a7a135`  
		Last Modified: Tue, 31 Aug 2021 05:07:16 GMT  
		Size: 2.0 KB (2024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1236b10237bb3e0a0bdbbcfc0be50417bcd7a0d003f5d31eac0eb12b146896b9`  
		Last Modified: Tue, 31 Aug 2021 05:07:23 GMT  
		Size: 22.1 MB (22108557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8e0df54953596c16dc36daeb3691b791b14cf9e04ba8734e31828a7285895c`  
		Last Modified: Tue, 31 Aug 2021 05:07:40 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a29bf8f81bb48cbcc321ad02c8677d5151e2076c4cc4fb2410f5e7cc1a5459`  
		Last Modified: Tue, 31 Aug 2021 05:07:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc32a80cea910fa49d27fa3ef8a06747f16e654d59a78d348e5f4dacb8b4bfc`  
		Last Modified: Tue, 31 Aug 2021 05:07:54 GMT  
		Size: 78.4 MB (78425289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e88331304f4b116379d4fea65bfc04f8077c27c230c5906925931be4d08d841`  
		Last Modified: Tue, 31 Aug 2021 05:07:43 GMT  
		Size: 16.4 MB (16363360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9597f00570c0fc4a2a273dbbd44d6c1647c1751d05a36bc3a1ae474ae37ad87`  
		Last Modified: Tue, 31 Aug 2021 05:07:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ee3aaa53b5dd9b2f6c0676fdb499beb43d3aa6eb5e7def7a7594da50b85f135c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.0 MB (314996851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9498f260b5eed9c2e2bdae18ec2ac543e03c00e6e934a013f8e6b3f148abe78`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:35:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 02:40:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 02:42:53 GMT
ENV ROS_DISTRO=galactic
# Tue, 31 Aug 2021 02:43:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:43:33 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 02:43:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 02:43:33 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:44:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:44:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 02:44:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 02:44:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:44:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 02:44:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:44:46 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 02:44:46 GMT
ENV ROS2_DISTRO=galactic
# Tue, 31 Aug 2021 02:45:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:45:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:45:21 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b869ca97320a7af4e9ce7c382543a1b04a7005c70779507cbb85ace89adde42e`  
		Last Modified: Tue, 31 Aug 2021 02:52:34 GMT  
		Size: 1.2 MB (1183579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c7b498b8e70b033b401f685710eb46ada1aab199891dfe061488eb0ba40831`  
		Last Modified: Tue, 31 Aug 2021 02:52:32 GMT  
		Size: 5.5 MB (5512786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153e16b4767757045ca5abd59a845a7b7cbc2916b1d1a63d930661eec9fc232b`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e90d25ecd370ffb201a02739df5a10f437fb2d2c95060875411cf40d5d0e12`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d77fc4622ebe94f4dbfef84290640d2b0a8cb645e806937cae119da66e0a32c`  
		Last Modified: Tue, 31 Aug 2021 02:57:26 GMT  
		Size: 100.0 MB (100037845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a1ce4ccd8df8c236b714872e85748b5011a9c784f1308d3e8b7cde6d55cdcf`  
		Last Modified: Tue, 31 Aug 2021 02:57:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f71bfc8c301186b7c6a5b38b04e91f5b5a52d664b2f8270051b08e762181c`  
		Last Modified: Tue, 31 Aug 2021 02:57:48 GMT  
		Size: 65.1 MB (65138271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44554f0d6a1dfdf9fb1da0b542b9e1bcbbecca7421118b2a705e78f5b956b609`  
		Last Modified: Tue, 31 Aug 2021 02:57:38 GMT  
		Size: 245.0 KB (245012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217cf8322ac9a1b82365a9710371636864d32637d22bd1d637b2bb97c4ddd306`  
		Last Modified: Tue, 31 Aug 2021 02:57:38 GMT  
		Size: 2.0 KB (2016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120720b5aa2190a67c0c60941709cb411d04a7bc7e208f954115857ef0529410`  
		Last Modified: Tue, 31 Aug 2021 02:57:41 GMT  
		Size: 21.4 MB (21435306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000b79fc3753c17e268692b74af07168e20ef832f41c2b6d51aa4ebdc9b0b584`  
		Last Modified: Tue, 31 Aug 2021 02:58:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcfa3302fc9ef900d7b52b011d213d5500e493f37186bf49394b21ab8667ad9`  
		Last Modified: Tue, 31 Aug 2021 02:58:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267cbfb8468f5b8c83aa8a80301a114a9cfbf2fa9ceecbfbc4199761e9d3a022`  
		Last Modified: Tue, 31 Aug 2021 02:58:21 GMT  
		Size: 78.4 MB (78375726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d60cd931079f2558a9451c7b49abf36df676a1d533d65e6a646fe8b96549293`  
		Last Modified: Tue, 31 Aug 2021 02:58:07 GMT  
		Size: 15.9 MB (15890170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9e59276ccde1a327278f910f28b22a92d0e79cfa1b7b11a53e064f99baab37`  
		Last Modified: Tue, 31 Aug 2021 02:58:04 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:7df70a68e8d6963b1e9c87eb4a8bb83987fb50f4ffc5f975a46e2562d8364a03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:2698d8c16d0ed15fbfdbf4a20e453898e2666b63b13dff040dc02d4bb4aac27f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.7 MB (236661450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95c9583cf6d6337f2faf2152edfa50d373b62bcc61607abdc49b1cb27c1327c3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 06:15:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:16:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:16:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:16:01 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:16:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:16:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:16:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 06:16:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a11bd747cd1c0f05aaf05f86b0b071e211e24fee36a2d1eba6287b56c3d495`  
		Last Modified: Fri, 01 Oct 2021 06:27:34 GMT  
		Size: 120.0 MB (119979073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048f14944693ffe48c11da0fab1a89302596d8549c164cbe52e259248057d6e4`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef60063893f6152f6d112c4e75ec931e39cfd94ccbec4dc7259b62f52162cc10`  
		Last Modified: Fri, 01 Oct 2021 06:27:54 GMT  
		Size: 70.8 MB (70844886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e04a47d5f112afff24a90ea8c4cde578be5ca1d6f55b453ca1ccc424451769e`  
		Last Modified: Fri, 01 Oct 2021 06:27:43 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfee6dd2516d9b2bcb3f166d23a07676af3a89c474295b071d2e522487bccb6`  
		Last Modified: Fri, 01 Oct 2021 06:27:43 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5954ec391e927d2012041b8cf4cc36623a8e9f5e5a3e07d3848803c74e6967a6`  
		Last Modified: Fri, 01 Oct 2021 06:27:45 GMT  
		Size: 10.3 MB (10288760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:31d63d88187a2b64f48d06510ece9c247b5cd1ec8f5b2d4cbab7f4dc37679ed7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212760655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb27d3c45f06609d31f288e9fd8d465a62944b0bc2504e1686e8e2537194be7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 04:10:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:11:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:11:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:11:01 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:11:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:11:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:11:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 04:11:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d02714a0c044608ab1f7859767d58d255098ee9cebea2c7c5fab4ff70a31b6c`  
		Last Modified: Fri, 01 Oct 2021 04:24:27 GMT  
		Size: 104.2 MB (104153975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f55c77ae30f9470c54c6ec75c59610b1c692ac602c8d71470e9ced72ae29481`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13085cdbcffdd38531e9a60254d6729a5b0a267c586ee7f0472f27d23a1d307`  
		Last Modified: Fri, 01 Oct 2021 04:24:50 GMT  
		Size: 65.2 MB (65182848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bb2811f8bc8e43b7bb19d1f1ff90e57d038989ad87a6c7b9427d908e8f7cd6`  
		Last Modified: Fri, 01 Oct 2021 04:24:40 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492e203009a6a167685712ebfb95726988183e06532dbec90f2ef8840e699e22`  
		Last Modified: Fri, 01 Oct 2021 04:24:39 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea6f51c2e6dcd600f529f77d8bf0dbc012628721de2acf0f203d57ba93ab1b3`  
		Last Modified: Fri, 01 Oct 2021 04:24:41 GMT  
		Size: 9.3 MB (9305836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:59f8ccd0305997c7c04c2ce734f061c6397a6f3d9982213de543a604a6dee1d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:6c99c80a97d9a6af8b830bd34c028e9a80d42138ab0d4ab9bfa78998c70c0954
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437374863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38caaa68c7ca79c4d362762f7247e2c807a9fd5f853a02aaae4e98b234c997e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:4b03d0e396887e99d465986c4abfcd28905e49492a9e65e48441a3c9cdc61d09
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385877981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65627f7ecb5effc290e9142cd68a86e1569dc3d79418a996161e3642bc50be1b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:47:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:48:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:48:06 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Aug 2021 03:51:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:51:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 03:51:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 03:51:21 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:52:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:52:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 03:53:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238fe4a9f5df4e59f4023f55c9904022b1bdc28c161ea1b0ccf7a0b0bf159ea7`  
		Last Modified: Tue, 31 Aug 2021 04:10:26 GMT  
		Size: 841.6 KB (841608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78204c8eec602e32c9035dbc573e847360a19233f2ffb88986618007712d52d9`  
		Last Modified: Tue, 31 Aug 2021 04:10:25 GMT  
		Size: 4.1 MB (4085868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ed86067b04c16476ddd5611175e233b1c1e9408b27ff5a5f7a75431933258a`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ba9e954473c22356b0980776ea31e72b79943027dc7a29cac0f59129662b26`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4872c59956163dc6560b62d05f0cfd3793ac76bfb638f96095e2622f23f81`  
		Last Modified: Tue, 31 Aug 2021 04:12:54 GMT  
		Size: 238.9 MB (238928640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16905b6ec851712f2f3247be87cadaeb78cdfb5b08d02ea181191e79e9562f88`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ba3a4202a313aceb5938c0aab8fba9f6dfda0c8d5994438331f57c3b723338`  
		Last Modified: Tue, 31 Aug 2021 04:13:37 GMT  
		Size: 54.7 MB (54695246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1794a46b1abe6ac50735c089db696c8f8da6ed7ac93088db09865fe88000de`  
		Last Modified: Tue, 31 Aug 2021 04:13:08 GMT  
		Size: 271.5 KB (271530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd9ba48b098a5f33eb9599d6f4b04f96360528ddd85dad5a8e2125716c6d2`  
		Last Modified: Tue, 31 Aug 2021 04:13:53 GMT  
		Size: 64.7 MB (64746191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8225d01167dfc81e8f524b9d72d3c2003b852121e54c0ec322e072f8e3cced54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411949279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb78205244108ca568a249807c4b5d93b0d41239e3703caa55ddccd9f4a0c2fb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:00:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 04:02:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:02:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:02:09 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:02:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:03:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703f9076c62d6a07ee4ac54a13d0cfcd29417e872bc88f5c170a4e31b2ee627`  
		Last Modified: Fri, 01 Oct 2021 04:18:40 GMT  
		Size: 841.5 KB (841467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f51453d2a9542a8e5552ed549fba6110526e6bba0d7dea78077ce930818d1`  
		Last Modified: Fri, 01 Oct 2021 04:18:39 GMT  
		Size: 4.5 MB (4453801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb854bd2d2160569f154fad52e3911260b4110a70c0410645d76246ddfd97ff5`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766db03a07190e4dc3fa1dee3a3ae601d2ff84f341678f1e723e096b1af877f`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91559fa0ccbc5993e820912de1e62ef86dde1022279bf6c2ea3ce22578dea1b4`  
		Last Modified: Fri, 01 Oct 2021 04:19:20 GMT  
		Size: 252.4 MB (252369365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022e4617917637f78d14e5e0ff5a67b9753ffd80528ab27ecc82078077d34d5c`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b78d023404d4cc6eb0e0116d7fe33f110d3d0037ab5a281daa0d867334ca48`  
		Last Modified: Fri, 01 Oct 2021 04:19:41 GMT  
		Size: 63.1 MB (63059707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a48409877036295323cd98bb5f3afdc9846c782bcea495aa268883a29d486aa`  
		Last Modified: Fri, 01 Oct 2021 04:19:32 GMT  
		Size: 273.0 KB (272994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb389997238be58731cc3f21699b7db36a2acba2c488fa7407bad3d48a40ec1e`  
		Last Modified: Fri, 01 Oct 2021 04:19:43 GMT  
		Size: 67.2 MB (67222055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:21b02d9f86b74f93061b47a0e6249e8117244f84cecc35da06efe748828d10a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:073274ee3ed4b8853373529777dc094d60f8a7690085cd8789f67e16608e3762
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742504012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eb9859ebf79cd993bb8f61e0a64932761983cf954bb32eb0dfb1220002a0958`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:01:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d2455ea11a3f51289e515125af2fd29538c49291c3d9de5bf605c367fd146c`  
		Last Modified: Fri, 01 Oct 2021 06:24:17 GMT  
		Size: 305.1 MB (305129149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:0d0b271cefece9d849742e548b1afcd6fbec30fd01d71a41b2469ffe80c0d3ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.8 MB (645755710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:475371a853eaad75e2747a0825878fb9487b24decd736155c7bfe08c830b60b0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:47:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:48:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:48:06 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Aug 2021 03:51:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:51:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 03:51:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 03:51:21 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:52:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:52:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 03:53:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:57:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238fe4a9f5df4e59f4023f55c9904022b1bdc28c161ea1b0ccf7a0b0bf159ea7`  
		Last Modified: Tue, 31 Aug 2021 04:10:26 GMT  
		Size: 841.6 KB (841608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78204c8eec602e32c9035dbc573e847360a19233f2ffb88986618007712d52d9`  
		Last Modified: Tue, 31 Aug 2021 04:10:25 GMT  
		Size: 4.1 MB (4085868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ed86067b04c16476ddd5611175e233b1c1e9408b27ff5a5f7a75431933258a`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ba9e954473c22356b0980776ea31e72b79943027dc7a29cac0f59129662b26`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4872c59956163dc6560b62d05f0cfd3793ac76bfb638f96095e2622f23f81`  
		Last Modified: Tue, 31 Aug 2021 04:12:54 GMT  
		Size: 238.9 MB (238928640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16905b6ec851712f2f3247be87cadaeb78cdfb5b08d02ea181191e79e9562f88`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ba3a4202a313aceb5938c0aab8fba9f6dfda0c8d5994438331f57c3b723338`  
		Last Modified: Tue, 31 Aug 2021 04:13:37 GMT  
		Size: 54.7 MB (54695246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1794a46b1abe6ac50735c089db696c8f8da6ed7ac93088db09865fe88000de`  
		Last Modified: Tue, 31 Aug 2021 04:13:08 GMT  
		Size: 271.5 KB (271530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd9ba48b098a5f33eb9599d6f4b04f96360528ddd85dad5a8e2125716c6d2`  
		Last Modified: Tue, 31 Aug 2021 04:13:53 GMT  
		Size: 64.7 MB (64746191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c6e087ef5b3f497715fda3ccbc7df571758e90ab212c4db508d80873296f37`  
		Last Modified: Tue, 31 Aug 2021 04:17:13 GMT  
		Size: 259.9 MB (259877729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:90cbdcadb40a69fb9c9af3076c43913647e0decfabab70796c571b35fea4fd15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.4 MB (703413809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b8dff296c7ff902c567db32969e245f3f6c73814572a8512817fdb32991f3b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:00:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 04:02:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:02:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:02:09 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:02:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:03:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703f9076c62d6a07ee4ac54a13d0cfcd29417e872bc88f5c170a4e31b2ee627`  
		Last Modified: Fri, 01 Oct 2021 04:18:40 GMT  
		Size: 841.5 KB (841467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f51453d2a9542a8e5552ed549fba6110526e6bba0d7dea78077ce930818d1`  
		Last Modified: Fri, 01 Oct 2021 04:18:39 GMT  
		Size: 4.5 MB (4453801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb854bd2d2160569f154fad52e3911260b4110a70c0410645d76246ddfd97ff5`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766db03a07190e4dc3fa1dee3a3ae601d2ff84f341678f1e723e096b1af877f`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91559fa0ccbc5993e820912de1e62ef86dde1022279bf6c2ea3ce22578dea1b4`  
		Last Modified: Fri, 01 Oct 2021 04:19:20 GMT  
		Size: 252.4 MB (252369365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022e4617917637f78d14e5e0ff5a67b9753ffd80528ab27ecc82078077d34d5c`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b78d023404d4cc6eb0e0116d7fe33f110d3d0037ab5a281daa0d867334ca48`  
		Last Modified: Fri, 01 Oct 2021 04:19:41 GMT  
		Size: 63.1 MB (63059707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a48409877036295323cd98bb5f3afdc9846c782bcea495aa268883a29d486aa`  
		Last Modified: Fri, 01 Oct 2021 04:19:32 GMT  
		Size: 273.0 KB (272994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb389997238be58731cc3f21699b7db36a2acba2c488fa7407bad3d48a40ec1e`  
		Last Modified: Fri, 01 Oct 2021 04:19:43 GMT  
		Size: 67.2 MB (67222055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c42f2f049dbe2df2b2e9101fd5b273df3b006c906cc94a31e261a4802b5e060`  
		Last Modified: Fri, 01 Oct 2021 04:21:00 GMT  
		Size: 291.5 MB (291464530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:21b02d9f86b74f93061b47a0e6249e8117244f84cecc35da06efe748828d10a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:073274ee3ed4b8853373529777dc094d60f8a7690085cd8789f67e16608e3762
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742504012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eb9859ebf79cd993bb8f61e0a64932761983cf954bb32eb0dfb1220002a0958`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:01:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d2455ea11a3f51289e515125af2fd29538c49291c3d9de5bf605c367fd146c`  
		Last Modified: Fri, 01 Oct 2021 06:24:17 GMT  
		Size: 305.1 MB (305129149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:0d0b271cefece9d849742e548b1afcd6fbec30fd01d71a41b2469ffe80c0d3ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.8 MB (645755710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:475371a853eaad75e2747a0825878fb9487b24decd736155c7bfe08c830b60b0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:47:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:48:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:48:06 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Aug 2021 03:51:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:51:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 03:51:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 03:51:21 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:52:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:52:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 03:53:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:57:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238fe4a9f5df4e59f4023f55c9904022b1bdc28c161ea1b0ccf7a0b0bf159ea7`  
		Last Modified: Tue, 31 Aug 2021 04:10:26 GMT  
		Size: 841.6 KB (841608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78204c8eec602e32c9035dbc573e847360a19233f2ffb88986618007712d52d9`  
		Last Modified: Tue, 31 Aug 2021 04:10:25 GMT  
		Size: 4.1 MB (4085868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ed86067b04c16476ddd5611175e233b1c1e9408b27ff5a5f7a75431933258a`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ba9e954473c22356b0980776ea31e72b79943027dc7a29cac0f59129662b26`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4872c59956163dc6560b62d05f0cfd3793ac76bfb638f96095e2622f23f81`  
		Last Modified: Tue, 31 Aug 2021 04:12:54 GMT  
		Size: 238.9 MB (238928640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16905b6ec851712f2f3247be87cadaeb78cdfb5b08d02ea181191e79e9562f88`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ba3a4202a313aceb5938c0aab8fba9f6dfda0c8d5994438331f57c3b723338`  
		Last Modified: Tue, 31 Aug 2021 04:13:37 GMT  
		Size: 54.7 MB (54695246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1794a46b1abe6ac50735c089db696c8f8da6ed7ac93088db09865fe88000de`  
		Last Modified: Tue, 31 Aug 2021 04:13:08 GMT  
		Size: 271.5 KB (271530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd9ba48b098a5f33eb9599d6f4b04f96360528ddd85dad5a8e2125716c6d2`  
		Last Modified: Tue, 31 Aug 2021 04:13:53 GMT  
		Size: 64.7 MB (64746191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c6e087ef5b3f497715fda3ccbc7df571758e90ab212c4db508d80873296f37`  
		Last Modified: Tue, 31 Aug 2021 04:17:13 GMT  
		Size: 259.9 MB (259877729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:90cbdcadb40a69fb9c9af3076c43913647e0decfabab70796c571b35fea4fd15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.4 MB (703413809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b8dff296c7ff902c567db32969e245f3f6c73814572a8512817fdb32991f3b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:00:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 04:02:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:02:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:02:09 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:02:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:03:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703f9076c62d6a07ee4ac54a13d0cfcd29417e872bc88f5c170a4e31b2ee627`  
		Last Modified: Fri, 01 Oct 2021 04:18:40 GMT  
		Size: 841.5 KB (841467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f51453d2a9542a8e5552ed549fba6110526e6bba0d7dea78077ce930818d1`  
		Last Modified: Fri, 01 Oct 2021 04:18:39 GMT  
		Size: 4.5 MB (4453801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb854bd2d2160569f154fad52e3911260b4110a70c0410645d76246ddfd97ff5`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766db03a07190e4dc3fa1dee3a3ae601d2ff84f341678f1e723e096b1af877f`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91559fa0ccbc5993e820912de1e62ef86dde1022279bf6c2ea3ce22578dea1b4`  
		Last Modified: Fri, 01 Oct 2021 04:19:20 GMT  
		Size: 252.4 MB (252369365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022e4617917637f78d14e5e0ff5a67b9753ffd80528ab27ecc82078077d34d5c`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b78d023404d4cc6eb0e0116d7fe33f110d3d0037ab5a281daa0d867334ca48`  
		Last Modified: Fri, 01 Oct 2021 04:19:41 GMT  
		Size: 63.1 MB (63059707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a48409877036295323cd98bb5f3afdc9846c782bcea495aa268883a29d486aa`  
		Last Modified: Fri, 01 Oct 2021 04:19:32 GMT  
		Size: 273.0 KB (272994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb389997238be58731cc3f21699b7db36a2acba2c488fa7407bad3d48a40ec1e`  
		Last Modified: Fri, 01 Oct 2021 04:19:43 GMT  
		Size: 67.2 MB (67222055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c42f2f049dbe2df2b2e9101fd5b273df3b006c906cc94a31e261a4802b5e060`  
		Last Modified: Fri, 01 Oct 2021 04:21:00 GMT  
		Size: 291.5 MB (291464530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:ee65bc6c342295cad8d6215d4864c2bba6418d39765dced00b20d17fda3e3b73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:2068a86fbf546af4d2cd04b0e08afa70e29d1381be8b26aa46a966da11982009
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448453243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b178cafe1ea49750b6b35cef8398a435e36e0fecde1734d6c237952eb817cc7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:55:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03991905598cbe2e1c4ae3b3c38af7910c05944eaaac7548daec1a84855a5bd4`  
		Last Modified: Fri, 01 Oct 2021 06:23:21 GMT  
		Size: 11.1 MB (11078380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:b85f43fa93d074d45a181a98d1c2dfd53b9168408ab1ca31427b4d6ec4f7eef8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (395998761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0441b27221188faa6bc1eee68e7281bea224a1ae775eab1f1bd07ea7f11acba3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:47:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:48:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:48:06 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Aug 2021 03:51:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:51:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 03:51:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 03:51:21 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:52:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:52:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 03:53:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:54:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238fe4a9f5df4e59f4023f55c9904022b1bdc28c161ea1b0ccf7a0b0bf159ea7`  
		Last Modified: Tue, 31 Aug 2021 04:10:26 GMT  
		Size: 841.6 KB (841608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78204c8eec602e32c9035dbc573e847360a19233f2ffb88986618007712d52d9`  
		Last Modified: Tue, 31 Aug 2021 04:10:25 GMT  
		Size: 4.1 MB (4085868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ed86067b04c16476ddd5611175e233b1c1e9408b27ff5a5f7a75431933258a`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ba9e954473c22356b0980776ea31e72b79943027dc7a29cac0f59129662b26`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4872c59956163dc6560b62d05f0cfd3793ac76bfb638f96095e2622f23f81`  
		Last Modified: Tue, 31 Aug 2021 04:12:54 GMT  
		Size: 238.9 MB (238928640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16905b6ec851712f2f3247be87cadaeb78cdfb5b08d02ea181191e79e9562f88`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ba3a4202a313aceb5938c0aab8fba9f6dfda0c8d5994438331f57c3b723338`  
		Last Modified: Tue, 31 Aug 2021 04:13:37 GMT  
		Size: 54.7 MB (54695246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1794a46b1abe6ac50735c089db696c8f8da6ed7ac93088db09865fe88000de`  
		Last Modified: Tue, 31 Aug 2021 04:13:08 GMT  
		Size: 271.5 KB (271530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd9ba48b098a5f33eb9599d6f4b04f96360528ddd85dad5a8e2125716c6d2`  
		Last Modified: Tue, 31 Aug 2021 04:13:53 GMT  
		Size: 64.7 MB (64746191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e0ae5bc44b30824963f57d998d8b90b4e7417977813d1ecbdd0e6fd690de8b`  
		Last Modified: Tue, 31 Aug 2021 04:14:17 GMT  
		Size: 10.1 MB (10120780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c26031da34c57662132aaa5ee349f6470f3bc47d0dad0a6715ccae5512248aa6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422682518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20ffc17695ed1d5e1473b6b4d5742d9368f0789bf67657688f0b67529d9a1f44`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:00:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 04:02:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:02:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:02:09 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:02:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:03:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:03:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703f9076c62d6a07ee4ac54a13d0cfcd29417e872bc88f5c170a4e31b2ee627`  
		Last Modified: Fri, 01 Oct 2021 04:18:40 GMT  
		Size: 841.5 KB (841467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f51453d2a9542a8e5552ed549fba6110526e6bba0d7dea78077ce930818d1`  
		Last Modified: Fri, 01 Oct 2021 04:18:39 GMT  
		Size: 4.5 MB (4453801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb854bd2d2160569f154fad52e3911260b4110a70c0410645d76246ddfd97ff5`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766db03a07190e4dc3fa1dee3a3ae601d2ff84f341678f1e723e096b1af877f`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91559fa0ccbc5993e820912de1e62ef86dde1022279bf6c2ea3ce22578dea1b4`  
		Last Modified: Fri, 01 Oct 2021 04:19:20 GMT  
		Size: 252.4 MB (252369365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022e4617917637f78d14e5e0ff5a67b9753ffd80528ab27ecc82078077d34d5c`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b78d023404d4cc6eb0e0116d7fe33f110d3d0037ab5a281daa0d867334ca48`  
		Last Modified: Fri, 01 Oct 2021 04:19:41 GMT  
		Size: 63.1 MB (63059707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a48409877036295323cd98bb5f3afdc9846c782bcea495aa268883a29d486aa`  
		Last Modified: Fri, 01 Oct 2021 04:19:32 GMT  
		Size: 273.0 KB (272994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb389997238be58731cc3f21699b7db36a2acba2c488fa7407bad3d48a40ec1e`  
		Last Modified: Fri, 01 Oct 2021 04:19:43 GMT  
		Size: 67.2 MB (67222055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcff5a64d5ce344006b02ba8c8402be2075066a2047945c1aaf770aec2f0e7ad`  
		Last Modified: Fri, 01 Oct 2021 04:20:00 GMT  
		Size: 10.7 MB (10733239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:ee65bc6c342295cad8d6215d4864c2bba6418d39765dced00b20d17fda3e3b73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:2068a86fbf546af4d2cd04b0e08afa70e29d1381be8b26aa46a966da11982009
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448453243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b178cafe1ea49750b6b35cef8398a435e36e0fecde1734d6c237952eb817cc7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:55:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03991905598cbe2e1c4ae3b3c38af7910c05944eaaac7548daec1a84855a5bd4`  
		Last Modified: Fri, 01 Oct 2021 06:23:21 GMT  
		Size: 11.1 MB (11078380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:b85f43fa93d074d45a181a98d1c2dfd53b9168408ab1ca31427b4d6ec4f7eef8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (395998761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0441b27221188faa6bc1eee68e7281bea224a1ae775eab1f1bd07ea7f11acba3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:47:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:48:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:48:06 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Aug 2021 03:51:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:51:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 03:51:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 03:51:21 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:52:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:52:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 03:53:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:54:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238fe4a9f5df4e59f4023f55c9904022b1bdc28c161ea1b0ccf7a0b0bf159ea7`  
		Last Modified: Tue, 31 Aug 2021 04:10:26 GMT  
		Size: 841.6 KB (841608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78204c8eec602e32c9035dbc573e847360a19233f2ffb88986618007712d52d9`  
		Last Modified: Tue, 31 Aug 2021 04:10:25 GMT  
		Size: 4.1 MB (4085868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ed86067b04c16476ddd5611175e233b1c1e9408b27ff5a5f7a75431933258a`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ba9e954473c22356b0980776ea31e72b79943027dc7a29cac0f59129662b26`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4872c59956163dc6560b62d05f0cfd3793ac76bfb638f96095e2622f23f81`  
		Last Modified: Tue, 31 Aug 2021 04:12:54 GMT  
		Size: 238.9 MB (238928640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16905b6ec851712f2f3247be87cadaeb78cdfb5b08d02ea181191e79e9562f88`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ba3a4202a313aceb5938c0aab8fba9f6dfda0c8d5994438331f57c3b723338`  
		Last Modified: Tue, 31 Aug 2021 04:13:37 GMT  
		Size: 54.7 MB (54695246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1794a46b1abe6ac50735c089db696c8f8da6ed7ac93088db09865fe88000de`  
		Last Modified: Tue, 31 Aug 2021 04:13:08 GMT  
		Size: 271.5 KB (271530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd9ba48b098a5f33eb9599d6f4b04f96360528ddd85dad5a8e2125716c6d2`  
		Last Modified: Tue, 31 Aug 2021 04:13:53 GMT  
		Size: 64.7 MB (64746191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e0ae5bc44b30824963f57d998d8b90b4e7417977813d1ecbdd0e6fd690de8b`  
		Last Modified: Tue, 31 Aug 2021 04:14:17 GMT  
		Size: 10.1 MB (10120780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c26031da34c57662132aaa5ee349f6470f3bc47d0dad0a6715ccae5512248aa6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422682518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20ffc17695ed1d5e1473b6b4d5742d9368f0789bf67657688f0b67529d9a1f44`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:00:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 04:02:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:02:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:02:09 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:02:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:03:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:03:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703f9076c62d6a07ee4ac54a13d0cfcd29417e872bc88f5c170a4e31b2ee627`  
		Last Modified: Fri, 01 Oct 2021 04:18:40 GMT  
		Size: 841.5 KB (841467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f51453d2a9542a8e5552ed549fba6110526e6bba0d7dea78077ce930818d1`  
		Last Modified: Fri, 01 Oct 2021 04:18:39 GMT  
		Size: 4.5 MB (4453801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb854bd2d2160569f154fad52e3911260b4110a70c0410645d76246ddfd97ff5`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766db03a07190e4dc3fa1dee3a3ae601d2ff84f341678f1e723e096b1af877f`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91559fa0ccbc5993e820912de1e62ef86dde1022279bf6c2ea3ce22578dea1b4`  
		Last Modified: Fri, 01 Oct 2021 04:19:20 GMT  
		Size: 252.4 MB (252369365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022e4617917637f78d14e5e0ff5a67b9753ffd80528ab27ecc82078077d34d5c`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b78d023404d4cc6eb0e0116d7fe33f110d3d0037ab5a281daa0d867334ca48`  
		Last Modified: Fri, 01 Oct 2021 04:19:41 GMT  
		Size: 63.1 MB (63059707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a48409877036295323cd98bb5f3afdc9846c782bcea495aa268883a29d486aa`  
		Last Modified: Fri, 01 Oct 2021 04:19:32 GMT  
		Size: 273.0 KB (272994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb389997238be58731cc3f21699b7db36a2acba2c488fa7407bad3d48a40ec1e`  
		Last Modified: Fri, 01 Oct 2021 04:19:43 GMT  
		Size: 67.2 MB (67222055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcff5a64d5ce344006b02ba8c8402be2075066a2047945c1aaf770aec2f0e7ad`  
		Last Modified: Fri, 01 Oct 2021 04:20:00 GMT  
		Size: 10.7 MB (10733239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:59f8ccd0305997c7c04c2ce734f061c6397a6f3d9982213de543a604a6dee1d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:6c99c80a97d9a6af8b830bd34c028e9a80d42138ab0d4ab9bfa78998c70c0954
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437374863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38caaa68c7ca79c4d362762f7247e2c807a9fd5f853a02aaae4e98b234c997e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:4b03d0e396887e99d465986c4abfcd28905e49492a9e65e48441a3c9cdc61d09
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385877981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65627f7ecb5effc290e9142cd68a86e1569dc3d79418a996161e3642bc50be1b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:47:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:48:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:48:06 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Aug 2021 03:51:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:51:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 03:51:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 03:51:21 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:52:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:52:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 03:53:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238fe4a9f5df4e59f4023f55c9904022b1bdc28c161ea1b0ccf7a0b0bf159ea7`  
		Last Modified: Tue, 31 Aug 2021 04:10:26 GMT  
		Size: 841.6 KB (841608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78204c8eec602e32c9035dbc573e847360a19233f2ffb88986618007712d52d9`  
		Last Modified: Tue, 31 Aug 2021 04:10:25 GMT  
		Size: 4.1 MB (4085868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ed86067b04c16476ddd5611175e233b1c1e9408b27ff5a5f7a75431933258a`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ba9e954473c22356b0980776ea31e72b79943027dc7a29cac0f59129662b26`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4872c59956163dc6560b62d05f0cfd3793ac76bfb638f96095e2622f23f81`  
		Last Modified: Tue, 31 Aug 2021 04:12:54 GMT  
		Size: 238.9 MB (238928640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16905b6ec851712f2f3247be87cadaeb78cdfb5b08d02ea181191e79e9562f88`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ba3a4202a313aceb5938c0aab8fba9f6dfda0c8d5994438331f57c3b723338`  
		Last Modified: Tue, 31 Aug 2021 04:13:37 GMT  
		Size: 54.7 MB (54695246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1794a46b1abe6ac50735c089db696c8f8da6ed7ac93088db09865fe88000de`  
		Last Modified: Tue, 31 Aug 2021 04:13:08 GMT  
		Size: 271.5 KB (271530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd9ba48b098a5f33eb9599d6f4b04f96360528ddd85dad5a8e2125716c6d2`  
		Last Modified: Tue, 31 Aug 2021 04:13:53 GMT  
		Size: 64.7 MB (64746191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8225d01167dfc81e8f524b9d72d3c2003b852121e54c0ec322e072f8e3cced54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411949279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb78205244108ca568a249807c4b5d93b0d41239e3703caa55ddccd9f4a0c2fb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:00:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 04:02:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:02:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:02:09 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:02:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:03:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703f9076c62d6a07ee4ac54a13d0cfcd29417e872bc88f5c170a4e31b2ee627`  
		Last Modified: Fri, 01 Oct 2021 04:18:40 GMT  
		Size: 841.5 KB (841467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f51453d2a9542a8e5552ed549fba6110526e6bba0d7dea78077ce930818d1`  
		Last Modified: Fri, 01 Oct 2021 04:18:39 GMT  
		Size: 4.5 MB (4453801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb854bd2d2160569f154fad52e3911260b4110a70c0410645d76246ddfd97ff5`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766db03a07190e4dc3fa1dee3a3ae601d2ff84f341678f1e723e096b1af877f`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91559fa0ccbc5993e820912de1e62ef86dde1022279bf6c2ea3ce22578dea1b4`  
		Last Modified: Fri, 01 Oct 2021 04:19:20 GMT  
		Size: 252.4 MB (252369365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022e4617917637f78d14e5e0ff5a67b9753ffd80528ab27ecc82078077d34d5c`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b78d023404d4cc6eb0e0116d7fe33f110d3d0037ab5a281daa0d867334ca48`  
		Last Modified: Fri, 01 Oct 2021 04:19:41 GMT  
		Size: 63.1 MB (63059707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a48409877036295323cd98bb5f3afdc9846c782bcea495aa268883a29d486aa`  
		Last Modified: Fri, 01 Oct 2021 04:19:32 GMT  
		Size: 273.0 KB (272994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb389997238be58731cc3f21699b7db36a2acba2c488fa7407bad3d48a40ec1e`  
		Last Modified: Fri, 01 Oct 2021 04:19:43 GMT  
		Size: 67.2 MB (67222055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:59f8ccd0305997c7c04c2ce734f061c6397a6f3d9982213de543a604a6dee1d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:6c99c80a97d9a6af8b830bd34c028e9a80d42138ab0d4ab9bfa78998c70c0954
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437374863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38caaa68c7ca79c4d362762f7247e2c807a9fd5f853a02aaae4e98b234c997e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:4b03d0e396887e99d465986c4abfcd28905e49492a9e65e48441a3c9cdc61d09
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385877981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65627f7ecb5effc290e9142cd68a86e1569dc3d79418a996161e3642bc50be1b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:47:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:48:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:48:06 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Aug 2021 03:51:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:51:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 03:51:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 03:51:21 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:52:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:52:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 03:53:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238fe4a9f5df4e59f4023f55c9904022b1bdc28c161ea1b0ccf7a0b0bf159ea7`  
		Last Modified: Tue, 31 Aug 2021 04:10:26 GMT  
		Size: 841.6 KB (841608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78204c8eec602e32c9035dbc573e847360a19233f2ffb88986618007712d52d9`  
		Last Modified: Tue, 31 Aug 2021 04:10:25 GMT  
		Size: 4.1 MB (4085868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ed86067b04c16476ddd5611175e233b1c1e9408b27ff5a5f7a75431933258a`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ba9e954473c22356b0980776ea31e72b79943027dc7a29cac0f59129662b26`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4872c59956163dc6560b62d05f0cfd3793ac76bfb638f96095e2622f23f81`  
		Last Modified: Tue, 31 Aug 2021 04:12:54 GMT  
		Size: 238.9 MB (238928640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16905b6ec851712f2f3247be87cadaeb78cdfb5b08d02ea181191e79e9562f88`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ba3a4202a313aceb5938c0aab8fba9f6dfda0c8d5994438331f57c3b723338`  
		Last Modified: Tue, 31 Aug 2021 04:13:37 GMT  
		Size: 54.7 MB (54695246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1794a46b1abe6ac50735c089db696c8f8da6ed7ac93088db09865fe88000de`  
		Last Modified: Tue, 31 Aug 2021 04:13:08 GMT  
		Size: 271.5 KB (271530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd9ba48b098a5f33eb9599d6f4b04f96360528ddd85dad5a8e2125716c6d2`  
		Last Modified: Tue, 31 Aug 2021 04:13:53 GMT  
		Size: 64.7 MB (64746191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8225d01167dfc81e8f524b9d72d3c2003b852121e54c0ec322e072f8e3cced54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411949279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb78205244108ca568a249807c4b5d93b0d41239e3703caa55ddccd9f4a0c2fb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:00:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 04:02:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:02:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:02:09 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:02:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:03:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703f9076c62d6a07ee4ac54a13d0cfcd29417e872bc88f5c170a4e31b2ee627`  
		Last Modified: Fri, 01 Oct 2021 04:18:40 GMT  
		Size: 841.5 KB (841467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f51453d2a9542a8e5552ed549fba6110526e6bba0d7dea78077ce930818d1`  
		Last Modified: Fri, 01 Oct 2021 04:18:39 GMT  
		Size: 4.5 MB (4453801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb854bd2d2160569f154fad52e3911260b4110a70c0410645d76246ddfd97ff5`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766db03a07190e4dc3fa1dee3a3ae601d2ff84f341678f1e723e096b1af877f`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91559fa0ccbc5993e820912de1e62ef86dde1022279bf6c2ea3ce22578dea1b4`  
		Last Modified: Fri, 01 Oct 2021 04:19:20 GMT  
		Size: 252.4 MB (252369365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022e4617917637f78d14e5e0ff5a67b9753ffd80528ab27ecc82078077d34d5c`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b78d023404d4cc6eb0e0116d7fe33f110d3d0037ab5a281daa0d867334ca48`  
		Last Modified: Fri, 01 Oct 2021 04:19:41 GMT  
		Size: 63.1 MB (63059707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a48409877036295323cd98bb5f3afdc9846c782bcea495aa268883a29d486aa`  
		Last Modified: Fri, 01 Oct 2021 04:19:32 GMT  
		Size: 273.0 KB (272994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb389997238be58731cc3f21699b7db36a2acba2c488fa7407bad3d48a40ec1e`  
		Last Modified: Fri, 01 Oct 2021 04:19:43 GMT  
		Size: 67.2 MB (67222055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:b0f161182c43d7ac34e4db52559119570e0e4b20fd867463979a2fdc561ccc3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:5da99077487fb6a23334589c87442544965eff9960b0aef3bb5b385f60d6264a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291875817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ddab15692c93b05ddb281246caa09b9c5d97794a953a331cf7a991ee9f7e8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:d3f037fed4337561cafeeeb154ff906161749d68f484f3fa0151c0e7edbee788
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266165014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e07be8dccd80381c769ac0d786fcf34a2755ea28b9a33678ff833e22c090e9f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:47:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:48:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:48:06 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Aug 2021 03:51:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:51:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 03:51:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 03:51:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238fe4a9f5df4e59f4023f55c9904022b1bdc28c161ea1b0ccf7a0b0bf159ea7`  
		Last Modified: Tue, 31 Aug 2021 04:10:26 GMT  
		Size: 841.6 KB (841608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78204c8eec602e32c9035dbc573e847360a19233f2ffb88986618007712d52d9`  
		Last Modified: Tue, 31 Aug 2021 04:10:25 GMT  
		Size: 4.1 MB (4085868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ed86067b04c16476ddd5611175e233b1c1e9408b27ff5a5f7a75431933258a`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ba9e954473c22356b0980776ea31e72b79943027dc7a29cac0f59129662b26`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4872c59956163dc6560b62d05f0cfd3793ac76bfb638f96095e2622f23f81`  
		Last Modified: Tue, 31 Aug 2021 04:12:54 GMT  
		Size: 238.9 MB (238928640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16905b6ec851712f2f3247be87cadaeb78cdfb5b08d02ea181191e79e9562f88`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2bc12f70d7412f29e9c8c5a6233b3024c9b95127c8eb57972f310761565fca27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281394523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9583134313a6bba2702d7dd1d42064e6609ff036c2e1a61bf2a50b9b322300ff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:00:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 04:02:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:02:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:02:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703f9076c62d6a07ee4ac54a13d0cfcd29417e872bc88f5c170a4e31b2ee627`  
		Last Modified: Fri, 01 Oct 2021 04:18:40 GMT  
		Size: 841.5 KB (841467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f51453d2a9542a8e5552ed549fba6110526e6bba0d7dea78077ce930818d1`  
		Last Modified: Fri, 01 Oct 2021 04:18:39 GMT  
		Size: 4.5 MB (4453801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb854bd2d2160569f154fad52e3911260b4110a70c0410645d76246ddfd97ff5`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766db03a07190e4dc3fa1dee3a3ae601d2ff84f341678f1e723e096b1af877f`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91559fa0ccbc5993e820912de1e62ef86dde1022279bf6c2ea3ce22578dea1b4`  
		Last Modified: Fri, 01 Oct 2021 04:19:20 GMT  
		Size: 252.4 MB (252369365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022e4617917637f78d14e5e0ff5a67b9753ffd80528ab27ecc82078077d34d5c`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:b0f161182c43d7ac34e4db52559119570e0e4b20fd867463979a2fdc561ccc3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:5da99077487fb6a23334589c87442544965eff9960b0aef3bb5b385f60d6264a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291875817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ddab15692c93b05ddb281246caa09b9c5d97794a953a331cf7a991ee9f7e8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:d3f037fed4337561cafeeeb154ff906161749d68f484f3fa0151c0e7edbee788
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266165014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e07be8dccd80381c769ac0d786fcf34a2755ea28b9a33678ff833e22c090e9f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:30 GMT
ADD file:5e191cb3774eee823ea256e960cb570c8ee5bb1a149dc1bfdaaa2adf7bc64007 in / 
# Tue, 31 Aug 2021 01:40:31 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:47:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:47:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:48:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:48:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:48:06 GMT
ENV ROS_DISTRO=melodic
# Tue, 31 Aug 2021 03:51:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:51:20 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 03:51:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 03:51:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:94f80e8eb1703fb9b4edfd10bf21f9967e116e6692f5dd4363fbe8f3ac04946e`  
		Last Modified: Tue, 31 Aug 2021 01:44:27 GMT  
		Size: 22.3 MB (22306479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238fe4a9f5df4e59f4023f55c9904022b1bdc28c161ea1b0ccf7a0b0bf159ea7`  
		Last Modified: Tue, 31 Aug 2021 04:10:26 GMT  
		Size: 841.6 KB (841608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78204c8eec602e32c9035dbc573e847360a19233f2ffb88986618007712d52d9`  
		Last Modified: Tue, 31 Aug 2021 04:10:25 GMT  
		Size: 4.1 MB (4085868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ed86067b04c16476ddd5611175e233b1c1e9408b27ff5a5f7a75431933258a`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ba9e954473c22356b0980776ea31e72b79943027dc7a29cac0f59129662b26`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4872c59956163dc6560b62d05f0cfd3793ac76bfb638f96095e2622f23f81`  
		Last Modified: Tue, 31 Aug 2021 04:12:54 GMT  
		Size: 238.9 MB (238928640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16905b6ec851712f2f3247be87cadaeb78cdfb5b08d02ea181191e79e9562f88`  
		Last Modified: Tue, 31 Aug 2021 04:10:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2bc12f70d7412f29e9c8c5a6233b3024c9b95127c8eb57972f310761565fca27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281394523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9583134313a6bba2702d7dd1d42064e6609ff036c2e1a61bf2a50b9b322300ff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:00:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 04:02:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:02:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:02:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703f9076c62d6a07ee4ac54a13d0cfcd29417e872bc88f5c170a4e31b2ee627`  
		Last Modified: Fri, 01 Oct 2021 04:18:40 GMT  
		Size: 841.5 KB (841467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f51453d2a9542a8e5552ed549fba6110526e6bba0d7dea78077ce930818d1`  
		Last Modified: Fri, 01 Oct 2021 04:18:39 GMT  
		Size: 4.5 MB (4453801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb854bd2d2160569f154fad52e3911260b4110a70c0410645d76246ddfd97ff5`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766db03a07190e4dc3fa1dee3a3ae601d2ff84f341678f1e723e096b1af877f`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91559fa0ccbc5993e820912de1e62ef86dde1022279bf6c2ea3ce22578dea1b4`  
		Last Modified: Fri, 01 Oct 2021 04:19:20 GMT  
		Size: 252.4 MB (252369365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022e4617917637f78d14e5e0ff5a67b9753ffd80528ab27ecc82078077d34d5c`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:ca310a19885c0aed922ac6d1936934d4740fe8b6be91437f0c18baedebcf636d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:ccaf1b2477838808d73663f41c34719386ad7ea977091fdcbd19c95b9feff8c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339184977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c618f40d6ef1b8f46c2c5e4114809283344e4b751a46ab67c77aa17f174d411`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 06:02:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 06:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 06:04:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:04:15 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:04:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:05:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8985568900a589503a6b64505536a7ed14c04be58f49125487546556e4bf16d2`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396a66dc135f942aded0cbf41869920dd471f4ae69a577ef485c7fad6ad26f6`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e67a2d329fca5d4ed9676dc99b6786e3b630fb2cdc61a582593ee9c0d2af6`  
		Last Modified: Fri, 01 Oct 2021 06:24:57 GMT  
		Size: 176.7 MB (176698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f46e6b695aaf67ea964cbc89cec1bb208303e42ef77d8ae91776e089bb5ca`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9999226e85f92a036c340a8cd8f6223dae10b187aabfcafcb3bf8db55c579c4c`  
		Last Modified: Fri, 01 Oct 2021 06:25:15 GMT  
		Size: 47.3 MB (47259853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d72ee051e2ffafedab97e53d9c1c7dd3d04e22c91edd5a6f5998bbc8649d9d`  
		Last Modified: Fri, 01 Oct 2021 06:25:07 GMT  
		Size: 321.5 KB (321468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e3373d9dd06236066e1567f04e4344c9a90b98b797e7f2ad101fbb541811bd`  
		Last Modified: Fri, 01 Oct 2021 06:25:20 GMT  
		Size: 79.6 MB (79603325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:3502680140f44f7d6e0f5d06694a932b440166eaaae3a7bb8459790377f695b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284639164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e9851a6cabd762aa85ab3b198ef0bac96359c28a5539db594ea18cfd4492bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:58:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:58:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:01:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:01:07 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:01:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:02:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597f16c1171caedee0148b09aba1a7c8b8ff2f29ffec5f8bc82f4a2d0c4a955`  
		Last Modified: Tue, 31 Aug 2021 04:17:31 GMT  
		Size: 1.2 MB (1183503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f278f986afdfeaabcdd6e3e66554d2851e9813dda91fc83341f7cdf3dca05`  
		Last Modified: Tue, 31 Aug 2021 04:17:30 GMT  
		Size: 4.7 MB (4676468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf026e89b16b8250a76b892191540bf0879aafa7e00242a2f6151d466ee9f283`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c21ec0037b0f9bae7c4c1a4415d768ebce97dc86e798bff4f6e544059ac5e`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db678ae234a6fe1d46c8463a559f04c415c2522d0effab08ae407178410d5db`  
		Last Modified: Tue, 31 Aug 2021 04:19:33 GMT  
		Size: 157.2 MB (157216591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79678cecea953d0568fb159f017c76dd5db59346cc095d3d118b734bade1037d`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7610242426bc226b21c63941458db4760063f2536207c80d92f79642ede166d`  
		Last Modified: Tue, 31 Aug 2021 04:20:05 GMT  
		Size: 36.7 MB (36691316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d75fec186326e68092c8c944a4991cf20df280505668146aeab88ef75f42f`  
		Last Modified: Tue, 31 Aug 2021 04:19:46 GMT  
		Size: 317.9 KB (317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891bd701076db5d3efe95bd46c285b538fbf4d20a17a3fdde54216d561a397d0`  
		Last Modified: Tue, 31 Aug 2021 04:20:24 GMT  
		Size: 60.5 MB (60482196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:66791732edf7e13167d9ea961d962152e5401ffa9d9ceb0f8c2cde65aec974f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.8 MB (318822332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78083a3273027cb4a7fd2603e6461c20f176f7f1dd44e1527c6b8236af556ced`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:05:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 04:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:06:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:06:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:07:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5955ec7390235db14b9c45d9030bd90295fdbfc2dd976b408668c1feaa0c16ba`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3177f1eddf2202fb915200162e8693b4fc55482d73411891f1184df5517140`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76170f07a4a0b1a928e2367788be540ac8379fbb9cdd2461ef5248e67f7ffb96`  
		Last Modified: Fri, 01 Oct 2021 04:21:43 GMT  
		Size: 171.1 MB (171135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ffa5ef1c6b2f2640d24037747e349bcb1b99eaba29240f0b7e62c35115462`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d780d95d984615f9091bcff4af07fbec2f87e83f046d35e9ab14912242c636ff`  
		Last Modified: Fri, 01 Oct 2021 04:22:03 GMT  
		Size: 41.5 MB (41521018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6924807e2d6734e0d3876de4e1a66637f28fa98b175e630040905e31e3bcf5`  
		Last Modified: Fri, 01 Oct 2021 04:21:56 GMT  
		Size: 321.5 KB (321466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a22ce1c357749088045cd1e5a809f080f05d6e6adc9a0f721bd15d6ff9b750`  
		Last Modified: Fri, 01 Oct 2021 04:22:07 GMT  
		Size: 72.0 MB (71972774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:1d357621cc38e1a4d09ad86f5c6e6f9ea2822a4a18cbfb54d215aec7282b3334
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:8ff176871535f3a09a7d11d26314d881ad42c944b63cf7e3a6daedfcf544011c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.7 MB (840658961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78e91c26d3138b63e62f54f114439797e8bff78b337ba0e5c9cba91b0a622090`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 06:02:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 06:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 06:04:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:04:15 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:04:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:05:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8985568900a589503a6b64505536a7ed14c04be58f49125487546556e4bf16d2`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396a66dc135f942aded0cbf41869920dd471f4ae69a577ef485c7fad6ad26f6`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e67a2d329fca5d4ed9676dc99b6786e3b630fb2cdc61a582593ee9c0d2af6`  
		Last Modified: Fri, 01 Oct 2021 06:24:57 GMT  
		Size: 176.7 MB (176698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f46e6b695aaf67ea964cbc89cec1bb208303e42ef77d8ae91776e089bb5ca`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9999226e85f92a036c340a8cd8f6223dae10b187aabfcafcb3bf8db55c579c4c`  
		Last Modified: Fri, 01 Oct 2021 06:25:15 GMT  
		Size: 47.3 MB (47259853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d72ee051e2ffafedab97e53d9c1c7dd3d04e22c91edd5a6f5998bbc8649d9d`  
		Last Modified: Fri, 01 Oct 2021 06:25:07 GMT  
		Size: 321.5 KB (321468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e3373d9dd06236066e1567f04e4344c9a90b98b797e7f2ad101fbb541811bd`  
		Last Modified: Fri, 01 Oct 2021 06:25:20 GMT  
		Size: 79.6 MB (79603325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8c92225baeee3737c60e0433c14c1a5d67f77aa6da87cc9c2fefecbce90b8a`  
		Last Modified: Fri, 01 Oct 2021 06:27:02 GMT  
		Size: 501.5 MB (501473984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:f40be954b42fdbf2c8658b0378454aff44e042a9dd0cd047fa1faf526993e0ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **730.2 MB (730245800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d65f25fc22d5b0aa108a74c05817159af01187025e7ef2e0e00644a7274356`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:58:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:58:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:01:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:01:07 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:01:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:02:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:08:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597f16c1171caedee0148b09aba1a7c8b8ff2f29ffec5f8bc82f4a2d0c4a955`  
		Last Modified: Tue, 31 Aug 2021 04:17:31 GMT  
		Size: 1.2 MB (1183503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f278f986afdfeaabcdd6e3e66554d2851e9813dda91fc83341f7cdf3dca05`  
		Last Modified: Tue, 31 Aug 2021 04:17:30 GMT  
		Size: 4.7 MB (4676468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf026e89b16b8250a76b892191540bf0879aafa7e00242a2f6151d466ee9f283`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c21ec0037b0f9bae7c4c1a4415d768ebce97dc86e798bff4f6e544059ac5e`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db678ae234a6fe1d46c8463a559f04c415c2522d0effab08ae407178410d5db`  
		Last Modified: Tue, 31 Aug 2021 04:19:33 GMT  
		Size: 157.2 MB (157216591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79678cecea953d0568fb159f017c76dd5db59346cc095d3d118b734bade1037d`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7610242426bc226b21c63941458db4760063f2536207c80d92f79642ede166d`  
		Last Modified: Tue, 31 Aug 2021 04:20:05 GMT  
		Size: 36.7 MB (36691316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d75fec186326e68092c8c944a4991cf20df280505668146aeab88ef75f42f`  
		Last Modified: Tue, 31 Aug 2021 04:19:46 GMT  
		Size: 317.9 KB (317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891bd701076db5d3efe95bd46c285b538fbf4d20a17a3fdde54216d561a397d0`  
		Last Modified: Tue, 31 Aug 2021 04:20:24 GMT  
		Size: 60.5 MB (60482196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb6760ee5d1314fbec6f42620c54f10eacb13ab219ff411714d6e2706987a45`  
		Last Modified: Tue, 31 Aug 2021 04:25:40 GMT  
		Size: 445.6 MB (445606636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a59d10cada697347393717ed37ed4ce2474f9427539ee17804d81757479f7d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **790.9 MB (790927813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eabb6eb581ac47318cca2b8ef351a73988712c5ed1ff2021a1ad06e7ad9cec4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:05:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 04:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:06:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:06:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:07:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:09:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5955ec7390235db14b9c45d9030bd90295fdbfc2dd976b408668c1feaa0c16ba`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3177f1eddf2202fb915200162e8693b4fc55482d73411891f1184df5517140`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76170f07a4a0b1a928e2367788be540ac8379fbb9cdd2461ef5248e67f7ffb96`  
		Last Modified: Fri, 01 Oct 2021 04:21:43 GMT  
		Size: 171.1 MB (171135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ffa5ef1c6b2f2640d24037747e349bcb1b99eaba29240f0b7e62c35115462`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d780d95d984615f9091bcff4af07fbec2f87e83f046d35e9ab14912242c636ff`  
		Last Modified: Fri, 01 Oct 2021 04:22:03 GMT  
		Size: 41.5 MB (41521018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6924807e2d6734e0d3876de4e1a66637f28fa98b175e630040905e31e3bcf5`  
		Last Modified: Fri, 01 Oct 2021 04:21:56 GMT  
		Size: 321.5 KB (321466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a22ce1c357749088045cd1e5a809f080f05d6e6adc9a0f721bd15d6ff9b750`  
		Last Modified: Fri, 01 Oct 2021 04:22:07 GMT  
		Size: 72.0 MB (71972774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a048aff215857f993c4474873a3ad80d194f16a3e39098731c04c14b35ef6e3d`  
		Last Modified: Fri, 01 Oct 2021 04:23:51 GMT  
		Size: 472.1 MB (472105481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:4832950f8b35421b1c5e5522c5d9499329c399331b0042c40f2f982068990d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:fc8ce6294d9c8546e7a8f7ef12e28310345338fcac520b48b1b07ef5ca7f0377
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **968.0 MB (968024174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2ab95b8b0305efe159887a22df55209c2c0251d8a7e5a7618325965ea33dc27`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 21:16:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:16:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 28 Sep 2021 21:17:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 28 Sep 2021 21:17:08 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 21:17:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 28 Sep 2021 21:17:08 GMT
ENV ROS_DISTRO=noetic
# Tue, 28 Sep 2021 21:18:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:18:23 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 28 Sep 2021 21:18:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 28 Sep 2021 21:18:24 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 21:19:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:19:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 28 Sep 2021 21:19:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:23:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057f5227de8f6db89935faceb04e14221b934ffc6724618581f7e8392970c3ed`  
		Last Modified: Tue, 28 Sep 2021 21:24:45 GMT  
		Size: 10.9 MB (10891832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd2be7e40d77e274ec22ddb4f87a6316ce568f810184a8e59e18ba01fc96932`  
		Last Modified: Tue, 28 Sep 2021 21:24:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6d934e0e2132b27cda2cacacb9088097b537f9a40cdf536e2abc5d225c6387`  
		Last Modified: Tue, 28 Sep 2021 21:24:44 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898c3d5d521ed7072839820050082135fe093df92e6924f017afc47ddbb42355`  
		Last Modified: Tue, 28 Sep 2021 21:25:19 GMT  
		Size: 239.1 MB (239056614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57e0d0e6e00100bc444c8c1ff5b4028e0de1a63fe406669810c494e10803f6a`  
		Last Modified: Tue, 28 Sep 2021 21:24:43 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7a76943e01f7c49865103cc39e2286c3b843b81a9c9c07e122dfeeb1c99f93`  
		Last Modified: Tue, 28 Sep 2021 21:25:41 GMT  
		Size: 86.6 MB (86566434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb2d48531002cdd91f487084f1be81a6be323f175934a6d8ee366927fc89efa`  
		Last Modified: Tue, 28 Sep 2021 21:25:27 GMT  
		Size: 315.2 KB (315239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce5ac6d6887766f72c3011574775084de91b975f55a84cd4347d3bc3e028e6`  
		Last Modified: Tue, 28 Sep 2021 21:25:38 GMT  
		Size: 76.0 MB (75975243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636df33d35487c2de510835c3d13e125d9bb867d0512a64ab54fc6dd002387e3`  
		Last Modified: Tue, 28 Sep 2021 21:27:19 GMT  
		Size: 504.8 MB (504780188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7ca031717582542aaa39f11604722d89d177f746e48eaaad369a7600361d03e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **884.8 MB (884800192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dd3c1343c557e7442d399fb0380f6b87362fb20379e162f2f24ee5eb737e8c9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 12:17:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:17:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 28 Sep 2021 12:18:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 28 Sep 2021 12:18:09 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 12:18:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 28 Sep 2021 12:18:09 GMT
ENV ROS_DISTRO=noetic
# Tue, 28 Sep 2021 12:19:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:19:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 28 Sep 2021 12:19:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 28 Sep 2021 12:19:16 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 12:19:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:20:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 28 Sep 2021 12:20:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:23:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b719e84e5c17a05db4cb91b65b25f4cecd9fda5ca86f7c93b9e8918c83ad07`  
		Last Modified: Tue, 28 Sep 2021 12:26:12 GMT  
		Size: 10.9 MB (10883372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b180205050ab5009747a1fa863a1467a5e672c5116542801e3f3890b57cc64`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0309f751216573b01fdef820a8e7c97a9ef1170563c0136c2e3faa29e4e99ed`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290538ca4b138960141fb0cf9d84a1ada042c2286a8714c2afa426ef9ea5baf9`  
		Last Modified: Tue, 28 Sep 2021 12:26:44 GMT  
		Size: 184.2 MB (184242688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8fe4a6c015780d0a432c652d6ac68724f7b7305a66625f3dde29654973d374`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570cd6760219c636efbd15651c975651d6776ef161e5daf5e95ca0d02cf74440`  
		Last Modified: Tue, 28 Sep 2021 12:27:04 GMT  
		Size: 84.4 MB (84358024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225d1354fc88caaadf4d1c8428bc28ea51f87d230c8889449d028a90955656a4`  
		Last Modified: Tue, 28 Sep 2021 12:26:52 GMT  
		Size: 315.2 KB (315237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b400ed504130934571dad558eea43e0360a76dce52a046e08a6ad9ca01b97e`  
		Last Modified: Tue, 28 Sep 2021 12:27:02 GMT  
		Size: 74.1 MB (74088130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab0fcd02a4c23ce4ead674fc0400593f9796826f4accf07f8121249de06589f`  
		Last Modified: Tue, 28 Sep 2021 12:28:37 GMT  
		Size: 481.7 MB (481687945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:1d357621cc38e1a4d09ad86f5c6e6f9ea2822a4a18cbfb54d215aec7282b3334
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:8ff176871535f3a09a7d11d26314d881ad42c944b63cf7e3a6daedfcf544011c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.7 MB (840658961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78e91c26d3138b63e62f54f114439797e8bff78b337ba0e5c9cba91b0a622090`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 06:02:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 06:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 06:04:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:04:15 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:04:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:05:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8985568900a589503a6b64505536a7ed14c04be58f49125487546556e4bf16d2`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396a66dc135f942aded0cbf41869920dd471f4ae69a577ef485c7fad6ad26f6`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e67a2d329fca5d4ed9676dc99b6786e3b630fb2cdc61a582593ee9c0d2af6`  
		Last Modified: Fri, 01 Oct 2021 06:24:57 GMT  
		Size: 176.7 MB (176698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f46e6b695aaf67ea964cbc89cec1bb208303e42ef77d8ae91776e089bb5ca`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9999226e85f92a036c340a8cd8f6223dae10b187aabfcafcb3bf8db55c579c4c`  
		Last Modified: Fri, 01 Oct 2021 06:25:15 GMT  
		Size: 47.3 MB (47259853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d72ee051e2ffafedab97e53d9c1c7dd3d04e22c91edd5a6f5998bbc8649d9d`  
		Last Modified: Fri, 01 Oct 2021 06:25:07 GMT  
		Size: 321.5 KB (321468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e3373d9dd06236066e1567f04e4344c9a90b98b797e7f2ad101fbb541811bd`  
		Last Modified: Fri, 01 Oct 2021 06:25:20 GMT  
		Size: 79.6 MB (79603325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8c92225baeee3737c60e0433c14c1a5d67f77aa6da87cc9c2fefecbce90b8a`  
		Last Modified: Fri, 01 Oct 2021 06:27:02 GMT  
		Size: 501.5 MB (501473984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:f40be954b42fdbf2c8658b0378454aff44e042a9dd0cd047fa1faf526993e0ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **730.2 MB (730245800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d65f25fc22d5b0aa108a74c05817159af01187025e7ef2e0e00644a7274356`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:58:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:58:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:01:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:01:07 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:01:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:02:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:08:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597f16c1171caedee0148b09aba1a7c8b8ff2f29ffec5f8bc82f4a2d0c4a955`  
		Last Modified: Tue, 31 Aug 2021 04:17:31 GMT  
		Size: 1.2 MB (1183503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f278f986afdfeaabcdd6e3e66554d2851e9813dda91fc83341f7cdf3dca05`  
		Last Modified: Tue, 31 Aug 2021 04:17:30 GMT  
		Size: 4.7 MB (4676468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf026e89b16b8250a76b892191540bf0879aafa7e00242a2f6151d466ee9f283`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c21ec0037b0f9bae7c4c1a4415d768ebce97dc86e798bff4f6e544059ac5e`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db678ae234a6fe1d46c8463a559f04c415c2522d0effab08ae407178410d5db`  
		Last Modified: Tue, 31 Aug 2021 04:19:33 GMT  
		Size: 157.2 MB (157216591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79678cecea953d0568fb159f017c76dd5db59346cc095d3d118b734bade1037d`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7610242426bc226b21c63941458db4760063f2536207c80d92f79642ede166d`  
		Last Modified: Tue, 31 Aug 2021 04:20:05 GMT  
		Size: 36.7 MB (36691316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d75fec186326e68092c8c944a4991cf20df280505668146aeab88ef75f42f`  
		Last Modified: Tue, 31 Aug 2021 04:19:46 GMT  
		Size: 317.9 KB (317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891bd701076db5d3efe95bd46c285b538fbf4d20a17a3fdde54216d561a397d0`  
		Last Modified: Tue, 31 Aug 2021 04:20:24 GMT  
		Size: 60.5 MB (60482196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb6760ee5d1314fbec6f42620c54f10eacb13ab219ff411714d6e2706987a45`  
		Last Modified: Tue, 31 Aug 2021 04:25:40 GMT  
		Size: 445.6 MB (445606636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a59d10cada697347393717ed37ed4ce2474f9427539ee17804d81757479f7d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **790.9 MB (790927813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eabb6eb581ac47318cca2b8ef351a73988712c5ed1ff2021a1ad06e7ad9cec4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:05:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 04:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:06:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:06:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:07:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:09:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5955ec7390235db14b9c45d9030bd90295fdbfc2dd976b408668c1feaa0c16ba`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3177f1eddf2202fb915200162e8693b4fc55482d73411891f1184df5517140`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76170f07a4a0b1a928e2367788be540ac8379fbb9cdd2461ef5248e67f7ffb96`  
		Last Modified: Fri, 01 Oct 2021 04:21:43 GMT  
		Size: 171.1 MB (171135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ffa5ef1c6b2f2640d24037747e349bcb1b99eaba29240f0b7e62c35115462`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d780d95d984615f9091bcff4af07fbec2f87e83f046d35e9ab14912242c636ff`  
		Last Modified: Fri, 01 Oct 2021 04:22:03 GMT  
		Size: 41.5 MB (41521018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6924807e2d6734e0d3876de4e1a66637f28fa98b175e630040905e31e3bcf5`  
		Last Modified: Fri, 01 Oct 2021 04:21:56 GMT  
		Size: 321.5 KB (321466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a22ce1c357749088045cd1e5a809f080f05d6e6adc9a0f721bd15d6ff9b750`  
		Last Modified: Fri, 01 Oct 2021 04:22:07 GMT  
		Size: 72.0 MB (71972774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a048aff215857f993c4474873a3ad80d194f16a3e39098731c04c14b35ef6e3d`  
		Last Modified: Fri, 01 Oct 2021 04:23:51 GMT  
		Size: 472.1 MB (472105481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:6ef3862758afe8d7fc34a6f2bf61a9443b00b8785af10be525b061e73aedc59a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:55837b1cb4d123a7d660ef72f2049c8f0549ec14d8880662d5df6bfd1c1b8f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.9 MB (354923887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dc39b9cef5aa66733784d741535e752bbb6d1588294e89ba4ecfc10d91eed3b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 06:02:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 06:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 06:04:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:04:15 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:04:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:05:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:06:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8985568900a589503a6b64505536a7ed14c04be58f49125487546556e4bf16d2`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396a66dc135f942aded0cbf41869920dd471f4ae69a577ef485c7fad6ad26f6`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e67a2d329fca5d4ed9676dc99b6786e3b630fb2cdc61a582593ee9c0d2af6`  
		Last Modified: Fri, 01 Oct 2021 06:24:57 GMT  
		Size: 176.7 MB (176698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f46e6b695aaf67ea964cbc89cec1bb208303e42ef77d8ae91776e089bb5ca`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9999226e85f92a036c340a8cd8f6223dae10b187aabfcafcb3bf8db55c579c4c`  
		Last Modified: Fri, 01 Oct 2021 06:25:15 GMT  
		Size: 47.3 MB (47259853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d72ee051e2ffafedab97e53d9c1c7dd3d04e22c91edd5a6f5998bbc8649d9d`  
		Last Modified: Fri, 01 Oct 2021 06:25:07 GMT  
		Size: 321.5 KB (321468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e3373d9dd06236066e1567f04e4344c9a90b98b797e7f2ad101fbb541811bd`  
		Last Modified: Fri, 01 Oct 2021 06:25:20 GMT  
		Size: 79.6 MB (79603325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d8971de91fa5cee1dee45e2e717a59c529854e5c18f2619545c3b5163bf712`  
		Last Modified: Fri, 01 Oct 2021 06:25:35 GMT  
		Size: 15.7 MB (15738910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:a93bc750dcb94b706e6890c2e20447a93695a36a9769025afe914236daa83513
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298599820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dabbf0fd6b1799fc6e97af3714e31f39e7f4b19652ca99176ee7e9e321424300`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:58:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:58:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:01:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:01:07 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:01:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:02:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:03:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597f16c1171caedee0148b09aba1a7c8b8ff2f29ffec5f8bc82f4a2d0c4a955`  
		Last Modified: Tue, 31 Aug 2021 04:17:31 GMT  
		Size: 1.2 MB (1183503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f278f986afdfeaabcdd6e3e66554d2851e9813dda91fc83341f7cdf3dca05`  
		Last Modified: Tue, 31 Aug 2021 04:17:30 GMT  
		Size: 4.7 MB (4676468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf026e89b16b8250a76b892191540bf0879aafa7e00242a2f6151d466ee9f283`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c21ec0037b0f9bae7c4c1a4415d768ebce97dc86e798bff4f6e544059ac5e`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db678ae234a6fe1d46c8463a559f04c415c2522d0effab08ae407178410d5db`  
		Last Modified: Tue, 31 Aug 2021 04:19:33 GMT  
		Size: 157.2 MB (157216591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79678cecea953d0568fb159f017c76dd5db59346cc095d3d118b734bade1037d`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7610242426bc226b21c63941458db4760063f2536207c80d92f79642ede166d`  
		Last Modified: Tue, 31 Aug 2021 04:20:05 GMT  
		Size: 36.7 MB (36691316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d75fec186326e68092c8c944a4991cf20df280505668146aeab88ef75f42f`  
		Last Modified: Tue, 31 Aug 2021 04:19:46 GMT  
		Size: 317.9 KB (317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891bd701076db5d3efe95bd46c285b538fbf4d20a17a3fdde54216d561a397d0`  
		Last Modified: Tue, 31 Aug 2021 04:20:24 GMT  
		Size: 60.5 MB (60482196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0442b6c688a80b7163819b34b289a2b5b96fb82af79d1621ce7fb8ba361ed83`  
		Last Modified: Tue, 31 Aug 2021 04:20:51 GMT  
		Size: 14.0 MB (13960656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ff822091f91909ac49b13bcb7a86799bb53dbd5e592d2ba47d9faa0f4fe46662
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334174646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b29bfaa4df7f8ee33f2acb5483d92c7db0754983dd3cf0ff12080a7d9c3e29`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:05:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 04:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:06:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:06:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:07:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:07:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5955ec7390235db14b9c45d9030bd90295fdbfc2dd976b408668c1feaa0c16ba`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3177f1eddf2202fb915200162e8693b4fc55482d73411891f1184df5517140`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76170f07a4a0b1a928e2367788be540ac8379fbb9cdd2461ef5248e67f7ffb96`  
		Last Modified: Fri, 01 Oct 2021 04:21:43 GMT  
		Size: 171.1 MB (171135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ffa5ef1c6b2f2640d24037747e349bcb1b99eaba29240f0b7e62c35115462`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d780d95d984615f9091bcff4af07fbec2f87e83f046d35e9ab14912242c636ff`  
		Last Modified: Fri, 01 Oct 2021 04:22:03 GMT  
		Size: 41.5 MB (41521018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6924807e2d6734e0d3876de4e1a66637f28fa98b175e630040905e31e3bcf5`  
		Last Modified: Fri, 01 Oct 2021 04:21:56 GMT  
		Size: 321.5 KB (321466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a22ce1c357749088045cd1e5a809f080f05d6e6adc9a0f721bd15d6ff9b750`  
		Last Modified: Fri, 01 Oct 2021 04:22:07 GMT  
		Size: 72.0 MB (71972774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79704614a0b1db0bec012342151b370647ee3190bd4d146666f34664af209faf`  
		Last Modified: Fri, 01 Oct 2021 04:22:25 GMT  
		Size: 15.4 MB (15352314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:c80aba4719caade37d5891ec0aa23af5e3c5b273a924ca0e96b145c6430aed27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:ea43430366af28857397cdd9c9123ae578d872de0c21b0f990581d4b97beae7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.5 MB (484462438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1748353699e09fa4e1ca656b6dbbbfc6f9bdedbf03126331ed3d8e9f1b09c7df`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 21:16:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:16:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 28 Sep 2021 21:17:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 28 Sep 2021 21:17:08 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 21:17:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 28 Sep 2021 21:17:08 GMT
ENV ROS_DISTRO=noetic
# Tue, 28 Sep 2021 21:18:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:18:23 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 28 Sep 2021 21:18:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 28 Sep 2021 21:18:24 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 21:19:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:19:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 28 Sep 2021 21:19:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057f5227de8f6db89935faceb04e14221b934ffc6724618581f7e8392970c3ed`  
		Last Modified: Tue, 28 Sep 2021 21:24:45 GMT  
		Size: 10.9 MB (10891832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd2be7e40d77e274ec22ddb4f87a6316ce568f810184a8e59e18ba01fc96932`  
		Last Modified: Tue, 28 Sep 2021 21:24:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6d934e0e2132b27cda2cacacb9088097b537f9a40cdf536e2abc5d225c6387`  
		Last Modified: Tue, 28 Sep 2021 21:24:44 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898c3d5d521ed7072839820050082135fe093df92e6924f017afc47ddbb42355`  
		Last Modified: Tue, 28 Sep 2021 21:25:19 GMT  
		Size: 239.1 MB (239056614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57e0d0e6e00100bc444c8c1ff5b4028e0de1a63fe406669810c494e10803f6a`  
		Last Modified: Tue, 28 Sep 2021 21:24:43 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7a76943e01f7c49865103cc39e2286c3b843b81a9c9c07e122dfeeb1c99f93`  
		Last Modified: Tue, 28 Sep 2021 21:25:41 GMT  
		Size: 86.6 MB (86566434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb2d48531002cdd91f487084f1be81a6be323f175934a6d8ee366927fc89efa`  
		Last Modified: Tue, 28 Sep 2021 21:25:27 GMT  
		Size: 315.2 KB (315239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce5ac6d6887766f72c3011574775084de91b975f55a84cd4347d3bc3e028e6`  
		Last Modified: Tue, 28 Sep 2021 21:25:38 GMT  
		Size: 76.0 MB (75975243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fd6684a9f68292269e59c38c40597d2bb34cd8c64cba4c3bcf51ad4a38c999`  
		Last Modified: Tue, 28 Sep 2021 21:25:51 GMT  
		Size: 21.2 MB (21218452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e73636a83790f9515f5f8c62844c1728a260f15e9f0cbe1f955f909fcd7cd38e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.0 MB (424008459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e71fd1e6ee7dc3aba8a056021e464f2ae44b0431ed0fb710f5a393091c1f8bd5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 12:17:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:17:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 28 Sep 2021 12:18:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 28 Sep 2021 12:18:09 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 12:18:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 28 Sep 2021 12:18:09 GMT
ENV ROS_DISTRO=noetic
# Tue, 28 Sep 2021 12:19:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:19:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 28 Sep 2021 12:19:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 28 Sep 2021 12:19:16 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 12:19:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:20:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 28 Sep 2021 12:20:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:20:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b719e84e5c17a05db4cb91b65b25f4cecd9fda5ca86f7c93b9e8918c83ad07`  
		Last Modified: Tue, 28 Sep 2021 12:26:12 GMT  
		Size: 10.9 MB (10883372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b180205050ab5009747a1fa863a1467a5e672c5116542801e3f3890b57cc64`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0309f751216573b01fdef820a8e7c97a9ef1170563c0136c2e3faa29e4e99ed`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290538ca4b138960141fb0cf9d84a1ada042c2286a8714c2afa426ef9ea5baf9`  
		Last Modified: Tue, 28 Sep 2021 12:26:44 GMT  
		Size: 184.2 MB (184242688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8fe4a6c015780d0a432c652d6ac68724f7b7305a66625f3dde29654973d374`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570cd6760219c636efbd15651c975651d6776ef161e5daf5e95ca0d02cf74440`  
		Last Modified: Tue, 28 Sep 2021 12:27:04 GMT  
		Size: 84.4 MB (84358024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225d1354fc88caaadf4d1c8428bc28ea51f87d230c8889449d028a90955656a4`  
		Last Modified: Tue, 28 Sep 2021 12:26:52 GMT  
		Size: 315.2 KB (315237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b400ed504130934571dad558eea43e0360a76dce52a046e08a6ad9ca01b97e`  
		Last Modified: Tue, 28 Sep 2021 12:27:02 GMT  
		Size: 74.1 MB (74088130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba06582da62bcb346f305b44da190ca143fc77649afc27d2199c4b836985aeb8`  
		Last Modified: Tue, 28 Sep 2021 12:27:15 GMT  
		Size: 20.9 MB (20896212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:6ef3862758afe8d7fc34a6f2bf61a9443b00b8785af10be525b061e73aedc59a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:55837b1cb4d123a7d660ef72f2049c8f0549ec14d8880662d5df6bfd1c1b8f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.9 MB (354923887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dc39b9cef5aa66733784d741535e752bbb6d1588294e89ba4ecfc10d91eed3b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 06:02:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 06:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 06:04:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:04:15 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:04:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:05:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:06:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8985568900a589503a6b64505536a7ed14c04be58f49125487546556e4bf16d2`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396a66dc135f942aded0cbf41869920dd471f4ae69a577ef485c7fad6ad26f6`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e67a2d329fca5d4ed9676dc99b6786e3b630fb2cdc61a582593ee9c0d2af6`  
		Last Modified: Fri, 01 Oct 2021 06:24:57 GMT  
		Size: 176.7 MB (176698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f46e6b695aaf67ea964cbc89cec1bb208303e42ef77d8ae91776e089bb5ca`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9999226e85f92a036c340a8cd8f6223dae10b187aabfcafcb3bf8db55c579c4c`  
		Last Modified: Fri, 01 Oct 2021 06:25:15 GMT  
		Size: 47.3 MB (47259853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d72ee051e2ffafedab97e53d9c1c7dd3d04e22c91edd5a6f5998bbc8649d9d`  
		Last Modified: Fri, 01 Oct 2021 06:25:07 GMT  
		Size: 321.5 KB (321468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e3373d9dd06236066e1567f04e4344c9a90b98b797e7f2ad101fbb541811bd`  
		Last Modified: Fri, 01 Oct 2021 06:25:20 GMT  
		Size: 79.6 MB (79603325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d8971de91fa5cee1dee45e2e717a59c529854e5c18f2619545c3b5163bf712`  
		Last Modified: Fri, 01 Oct 2021 06:25:35 GMT  
		Size: 15.7 MB (15738910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:a93bc750dcb94b706e6890c2e20447a93695a36a9769025afe914236daa83513
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298599820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dabbf0fd6b1799fc6e97af3714e31f39e7f4b19652ca99176ee7e9e321424300`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:58:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:58:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:01:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:01:07 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:01:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:02:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:03:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597f16c1171caedee0148b09aba1a7c8b8ff2f29ffec5f8bc82f4a2d0c4a955`  
		Last Modified: Tue, 31 Aug 2021 04:17:31 GMT  
		Size: 1.2 MB (1183503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f278f986afdfeaabcdd6e3e66554d2851e9813dda91fc83341f7cdf3dca05`  
		Last Modified: Tue, 31 Aug 2021 04:17:30 GMT  
		Size: 4.7 MB (4676468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf026e89b16b8250a76b892191540bf0879aafa7e00242a2f6151d466ee9f283`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c21ec0037b0f9bae7c4c1a4415d768ebce97dc86e798bff4f6e544059ac5e`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db678ae234a6fe1d46c8463a559f04c415c2522d0effab08ae407178410d5db`  
		Last Modified: Tue, 31 Aug 2021 04:19:33 GMT  
		Size: 157.2 MB (157216591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79678cecea953d0568fb159f017c76dd5db59346cc095d3d118b734bade1037d`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7610242426bc226b21c63941458db4760063f2536207c80d92f79642ede166d`  
		Last Modified: Tue, 31 Aug 2021 04:20:05 GMT  
		Size: 36.7 MB (36691316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d75fec186326e68092c8c944a4991cf20df280505668146aeab88ef75f42f`  
		Last Modified: Tue, 31 Aug 2021 04:19:46 GMT  
		Size: 317.9 KB (317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891bd701076db5d3efe95bd46c285b538fbf4d20a17a3fdde54216d561a397d0`  
		Last Modified: Tue, 31 Aug 2021 04:20:24 GMT  
		Size: 60.5 MB (60482196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0442b6c688a80b7163819b34b289a2b5b96fb82af79d1621ce7fb8ba361ed83`  
		Last Modified: Tue, 31 Aug 2021 04:20:51 GMT  
		Size: 14.0 MB (13960656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ff822091f91909ac49b13bcb7a86799bb53dbd5e592d2ba47d9faa0f4fe46662
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334174646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b29bfaa4df7f8ee33f2acb5483d92c7db0754983dd3cf0ff12080a7d9c3e29`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:05:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 04:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:06:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:06:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:07:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:07:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5955ec7390235db14b9c45d9030bd90295fdbfc2dd976b408668c1feaa0c16ba`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3177f1eddf2202fb915200162e8693b4fc55482d73411891f1184df5517140`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76170f07a4a0b1a928e2367788be540ac8379fbb9cdd2461ef5248e67f7ffb96`  
		Last Modified: Fri, 01 Oct 2021 04:21:43 GMT  
		Size: 171.1 MB (171135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ffa5ef1c6b2f2640d24037747e349bcb1b99eaba29240f0b7e62c35115462`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d780d95d984615f9091bcff4af07fbec2f87e83f046d35e9ab14912242c636ff`  
		Last Modified: Fri, 01 Oct 2021 04:22:03 GMT  
		Size: 41.5 MB (41521018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6924807e2d6734e0d3876de4e1a66637f28fa98b175e630040905e31e3bcf5`  
		Last Modified: Fri, 01 Oct 2021 04:21:56 GMT  
		Size: 321.5 KB (321466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a22ce1c357749088045cd1e5a809f080f05d6e6adc9a0f721bd15d6ff9b750`  
		Last Modified: Fri, 01 Oct 2021 04:22:07 GMT  
		Size: 72.0 MB (71972774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79704614a0b1db0bec012342151b370647ee3190bd4d146666f34664af209faf`  
		Last Modified: Fri, 01 Oct 2021 04:22:25 GMT  
		Size: 15.4 MB (15352314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:ca310a19885c0aed922ac6d1936934d4740fe8b6be91437f0c18baedebcf636d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:ccaf1b2477838808d73663f41c34719386ad7ea977091fdcbd19c95b9feff8c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339184977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c618f40d6ef1b8f46c2c5e4114809283344e4b751a46ab67c77aa17f174d411`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 06:02:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 06:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 06:04:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:04:15 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:04:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:05:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8985568900a589503a6b64505536a7ed14c04be58f49125487546556e4bf16d2`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396a66dc135f942aded0cbf41869920dd471f4ae69a577ef485c7fad6ad26f6`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e67a2d329fca5d4ed9676dc99b6786e3b630fb2cdc61a582593ee9c0d2af6`  
		Last Modified: Fri, 01 Oct 2021 06:24:57 GMT  
		Size: 176.7 MB (176698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f46e6b695aaf67ea964cbc89cec1bb208303e42ef77d8ae91776e089bb5ca`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9999226e85f92a036c340a8cd8f6223dae10b187aabfcafcb3bf8db55c579c4c`  
		Last Modified: Fri, 01 Oct 2021 06:25:15 GMT  
		Size: 47.3 MB (47259853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d72ee051e2ffafedab97e53d9c1c7dd3d04e22c91edd5a6f5998bbc8649d9d`  
		Last Modified: Fri, 01 Oct 2021 06:25:07 GMT  
		Size: 321.5 KB (321468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e3373d9dd06236066e1567f04e4344c9a90b98b797e7f2ad101fbb541811bd`  
		Last Modified: Fri, 01 Oct 2021 06:25:20 GMT  
		Size: 79.6 MB (79603325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:3502680140f44f7d6e0f5d06694a932b440166eaaae3a7bb8459790377f695b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284639164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e9851a6cabd762aa85ab3b198ef0bac96359c28a5539db594ea18cfd4492bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:58:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:58:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:01:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:01:07 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:01:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:02:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597f16c1171caedee0148b09aba1a7c8b8ff2f29ffec5f8bc82f4a2d0c4a955`  
		Last Modified: Tue, 31 Aug 2021 04:17:31 GMT  
		Size: 1.2 MB (1183503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f278f986afdfeaabcdd6e3e66554d2851e9813dda91fc83341f7cdf3dca05`  
		Last Modified: Tue, 31 Aug 2021 04:17:30 GMT  
		Size: 4.7 MB (4676468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf026e89b16b8250a76b892191540bf0879aafa7e00242a2f6151d466ee9f283`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c21ec0037b0f9bae7c4c1a4415d768ebce97dc86e798bff4f6e544059ac5e`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db678ae234a6fe1d46c8463a559f04c415c2522d0effab08ae407178410d5db`  
		Last Modified: Tue, 31 Aug 2021 04:19:33 GMT  
		Size: 157.2 MB (157216591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79678cecea953d0568fb159f017c76dd5db59346cc095d3d118b734bade1037d`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7610242426bc226b21c63941458db4760063f2536207c80d92f79642ede166d`  
		Last Modified: Tue, 31 Aug 2021 04:20:05 GMT  
		Size: 36.7 MB (36691316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d75fec186326e68092c8c944a4991cf20df280505668146aeab88ef75f42f`  
		Last Modified: Tue, 31 Aug 2021 04:19:46 GMT  
		Size: 317.9 KB (317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891bd701076db5d3efe95bd46c285b538fbf4d20a17a3fdde54216d561a397d0`  
		Last Modified: Tue, 31 Aug 2021 04:20:24 GMT  
		Size: 60.5 MB (60482196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:66791732edf7e13167d9ea961d962152e5401ffa9d9ceb0f8c2cde65aec974f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.8 MB (318822332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78083a3273027cb4a7fd2603e6461c20f176f7f1dd44e1527c6b8236af556ced`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:05:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 04:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:06:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:06:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:07:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5955ec7390235db14b9c45d9030bd90295fdbfc2dd976b408668c1feaa0c16ba`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3177f1eddf2202fb915200162e8693b4fc55482d73411891f1184df5517140`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76170f07a4a0b1a928e2367788be540ac8379fbb9cdd2461ef5248e67f7ffb96`  
		Last Modified: Fri, 01 Oct 2021 04:21:43 GMT  
		Size: 171.1 MB (171135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ffa5ef1c6b2f2640d24037747e349bcb1b99eaba29240f0b7e62c35115462`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d780d95d984615f9091bcff4af07fbec2f87e83f046d35e9ab14912242c636ff`  
		Last Modified: Fri, 01 Oct 2021 04:22:03 GMT  
		Size: 41.5 MB (41521018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6924807e2d6734e0d3876de4e1a66637f28fa98b175e630040905e31e3bcf5`  
		Last Modified: Fri, 01 Oct 2021 04:21:56 GMT  
		Size: 321.5 KB (321466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a22ce1c357749088045cd1e5a809f080f05d6e6adc9a0f721bd15d6ff9b750`  
		Last Modified: Fri, 01 Oct 2021 04:22:07 GMT  
		Size: 72.0 MB (71972774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:9ca6a30b5a5955c1eaf3dd5f6861159e64a0e541c5a41931dd6dcaece396f7e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:6c5832e2d84090112679bdf9555940df7945a6fc5ac833b74bd4b3a0919ce99b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.2 MB (463243986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c72680f96123b9225bb0b5efb2484df6119d69ca2bbe8520ab36d53cf7a9b02e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 21:16:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:16:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 28 Sep 2021 21:17:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 28 Sep 2021 21:17:08 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 21:17:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 28 Sep 2021 21:17:08 GMT
ENV ROS_DISTRO=noetic
# Tue, 28 Sep 2021 21:18:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:18:23 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 28 Sep 2021 21:18:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 28 Sep 2021 21:18:24 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 21:19:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:19:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 28 Sep 2021 21:19:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057f5227de8f6db89935faceb04e14221b934ffc6724618581f7e8392970c3ed`  
		Last Modified: Tue, 28 Sep 2021 21:24:45 GMT  
		Size: 10.9 MB (10891832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd2be7e40d77e274ec22ddb4f87a6316ce568f810184a8e59e18ba01fc96932`  
		Last Modified: Tue, 28 Sep 2021 21:24:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6d934e0e2132b27cda2cacacb9088097b537f9a40cdf536e2abc5d225c6387`  
		Last Modified: Tue, 28 Sep 2021 21:24:44 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898c3d5d521ed7072839820050082135fe093df92e6924f017afc47ddbb42355`  
		Last Modified: Tue, 28 Sep 2021 21:25:19 GMT  
		Size: 239.1 MB (239056614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57e0d0e6e00100bc444c8c1ff5b4028e0de1a63fe406669810c494e10803f6a`  
		Last Modified: Tue, 28 Sep 2021 21:24:43 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7a76943e01f7c49865103cc39e2286c3b843b81a9c9c07e122dfeeb1c99f93`  
		Last Modified: Tue, 28 Sep 2021 21:25:41 GMT  
		Size: 86.6 MB (86566434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb2d48531002cdd91f487084f1be81a6be323f175934a6d8ee366927fc89efa`  
		Last Modified: Tue, 28 Sep 2021 21:25:27 GMT  
		Size: 315.2 KB (315239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce5ac6d6887766f72c3011574775084de91b975f55a84cd4347d3bc3e028e6`  
		Last Modified: Tue, 28 Sep 2021 21:25:38 GMT  
		Size: 76.0 MB (75975243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cdf99750830dd20baaff40832d809188c310cc50e756a5ebda57f957fb0d4bb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.1 MB (403112247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91640fff9a9235c79504f2d762e335c216d45f35a30c06904aeeaebba5b0bd6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 12:17:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:17:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 28 Sep 2021 12:18:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 28 Sep 2021 12:18:09 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 12:18:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 28 Sep 2021 12:18:09 GMT
ENV ROS_DISTRO=noetic
# Tue, 28 Sep 2021 12:19:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:19:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 28 Sep 2021 12:19:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 28 Sep 2021 12:19:16 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 12:19:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:20:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 28 Sep 2021 12:20:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b719e84e5c17a05db4cb91b65b25f4cecd9fda5ca86f7c93b9e8918c83ad07`  
		Last Modified: Tue, 28 Sep 2021 12:26:12 GMT  
		Size: 10.9 MB (10883372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b180205050ab5009747a1fa863a1467a5e672c5116542801e3f3890b57cc64`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0309f751216573b01fdef820a8e7c97a9ef1170563c0136c2e3faa29e4e99ed`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290538ca4b138960141fb0cf9d84a1ada042c2286a8714c2afa426ef9ea5baf9`  
		Last Modified: Tue, 28 Sep 2021 12:26:44 GMT  
		Size: 184.2 MB (184242688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8fe4a6c015780d0a432c652d6ac68724f7b7305a66625f3dde29654973d374`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570cd6760219c636efbd15651c975651d6776ef161e5daf5e95ca0d02cf74440`  
		Last Modified: Tue, 28 Sep 2021 12:27:04 GMT  
		Size: 84.4 MB (84358024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225d1354fc88caaadf4d1c8428bc28ea51f87d230c8889449d028a90955656a4`  
		Last Modified: Tue, 28 Sep 2021 12:26:52 GMT  
		Size: 315.2 KB (315237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b400ed504130934571dad558eea43e0360a76dce52a046e08a6ad9ca01b97e`  
		Last Modified: Tue, 28 Sep 2021 12:27:02 GMT  
		Size: 74.1 MB (74088130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:ca310a19885c0aed922ac6d1936934d4740fe8b6be91437f0c18baedebcf636d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:ccaf1b2477838808d73663f41c34719386ad7ea977091fdcbd19c95b9feff8c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339184977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c618f40d6ef1b8f46c2c5e4114809283344e4b751a46ab67c77aa17f174d411`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 06:02:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 06:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 06:04:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:04:15 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:04:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:05:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8985568900a589503a6b64505536a7ed14c04be58f49125487546556e4bf16d2`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396a66dc135f942aded0cbf41869920dd471f4ae69a577ef485c7fad6ad26f6`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e67a2d329fca5d4ed9676dc99b6786e3b630fb2cdc61a582593ee9c0d2af6`  
		Last Modified: Fri, 01 Oct 2021 06:24:57 GMT  
		Size: 176.7 MB (176698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f46e6b695aaf67ea964cbc89cec1bb208303e42ef77d8ae91776e089bb5ca`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9999226e85f92a036c340a8cd8f6223dae10b187aabfcafcb3bf8db55c579c4c`  
		Last Modified: Fri, 01 Oct 2021 06:25:15 GMT  
		Size: 47.3 MB (47259853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d72ee051e2ffafedab97e53d9c1c7dd3d04e22c91edd5a6f5998bbc8649d9d`  
		Last Modified: Fri, 01 Oct 2021 06:25:07 GMT  
		Size: 321.5 KB (321468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e3373d9dd06236066e1567f04e4344c9a90b98b797e7f2ad101fbb541811bd`  
		Last Modified: Fri, 01 Oct 2021 06:25:20 GMT  
		Size: 79.6 MB (79603325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:3502680140f44f7d6e0f5d06694a932b440166eaaae3a7bb8459790377f695b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284639164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e9851a6cabd762aa85ab3b198ef0bac96359c28a5539db594ea18cfd4492bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:58:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:58:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:01:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:01:07 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:01:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:02:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597f16c1171caedee0148b09aba1a7c8b8ff2f29ffec5f8bc82f4a2d0c4a955`  
		Last Modified: Tue, 31 Aug 2021 04:17:31 GMT  
		Size: 1.2 MB (1183503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f278f986afdfeaabcdd6e3e66554d2851e9813dda91fc83341f7cdf3dca05`  
		Last Modified: Tue, 31 Aug 2021 04:17:30 GMT  
		Size: 4.7 MB (4676468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf026e89b16b8250a76b892191540bf0879aafa7e00242a2f6151d466ee9f283`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c21ec0037b0f9bae7c4c1a4415d768ebce97dc86e798bff4f6e544059ac5e`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db678ae234a6fe1d46c8463a559f04c415c2522d0effab08ae407178410d5db`  
		Last Modified: Tue, 31 Aug 2021 04:19:33 GMT  
		Size: 157.2 MB (157216591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79678cecea953d0568fb159f017c76dd5db59346cc095d3d118b734bade1037d`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7610242426bc226b21c63941458db4760063f2536207c80d92f79642ede166d`  
		Last Modified: Tue, 31 Aug 2021 04:20:05 GMT  
		Size: 36.7 MB (36691316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d75fec186326e68092c8c944a4991cf20df280505668146aeab88ef75f42f`  
		Last Modified: Tue, 31 Aug 2021 04:19:46 GMT  
		Size: 317.9 KB (317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891bd701076db5d3efe95bd46c285b538fbf4d20a17a3fdde54216d561a397d0`  
		Last Modified: Tue, 31 Aug 2021 04:20:24 GMT  
		Size: 60.5 MB (60482196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:66791732edf7e13167d9ea961d962152e5401ffa9d9ceb0f8c2cde65aec974f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.8 MB (318822332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78083a3273027cb4a7fd2603e6461c20f176f7f1dd44e1527c6b8236af556ced`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:05:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 04:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:06:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:06:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:07:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5955ec7390235db14b9c45d9030bd90295fdbfc2dd976b408668c1feaa0c16ba`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3177f1eddf2202fb915200162e8693b4fc55482d73411891f1184df5517140`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76170f07a4a0b1a928e2367788be540ac8379fbb9cdd2461ef5248e67f7ffb96`  
		Last Modified: Fri, 01 Oct 2021 04:21:43 GMT  
		Size: 171.1 MB (171135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ffa5ef1c6b2f2640d24037747e349bcb1b99eaba29240f0b7e62c35115462`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d780d95d984615f9091bcff4af07fbec2f87e83f046d35e9ab14912242c636ff`  
		Last Modified: Fri, 01 Oct 2021 04:22:03 GMT  
		Size: 41.5 MB (41521018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6924807e2d6734e0d3876de4e1a66637f28fa98b175e630040905e31e3bcf5`  
		Last Modified: Fri, 01 Oct 2021 04:21:56 GMT  
		Size: 321.5 KB (321466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a22ce1c357749088045cd1e5a809f080f05d6e6adc9a0f721bd15d6ff9b750`  
		Last Modified: Fri, 01 Oct 2021 04:22:07 GMT  
		Size: 72.0 MB (71972774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:b8217be1fc3e6b6ff050a3240c45a7b22afc4b666ba37be64b663dc015742f34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:6c08c842014ab47086b7c7cf44822c1c38eb29021e3a507dd15f96c91bd80ef7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (212000331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34ca8509b2bc392cc43532c37d24093e0f2f9a034d86a6fca08aba57f40c5d59`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 06:02:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 06:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 06:04:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:04:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8985568900a589503a6b64505536a7ed14c04be58f49125487546556e4bf16d2`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396a66dc135f942aded0cbf41869920dd471f4ae69a577ef485c7fad6ad26f6`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e67a2d329fca5d4ed9676dc99b6786e3b630fb2cdc61a582593ee9c0d2af6`  
		Last Modified: Fri, 01 Oct 2021 06:24:57 GMT  
		Size: 176.7 MB (176698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f46e6b695aaf67ea964cbc89cec1bb208303e42ef77d8ae91776e089bb5ca`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:16e7b5ad0816dfb995956431231354e9108fc4bf112b8837081c4df3804bfec7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187147799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a616ba0d071ae4bd5b86fb577470a9d32a66c3c8fb9b569bfc03c1149ac6dc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:58:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:58:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:01:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:01:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597f16c1171caedee0148b09aba1a7c8b8ff2f29ffec5f8bc82f4a2d0c4a955`  
		Last Modified: Tue, 31 Aug 2021 04:17:31 GMT  
		Size: 1.2 MB (1183503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f278f986afdfeaabcdd6e3e66554d2851e9813dda91fc83341f7cdf3dca05`  
		Last Modified: Tue, 31 Aug 2021 04:17:30 GMT  
		Size: 4.7 MB (4676468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf026e89b16b8250a76b892191540bf0879aafa7e00242a2f6151d466ee9f283`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c21ec0037b0f9bae7c4c1a4415d768ebce97dc86e798bff4f6e544059ac5e`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db678ae234a6fe1d46c8463a559f04c415c2522d0effab08ae407178410d5db`  
		Last Modified: Tue, 31 Aug 2021 04:19:33 GMT  
		Size: 157.2 MB (157216591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79678cecea953d0568fb159f017c76dd5db59346cc095d3d118b734bade1037d`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6facbfe8fce44d9ee05d3b498a246e9f803369ec0409cca79b8317d52ff417be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205007074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1316784178101ce1bbeecbf3774b544a6e8e8741e4a498bccbae95017b7c74b4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:05:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 04:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:06:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5955ec7390235db14b9c45d9030bd90295fdbfc2dd976b408668c1feaa0c16ba`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3177f1eddf2202fb915200162e8693b4fc55482d73411891f1184df5517140`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76170f07a4a0b1a928e2367788be540ac8379fbb9cdd2461ef5248e67f7ffb96`  
		Last Modified: Fri, 01 Oct 2021 04:21:43 GMT  
		Size: 171.1 MB (171135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ffa5ef1c6b2f2640d24037747e349bcb1b99eaba29240f0b7e62c35115462`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:4121b39e6231399eb8d570b9d0f0d8bcadf105f604612c98f5e04902cac693df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:3f591f862d8faa3f59b80fe8672d369bd9b4667334e477412ab83626948f956c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300387070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62e0383210b61353f3b634a63f486a7cafda7453ec758fc23cbbd59375f63e2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 21:16:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:16:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 28 Sep 2021 21:17:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 28 Sep 2021 21:17:08 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 21:17:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 28 Sep 2021 21:17:08 GMT
ENV ROS_DISTRO=noetic
# Tue, 28 Sep 2021 21:18:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 21:18:23 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 28 Sep 2021 21:18:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 28 Sep 2021 21:18:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057f5227de8f6db89935faceb04e14221b934ffc6724618581f7e8392970c3ed`  
		Last Modified: Tue, 28 Sep 2021 21:24:45 GMT  
		Size: 10.9 MB (10891832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd2be7e40d77e274ec22ddb4f87a6316ce568f810184a8e59e18ba01fc96932`  
		Last Modified: Tue, 28 Sep 2021 21:24:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6d934e0e2132b27cda2cacacb9088097b537f9a40cdf536e2abc5d225c6387`  
		Last Modified: Tue, 28 Sep 2021 21:24:44 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898c3d5d521ed7072839820050082135fe093df92e6924f017afc47ddbb42355`  
		Last Modified: Tue, 28 Sep 2021 21:25:19 GMT  
		Size: 239.1 MB (239056614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57e0d0e6e00100bc444c8c1ff5b4028e0de1a63fe406669810c494e10803f6a`  
		Last Modified: Tue, 28 Sep 2021 21:24:43 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:99d1fc5a37c0866b5f8cc0b68ae004f80f762c86846ccece5140ba8849c421a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.4 MB (244350856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8594ef58160f3763d96577a1dd5bbe2e3e8da1909d605780cf98fa4669ec7dbd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 12:17:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:17:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 28 Sep 2021 12:18:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 28 Sep 2021 12:18:09 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 12:18:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 28 Sep 2021 12:18:09 GMT
ENV ROS_DISTRO=noetic
# Tue, 28 Sep 2021 12:19:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 12:19:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 28 Sep 2021 12:19:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 28 Sep 2021 12:19:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b719e84e5c17a05db4cb91b65b25f4cecd9fda5ca86f7c93b9e8918c83ad07`  
		Last Modified: Tue, 28 Sep 2021 12:26:12 GMT  
		Size: 10.9 MB (10883372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b180205050ab5009747a1fa863a1467a5e672c5116542801e3f3890b57cc64`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0309f751216573b01fdef820a8e7c97a9ef1170563c0136c2e3faa29e4e99ed`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290538ca4b138960141fb0cf9d84a1ada042c2286a8714c2afa426ef9ea5baf9`  
		Last Modified: Tue, 28 Sep 2021 12:26:44 GMT  
		Size: 184.2 MB (184242688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8fe4a6c015780d0a432c652d6ac68724f7b7305a66625f3dde29654973d374`  
		Last Modified: Tue, 28 Sep 2021 12:26:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:b8217be1fc3e6b6ff050a3240c45a7b22afc4b666ba37be64b663dc015742f34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:6c08c842014ab47086b7c7cf44822c1c38eb29021e3a507dd15f96c91bd80ef7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (212000331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34ca8509b2bc392cc43532c37d24093e0f2f9a034d86a6fca08aba57f40c5d59`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 06:02:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 06:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 06:04:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:04:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8985568900a589503a6b64505536a7ed14c04be58f49125487546556e4bf16d2`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396a66dc135f942aded0cbf41869920dd471f4ae69a577ef485c7fad6ad26f6`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e67a2d329fca5d4ed9676dc99b6786e3b630fb2cdc61a582593ee9c0d2af6`  
		Last Modified: Fri, 01 Oct 2021 06:24:57 GMT  
		Size: 176.7 MB (176698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f46e6b695aaf67ea964cbc89cec1bb208303e42ef77d8ae91776e089bb5ca`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:16e7b5ad0816dfb995956431231354e9108fc4bf112b8837081c4df3804bfec7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187147799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a616ba0d071ae4bd5b86fb577470a9d32a66c3c8fb9b569bfc03c1149ac6dc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:58:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:58:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:01:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:01:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597f16c1171caedee0148b09aba1a7c8b8ff2f29ffec5f8bc82f4a2d0c4a955`  
		Last Modified: Tue, 31 Aug 2021 04:17:31 GMT  
		Size: 1.2 MB (1183503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f278f986afdfeaabcdd6e3e66554d2851e9813dda91fc83341f7cdf3dca05`  
		Last Modified: Tue, 31 Aug 2021 04:17:30 GMT  
		Size: 4.7 MB (4676468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf026e89b16b8250a76b892191540bf0879aafa7e00242a2f6151d466ee9f283`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c21ec0037b0f9bae7c4c1a4415d768ebce97dc86e798bff4f6e544059ac5e`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db678ae234a6fe1d46c8463a559f04c415c2522d0effab08ae407178410d5db`  
		Last Modified: Tue, 31 Aug 2021 04:19:33 GMT  
		Size: 157.2 MB (157216591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79678cecea953d0568fb159f017c76dd5db59346cc095d3d118b734bade1037d`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6facbfe8fce44d9ee05d3b498a246e9f803369ec0409cca79b8317d52ff417be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205007074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1316784178101ce1bbeecbf3774b544a6e8e8741e4a498bccbae95017b7c74b4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:05:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 04:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:06:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5955ec7390235db14b9c45d9030bd90295fdbfc2dd976b408668c1feaa0c16ba`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3177f1eddf2202fb915200162e8693b4fc55482d73411891f1184df5517140`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76170f07a4a0b1a928e2367788be540ac8379fbb9cdd2461ef5248e67f7ffb96`  
		Last Modified: Fri, 01 Oct 2021 04:21:43 GMT  
		Size: 171.1 MB (171135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ffa5ef1c6b2f2640d24037747e349bcb1b99eaba29240f0b7e62c35115462`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:4ee61443ab81fadfcda087198b0cab898ecec782b6db3f7863362034d857d345
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:3aa63d43dfebbd5a6cefc413732c534afba950cc22fd6509b672d82772c268a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.7 MB (232729097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2574d7bc56da9c2886cd2eed096c23d94e8b36fb6137874207750e1d2b7f0d84`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:19:35 GMT
ENV ROS_DISTRO=rolling
# Fri, 01 Oct 2021 06:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:20:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:20:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:20:20 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:20:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:20:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:20:51 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 06:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b554d81fe16e0e94a43e8b06d838c8f786d52a9a0b89ecc0e8efb40c1a29aefb`  
		Last Modified: Fri, 01 Oct 2021 06:29:18 GMT  
		Size: 104.2 MB (104197012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d563e32523bf169883756bc09604daa8bf3bbbab8d20a0b1349afe202a434ea`  
		Last Modified: Fri, 01 Oct 2021 06:29:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32897aa3db60b88f4b19dc1072577c8e618ea9ec9ac9572e3f456f8a6df83871`  
		Last Modified: Fri, 01 Oct 2021 06:29:38 GMT  
		Size: 70.8 MB (70796896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18badf94b2b42a43cb4073ca4ed7a0d4a3bff87d40210af1205c9d866ca7beea`  
		Last Modified: Fri, 01 Oct 2021 06:29:28 GMT  
		Size: 246.1 KB (246073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a08879a1756fb090aa917136637f44131517da1fa1fc60ff224cc782071b84`  
		Last Modified: Fri, 01 Oct 2021 06:29:28 GMT  
		Size: 2.0 KB (2017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0552cadc20be7acdc95b229c976252440b8e57b9a228c86c5396d06528134d95`  
		Last Modified: Fri, 01 Oct 2021 06:29:32 GMT  
		Size: 22.2 MB (22185027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c96a54b08d6622f913c50b399e3d012a6cf6f162b829a326ec6603519d8bf4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221353385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a1306ab4a113218c9f4d0ace561ba41d3ccf9adab7a89da756acaaf81706f49`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:14:48 GMT
ENV ROS_DISTRO=rolling
# Fri, 01 Oct 2021 04:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:15:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:15:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:15:43 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:16:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:16:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:16:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 04:16:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08513d2f3e9188ae8ea6d5851048f335e9c160d03ee48ae75c7fb8c9afad07fa`  
		Last Modified: Fri, 01 Oct 2021 04:26:25 GMT  
		Size: 100.6 MB (100568224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c5264a8b044c054fe5d9dc04a5a0cf3c914e4cd3535ad6c8596a0b96a15d8b`  
		Last Modified: Fri, 01 Oct 2021 04:26:07 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0eff781a6f77828c4915114584bf3e9edd8f1308a168ac79afb665152fdf4a`  
		Last Modified: Fri, 01 Oct 2021 04:26:50 GMT  
		Size: 65.1 MB (65138693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a016822bb5cd49ab4e71c1082464dd37689aa7471fb306ede1cfca5eff18220`  
		Last Modified: Fri, 01 Oct 2021 04:26:39 GMT  
		Size: 246.1 KB (246075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6383fd0264d5da6acd9e3196f0af5956a67341cb79394c65199650516764b90`  
		Last Modified: Fri, 01 Oct 2021 04:26:39 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de74966aa3dcc6e30ddb16cb05a7df14f98ddc6802642e40a280e6a3bfad557c`  
		Last Modified: Fri, 01 Oct 2021 04:26:43 GMT  
		Size: 21.5 MB (21527018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:4ee61443ab81fadfcda087198b0cab898ecec782b6db3f7863362034d857d345
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:3aa63d43dfebbd5a6cefc413732c534afba950cc22fd6509b672d82772c268a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.7 MB (232729097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2574d7bc56da9c2886cd2eed096c23d94e8b36fb6137874207750e1d2b7f0d84`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:19:35 GMT
ENV ROS_DISTRO=rolling
# Fri, 01 Oct 2021 06:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:20:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:20:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:20:20 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:20:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:20:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:20:51 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 06:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b554d81fe16e0e94a43e8b06d838c8f786d52a9a0b89ecc0e8efb40c1a29aefb`  
		Last Modified: Fri, 01 Oct 2021 06:29:18 GMT  
		Size: 104.2 MB (104197012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d563e32523bf169883756bc09604daa8bf3bbbab8d20a0b1349afe202a434ea`  
		Last Modified: Fri, 01 Oct 2021 06:29:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32897aa3db60b88f4b19dc1072577c8e618ea9ec9ac9572e3f456f8a6df83871`  
		Last Modified: Fri, 01 Oct 2021 06:29:38 GMT  
		Size: 70.8 MB (70796896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18badf94b2b42a43cb4073ca4ed7a0d4a3bff87d40210af1205c9d866ca7beea`  
		Last Modified: Fri, 01 Oct 2021 06:29:28 GMT  
		Size: 246.1 KB (246073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a08879a1756fb090aa917136637f44131517da1fa1fc60ff224cc782071b84`  
		Last Modified: Fri, 01 Oct 2021 06:29:28 GMT  
		Size: 2.0 KB (2017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0552cadc20be7acdc95b229c976252440b8e57b9a228c86c5396d06528134d95`  
		Last Modified: Fri, 01 Oct 2021 06:29:32 GMT  
		Size: 22.2 MB (22185027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c96a54b08d6622f913c50b399e3d012a6cf6f162b829a326ec6603519d8bf4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221353385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a1306ab4a113218c9f4d0ace561ba41d3ccf9adab7a89da756acaaf81706f49`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:14:48 GMT
ENV ROS_DISTRO=rolling
# Fri, 01 Oct 2021 04:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:15:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:15:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:15:43 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:16:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:16:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:16:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 04:16:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08513d2f3e9188ae8ea6d5851048f335e9c160d03ee48ae75c7fb8c9afad07fa`  
		Last Modified: Fri, 01 Oct 2021 04:26:25 GMT  
		Size: 100.6 MB (100568224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c5264a8b044c054fe5d9dc04a5a0cf3c914e4cd3535ad6c8596a0b96a15d8b`  
		Last Modified: Fri, 01 Oct 2021 04:26:07 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0eff781a6f77828c4915114584bf3e9edd8f1308a168ac79afb665152fdf4a`  
		Last Modified: Fri, 01 Oct 2021 04:26:50 GMT  
		Size: 65.1 MB (65138693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a016822bb5cd49ab4e71c1082464dd37689aa7471fb306ede1cfca5eff18220`  
		Last Modified: Fri, 01 Oct 2021 04:26:39 GMT  
		Size: 246.1 KB (246075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6383fd0264d5da6acd9e3196f0af5956a67341cb79394c65199650516764b90`  
		Last Modified: Fri, 01 Oct 2021 04:26:39 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de74966aa3dcc6e30ddb16cb05a7df14f98ddc6802642e40a280e6a3bfad557c`  
		Last Modified: Fri, 01 Oct 2021 04:26:43 GMT  
		Size: 21.5 MB (21527018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-focal`

```console
$ docker pull ros@sha256:4ee61443ab81fadfcda087198b0cab898ecec782b6db3f7863362034d857d345
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:3aa63d43dfebbd5a6cefc413732c534afba950cc22fd6509b672d82772c268a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.7 MB (232729097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2574d7bc56da9c2886cd2eed096c23d94e8b36fb6137874207750e1d2b7f0d84`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:19:35 GMT
ENV ROS_DISTRO=rolling
# Fri, 01 Oct 2021 06:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:20:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:20:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:20:20 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 06:20:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:20:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 06:20:51 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 06:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b554d81fe16e0e94a43e8b06d838c8f786d52a9a0b89ecc0e8efb40c1a29aefb`  
		Last Modified: Fri, 01 Oct 2021 06:29:18 GMT  
		Size: 104.2 MB (104197012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d563e32523bf169883756bc09604daa8bf3bbbab8d20a0b1349afe202a434ea`  
		Last Modified: Fri, 01 Oct 2021 06:29:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32897aa3db60b88f4b19dc1072577c8e618ea9ec9ac9572e3f456f8a6df83871`  
		Last Modified: Fri, 01 Oct 2021 06:29:38 GMT  
		Size: 70.8 MB (70796896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18badf94b2b42a43cb4073ca4ed7a0d4a3bff87d40210af1205c9d866ca7beea`  
		Last Modified: Fri, 01 Oct 2021 06:29:28 GMT  
		Size: 246.1 KB (246073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a08879a1756fb090aa917136637f44131517da1fa1fc60ff224cc782071b84`  
		Last Modified: Fri, 01 Oct 2021 06:29:28 GMT  
		Size: 2.0 KB (2017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0552cadc20be7acdc95b229c976252440b8e57b9a228c86c5396d06528134d95`  
		Last Modified: Fri, 01 Oct 2021 06:29:32 GMT  
		Size: 22.2 MB (22185027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c96a54b08d6622f913c50b399e3d012a6cf6f162b829a326ec6603519d8bf4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221353385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a1306ab4a113218c9f4d0ace561ba41d3ccf9adab7a89da756acaaf81706f49`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:14:48 GMT
ENV ROS_DISTRO=rolling
# Fri, 01 Oct 2021 04:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:15:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:15:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:15:43 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:16:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:16:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:16:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 01 Oct 2021 04:16:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08513d2f3e9188ae8ea6d5851048f335e9c160d03ee48ae75c7fb8c9afad07fa`  
		Last Modified: Fri, 01 Oct 2021 04:26:25 GMT  
		Size: 100.6 MB (100568224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c5264a8b044c054fe5d9dc04a5a0cf3c914e4cd3535ad6c8596a0b96a15d8b`  
		Last Modified: Fri, 01 Oct 2021 04:26:07 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0eff781a6f77828c4915114584bf3e9edd8f1308a168ac79afb665152fdf4a`  
		Last Modified: Fri, 01 Oct 2021 04:26:50 GMT  
		Size: 65.1 MB (65138693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a016822bb5cd49ab4e71c1082464dd37689aa7471fb306ede1cfca5eff18220`  
		Last Modified: Fri, 01 Oct 2021 04:26:39 GMT  
		Size: 246.1 KB (246075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6383fd0264d5da6acd9e3196f0af5956a67341cb79394c65199650516764b90`  
		Last Modified: Fri, 01 Oct 2021 04:26:39 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de74966aa3dcc6e30ddb16cb05a7df14f98ddc6802642e40a280e6a3bfad557c`  
		Last Modified: Fri, 01 Oct 2021 04:26:43 GMT  
		Size: 21.5 MB (21527018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:383652aba1636ffbee14e7513b5e0b1ea08f4117e0f1563502d82b45372624af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:c746fc2c8542019474eeef83775035b31d3259d0580a52df340bb0ea90ddf003
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139499084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d61328b6b001f58935a0edf95acaf280caf479fc2d0374f5981e5ed5c6222d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:19:35 GMT
ENV ROS_DISTRO=rolling
# Fri, 01 Oct 2021 06:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:20:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:20:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:20:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b554d81fe16e0e94a43e8b06d838c8f786d52a9a0b89ecc0e8efb40c1a29aefb`  
		Last Modified: Fri, 01 Oct 2021 06:29:18 GMT  
		Size: 104.2 MB (104197012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d563e32523bf169883756bc09604daa8bf3bbbab8d20a0b1349afe202a434ea`  
		Last Modified: Fri, 01 Oct 2021 06:29:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bd3ab8f5f560533db8eb174f02b70203428eb6e2d5c227c1d976f60ffa9e076a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134439553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59285d785f69077e3ea373b23880dd5f0307a9f529d2556e35dbe613705b44bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:14:48 GMT
ENV ROS_DISTRO=rolling
# Fri, 01 Oct 2021 04:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:15:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:15:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:15:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08513d2f3e9188ae8ea6d5851048f335e9c160d03ee48ae75c7fb8c9afad07fa`  
		Last Modified: Fri, 01 Oct 2021 04:26:25 GMT  
		Size: 100.6 MB (100568224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c5264a8b044c054fe5d9dc04a5a0cf3c914e4cd3535ad6c8596a0b96a15d8b`  
		Last Modified: Fri, 01 Oct 2021 04:26:07 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-focal`

```console
$ docker pull ros@sha256:383652aba1636ffbee14e7513b5e0b1ea08f4117e0f1563502d82b45372624af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:c746fc2c8542019474eeef83775035b31d3259d0580a52df340bb0ea90ddf003
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139499084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d61328b6b001f58935a0edf95acaf280caf479fc2d0374f5981e5ed5c6222d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:19:35 GMT
ENV ROS_DISTRO=rolling
# Fri, 01 Oct 2021 06:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:20:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:20:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:20:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b554d81fe16e0e94a43e8b06d838c8f786d52a9a0b89ecc0e8efb40c1a29aefb`  
		Last Modified: Fri, 01 Oct 2021 06:29:18 GMT  
		Size: 104.2 MB (104197012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d563e32523bf169883756bc09604daa8bf3bbbab8d20a0b1349afe202a434ea`  
		Last Modified: Fri, 01 Oct 2021 06:29:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bd3ab8f5f560533db8eb174f02b70203428eb6e2d5c227c1d976f60ffa9e076a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134439553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59285d785f69077e3ea373b23880dd5f0307a9f529d2556e35dbe613705b44bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:14:48 GMT
ENV ROS_DISTRO=rolling
# Fri, 01 Oct 2021 04:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:15:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:15:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:15:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08513d2f3e9188ae8ea6d5851048f335e9c160d03ee48ae75c7fb8c9afad07fa`  
		Last Modified: Fri, 01 Oct 2021 04:26:25 GMT  
		Size: 100.6 MB (100568224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c5264a8b044c054fe5d9dc04a5a0cf3c914e4cd3535ad6c8596a0b96a15d8b`  
		Last Modified: Fri, 01 Oct 2021 04:26:07 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge`

```console
$ docker pull ros@sha256:36fb8d5de195e34e1949a2cc457d69319b1f180f1cd3483db8ff7551aa15b05a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:fd02fcae6ef30633920f78f998ffbf61b20236819bbeb8f1cdbd46883ed386a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.2 MB (326244769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0a397657f3c7a58bd6c4f8c9e98d5eac807d5f6a83ac8136a8a3bc2b17a343`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:36:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:37:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:51:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 04:51:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 04:56:50 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Aug 2021 04:57:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:57:31 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 04:57:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:57:32 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:57:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:58:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:58:07 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 04:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:58:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 04:58:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:58:37 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 04:58:37 GMT
ENV ROS2_DISTRO=rolling
# Tue, 31 Aug 2021 04:59:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.16.0-1*     ros-rolling-demo-nodes-py=0.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:59:11 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a41ae3b013398d2c13b5bceb3338e9582560c6d0ffd908463d766628be0a9c`  
		Last Modified: Tue, 31 Aug 2021 05:02:39 GMT  
		Size: 1.2 MB (1182916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8296a87df0b7498eeb5c80b365dfd866191372bea87427717ea787d78a5a7`  
		Last Modified: Tue, 31 Aug 2021 05:02:37 GMT  
		Size: 5.5 MB (5547451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f6733b55cc5feea2d4ee150c8dea08c02292286df2ded324ce1cce11cafe5e`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a37fcb7b853af691c37b315d95d9c1f6192ce41615e3588a9a36e174207371`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40bab908ffddd202a577d5bef2464f31547c2841e94e6a23fcfeeac00017515`  
		Last Modified: Tue, 31 Aug 2021 05:08:26 GMT  
		Size: 104.1 MB (104146807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf1c154560e156f2f4805693aaca2126fcb386eae3cd6825f0168543b51923d`  
		Last Modified: Tue, 31 Aug 2021 05:08:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f18c8918f43ab9c83750978f0b039de19d588b7005c24bd8f3ba1719a1cb6`  
		Last Modified: Tue, 31 Aug 2021 05:08:47 GMT  
		Size: 70.8 MB (70797635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ec3aca55a5a8332b228264f2d8a9579042a7b0732b23e4690ef77708970b7`  
		Last Modified: Tue, 31 Aug 2021 05:08:37 GMT  
		Size: 243.4 KB (243353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea6102c8c7f36c55a6d032dfaf36550669a7dcf8743b74915b32ce96165fe35`  
		Last Modified: Tue, 31 Aug 2021 05:08:36 GMT  
		Size: 2.0 KB (2017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec08e1246064b55c16dfbfce20bbebb65942cd2a01f12a8f893409e23837405f`  
		Last Modified: Tue, 31 Aug 2021 05:08:40 GMT  
		Size: 22.2 MB (22184233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57d0222bda6193c1c3877320cdbe8ca07509358658a805a7c83aaa9edb77777`  
		Last Modified: Tue, 31 Aug 2021 05:09:02 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25edb2a8e70c9a3ef372c7c84972b1efb20524c77aafbe913f5a714370d2944e`  
		Last Modified: Tue, 31 Aug 2021 05:09:02 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e017aaac77fb5e81b2592fe22095b3dd661f0c95cb3dd7760a8ea6ee5fc82727`  
		Last Modified: Tue, 31 Aug 2021 05:09:16 GMT  
		Size: 78.4 MB (78425179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebe9a2a06524d2a6d16bfdc3ba1ba60899aa0cccd9c711a5739ef284bc05707`  
		Last Modified: Tue, 31 Aug 2021 05:09:05 GMT  
		Size: 15.1 MB (15142071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6384ded0d228c843b661dcc9a8c1783535ef642c0beb6183919ca7d8654d906c`  
		Last Modified: Tue, 31 Aug 2021 05:09:02 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:68468ac2b592b84dfaf20f49bb60edc59b0afa216eb47435803f5b68171cc498
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.4 MB (314397076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c88b7492ee1a3327220ba723459be0df41a8a1c4cfa1997003ca073e08b325e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:35:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 02:40:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 02:45:28 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Aug 2021 02:46:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:46:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 02:46:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 02:46:09 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:46:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:46:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 02:46:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 02:47:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:47:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 02:47:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:47:18 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 02:47:18 GMT
ENV ROS2_DISTRO=rolling
# Tue, 31 Aug 2021 02:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:47:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.16.0-1*     ros-rolling-demo-nodes-py=0.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:47:53 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b869ca97320a7af4e9ce7c382543a1b04a7005c70779507cbb85ace89adde42e`  
		Last Modified: Tue, 31 Aug 2021 02:52:34 GMT  
		Size: 1.2 MB (1183579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c7b498b8e70b033b401f685710eb46ada1aab199891dfe061488eb0ba40831`  
		Last Modified: Tue, 31 Aug 2021 02:52:32 GMT  
		Size: 5.5 MB (5512786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153e16b4767757045ca5abd59a845a7b7cbc2916b1d1a63d930661eec9fc232b`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e90d25ecd370ffb201a02739df5a10f437fb2d2c95060875411cf40d5d0e12`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b5c1e17fbe503ccf8bebc08da06f5478b90f03326ea7cc016d9e73507f10ce`  
		Last Modified: Tue, 31 Aug 2021 02:58:52 GMT  
		Size: 100.5 MB (100535790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45400d8e0bf75fe9e077d037d3f7b0e895432f5540ae74445ce40f4b797111a7`  
		Last Modified: Tue, 31 Aug 2021 02:58:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1497a728946ec991c8b236b4101cde77517a464c2b22ebc0c2853c613f8edc`  
		Last Modified: Tue, 31 Aug 2021 02:59:15 GMT  
		Size: 65.1 MB (65137816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cb14f8cc4408bc999a0012920c6670355132f9cd04cfa6f3632da05868c24b`  
		Last Modified: Tue, 31 Aug 2021 02:59:04 GMT  
		Size: 243.4 KB (243377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a36f33083ce43a2fe6e2a6de6c0ef97f01bfded87f9bb0c50615c85cb4e312`  
		Last Modified: Tue, 31 Aug 2021 02:59:04 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177b7dcdd13b2c3e4ae37d2c849c4d4f5288ac23426c57d481e802f7cc6d6d96`  
		Last Modified: Tue, 31 Aug 2021 02:59:07 GMT  
		Size: 21.5 MB (21526088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda22c832442974a0ad5794123fbb4e6221cdb2bc0453dae21d103dbfec86f5`  
		Last Modified: Tue, 31 Aug 2021 02:59:31 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82725bf8c13207af80944626bf8589affa0081f57afc0ac9909f1593c083bef8`  
		Last Modified: Tue, 31 Aug 2021 02:59:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d686b241380f7b3f8cfa70ef4d17a3aa23b8aa004ed5a0b058f2ef1297a313`  
		Last Modified: Tue, 31 Aug 2021 02:59:47 GMT  
		Size: 78.4 MB (78374994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4acdaad577df7d049bf04dedb300fb427799c94a4b55e063a1b5127c5e31d45`  
		Last Modified: Tue, 31 Aug 2021 02:59:34 GMT  
		Size: 14.7 MB (14704492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7e46de183de8b86fe1c86ff9b994c58a22b11e9a8d9327c1f58b6bcc729ec7`  
		Last Modified: Tue, 31 Aug 2021 02:59:31 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:36fb8d5de195e34e1949a2cc457d69319b1f180f1cd3483db8ff7551aa15b05a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:fd02fcae6ef30633920f78f998ffbf61b20236819bbeb8f1cdbd46883ed386a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.2 MB (326244769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0a397657f3c7a58bd6c4f8c9e98d5eac807d5f6a83ac8136a8a3bc2b17a343`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:36:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:37:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:51:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 04:51:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 04:51:14 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 04:56:50 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Aug 2021 04:57:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:57:31 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 04:57:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:57:32 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:57:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:58:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:58:07 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 04:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:58:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 04:58:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:58:37 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 04:58:37 GMT
ENV ROS2_DISTRO=rolling
# Tue, 31 Aug 2021 04:59:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.16.0-1*     ros-rolling-demo-nodes-py=0.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:59:11 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a41ae3b013398d2c13b5bceb3338e9582560c6d0ffd908463d766628be0a9c`  
		Last Modified: Tue, 31 Aug 2021 05:02:39 GMT  
		Size: 1.2 MB (1182916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8296a87df0b7498eeb5c80b365dfd866191372bea87427717ea787d78a5a7`  
		Last Modified: Tue, 31 Aug 2021 05:02:37 GMT  
		Size: 5.5 MB (5547451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f6733b55cc5feea2d4ee150c8dea08c02292286df2ded324ce1cce11cafe5e`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a37fcb7b853af691c37b315d95d9c1f6192ce41615e3588a9a36e174207371`  
		Last Modified: Tue, 31 Aug 2021 05:05:22 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40bab908ffddd202a577d5bef2464f31547c2841e94e6a23fcfeeac00017515`  
		Last Modified: Tue, 31 Aug 2021 05:08:26 GMT  
		Size: 104.1 MB (104146807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf1c154560e156f2f4805693aaca2126fcb386eae3cd6825f0168543b51923d`  
		Last Modified: Tue, 31 Aug 2021 05:08:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f18c8918f43ab9c83750978f0b039de19d588b7005c24bd8f3ba1719a1cb6`  
		Last Modified: Tue, 31 Aug 2021 05:08:47 GMT  
		Size: 70.8 MB (70797635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2ec3aca55a5a8332b228264f2d8a9579042a7b0732b23e4690ef77708970b7`  
		Last Modified: Tue, 31 Aug 2021 05:08:37 GMT  
		Size: 243.4 KB (243353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea6102c8c7f36c55a6d032dfaf36550669a7dcf8743b74915b32ce96165fe35`  
		Last Modified: Tue, 31 Aug 2021 05:08:36 GMT  
		Size: 2.0 KB (2017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec08e1246064b55c16dfbfce20bbebb65942cd2a01f12a8f893409e23837405f`  
		Last Modified: Tue, 31 Aug 2021 05:08:40 GMT  
		Size: 22.2 MB (22184233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57d0222bda6193c1c3877320cdbe8ca07509358658a805a7c83aaa9edb77777`  
		Last Modified: Tue, 31 Aug 2021 05:09:02 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25edb2a8e70c9a3ef372c7c84972b1efb20524c77aafbe913f5a714370d2944e`  
		Last Modified: Tue, 31 Aug 2021 05:09:02 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e017aaac77fb5e81b2592fe22095b3dd661f0c95cb3dd7760a8ea6ee5fc82727`  
		Last Modified: Tue, 31 Aug 2021 05:09:16 GMT  
		Size: 78.4 MB (78425179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebe9a2a06524d2a6d16bfdc3ba1ba60899aa0cccd9c711a5739ef284bc05707`  
		Last Modified: Tue, 31 Aug 2021 05:09:05 GMT  
		Size: 15.1 MB (15142071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6384ded0d228c843b661dcc9a8c1783535ef642c0beb6183919ca7d8654d906c`  
		Last Modified: Tue, 31 Aug 2021 05:09:02 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:68468ac2b592b84dfaf20f49bb60edc59b0afa216eb47435803f5b68171cc498
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.4 MB (314397076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c88b7492ee1a3327220ba723459be0df41a8a1c4cfa1997003ca073e08b325e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:35:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:40:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Aug 2021 02:40:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 02:40:15 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 02:45:28 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Aug 2021 02:46:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:46:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 31 Aug 2021 02:46:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 02:46:09 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:46:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:46:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 02:46:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Aug 2021 02:47:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:47:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 02:47:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:47:18 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Aug 2021 02:47:18 GMT
ENV ROS2_DISTRO=rolling
# Tue, 31 Aug 2021 02:47:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:47:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.16.0-1*     ros-rolling-demo-nodes-py=0.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:47:53 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b869ca97320a7af4e9ce7c382543a1b04a7005c70779507cbb85ace89adde42e`  
		Last Modified: Tue, 31 Aug 2021 02:52:34 GMT  
		Size: 1.2 MB (1183579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c7b498b8e70b033b401f685710eb46ada1aab199891dfe061488eb0ba40831`  
		Last Modified: Tue, 31 Aug 2021 02:52:32 GMT  
		Size: 5.5 MB (5512786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153e16b4767757045ca5abd59a845a7b7cbc2916b1d1a63d930661eec9fc232b`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e90d25ecd370ffb201a02739df5a10f437fb2d2c95060875411cf40d5d0e12`  
		Last Modified: Tue, 31 Aug 2021 02:55:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b5c1e17fbe503ccf8bebc08da06f5478b90f03326ea7cc016d9e73507f10ce`  
		Last Modified: Tue, 31 Aug 2021 02:58:52 GMT  
		Size: 100.5 MB (100535790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45400d8e0bf75fe9e077d037d3f7b0e895432f5540ae74445ce40f4b797111a7`  
		Last Modified: Tue, 31 Aug 2021 02:58:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1497a728946ec991c8b236b4101cde77517a464c2b22ebc0c2853c613f8edc`  
		Last Modified: Tue, 31 Aug 2021 02:59:15 GMT  
		Size: 65.1 MB (65137816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cb14f8cc4408bc999a0012920c6670355132f9cd04cfa6f3632da05868c24b`  
		Last Modified: Tue, 31 Aug 2021 02:59:04 GMT  
		Size: 243.4 KB (243377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a36f33083ce43a2fe6e2a6de6c0ef97f01bfded87f9bb0c50615c85cb4e312`  
		Last Modified: Tue, 31 Aug 2021 02:59:04 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177b7dcdd13b2c3e4ae37d2c849c4d4f5288ac23426c57d481e802f7cc6d6d96`  
		Last Modified: Tue, 31 Aug 2021 02:59:07 GMT  
		Size: 21.5 MB (21526088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda22c832442974a0ad5794123fbb4e6221cdb2bc0453dae21d103dbfec86f5`  
		Last Modified: Tue, 31 Aug 2021 02:59:31 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82725bf8c13207af80944626bf8589affa0081f57afc0ac9909f1593c083bef8`  
		Last Modified: Tue, 31 Aug 2021 02:59:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d686b241380f7b3f8cfa70ef4d17a3aa23b8aa004ed5a0b058f2ef1297a313`  
		Last Modified: Tue, 31 Aug 2021 02:59:47 GMT  
		Size: 78.4 MB (78374994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4acdaad577df7d049bf04dedb300fb427799c94a4b55e063a1b5127c5e31d45`  
		Last Modified: Tue, 31 Aug 2021 02:59:34 GMT  
		Size: 14.7 MB (14704492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7e46de183de8b86fe1c86ff9b994c58a22b11e9a8d9327c1f58b6bcc729ec7`  
		Last Modified: Tue, 31 Aug 2021 02:59:31 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
