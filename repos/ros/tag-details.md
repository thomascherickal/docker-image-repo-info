<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ros`

-	[`ros:foxy`](#rosfoxy)
-	[`ros:foxy-ros-base`](#rosfoxy-ros-base)
-	[`ros:foxy-ros-base-focal`](#rosfoxy-ros-base-focal)
-	[`ros:foxy-ros-core`](#rosfoxy-ros-core)
-	[`ros:foxy-ros-core-focal`](#rosfoxy-ros-core-focal)
-	[`ros:foxy-ros1-bridge`](#rosfoxy-ros1-bridge)
-	[`ros:foxy-ros1-bridge-focal`](#rosfoxy-ros1-bridge-focal)
-	[`ros:humble`](#roshumble)
-	[`ros:humble-perception`](#roshumble-perception)
-	[`ros:humble-perception-jammy`](#roshumble-perception-jammy)
-	[`ros:humble-ros-base`](#roshumble-ros-base)
-	[`ros:humble-ros-base-jammy`](#roshumble-ros-base-jammy)
-	[`ros:humble-ros-core`](#roshumble-ros-core)
-	[`ros:humble-ros-core-jammy`](#roshumble-ros-core-jammy)
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
-	[`ros:rolling-perception`](#rosrolling-perception)
-	[`ros:rolling-perception-jammy`](#rosrolling-perception-jammy)
-	[`ros:rolling-ros-base`](#rosrolling-ros-base)
-	[`ros:rolling-ros-base-jammy`](#rosrolling-ros-base-jammy)
-	[`ros:rolling-ros-core`](#rosrolling-ros-core)
-	[`ros:rolling-ros-core-jammy`](#rosrolling-ros-core-jammy)

## `ros:foxy`

```console
$ docker pull ros@sha256:b07174ed1fb9f692554f95c4e5e895974da6a233393ffca9d12bbd2369544ba7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:5991759125bfb3b5f7b99ea8d89519c620973f2fafe9f578b06683a187dd4b90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.0 MB (250986541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9001fb3c6d9cbfb1fc4f48fbc9912c8a1f645faf74fc77738e7f39a8277d13a7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:11:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 01:11:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:12:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 01:12:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:12:40 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:13:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:13:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:13:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 01:13:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11384cc19c203f12069b104485229b1cde3e07fb646ecb09f115a1ed23251042`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8e1899a5dd0280e2bbb519c2cede595b7705867c7e57a775237ac5d972976d`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed172a7f8a3773d473ad96809401a410d4517ae43bc854da56d2c3ed28f0ee8`  
		Last Modified: Tue, 18 Apr 2023 01:17:45 GMT  
		Size: 120.4 MB (120409529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697c4bfe41b1cdea0ed9cd295f48b4d9acb1711ae5a550c0b0c460c903020520`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275738f8603356f715759926c672904eafa8bfac12a6f4fc1bb25f30a2f2e67e`  
		Last Modified: Tue, 18 Apr 2023 01:18:03 GMT  
		Size: 73.3 MB (73341056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0cfeddf32468988708b8205f0dd73996e224c00857773fa9557bdbfa385e4d`  
		Last Modified: Tue, 18 Apr 2023 01:17:54 GMT  
		Size: 260.0 KB (259961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3049fa8b21143456bf6302da9c1f5d27a1c4f9e8b05028511aa67f3bbabd481`  
		Last Modified: Tue, 18 Apr 2023 01:17:53 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288a0278b454639d3064fd38db41ae5a3d05e16ffa4bf223b9e78fb59d37f8a6`  
		Last Modified: Tue, 18 Apr 2023 01:17:57 GMT  
		Size: 21.7 MB (21681848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0100f19528d75e9b1a1e4293b927ba9b24281ae62def2506974c6705ab69fbca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226837338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7ab5d27179b84b95292d4a32ae01849dfc27c92375bcceaa0e89a867d32842`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:18:46 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 02:18:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 02:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:19:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 02:19:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:19:47 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:20:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:20:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:20:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 02:20:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a853bc3a2b57f4e614f18894ea2c9fa2bd207ca085df3779c55741802d76805`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857ff93c26851761be6757c4cd103514d5a5627e3d6b10c30e7ed284dbb35f3`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c281cda2781fc73b9a6b017b1aa330d38d3591da37fb835ba08c03f3958f204b`  
		Last Modified: Tue, 18 Apr 2023 02:24:11 GMT  
		Size: 104.6 MB (104592055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c8b5760d420f841c64e29370ce3b911d1205171a9a66197935f349aa7dbf9`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1542c121861076309738d45ca122ce9226e3ae7b21ce08ab861c95a66c4ed6d5`  
		Last Modified: Tue, 18 Apr 2023 02:24:26 GMT  
		Size: 67.7 MB (67686900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ccb99230453021ceb67c88f4ad0f60b938ad64160c5fb83dbc7349abd6c00`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 260.0 KB (259959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de229310fdd44a856f4c3aa202e5c38eda5342328e3f890fc486b4178be68007`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a74b94f680052b89e94e45989edce2610e247ef9fbd7629c0851d7c04f3d6d`  
		Last Modified: Tue, 18 Apr 2023 02:24:21 GMT  
		Size: 20.4 MB (20406633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:b07174ed1fb9f692554f95c4e5e895974da6a233393ffca9d12bbd2369544ba7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:5991759125bfb3b5f7b99ea8d89519c620973f2fafe9f578b06683a187dd4b90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.0 MB (250986541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9001fb3c6d9cbfb1fc4f48fbc9912c8a1f645faf74fc77738e7f39a8277d13a7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:11:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 01:11:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:12:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 01:12:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:12:40 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:13:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:13:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:13:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 01:13:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11384cc19c203f12069b104485229b1cde3e07fb646ecb09f115a1ed23251042`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8e1899a5dd0280e2bbb519c2cede595b7705867c7e57a775237ac5d972976d`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed172a7f8a3773d473ad96809401a410d4517ae43bc854da56d2c3ed28f0ee8`  
		Last Modified: Tue, 18 Apr 2023 01:17:45 GMT  
		Size: 120.4 MB (120409529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697c4bfe41b1cdea0ed9cd295f48b4d9acb1711ae5a550c0b0c460c903020520`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275738f8603356f715759926c672904eafa8bfac12a6f4fc1bb25f30a2f2e67e`  
		Last Modified: Tue, 18 Apr 2023 01:18:03 GMT  
		Size: 73.3 MB (73341056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0cfeddf32468988708b8205f0dd73996e224c00857773fa9557bdbfa385e4d`  
		Last Modified: Tue, 18 Apr 2023 01:17:54 GMT  
		Size: 260.0 KB (259961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3049fa8b21143456bf6302da9c1f5d27a1c4f9e8b05028511aa67f3bbabd481`  
		Last Modified: Tue, 18 Apr 2023 01:17:53 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288a0278b454639d3064fd38db41ae5a3d05e16ffa4bf223b9e78fb59d37f8a6`  
		Last Modified: Tue, 18 Apr 2023 01:17:57 GMT  
		Size: 21.7 MB (21681848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0100f19528d75e9b1a1e4293b927ba9b24281ae62def2506974c6705ab69fbca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226837338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7ab5d27179b84b95292d4a32ae01849dfc27c92375bcceaa0e89a867d32842`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:18:46 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 02:18:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 02:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:19:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 02:19:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:19:47 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:20:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:20:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:20:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 02:20:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a853bc3a2b57f4e614f18894ea2c9fa2bd207ca085df3779c55741802d76805`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857ff93c26851761be6757c4cd103514d5a5627e3d6b10c30e7ed284dbb35f3`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c281cda2781fc73b9a6b017b1aa330d38d3591da37fb835ba08c03f3958f204b`  
		Last Modified: Tue, 18 Apr 2023 02:24:11 GMT  
		Size: 104.6 MB (104592055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c8b5760d420f841c64e29370ce3b911d1205171a9a66197935f349aa7dbf9`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1542c121861076309738d45ca122ce9226e3ae7b21ce08ab861c95a66c4ed6d5`  
		Last Modified: Tue, 18 Apr 2023 02:24:26 GMT  
		Size: 67.7 MB (67686900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ccb99230453021ceb67c88f4ad0f60b938ad64160c5fb83dbc7349abd6c00`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 260.0 KB (259959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de229310fdd44a856f4c3aa202e5c38eda5342328e3f890fc486b4178be68007`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a74b94f680052b89e94e45989edce2610e247ef9fbd7629c0851d7c04f3d6d`  
		Last Modified: Tue, 18 Apr 2023 02:24:21 GMT  
		Size: 20.4 MB (20406633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:b07174ed1fb9f692554f95c4e5e895974da6a233393ffca9d12bbd2369544ba7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:5991759125bfb3b5f7b99ea8d89519c620973f2fafe9f578b06683a187dd4b90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.0 MB (250986541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9001fb3c6d9cbfb1fc4f48fbc9912c8a1f645faf74fc77738e7f39a8277d13a7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:11:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 01:11:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:12:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 01:12:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:12:40 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:13:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:13:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:13:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 01:13:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11384cc19c203f12069b104485229b1cde3e07fb646ecb09f115a1ed23251042`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8e1899a5dd0280e2bbb519c2cede595b7705867c7e57a775237ac5d972976d`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed172a7f8a3773d473ad96809401a410d4517ae43bc854da56d2c3ed28f0ee8`  
		Last Modified: Tue, 18 Apr 2023 01:17:45 GMT  
		Size: 120.4 MB (120409529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697c4bfe41b1cdea0ed9cd295f48b4d9acb1711ae5a550c0b0c460c903020520`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275738f8603356f715759926c672904eafa8bfac12a6f4fc1bb25f30a2f2e67e`  
		Last Modified: Tue, 18 Apr 2023 01:18:03 GMT  
		Size: 73.3 MB (73341056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0cfeddf32468988708b8205f0dd73996e224c00857773fa9557bdbfa385e4d`  
		Last Modified: Tue, 18 Apr 2023 01:17:54 GMT  
		Size: 260.0 KB (259961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3049fa8b21143456bf6302da9c1f5d27a1c4f9e8b05028511aa67f3bbabd481`  
		Last Modified: Tue, 18 Apr 2023 01:17:53 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288a0278b454639d3064fd38db41ae5a3d05e16ffa4bf223b9e78fb59d37f8a6`  
		Last Modified: Tue, 18 Apr 2023 01:17:57 GMT  
		Size: 21.7 MB (21681848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0100f19528d75e9b1a1e4293b927ba9b24281ae62def2506974c6705ab69fbca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226837338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7ab5d27179b84b95292d4a32ae01849dfc27c92375bcceaa0e89a867d32842`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:18:46 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 02:18:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 02:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:19:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 02:19:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:19:47 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:20:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:20:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:20:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 02:20:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a853bc3a2b57f4e614f18894ea2c9fa2bd207ca085df3779c55741802d76805`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857ff93c26851761be6757c4cd103514d5a5627e3d6b10c30e7ed284dbb35f3`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c281cda2781fc73b9a6b017b1aa330d38d3591da37fb835ba08c03f3958f204b`  
		Last Modified: Tue, 18 Apr 2023 02:24:11 GMT  
		Size: 104.6 MB (104592055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c8b5760d420f841c64e29370ce3b911d1205171a9a66197935f349aa7dbf9`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1542c121861076309738d45ca122ce9226e3ae7b21ce08ab861c95a66c4ed6d5`  
		Last Modified: Tue, 18 Apr 2023 02:24:26 GMT  
		Size: 67.7 MB (67686900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ccb99230453021ceb67c88f4ad0f60b938ad64160c5fb83dbc7349abd6c00`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 260.0 KB (259959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de229310fdd44a856f4c3aa202e5c38eda5342328e3f890fc486b4178be68007`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a74b94f680052b89e94e45989edce2610e247ef9fbd7629c0851d7c04f3d6d`  
		Last Modified: Tue, 18 Apr 2023 02:24:21 GMT  
		Size: 20.4 MB (20406633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:7c8ad9fe026c414fe61363ec34b4ee285ad1b5d81720f95caef71e3d8870a2f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:3831fd8f11b7efc64d6d978b5d4e017a196e332a39fd7389a365f827f4942651
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155701249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4c6fb61f47b190c5e1408b17f6a28a4d01417acda2f4498edcbc7fa2c0a79c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:11:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 01:11:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:12:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 01:12:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:12:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11384cc19c203f12069b104485229b1cde3e07fb646ecb09f115a1ed23251042`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8e1899a5dd0280e2bbb519c2cede595b7705867c7e57a775237ac5d972976d`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed172a7f8a3773d473ad96809401a410d4517ae43bc854da56d2c3ed28f0ee8`  
		Last Modified: Tue, 18 Apr 2023 01:17:45 GMT  
		Size: 120.4 MB (120409529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697c4bfe41b1cdea0ed9cd295f48b4d9acb1711ae5a550c0b0c460c903020520`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0015e51d696a9e49cbd7d2466550b685f9736813e8fcee4fda6cffde07ce63ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138481404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ddbfbed62def523d109aab257570284e66fa1f7578db60de6a5a1ad26801017`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:18:46 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 02:18:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 02:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:19:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 02:19:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:19:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a853bc3a2b57f4e614f18894ea2c9fa2bd207ca085df3779c55741802d76805`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857ff93c26851761be6757c4cd103514d5a5627e3d6b10c30e7ed284dbb35f3`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c281cda2781fc73b9a6b017b1aa330d38d3591da37fb835ba08c03f3958f204b`  
		Last Modified: Tue, 18 Apr 2023 02:24:11 GMT  
		Size: 104.6 MB (104592055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c8b5760d420f841c64e29370ce3b911d1205171a9a66197935f349aa7dbf9`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:7c8ad9fe026c414fe61363ec34b4ee285ad1b5d81720f95caef71e3d8870a2f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:3831fd8f11b7efc64d6d978b5d4e017a196e332a39fd7389a365f827f4942651
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155701249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4c6fb61f47b190c5e1408b17f6a28a4d01417acda2f4498edcbc7fa2c0a79c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:11:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 01:11:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:12:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 01:12:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:12:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11384cc19c203f12069b104485229b1cde3e07fb646ecb09f115a1ed23251042`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8e1899a5dd0280e2bbb519c2cede595b7705867c7e57a775237ac5d972976d`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed172a7f8a3773d473ad96809401a410d4517ae43bc854da56d2c3ed28f0ee8`  
		Last Modified: Tue, 18 Apr 2023 01:17:45 GMT  
		Size: 120.4 MB (120409529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697c4bfe41b1cdea0ed9cd295f48b4d9acb1711ae5a550c0b0c460c903020520`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0015e51d696a9e49cbd7d2466550b685f9736813e8fcee4fda6cffde07ce63ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138481404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ddbfbed62def523d109aab257570284e66fa1f7578db60de6a5a1ad26801017`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:18:46 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 02:18:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 02:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:19:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 02:19:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:19:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a853bc3a2b57f4e614f18894ea2c9fa2bd207ca085df3779c55741802d76805`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857ff93c26851761be6757c4cd103514d5a5627e3d6b10c30e7ed284dbb35f3`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c281cda2781fc73b9a6b017b1aa330d38d3591da37fb835ba08c03f3958f204b`  
		Last Modified: Tue, 18 Apr 2023 02:24:11 GMT  
		Size: 104.6 MB (104592055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c8b5760d420f841c64e29370ce3b911d1205171a9a66197935f349aa7dbf9`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:305309d77c82b932b0f39274107f20dace64722bbe74c9594b5708cad2db8698
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:a917c84926ec2df2be30f4ae025e4246c1e1040048dc6f4ca2d94147aea88322
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.1 MB (349090769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f4ade7aad1eb1539c25aa29307372f260775bcfec5f1058c5f976632452cbaa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:11:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 01:11:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:12:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 01:12:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:12:40 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:13:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:13:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:13:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 01:13:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:13:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:13:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:13:42 GMT
ENV ROS1_DISTRO=noetic
# Tue, 18 Apr 2023 01:13:42 GMT
ENV ROS2_DISTRO=foxy
# Tue, 18 Apr 2023 01:14:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:14:17 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11384cc19c203f12069b104485229b1cde3e07fb646ecb09f115a1ed23251042`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8e1899a5dd0280e2bbb519c2cede595b7705867c7e57a775237ac5d972976d`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed172a7f8a3773d473ad96809401a410d4517ae43bc854da56d2c3ed28f0ee8`  
		Last Modified: Tue, 18 Apr 2023 01:17:45 GMT  
		Size: 120.4 MB (120409529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697c4bfe41b1cdea0ed9cd295f48b4d9acb1711ae5a550c0b0c460c903020520`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275738f8603356f715759926c672904eafa8bfac12a6f4fc1bb25f30a2f2e67e`  
		Last Modified: Tue, 18 Apr 2023 01:18:03 GMT  
		Size: 73.3 MB (73341056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0cfeddf32468988708b8205f0dd73996e224c00857773fa9557bdbfa385e4d`  
		Last Modified: Tue, 18 Apr 2023 01:17:54 GMT  
		Size: 260.0 KB (259961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3049fa8b21143456bf6302da9c1f5d27a1c4f9e8b05028511aa67f3bbabd481`  
		Last Modified: Tue, 18 Apr 2023 01:17:53 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288a0278b454639d3064fd38db41ae5a3d05e16ffa4bf223b9e78fb59d37f8a6`  
		Last Modified: Tue, 18 Apr 2023 01:17:57 GMT  
		Size: 21.7 MB (21681848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959a237f51a7ce837970a1a3147689c6e320812c6e113379b34a4ede309865b9`  
		Last Modified: Tue, 18 Apr 2023 01:18:14 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099dcbb0d68914ea8e128b9ba5bfd6dc295a0df1df6dee77077e5c41c02fd09a`  
		Last Modified: Tue, 18 Apr 2023 01:18:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f219045d848c72ef970168d3d659ecc472d96ce1ddd0b941afa86e942eeed327`  
		Last Modified: Tue, 18 Apr 2023 01:18:27 GMT  
		Size: 76.4 MB (76429430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e95e56ab27365bbf52b85a050085d25498a5cb779cbecc348312453c755ecc9`  
		Last Modified: Tue, 18 Apr 2023 01:18:18 GMT  
		Size: 21.7 MB (21674170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bac345354e272b6a28e6a211fdbe0140442e7945f38f1a4456c97b3c013dd7`  
		Last Modified: Tue, 18 Apr 2023 01:18:14 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3eb948c5217a16ff7fcfb7d9e22efaf54ab2d16f82cb3d10df0fb492fafd6370
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.7 MB (317659720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f76a3adf578db9fa908cb48f4597a414e3c146fed3a0d860dd5b9ee2da5c1c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:18:46 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 02:18:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 02:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:19:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 02:19:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:19:47 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:20:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:20:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:20:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 02:20:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:20:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:20:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:20:53 GMT
ENV ROS1_DISTRO=noetic
# Tue, 18 Apr 2023 02:20:53 GMT
ENV ROS2_DISTRO=foxy
# Tue, 18 Apr 2023 02:21:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:21:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:21:24 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a853bc3a2b57f4e614f18894ea2c9fa2bd207ca085df3779c55741802d76805`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857ff93c26851761be6757c4cd103514d5a5627e3d6b10c30e7ed284dbb35f3`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c281cda2781fc73b9a6b017b1aa330d38d3591da37fb835ba08c03f3958f204b`  
		Last Modified: Tue, 18 Apr 2023 02:24:11 GMT  
		Size: 104.6 MB (104592055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c8b5760d420f841c64e29370ce3b911d1205171a9a66197935f349aa7dbf9`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1542c121861076309738d45ca122ce9226e3ae7b21ce08ab861c95a66c4ed6d5`  
		Last Modified: Tue, 18 Apr 2023 02:24:26 GMT  
		Size: 67.7 MB (67686900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ccb99230453021ceb67c88f4ad0f60b938ad64160c5fb83dbc7349abd6c00`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 260.0 KB (259959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de229310fdd44a856f4c3aa202e5c38eda5342328e3f890fc486b4178be68007`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a74b94f680052b89e94e45989edce2610e247ef9fbd7629c0851d7c04f3d6d`  
		Last Modified: Tue, 18 Apr 2023 02:24:21 GMT  
		Size: 20.4 MB (20406633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f9d68432b2d7450ddf62a0c75dbefc697f27fe5cb8fb1fb52acc60cb96bc70`  
		Last Modified: Tue, 18 Apr 2023 02:24:37 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8935466a6297cbe16a3d6d8445036f9ffe2ab0078e98a0ad5e737c27444fea6`  
		Last Modified: Tue, 18 Apr 2023 02:24:37 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1ae7d7ef45a74fd1945390dfdaa493a7e91fb43ea0e6b6fa7a4248e8e1c42f`  
		Last Modified: Tue, 18 Apr 2023 02:24:47 GMT  
		Size: 76.5 MB (76496301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df84ef9c108d7326c078732759bbb9ae47b5c4ba4d59e3509127dd8bdf8f9f03`  
		Last Modified: Tue, 18 Apr 2023 02:24:44 GMT  
		Size: 14.3 MB (14325458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21af496781b7139843b526b25641e3fc46797877d26b5ebb0f035710286ea258`  
		Last Modified: Tue, 18 Apr 2023 02:24:37 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:305309d77c82b932b0f39274107f20dace64722bbe74c9594b5708cad2db8698
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:a917c84926ec2df2be30f4ae025e4246c1e1040048dc6f4ca2d94147aea88322
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.1 MB (349090769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f4ade7aad1eb1539c25aa29307372f260775bcfec5f1058c5f976632452cbaa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:11:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 01:11:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:11:44 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:12:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 01:12:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:12:40 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:13:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:13:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:13:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 01:13:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:13:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:13:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:13:42 GMT
ENV ROS1_DISTRO=noetic
# Tue, 18 Apr 2023 01:13:42 GMT
ENV ROS2_DISTRO=foxy
# Tue, 18 Apr 2023 01:14:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:14:17 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11384cc19c203f12069b104485229b1cde3e07fb646ecb09f115a1ed23251042`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8e1899a5dd0280e2bbb519c2cede595b7705867c7e57a775237ac5d972976d`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed172a7f8a3773d473ad96809401a410d4517ae43bc854da56d2c3ed28f0ee8`  
		Last Modified: Tue, 18 Apr 2023 01:17:45 GMT  
		Size: 120.4 MB (120409529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697c4bfe41b1cdea0ed9cd295f48b4d9acb1711ae5a550c0b0c460c903020520`  
		Last Modified: Tue, 18 Apr 2023 01:17:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275738f8603356f715759926c672904eafa8bfac12a6f4fc1bb25f30a2f2e67e`  
		Last Modified: Tue, 18 Apr 2023 01:18:03 GMT  
		Size: 73.3 MB (73341056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0cfeddf32468988708b8205f0dd73996e224c00857773fa9557bdbfa385e4d`  
		Last Modified: Tue, 18 Apr 2023 01:17:54 GMT  
		Size: 260.0 KB (259961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3049fa8b21143456bf6302da9c1f5d27a1c4f9e8b05028511aa67f3bbabd481`  
		Last Modified: Tue, 18 Apr 2023 01:17:53 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288a0278b454639d3064fd38db41ae5a3d05e16ffa4bf223b9e78fb59d37f8a6`  
		Last Modified: Tue, 18 Apr 2023 01:17:57 GMT  
		Size: 21.7 MB (21681848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959a237f51a7ce837970a1a3147689c6e320812c6e113379b34a4ede309865b9`  
		Last Modified: Tue, 18 Apr 2023 01:18:14 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099dcbb0d68914ea8e128b9ba5bfd6dc295a0df1df6dee77077e5c41c02fd09a`  
		Last Modified: Tue, 18 Apr 2023 01:18:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f219045d848c72ef970168d3d659ecc472d96ce1ddd0b941afa86e942eeed327`  
		Last Modified: Tue, 18 Apr 2023 01:18:27 GMT  
		Size: 76.4 MB (76429430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e95e56ab27365bbf52b85a050085d25498a5cb779cbecc348312453c755ecc9`  
		Last Modified: Tue, 18 Apr 2023 01:18:18 GMT  
		Size: 21.7 MB (21674170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bac345354e272b6a28e6a211fdbe0140442e7945f38f1a4456c97b3c013dd7`  
		Last Modified: Tue, 18 Apr 2023 01:18:14 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3eb948c5217a16ff7fcfb7d9e22efaf54ab2d16f82cb3d10df0fb492fafd6370
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.7 MB (317659720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f76a3adf578db9fa908cb48f4597a414e3c146fed3a0d860dd5b9ee2da5c1c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:18:46 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 18 Apr 2023 02:18:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:18:47 GMT
ENV ROS_DISTRO=foxy
# Tue, 18 Apr 2023 02:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:19:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 18 Apr 2023 02:19:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:19:47 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:20:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:20:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:20:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 18 Apr 2023 02:20:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:20:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:20:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:20:53 GMT
ENV ROS1_DISTRO=noetic
# Tue, 18 Apr 2023 02:20:53 GMT
ENV ROS2_DISTRO=foxy
# Tue, 18 Apr 2023 02:21:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:21:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:21:24 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a853bc3a2b57f4e614f18894ea2c9fa2bd207ca085df3779c55741802d76805`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857ff93c26851761be6757c4cd103514d5a5627e3d6b10c30e7ed284dbb35f3`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c281cda2781fc73b9a6b017b1aa330d38d3591da37fb835ba08c03f3958f204b`  
		Last Modified: Tue, 18 Apr 2023 02:24:11 GMT  
		Size: 104.6 MB (104592055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14c8b5760d420f841c64e29370ce3b911d1205171a9a66197935f349aa7dbf9`  
		Last Modified: Tue, 18 Apr 2023 02:23:58 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1542c121861076309738d45ca122ce9226e3ae7b21ce08ab861c95a66c4ed6d5`  
		Last Modified: Tue, 18 Apr 2023 02:24:26 GMT  
		Size: 67.7 MB (67686900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1ccb99230453021ceb67c88f4ad0f60b938ad64160c5fb83dbc7349abd6c00`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 260.0 KB (259959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de229310fdd44a856f4c3aa202e5c38eda5342328e3f890fc486b4178be68007`  
		Last Modified: Tue, 18 Apr 2023 02:24:18 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a74b94f680052b89e94e45989edce2610e247ef9fbd7629c0851d7c04f3d6d`  
		Last Modified: Tue, 18 Apr 2023 02:24:21 GMT  
		Size: 20.4 MB (20406633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f9d68432b2d7450ddf62a0c75dbefc697f27fe5cb8fb1fb52acc60cb96bc70`  
		Last Modified: Tue, 18 Apr 2023 02:24:37 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8935466a6297cbe16a3d6d8445036f9ffe2ab0078e98a0ad5e737c27444fea6`  
		Last Modified: Tue, 18 Apr 2023 02:24:37 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1ae7d7ef45a74fd1945390dfdaa493a7e91fb43ea0e6b6fa7a4248e8e1c42f`  
		Last Modified: Tue, 18 Apr 2023 02:24:47 GMT  
		Size: 76.5 MB (76496301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df84ef9c108d7326c078732759bbb9ae47b5c4ba4d59e3509127dd8bdf8f9f03`  
		Last Modified: Tue, 18 Apr 2023 02:24:44 GMT  
		Size: 14.3 MB (14325458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21af496781b7139843b526b25641e3fc46797877d26b5ebb0f035710286ea258`  
		Last Modified: Tue, 18 Apr 2023 02:24:37 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble`

```console
$ docker pull ros@sha256:b83e9c62a610b62415c8118028c8c32fc46eeca82e63ab69edda0b5b3e8accd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:f05e713cd384afe798581f9bbf312a249102fb37a184049b9457e9fef90d137e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263174534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e9065680771dc75b9640d663e4e5c2c96952c91b485681b427be72ed07e5e4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 21:47:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:47:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:47:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:47:17 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:48:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:48:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:48:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 21:49:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde6a04e024906cded5edf825e781c98cf96fbbf94fa12b76c330722940eceb8`  
		Last Modified: Wed, 03 May 2023 22:05:05 GMT  
		Size: 106.3 MB (106336297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9588c9c20d7b8f44868b7fc58557ac21f8e7e305a1d876de9f1074e10f95050`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae8aa1e91cbff4c3f988a146ffc0206d3e1f66955d42de907bb2e1422ac312`  
		Last Modified: Wed, 03 May 2023 22:05:27 GMT  
		Size: 98.0 MB (97953962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563b38330c500c2d1dc3ba3fc3436efb4fe69c77e3eefb798da0dbf2f045741b`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71be3bc7a9e9be52aa054f3abbfe1466bad3c982a4b5df0139365a1e8d8aa99f`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce9eacb30f5cbc4a5b4fef0e07ec3d7e292008bb2429d9a7c5b47c1f424c0c2`  
		Last Modified: Wed, 03 May 2023 22:05:18 GMT  
		Size: 23.1 MB (23080914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:13eed2b61402a7be4dcfb1463398966f27fe807e81e447456d167627ce9ee8ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255874696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d598e466f229fa6b8fddc844d25cb079f5e0bab536b0339e60a75494f215591d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 18:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:42:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:42:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:42:45 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:43:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:43:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:44:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbdf371ac8debb00b1e7563e8d541adf3d0572e0bedd653b80ffdd7e412fd27`  
		Last Modified: Wed, 03 May 2023 19:01:34 GMT  
		Size: 104.1 MB (104070627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd914e1358e1340af31540c95795b2fd17a1441051676d24414fd193dc125b`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffcc22bad3dce5f0ab64c8aca68f087009e100593c51a2ec51e6c3e61cd528`  
		Last Modified: Wed, 03 May 2023 19:01:52 GMT  
		Size: 95.6 MB (95569322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69f93bf06fe6d5dae8bd1de95e13efcef037ac11f15e0ed29d1ea86a182ddb1`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 299.9 KB (299931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54479b6a61d4ae55c24245d493dc309a5838f5f621fbcdfb2ffafdae989ab203`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca38a3f9a26e9c8f8f5254415b93e12a538a4c0534e6e2693060d9571a0382d4`  
		Last Modified: Wed, 03 May 2023 19:01:45 GMT  
		Size: 22.5 MB (22499355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:d9399a09966af2cb28ab9e3d8872b7e3fb757ba54012eede4ec0f6df76a838f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:59f7914601c3f2428fb352a8f000d72643f7bb998029a337bca9c80777ee9ec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1092269411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7761d63295e0575cf066943b92b87fb53f872cae1d10508e0b2262caf1c036`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 21:47:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:47:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:47:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:47:17 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:48:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:48:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:48:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 21:49:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:57:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde6a04e024906cded5edf825e781c98cf96fbbf94fa12b76c330722940eceb8`  
		Last Modified: Wed, 03 May 2023 22:05:05 GMT  
		Size: 106.3 MB (106336297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9588c9c20d7b8f44868b7fc58557ac21f8e7e305a1d876de9f1074e10f95050`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae8aa1e91cbff4c3f988a146ffc0206d3e1f66955d42de907bb2e1422ac312`  
		Last Modified: Wed, 03 May 2023 22:05:27 GMT  
		Size: 98.0 MB (97953962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563b38330c500c2d1dc3ba3fc3436efb4fe69c77e3eefb798da0dbf2f045741b`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71be3bc7a9e9be52aa054f3abbfe1466bad3c982a4b5df0139365a1e8d8aa99f`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce9eacb30f5cbc4a5b4fef0e07ec3d7e292008bb2429d9a7c5b47c1f424c0c2`  
		Last Modified: Wed, 03 May 2023 22:05:18 GMT  
		Size: 23.1 MB (23080914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5ee937fa8706cfdfea318f0dc54ff137be72fa361123f7d0d721b9942541e`  
		Last Modified: Wed, 03 May 2023 22:07:11 GMT  
		Size: 829.1 MB (829094877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:092721b022aef0d18a99a5df806602641eb75844cc444dc95d64c886f0343d4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1043801716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27ddffb4af3d1de36054fcce70f2ce31fd65babde08e89332e47bafa0a4b70cf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 18:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:42:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:42:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:42:45 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:43:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:43:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:44:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:55:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbdf371ac8debb00b1e7563e8d541adf3d0572e0bedd653b80ffdd7e412fd27`  
		Last Modified: Wed, 03 May 2023 19:01:34 GMT  
		Size: 104.1 MB (104070627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd914e1358e1340af31540c95795b2fd17a1441051676d24414fd193dc125b`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffcc22bad3dce5f0ab64c8aca68f087009e100593c51a2ec51e6c3e61cd528`  
		Last Modified: Wed, 03 May 2023 19:01:52 GMT  
		Size: 95.6 MB (95569322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69f93bf06fe6d5dae8bd1de95e13efcef037ac11f15e0ed29d1ea86a182ddb1`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 299.9 KB (299931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54479b6a61d4ae55c24245d493dc309a5838f5f621fbcdfb2ffafdae989ab203`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca38a3f9a26e9c8f8f5254415b93e12a538a4c0534e6e2693060d9571a0382d4`  
		Last Modified: Wed, 03 May 2023 19:01:45 GMT  
		Size: 22.5 MB (22499355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf8b6ace71b756feb5407501c6b54a1821a44d8e8750072d71c8e1462d39b45`  
		Last Modified: Wed, 03 May 2023 19:03:18 GMT  
		Size: 787.9 MB (787927020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:d9399a09966af2cb28ab9e3d8872b7e3fb757ba54012eede4ec0f6df76a838f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:59f7914601c3f2428fb352a8f000d72643f7bb998029a337bca9c80777ee9ec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1092269411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7761d63295e0575cf066943b92b87fb53f872cae1d10508e0b2262caf1c036`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 21:47:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:47:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:47:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:47:17 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:48:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:48:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:48:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 21:49:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:57:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde6a04e024906cded5edf825e781c98cf96fbbf94fa12b76c330722940eceb8`  
		Last Modified: Wed, 03 May 2023 22:05:05 GMT  
		Size: 106.3 MB (106336297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9588c9c20d7b8f44868b7fc58557ac21f8e7e305a1d876de9f1074e10f95050`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae8aa1e91cbff4c3f988a146ffc0206d3e1f66955d42de907bb2e1422ac312`  
		Last Modified: Wed, 03 May 2023 22:05:27 GMT  
		Size: 98.0 MB (97953962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563b38330c500c2d1dc3ba3fc3436efb4fe69c77e3eefb798da0dbf2f045741b`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71be3bc7a9e9be52aa054f3abbfe1466bad3c982a4b5df0139365a1e8d8aa99f`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce9eacb30f5cbc4a5b4fef0e07ec3d7e292008bb2429d9a7c5b47c1f424c0c2`  
		Last Modified: Wed, 03 May 2023 22:05:18 GMT  
		Size: 23.1 MB (23080914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5ee937fa8706cfdfea318f0dc54ff137be72fa361123f7d0d721b9942541e`  
		Last Modified: Wed, 03 May 2023 22:07:11 GMT  
		Size: 829.1 MB (829094877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:092721b022aef0d18a99a5df806602641eb75844cc444dc95d64c886f0343d4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1043801716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27ddffb4af3d1de36054fcce70f2ce31fd65babde08e89332e47bafa0a4b70cf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 18:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:42:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:42:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:42:45 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:43:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:43:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:44:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:55:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbdf371ac8debb00b1e7563e8d541adf3d0572e0bedd653b80ffdd7e412fd27`  
		Last Modified: Wed, 03 May 2023 19:01:34 GMT  
		Size: 104.1 MB (104070627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd914e1358e1340af31540c95795b2fd17a1441051676d24414fd193dc125b`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffcc22bad3dce5f0ab64c8aca68f087009e100593c51a2ec51e6c3e61cd528`  
		Last Modified: Wed, 03 May 2023 19:01:52 GMT  
		Size: 95.6 MB (95569322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69f93bf06fe6d5dae8bd1de95e13efcef037ac11f15e0ed29d1ea86a182ddb1`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 299.9 KB (299931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54479b6a61d4ae55c24245d493dc309a5838f5f621fbcdfb2ffafdae989ab203`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca38a3f9a26e9c8f8f5254415b93e12a538a4c0534e6e2693060d9571a0382d4`  
		Last Modified: Wed, 03 May 2023 19:01:45 GMT  
		Size: 22.5 MB (22499355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf8b6ace71b756feb5407501c6b54a1821a44d8e8750072d71c8e1462d39b45`  
		Last Modified: Wed, 03 May 2023 19:03:18 GMT  
		Size: 787.9 MB (787927020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:b83e9c62a610b62415c8118028c8c32fc46eeca82e63ab69edda0b5b3e8accd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:f05e713cd384afe798581f9bbf312a249102fb37a184049b9457e9fef90d137e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263174534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e9065680771dc75b9640d663e4e5c2c96952c91b485681b427be72ed07e5e4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 21:47:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:47:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:47:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:47:17 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:48:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:48:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:48:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 21:49:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde6a04e024906cded5edf825e781c98cf96fbbf94fa12b76c330722940eceb8`  
		Last Modified: Wed, 03 May 2023 22:05:05 GMT  
		Size: 106.3 MB (106336297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9588c9c20d7b8f44868b7fc58557ac21f8e7e305a1d876de9f1074e10f95050`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae8aa1e91cbff4c3f988a146ffc0206d3e1f66955d42de907bb2e1422ac312`  
		Last Modified: Wed, 03 May 2023 22:05:27 GMT  
		Size: 98.0 MB (97953962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563b38330c500c2d1dc3ba3fc3436efb4fe69c77e3eefb798da0dbf2f045741b`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71be3bc7a9e9be52aa054f3abbfe1466bad3c982a4b5df0139365a1e8d8aa99f`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce9eacb30f5cbc4a5b4fef0e07ec3d7e292008bb2429d9a7c5b47c1f424c0c2`  
		Last Modified: Wed, 03 May 2023 22:05:18 GMT  
		Size: 23.1 MB (23080914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:13eed2b61402a7be4dcfb1463398966f27fe807e81e447456d167627ce9ee8ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255874696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d598e466f229fa6b8fddc844d25cb079f5e0bab536b0339e60a75494f215591d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 18:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:42:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:42:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:42:45 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:43:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:43:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:44:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbdf371ac8debb00b1e7563e8d541adf3d0572e0bedd653b80ffdd7e412fd27`  
		Last Modified: Wed, 03 May 2023 19:01:34 GMT  
		Size: 104.1 MB (104070627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd914e1358e1340af31540c95795b2fd17a1441051676d24414fd193dc125b`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffcc22bad3dce5f0ab64c8aca68f087009e100593c51a2ec51e6c3e61cd528`  
		Last Modified: Wed, 03 May 2023 19:01:52 GMT  
		Size: 95.6 MB (95569322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69f93bf06fe6d5dae8bd1de95e13efcef037ac11f15e0ed29d1ea86a182ddb1`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 299.9 KB (299931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54479b6a61d4ae55c24245d493dc309a5838f5f621fbcdfb2ffafdae989ab203`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca38a3f9a26e9c8f8f5254415b93e12a538a4c0534e6e2693060d9571a0382d4`  
		Last Modified: Wed, 03 May 2023 19:01:45 GMT  
		Size: 22.5 MB (22499355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:b83e9c62a610b62415c8118028c8c32fc46eeca82e63ab69edda0b5b3e8accd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:f05e713cd384afe798581f9bbf312a249102fb37a184049b9457e9fef90d137e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263174534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e9065680771dc75b9640d663e4e5c2c96952c91b485681b427be72ed07e5e4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 21:47:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:47:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:47:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:47:17 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:48:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:48:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:48:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 21:49:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde6a04e024906cded5edf825e781c98cf96fbbf94fa12b76c330722940eceb8`  
		Last Modified: Wed, 03 May 2023 22:05:05 GMT  
		Size: 106.3 MB (106336297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9588c9c20d7b8f44868b7fc58557ac21f8e7e305a1d876de9f1074e10f95050`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae8aa1e91cbff4c3f988a146ffc0206d3e1f66955d42de907bb2e1422ac312`  
		Last Modified: Wed, 03 May 2023 22:05:27 GMT  
		Size: 98.0 MB (97953962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563b38330c500c2d1dc3ba3fc3436efb4fe69c77e3eefb798da0dbf2f045741b`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71be3bc7a9e9be52aa054f3abbfe1466bad3c982a4b5df0139365a1e8d8aa99f`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce9eacb30f5cbc4a5b4fef0e07ec3d7e292008bb2429d9a7c5b47c1f424c0c2`  
		Last Modified: Wed, 03 May 2023 22:05:18 GMT  
		Size: 23.1 MB (23080914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:13eed2b61402a7be4dcfb1463398966f27fe807e81e447456d167627ce9ee8ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255874696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d598e466f229fa6b8fddc844d25cb079f5e0bab536b0339e60a75494f215591d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 18:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:42:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:42:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:42:45 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:43:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:43:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:44:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbdf371ac8debb00b1e7563e8d541adf3d0572e0bedd653b80ffdd7e412fd27`  
		Last Modified: Wed, 03 May 2023 19:01:34 GMT  
		Size: 104.1 MB (104070627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd914e1358e1340af31540c95795b2fd17a1441051676d24414fd193dc125b`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffcc22bad3dce5f0ab64c8aca68f087009e100593c51a2ec51e6c3e61cd528`  
		Last Modified: Wed, 03 May 2023 19:01:52 GMT  
		Size: 95.6 MB (95569322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69f93bf06fe6d5dae8bd1de95e13efcef037ac11f15e0ed29d1ea86a182ddb1`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 299.9 KB (299931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54479b6a61d4ae55c24245d493dc309a5838f5f621fbcdfb2ffafdae989ab203`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca38a3f9a26e9c8f8f5254415b93e12a538a4c0534e6e2693060d9571a0382d4`  
		Last Modified: Wed, 03 May 2023 19:01:45 GMT  
		Size: 22.5 MB (22499355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:4d4dd9ef0e4bb36544132f67cb635ea1f52d1969aa45e9423a3c84e4e518ee88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:c5f33d0d9971bcd19ad58b3bd05d74d6ffa0596ecf49b01a6358aa18f87ed1db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141837129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f76ed34174594a4fa62f9ca6e95593b475e565ce05400e1c5d06a65d931bf35`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 21:47:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:47:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:47:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:47:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde6a04e024906cded5edf825e781c98cf96fbbf94fa12b76c330722940eceb8`  
		Last Modified: Wed, 03 May 2023 22:05:05 GMT  
		Size: 106.3 MB (106336297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9588c9c20d7b8f44868b7fc58557ac21f8e7e305a1d876de9f1074e10f95050`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b58d5d27371fac49e2d50649cb37effa390a3f854a473689a333c44e64a66f81
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137503666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0bf13d2eb15cb48b06348eda219e7cc115f23e04356fbcd0f4c5d2448618ef9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 18:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:42:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:42:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:42:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbdf371ac8debb00b1e7563e8d541adf3d0572e0bedd653b80ffdd7e412fd27`  
		Last Modified: Wed, 03 May 2023 19:01:34 GMT  
		Size: 104.1 MB (104070627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd914e1358e1340af31540c95795b2fd17a1441051676d24414fd193dc125b`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:4d4dd9ef0e4bb36544132f67cb635ea1f52d1969aa45e9423a3c84e4e518ee88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:c5f33d0d9971bcd19ad58b3bd05d74d6ffa0596ecf49b01a6358aa18f87ed1db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141837129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f76ed34174594a4fa62f9ca6e95593b475e565ce05400e1c5d06a65d931bf35`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 21:47:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:47:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:47:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:47:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde6a04e024906cded5edf825e781c98cf96fbbf94fa12b76c330722940eceb8`  
		Last Modified: Wed, 03 May 2023 22:05:05 GMT  
		Size: 106.3 MB (106336297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9588c9c20d7b8f44868b7fc58557ac21f8e7e305a1d876de9f1074e10f95050`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b58d5d27371fac49e2d50649cb37effa390a3f854a473689a333c44e64a66f81
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137503666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0bf13d2eb15cb48b06348eda219e7cc115f23e04356fbcd0f4c5d2448618ef9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 18:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:42:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:42:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:42:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbdf371ac8debb00b1e7563e8d541adf3d0572e0bedd653b80ffdd7e412fd27`  
		Last Modified: Wed, 03 May 2023 19:01:34 GMT  
		Size: 104.1 MB (104070627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd914e1358e1340af31540c95795b2fd17a1441051676d24414fd193dc125b`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:b83e9c62a610b62415c8118028c8c32fc46eeca82e63ab69edda0b5b3e8accd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:f05e713cd384afe798581f9bbf312a249102fb37a184049b9457e9fef90d137e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263174534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e9065680771dc75b9640d663e4e5c2c96952c91b485681b427be72ed07e5e4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 21:47:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:47:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:47:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:47:17 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:48:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:48:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:48:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 21:49:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde6a04e024906cded5edf825e781c98cf96fbbf94fa12b76c330722940eceb8`  
		Last Modified: Wed, 03 May 2023 22:05:05 GMT  
		Size: 106.3 MB (106336297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9588c9c20d7b8f44868b7fc58557ac21f8e7e305a1d876de9f1074e10f95050`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae8aa1e91cbff4c3f988a146ffc0206d3e1f66955d42de907bb2e1422ac312`  
		Last Modified: Wed, 03 May 2023 22:05:27 GMT  
		Size: 98.0 MB (97953962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563b38330c500c2d1dc3ba3fc3436efb4fe69c77e3eefb798da0dbf2f045741b`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71be3bc7a9e9be52aa054f3abbfe1466bad3c982a4b5df0139365a1e8d8aa99f`  
		Last Modified: Wed, 03 May 2023 22:05:14 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce9eacb30f5cbc4a5b4fef0e07ec3d7e292008bb2429d9a7c5b47c1f424c0c2`  
		Last Modified: Wed, 03 May 2023 22:05:18 GMT  
		Size: 23.1 MB (23080914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:13eed2b61402a7be4dcfb1463398966f27fe807e81e447456d167627ce9ee8ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255874696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d598e466f229fa6b8fddc844d25cb079f5e0bab536b0339e60a75494f215591d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV ROS_DISTRO=humble
# Wed, 03 May 2023 18:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:42:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:42:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:42:45 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:43:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:43:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:44:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbdf371ac8debb00b1e7563e8d541adf3d0572e0bedd653b80ffdd7e412fd27`  
		Last Modified: Wed, 03 May 2023 19:01:34 GMT  
		Size: 104.1 MB (104070627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd914e1358e1340af31540c95795b2fd17a1441051676d24414fd193dc125b`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ffcc22bad3dce5f0ab64c8aca68f087009e100593c51a2ec51e6c3e61cd528`  
		Last Modified: Wed, 03 May 2023 19:01:52 GMT  
		Size: 95.6 MB (95569322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69f93bf06fe6d5dae8bd1de95e13efcef037ac11f15e0ed29d1ea86a182ddb1`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 299.9 KB (299931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54479b6a61d4ae55c24245d493dc309a5838f5f621fbcdfb2ffafdae989ab203`  
		Last Modified: Wed, 03 May 2023 19:01:43 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca38a3f9a26e9c8f8f5254415b93e12a538a4c0534e6e2693060d9571a0382d4`  
		Last Modified: Wed, 03 May 2023 19:01:45 GMT  
		Size: 22.5 MB (22499355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:4c16420fc4f1f71dd59278ea8f881eef389cb3d9417faaa12edc6553615d767d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:21bb4ad490af560bb44192eed50c1c493358c59c01d70171814c9afbec151bbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.7 MB (437749392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77f179e2e80523fb74868ca6cc6d867b9fc5131cdeb36db2e4e9f1fc9ea0e2f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:04:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:05:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:05:05 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:08:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:08:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:08:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:08:45 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:09:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:09:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:10:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8112c7660661f5d395aac99b0d2403ccaaf47cfce01b40167688a866847d540`  
		Last Modified: Tue, 16 May 2023 01:17:48 GMT  
		Size: 819.1 KB (819098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64664c88569b54e7b2cace7a7eff36f63ca10a75b05e5c1ddceb69bbff1d387b`  
		Last Modified: Tue, 16 May 2023 01:17:47 GMT  
		Size: 4.9 MB (4878519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20548c67c76407d9f268011684621401f1bb204c67b556072a06759d86b2cd82`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96bc2cae0fba817ecce5d15aafad4eee15610dfe2178708ed47f732f7f71bd`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60000963f8bb247e6b22511e73ce54d4b3fefb24047ab49992acd24f8272aab5`  
		Last Modified: Tue, 16 May 2023 01:18:20 GMT  
		Size: 259.6 MB (259592143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af96a47a2aa7f522fcdf38f50ca1ff4abda4c7efd140a1d960f59b90f47d7788`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b12ba5acbea014d663262f916b8adc37a9271199290d917abd458538df9cb70`  
		Last Modified: Tue, 16 May 2023 01:18:38 GMT  
		Size: 70.5 MB (70459679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41bbf0250a9904f7b67e9257aa660ab936db8911b99cd58d9350b109b920e31`  
		Last Modified: Tue, 16 May 2023 01:18:29 GMT  
		Size: 282.3 KB (282294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f25d5aeddde8c1ec7ab0e2e9b51e8c30c5e7d69ad7cb00cb679682e3a47b3`  
		Last Modified: Tue, 16 May 2023 01:18:40 GMT  
		Size: 75.0 MB (75000304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:0deb73ef8cdb24db1b6e38252bdcd582b97c120df9883c5e2d92c29503d1080a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.4 MB (386361722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce96880b22806db09af180be813a22b103b113db2f5cb686151ae7b771b0c4a5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:36:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:36:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:36:36 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:39:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:39:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:39:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:39:46 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:40:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:40:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:41:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:104619cc05a86891fa549978d70aed0cbcdf1e0a3f254eaa4f6c74fd7986232a`  
		Last Modified: Tue, 16 May 2023 01:34:52 GMT  
		Size: 22.3 MB (22308796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7662c0a09033f259cfefea66bfc47c3b9bbb307562a6b6998fc3a682c979fd`  
		Last Modified: Tue, 16 May 2023 01:47:49 GMT  
		Size: 819.9 KB (819940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde6eeba47f86346580f9fa91a059b60c0bb4cf3e5f6ed1e3679d9e2f39334`  
		Last Modified: Tue, 16 May 2023 01:47:48 GMT  
		Size: 4.1 MB (4090344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe51f70da36d055f10883024bfa76e76dcac9b4a97f98f52e77f33d0f99750b`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93559bbce6b99ec39b7cebb965a74180e140fbf1acaf77920e6814d4bee23715`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e765f9104d488baefed27a632f77947aa964a46dd9fa433b0e1f8775135c2`  
		Last Modified: Tue, 16 May 2023 01:48:20 GMT  
		Size: 239.1 MB (239074877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3a534b843be989ab6bcffda10cab7a25d9e89e372b418982beed4a5bd53e8d`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7a6b5a08e51594b5b48996514c854e0f9962e92af84647500c01e694a1a37f`  
		Last Modified: Tue, 16 May 2023 01:48:39 GMT  
		Size: 55.0 MB (55033552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e353beb4991a434beec1fc72cbb1bf5fbc88d61b103943cbd7edbaff3adf4e`  
		Last Modified: Tue, 16 May 2023 01:48:32 GMT  
		Size: 282.3 KB (282293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927d2ccabcebe45f8c2eaef683482295a9b01cd8ab7221cbc6b6234fceaae72e`  
		Last Modified: Tue, 16 May 2023 01:48:43 GMT  
		Size: 64.8 MB (64750073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:598eef934e9a0771c770be071bd381472cc667fbdd566290db95cf6d1448656d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.3 MB (412347336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a267fa349af659c76cdfb1f050f322f0584799eddf7902aa2bf7b22944db4a82`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:26:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:27:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:31:25 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:31:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:31:25 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:32:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:32:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:33:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac2eb781401fa2e4b052e397dc9f928e12a514dc36ae819c2a7abbade3a2ac0`  
		Last Modified: Tue, 16 May 2023 01:41:23 GMT  
		Size: 820.0 KB (819997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cee73a0939d3c0134856984b0f59e574b09845f42141f0e51a3ad7d3aa952b`  
		Last Modified: Tue, 16 May 2023 01:41:22 GMT  
		Size: 4.5 MB (4462716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bc25c9e9a20886e1895f9865c0ab6c367804dcf7d1fa93c4db637031e63b24`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600aba81d478ae55b4e43692c01f6987669b31e0770674637eeadca7daa54ce8`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c8797a2596b236b679b23d44b862b8b31161d06f60c4be964bb68508bad8`  
		Last Modified: Tue, 16 May 2023 01:41:46 GMT  
		Size: 252.5 MB (252523134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aa5b2cfcaaee2696bef62d280da0a68b762aa0c0eae563b386d61d563effb4`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101d4df18e2c0c39b90e2ddfb1834e3a24830c29592bd99b0a67138423030d1`  
		Last Modified: Tue, 16 May 2023 01:42:03 GMT  
		Size: 63.3 MB (63280661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776ca8ab0bde6eb881ce4739f6c994fc6ae802b5b51684190027fec142d14c7`  
		Last Modified: Tue, 16 May 2023 01:41:56 GMT  
		Size: 282.3 KB (282297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8c936e17cc88e7625757bb4c92076a187e149b9ccf4482a396d2a314b5ca6f`  
		Last Modified: Tue, 16 May 2023 01:42:04 GMT  
		Size: 67.2 MB (67235761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:70ae4f328ac4de6a63e408ce5aadc96890d11e597ff02ab8ccf429c40522e68b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:6b33f0fda8ca97ca7a2d1b2fc8a159c74a7b528dc614d6af292c80f5824117b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **743.5 MB (743457347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c5fbbea60e6db341a0ace94217b0c63753f06d76de44e1227b97471eec8894`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:04:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:05:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:05:05 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:08:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:08:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:08:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:08:45 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:09:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:09:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:10:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:16:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8112c7660661f5d395aac99b0d2403ccaaf47cfce01b40167688a866847d540`  
		Last Modified: Tue, 16 May 2023 01:17:48 GMT  
		Size: 819.1 KB (819098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64664c88569b54e7b2cace7a7eff36f63ca10a75b05e5c1ddceb69bbff1d387b`  
		Last Modified: Tue, 16 May 2023 01:17:47 GMT  
		Size: 4.9 MB (4878519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20548c67c76407d9f268011684621401f1bb204c67b556072a06759d86b2cd82`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96bc2cae0fba817ecce5d15aafad4eee15610dfe2178708ed47f732f7f71bd`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60000963f8bb247e6b22511e73ce54d4b3fefb24047ab49992acd24f8272aab5`  
		Last Modified: Tue, 16 May 2023 01:18:20 GMT  
		Size: 259.6 MB (259592143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af96a47a2aa7f522fcdf38f50ca1ff4abda4c7efd140a1d960f59b90f47d7788`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b12ba5acbea014d663262f916b8adc37a9271199290d917abd458538df9cb70`  
		Last Modified: Tue, 16 May 2023 01:18:38 GMT  
		Size: 70.5 MB (70459679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41bbf0250a9904f7b67e9257aa660ab936db8911b99cd58d9350b109b920e31`  
		Last Modified: Tue, 16 May 2023 01:18:29 GMT  
		Size: 282.3 KB (282294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f25d5aeddde8c1ec7ab0e2e9b51e8c30c5e7d69ad7cb00cb679682e3a47b3`  
		Last Modified: Tue, 16 May 2023 01:18:40 GMT  
		Size: 75.0 MB (75000304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff300cf21da0901eb6b3cdb1525000d29a65eb9aa9061dbbee9d2703cd4dff67`  
		Last Modified: Tue, 16 May 2023 01:19:45 GMT  
		Size: 305.7 MB (305707955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:646adcf1f16d3e1d3bc48f92290f0805024e9d94bbfe46a680dfedaaf97dc1d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.7 MB (646685667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a456c812a0c414ad53f02d28e85c190391d1bd50325791e430770060ac6983c3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:36:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:36:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:36:36 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:39:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:39:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:39:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:39:46 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:40:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:40:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:41:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:47:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:104619cc05a86891fa549978d70aed0cbcdf1e0a3f254eaa4f6c74fd7986232a`  
		Last Modified: Tue, 16 May 2023 01:34:52 GMT  
		Size: 22.3 MB (22308796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7662c0a09033f259cfefea66bfc47c3b9bbb307562a6b6998fc3a682c979fd`  
		Last Modified: Tue, 16 May 2023 01:47:49 GMT  
		Size: 819.9 KB (819940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde6eeba47f86346580f9fa91a059b60c0bb4cf3e5f6ed1e3679d9e2f39334`  
		Last Modified: Tue, 16 May 2023 01:47:48 GMT  
		Size: 4.1 MB (4090344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe51f70da36d055f10883024bfa76e76dcac9b4a97f98f52e77f33d0f99750b`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93559bbce6b99ec39b7cebb965a74180e140fbf1acaf77920e6814d4bee23715`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e765f9104d488baefed27a632f77947aa964a46dd9fa433b0e1f8775135c2`  
		Last Modified: Tue, 16 May 2023 01:48:20 GMT  
		Size: 239.1 MB (239074877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3a534b843be989ab6bcffda10cab7a25d9e89e372b418982beed4a5bd53e8d`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7a6b5a08e51594b5b48996514c854e0f9962e92af84647500c01e694a1a37f`  
		Last Modified: Tue, 16 May 2023 01:48:39 GMT  
		Size: 55.0 MB (55033552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e353beb4991a434beec1fc72cbb1bf5fbc88d61b103943cbd7edbaff3adf4e`  
		Last Modified: Tue, 16 May 2023 01:48:32 GMT  
		Size: 282.3 KB (282293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927d2ccabcebe45f8c2eaef683482295a9b01cd8ab7221cbc6b6234fceaae72e`  
		Last Modified: Tue, 16 May 2023 01:48:43 GMT  
		Size: 64.8 MB (64750073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc44d0bab65d62c64a227224cc0327696603ea1003eb74ee1a08b07ff7358897`  
		Last Modified: Tue, 16 May 2023 01:49:40 GMT  
		Size: 260.3 MB (260323945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cca7d182c039948f7dbb604818031776ca017764055a20d44dfea82a6526bb8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.4 MB (704354319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed00e75fdcc4dd708cc5dd59660b8cc81cdeaae3834881daea3c000fbd0acab4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:26:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:27:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:31:25 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:31:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:31:25 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:32:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:32:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:33:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:40:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac2eb781401fa2e4b052e397dc9f928e12a514dc36ae819c2a7abbade3a2ac0`  
		Last Modified: Tue, 16 May 2023 01:41:23 GMT  
		Size: 820.0 KB (819997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cee73a0939d3c0134856984b0f59e574b09845f42141f0e51a3ad7d3aa952b`  
		Last Modified: Tue, 16 May 2023 01:41:22 GMT  
		Size: 4.5 MB (4462716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bc25c9e9a20886e1895f9865c0ab6c367804dcf7d1fa93c4db637031e63b24`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600aba81d478ae55b4e43692c01f6987669b31e0770674637eeadca7daa54ce8`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c8797a2596b236b679b23d44b862b8b31161d06f60c4be964bb68508bad8`  
		Last Modified: Tue, 16 May 2023 01:41:46 GMT  
		Size: 252.5 MB (252523134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aa5b2cfcaaee2696bef62d280da0a68b762aa0c0eae563b386d61d563effb4`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101d4df18e2c0c39b90e2ddfb1834e3a24830c29592bd99b0a67138423030d1`  
		Last Modified: Tue, 16 May 2023 01:42:03 GMT  
		Size: 63.3 MB (63280661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776ca8ab0bde6eb881ce4739f6c994fc6ae802b5b51684190027fec142d14c7`  
		Last Modified: Tue, 16 May 2023 01:41:56 GMT  
		Size: 282.3 KB (282297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8c936e17cc88e7625757bb4c92076a187e149b9ccf4482a396d2a314b5ca6f`  
		Last Modified: Tue, 16 May 2023 01:42:04 GMT  
		Size: 67.2 MB (67235761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea10d3f21790e7bb555aa06a9aa7ad94499d2cd8771ab713e1946affdc321f49`  
		Last Modified: Tue, 16 May 2023 01:42:55 GMT  
		Size: 292.0 MB (292006983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:70ae4f328ac4de6a63e408ce5aadc96890d11e597ff02ab8ccf429c40522e68b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:6b33f0fda8ca97ca7a2d1b2fc8a159c74a7b528dc614d6af292c80f5824117b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **743.5 MB (743457347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c5fbbea60e6db341a0ace94217b0c63753f06d76de44e1227b97471eec8894`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:04:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:05:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:05:05 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:08:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:08:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:08:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:08:45 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:09:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:09:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:10:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:16:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8112c7660661f5d395aac99b0d2403ccaaf47cfce01b40167688a866847d540`  
		Last Modified: Tue, 16 May 2023 01:17:48 GMT  
		Size: 819.1 KB (819098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64664c88569b54e7b2cace7a7eff36f63ca10a75b05e5c1ddceb69bbff1d387b`  
		Last Modified: Tue, 16 May 2023 01:17:47 GMT  
		Size: 4.9 MB (4878519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20548c67c76407d9f268011684621401f1bb204c67b556072a06759d86b2cd82`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96bc2cae0fba817ecce5d15aafad4eee15610dfe2178708ed47f732f7f71bd`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60000963f8bb247e6b22511e73ce54d4b3fefb24047ab49992acd24f8272aab5`  
		Last Modified: Tue, 16 May 2023 01:18:20 GMT  
		Size: 259.6 MB (259592143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af96a47a2aa7f522fcdf38f50ca1ff4abda4c7efd140a1d960f59b90f47d7788`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b12ba5acbea014d663262f916b8adc37a9271199290d917abd458538df9cb70`  
		Last Modified: Tue, 16 May 2023 01:18:38 GMT  
		Size: 70.5 MB (70459679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41bbf0250a9904f7b67e9257aa660ab936db8911b99cd58d9350b109b920e31`  
		Last Modified: Tue, 16 May 2023 01:18:29 GMT  
		Size: 282.3 KB (282294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f25d5aeddde8c1ec7ab0e2e9b51e8c30c5e7d69ad7cb00cb679682e3a47b3`  
		Last Modified: Tue, 16 May 2023 01:18:40 GMT  
		Size: 75.0 MB (75000304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff300cf21da0901eb6b3cdb1525000d29a65eb9aa9061dbbee9d2703cd4dff67`  
		Last Modified: Tue, 16 May 2023 01:19:45 GMT  
		Size: 305.7 MB (305707955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:646adcf1f16d3e1d3bc48f92290f0805024e9d94bbfe46a680dfedaaf97dc1d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.7 MB (646685667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a456c812a0c414ad53f02d28e85c190391d1bd50325791e430770060ac6983c3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:36:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:36:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:36:36 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:39:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:39:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:39:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:39:46 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:40:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:40:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:41:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:47:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:104619cc05a86891fa549978d70aed0cbcdf1e0a3f254eaa4f6c74fd7986232a`  
		Last Modified: Tue, 16 May 2023 01:34:52 GMT  
		Size: 22.3 MB (22308796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7662c0a09033f259cfefea66bfc47c3b9bbb307562a6b6998fc3a682c979fd`  
		Last Modified: Tue, 16 May 2023 01:47:49 GMT  
		Size: 819.9 KB (819940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde6eeba47f86346580f9fa91a059b60c0bb4cf3e5f6ed1e3679d9e2f39334`  
		Last Modified: Tue, 16 May 2023 01:47:48 GMT  
		Size: 4.1 MB (4090344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe51f70da36d055f10883024bfa76e76dcac9b4a97f98f52e77f33d0f99750b`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93559bbce6b99ec39b7cebb965a74180e140fbf1acaf77920e6814d4bee23715`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e765f9104d488baefed27a632f77947aa964a46dd9fa433b0e1f8775135c2`  
		Last Modified: Tue, 16 May 2023 01:48:20 GMT  
		Size: 239.1 MB (239074877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3a534b843be989ab6bcffda10cab7a25d9e89e372b418982beed4a5bd53e8d`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7a6b5a08e51594b5b48996514c854e0f9962e92af84647500c01e694a1a37f`  
		Last Modified: Tue, 16 May 2023 01:48:39 GMT  
		Size: 55.0 MB (55033552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e353beb4991a434beec1fc72cbb1bf5fbc88d61b103943cbd7edbaff3adf4e`  
		Last Modified: Tue, 16 May 2023 01:48:32 GMT  
		Size: 282.3 KB (282293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927d2ccabcebe45f8c2eaef683482295a9b01cd8ab7221cbc6b6234fceaae72e`  
		Last Modified: Tue, 16 May 2023 01:48:43 GMT  
		Size: 64.8 MB (64750073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc44d0bab65d62c64a227224cc0327696603ea1003eb74ee1a08b07ff7358897`  
		Last Modified: Tue, 16 May 2023 01:49:40 GMT  
		Size: 260.3 MB (260323945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cca7d182c039948f7dbb604818031776ca017764055a20d44dfea82a6526bb8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.4 MB (704354319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed00e75fdcc4dd708cc5dd59660b8cc81cdeaae3834881daea3c000fbd0acab4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:26:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:27:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:31:25 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:31:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:31:25 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:32:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:32:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:33:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:40:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac2eb781401fa2e4b052e397dc9f928e12a514dc36ae819c2a7abbade3a2ac0`  
		Last Modified: Tue, 16 May 2023 01:41:23 GMT  
		Size: 820.0 KB (819997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cee73a0939d3c0134856984b0f59e574b09845f42141f0e51a3ad7d3aa952b`  
		Last Modified: Tue, 16 May 2023 01:41:22 GMT  
		Size: 4.5 MB (4462716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bc25c9e9a20886e1895f9865c0ab6c367804dcf7d1fa93c4db637031e63b24`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600aba81d478ae55b4e43692c01f6987669b31e0770674637eeadca7daa54ce8`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c8797a2596b236b679b23d44b862b8b31161d06f60c4be964bb68508bad8`  
		Last Modified: Tue, 16 May 2023 01:41:46 GMT  
		Size: 252.5 MB (252523134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aa5b2cfcaaee2696bef62d280da0a68b762aa0c0eae563b386d61d563effb4`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101d4df18e2c0c39b90e2ddfb1834e3a24830c29592bd99b0a67138423030d1`  
		Last Modified: Tue, 16 May 2023 01:42:03 GMT  
		Size: 63.3 MB (63280661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776ca8ab0bde6eb881ce4739f6c994fc6ae802b5b51684190027fec142d14c7`  
		Last Modified: Tue, 16 May 2023 01:41:56 GMT  
		Size: 282.3 KB (282297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8c936e17cc88e7625757bb4c92076a187e149b9ccf4482a396d2a314b5ca6f`  
		Last Modified: Tue, 16 May 2023 01:42:04 GMT  
		Size: 67.2 MB (67235761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea10d3f21790e7bb555aa06a9aa7ad94499d2cd8771ab713e1946affdc321f49`  
		Last Modified: Tue, 16 May 2023 01:42:55 GMT  
		Size: 292.0 MB (292006983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:148b748629ba34c6abd4e9862551777c77018009bee31d26829cee98834c2e69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:23456582011b89ff5a83e718b36bbcc9bb96f689f430f702de455580c981dfa4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.8 MB (448835699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b9d9052510148a9741a3d24dba79d85bfabca8b35f04cdfde4e4cdd9aa00c6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:04:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:05:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:05:05 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:08:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:08:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:08:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:08:45 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:09:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:09:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:10:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:11:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8112c7660661f5d395aac99b0d2403ccaaf47cfce01b40167688a866847d540`  
		Last Modified: Tue, 16 May 2023 01:17:48 GMT  
		Size: 819.1 KB (819098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64664c88569b54e7b2cace7a7eff36f63ca10a75b05e5c1ddceb69bbff1d387b`  
		Last Modified: Tue, 16 May 2023 01:17:47 GMT  
		Size: 4.9 MB (4878519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20548c67c76407d9f268011684621401f1bb204c67b556072a06759d86b2cd82`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96bc2cae0fba817ecce5d15aafad4eee15610dfe2178708ed47f732f7f71bd`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60000963f8bb247e6b22511e73ce54d4b3fefb24047ab49992acd24f8272aab5`  
		Last Modified: Tue, 16 May 2023 01:18:20 GMT  
		Size: 259.6 MB (259592143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af96a47a2aa7f522fcdf38f50ca1ff4abda4c7efd140a1d960f59b90f47d7788`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b12ba5acbea014d663262f916b8adc37a9271199290d917abd458538df9cb70`  
		Last Modified: Tue, 16 May 2023 01:18:38 GMT  
		Size: 70.5 MB (70459679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41bbf0250a9904f7b67e9257aa660ab936db8911b99cd58d9350b109b920e31`  
		Last Modified: Tue, 16 May 2023 01:18:29 GMT  
		Size: 282.3 KB (282294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f25d5aeddde8c1ec7ab0e2e9b51e8c30c5e7d69ad7cb00cb679682e3a47b3`  
		Last Modified: Tue, 16 May 2023 01:18:40 GMT  
		Size: 75.0 MB (75000304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63750a48b8c413627810e36f792a3f745a8f70ef9615e698c1486f634756d35`  
		Last Modified: Tue, 16 May 2023 01:18:52 GMT  
		Size: 11.1 MB (11086307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:b067910b1094d3a3abbaad75eb317c0060cd70ffd7874c7ec2fd7bb7e9c7ca8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.5 MB (396484812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3bcc3b429e2448b27633206e46f793f627aa4ee24f19a38c9dfd49f2e18b1bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:36:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:36:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:36:36 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:39:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:39:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:39:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:39:46 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:40:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:40:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:41:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:104619cc05a86891fa549978d70aed0cbcdf1e0a3f254eaa4f6c74fd7986232a`  
		Last Modified: Tue, 16 May 2023 01:34:52 GMT  
		Size: 22.3 MB (22308796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7662c0a09033f259cfefea66bfc47c3b9bbb307562a6b6998fc3a682c979fd`  
		Last Modified: Tue, 16 May 2023 01:47:49 GMT  
		Size: 819.9 KB (819940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde6eeba47f86346580f9fa91a059b60c0bb4cf3e5f6ed1e3679d9e2f39334`  
		Last Modified: Tue, 16 May 2023 01:47:48 GMT  
		Size: 4.1 MB (4090344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe51f70da36d055f10883024bfa76e76dcac9b4a97f98f52e77f33d0f99750b`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93559bbce6b99ec39b7cebb965a74180e140fbf1acaf77920e6814d4bee23715`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e765f9104d488baefed27a632f77947aa964a46dd9fa433b0e1f8775135c2`  
		Last Modified: Tue, 16 May 2023 01:48:20 GMT  
		Size: 239.1 MB (239074877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3a534b843be989ab6bcffda10cab7a25d9e89e372b418982beed4a5bd53e8d`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7a6b5a08e51594b5b48996514c854e0f9962e92af84647500c01e694a1a37f`  
		Last Modified: Tue, 16 May 2023 01:48:39 GMT  
		Size: 55.0 MB (55033552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e353beb4991a434beec1fc72cbb1bf5fbc88d61b103943cbd7edbaff3adf4e`  
		Last Modified: Tue, 16 May 2023 01:48:32 GMT  
		Size: 282.3 KB (282293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927d2ccabcebe45f8c2eaef683482295a9b01cd8ab7221cbc6b6234fceaae72e`  
		Last Modified: Tue, 16 May 2023 01:48:43 GMT  
		Size: 64.8 MB (64750073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8677cdd8ae6161323a7c34b75e3960a456492760fb6789308162f2947bc15fdb`  
		Last Modified: Tue, 16 May 2023 01:48:55 GMT  
		Size: 10.1 MB (10123090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9425ff9301d11197a6df04fe6b52790d5fb67ca22bd7839b6da94b05260c62df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.1 MB (423088622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:144efd1daa2cb59cc73648b114e06e54fd321deef7f39f97a9e10604093dc64c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:26:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:27:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:31:25 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:31:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:31:25 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:32:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:32:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:33:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:34:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac2eb781401fa2e4b052e397dc9f928e12a514dc36ae819c2a7abbade3a2ac0`  
		Last Modified: Tue, 16 May 2023 01:41:23 GMT  
		Size: 820.0 KB (819997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cee73a0939d3c0134856984b0f59e574b09845f42141f0e51a3ad7d3aa952b`  
		Last Modified: Tue, 16 May 2023 01:41:22 GMT  
		Size: 4.5 MB (4462716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bc25c9e9a20886e1895f9865c0ab6c367804dcf7d1fa93c4db637031e63b24`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600aba81d478ae55b4e43692c01f6987669b31e0770674637eeadca7daa54ce8`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c8797a2596b236b679b23d44b862b8b31161d06f60c4be964bb68508bad8`  
		Last Modified: Tue, 16 May 2023 01:41:46 GMT  
		Size: 252.5 MB (252523134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aa5b2cfcaaee2696bef62d280da0a68b762aa0c0eae563b386d61d563effb4`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101d4df18e2c0c39b90e2ddfb1834e3a24830c29592bd99b0a67138423030d1`  
		Last Modified: Tue, 16 May 2023 01:42:03 GMT  
		Size: 63.3 MB (63280661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776ca8ab0bde6eb881ce4739f6c994fc6ae802b5b51684190027fec142d14c7`  
		Last Modified: Tue, 16 May 2023 01:41:56 GMT  
		Size: 282.3 KB (282297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8c936e17cc88e7625757bb4c92076a187e149b9ccf4482a396d2a314b5ca6f`  
		Last Modified: Tue, 16 May 2023 01:42:04 GMT  
		Size: 67.2 MB (67235761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955dc7d42aaa7e345f471d6599e31886f6619fc15a5992bc0281b1bda830be98`  
		Last Modified: Tue, 16 May 2023 01:42:16 GMT  
		Size: 10.7 MB (10741286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:148b748629ba34c6abd4e9862551777c77018009bee31d26829cee98834c2e69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:23456582011b89ff5a83e718b36bbcc9bb96f689f430f702de455580c981dfa4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.8 MB (448835699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b9d9052510148a9741a3d24dba79d85bfabca8b35f04cdfde4e4cdd9aa00c6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:04:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:05:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:05:05 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:08:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:08:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:08:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:08:45 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:09:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:09:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:10:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:11:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8112c7660661f5d395aac99b0d2403ccaaf47cfce01b40167688a866847d540`  
		Last Modified: Tue, 16 May 2023 01:17:48 GMT  
		Size: 819.1 KB (819098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64664c88569b54e7b2cace7a7eff36f63ca10a75b05e5c1ddceb69bbff1d387b`  
		Last Modified: Tue, 16 May 2023 01:17:47 GMT  
		Size: 4.9 MB (4878519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20548c67c76407d9f268011684621401f1bb204c67b556072a06759d86b2cd82`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96bc2cae0fba817ecce5d15aafad4eee15610dfe2178708ed47f732f7f71bd`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60000963f8bb247e6b22511e73ce54d4b3fefb24047ab49992acd24f8272aab5`  
		Last Modified: Tue, 16 May 2023 01:18:20 GMT  
		Size: 259.6 MB (259592143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af96a47a2aa7f522fcdf38f50ca1ff4abda4c7efd140a1d960f59b90f47d7788`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b12ba5acbea014d663262f916b8adc37a9271199290d917abd458538df9cb70`  
		Last Modified: Tue, 16 May 2023 01:18:38 GMT  
		Size: 70.5 MB (70459679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41bbf0250a9904f7b67e9257aa660ab936db8911b99cd58d9350b109b920e31`  
		Last Modified: Tue, 16 May 2023 01:18:29 GMT  
		Size: 282.3 KB (282294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f25d5aeddde8c1ec7ab0e2e9b51e8c30c5e7d69ad7cb00cb679682e3a47b3`  
		Last Modified: Tue, 16 May 2023 01:18:40 GMT  
		Size: 75.0 MB (75000304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63750a48b8c413627810e36f792a3f745a8f70ef9615e698c1486f634756d35`  
		Last Modified: Tue, 16 May 2023 01:18:52 GMT  
		Size: 11.1 MB (11086307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:b067910b1094d3a3abbaad75eb317c0060cd70ffd7874c7ec2fd7bb7e9c7ca8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.5 MB (396484812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3bcc3b429e2448b27633206e46f793f627aa4ee24f19a38c9dfd49f2e18b1bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:36:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:36:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:36:36 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:39:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:39:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:39:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:39:46 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:40:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:40:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:41:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:104619cc05a86891fa549978d70aed0cbcdf1e0a3f254eaa4f6c74fd7986232a`  
		Last Modified: Tue, 16 May 2023 01:34:52 GMT  
		Size: 22.3 MB (22308796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7662c0a09033f259cfefea66bfc47c3b9bbb307562a6b6998fc3a682c979fd`  
		Last Modified: Tue, 16 May 2023 01:47:49 GMT  
		Size: 819.9 KB (819940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde6eeba47f86346580f9fa91a059b60c0bb4cf3e5f6ed1e3679d9e2f39334`  
		Last Modified: Tue, 16 May 2023 01:47:48 GMT  
		Size: 4.1 MB (4090344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe51f70da36d055f10883024bfa76e76dcac9b4a97f98f52e77f33d0f99750b`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93559bbce6b99ec39b7cebb965a74180e140fbf1acaf77920e6814d4bee23715`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e765f9104d488baefed27a632f77947aa964a46dd9fa433b0e1f8775135c2`  
		Last Modified: Tue, 16 May 2023 01:48:20 GMT  
		Size: 239.1 MB (239074877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3a534b843be989ab6bcffda10cab7a25d9e89e372b418982beed4a5bd53e8d`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7a6b5a08e51594b5b48996514c854e0f9962e92af84647500c01e694a1a37f`  
		Last Modified: Tue, 16 May 2023 01:48:39 GMT  
		Size: 55.0 MB (55033552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e353beb4991a434beec1fc72cbb1bf5fbc88d61b103943cbd7edbaff3adf4e`  
		Last Modified: Tue, 16 May 2023 01:48:32 GMT  
		Size: 282.3 KB (282293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927d2ccabcebe45f8c2eaef683482295a9b01cd8ab7221cbc6b6234fceaae72e`  
		Last Modified: Tue, 16 May 2023 01:48:43 GMT  
		Size: 64.8 MB (64750073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8677cdd8ae6161323a7c34b75e3960a456492760fb6789308162f2947bc15fdb`  
		Last Modified: Tue, 16 May 2023 01:48:55 GMT  
		Size: 10.1 MB (10123090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9425ff9301d11197a6df04fe6b52790d5fb67ca22bd7839b6da94b05260c62df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.1 MB (423088622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:144efd1daa2cb59cc73648b114e06e54fd321deef7f39f97a9e10604093dc64c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:26:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:27:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:31:25 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:31:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:31:25 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:32:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:32:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:33:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:34:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac2eb781401fa2e4b052e397dc9f928e12a514dc36ae819c2a7abbade3a2ac0`  
		Last Modified: Tue, 16 May 2023 01:41:23 GMT  
		Size: 820.0 KB (819997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cee73a0939d3c0134856984b0f59e574b09845f42141f0e51a3ad7d3aa952b`  
		Last Modified: Tue, 16 May 2023 01:41:22 GMT  
		Size: 4.5 MB (4462716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bc25c9e9a20886e1895f9865c0ab6c367804dcf7d1fa93c4db637031e63b24`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600aba81d478ae55b4e43692c01f6987669b31e0770674637eeadca7daa54ce8`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c8797a2596b236b679b23d44b862b8b31161d06f60c4be964bb68508bad8`  
		Last Modified: Tue, 16 May 2023 01:41:46 GMT  
		Size: 252.5 MB (252523134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aa5b2cfcaaee2696bef62d280da0a68b762aa0c0eae563b386d61d563effb4`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101d4df18e2c0c39b90e2ddfb1834e3a24830c29592bd99b0a67138423030d1`  
		Last Modified: Tue, 16 May 2023 01:42:03 GMT  
		Size: 63.3 MB (63280661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776ca8ab0bde6eb881ce4739f6c994fc6ae802b5b51684190027fec142d14c7`  
		Last Modified: Tue, 16 May 2023 01:41:56 GMT  
		Size: 282.3 KB (282297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8c936e17cc88e7625757bb4c92076a187e149b9ccf4482a396d2a314b5ca6f`  
		Last Modified: Tue, 16 May 2023 01:42:04 GMT  
		Size: 67.2 MB (67235761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955dc7d42aaa7e345f471d6599e31886f6619fc15a5992bc0281b1bda830be98`  
		Last Modified: Tue, 16 May 2023 01:42:16 GMT  
		Size: 10.7 MB (10741286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:4c16420fc4f1f71dd59278ea8f881eef389cb3d9417faaa12edc6553615d767d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:21bb4ad490af560bb44192eed50c1c493358c59c01d70171814c9afbec151bbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.7 MB (437749392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77f179e2e80523fb74868ca6cc6d867b9fc5131cdeb36db2e4e9f1fc9ea0e2f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:04:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:05:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:05:05 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:08:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:08:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:08:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:08:45 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:09:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:09:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:10:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8112c7660661f5d395aac99b0d2403ccaaf47cfce01b40167688a866847d540`  
		Last Modified: Tue, 16 May 2023 01:17:48 GMT  
		Size: 819.1 KB (819098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64664c88569b54e7b2cace7a7eff36f63ca10a75b05e5c1ddceb69bbff1d387b`  
		Last Modified: Tue, 16 May 2023 01:17:47 GMT  
		Size: 4.9 MB (4878519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20548c67c76407d9f268011684621401f1bb204c67b556072a06759d86b2cd82`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96bc2cae0fba817ecce5d15aafad4eee15610dfe2178708ed47f732f7f71bd`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60000963f8bb247e6b22511e73ce54d4b3fefb24047ab49992acd24f8272aab5`  
		Last Modified: Tue, 16 May 2023 01:18:20 GMT  
		Size: 259.6 MB (259592143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af96a47a2aa7f522fcdf38f50ca1ff4abda4c7efd140a1d960f59b90f47d7788`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b12ba5acbea014d663262f916b8adc37a9271199290d917abd458538df9cb70`  
		Last Modified: Tue, 16 May 2023 01:18:38 GMT  
		Size: 70.5 MB (70459679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41bbf0250a9904f7b67e9257aa660ab936db8911b99cd58d9350b109b920e31`  
		Last Modified: Tue, 16 May 2023 01:18:29 GMT  
		Size: 282.3 KB (282294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f25d5aeddde8c1ec7ab0e2e9b51e8c30c5e7d69ad7cb00cb679682e3a47b3`  
		Last Modified: Tue, 16 May 2023 01:18:40 GMT  
		Size: 75.0 MB (75000304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:0deb73ef8cdb24db1b6e38252bdcd582b97c120df9883c5e2d92c29503d1080a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.4 MB (386361722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce96880b22806db09af180be813a22b103b113db2f5cb686151ae7b771b0c4a5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:36:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:36:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:36:36 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:39:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:39:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:39:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:39:46 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:40:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:40:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:41:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:104619cc05a86891fa549978d70aed0cbcdf1e0a3f254eaa4f6c74fd7986232a`  
		Last Modified: Tue, 16 May 2023 01:34:52 GMT  
		Size: 22.3 MB (22308796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7662c0a09033f259cfefea66bfc47c3b9bbb307562a6b6998fc3a682c979fd`  
		Last Modified: Tue, 16 May 2023 01:47:49 GMT  
		Size: 819.9 KB (819940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde6eeba47f86346580f9fa91a059b60c0bb4cf3e5f6ed1e3679d9e2f39334`  
		Last Modified: Tue, 16 May 2023 01:47:48 GMT  
		Size: 4.1 MB (4090344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe51f70da36d055f10883024bfa76e76dcac9b4a97f98f52e77f33d0f99750b`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93559bbce6b99ec39b7cebb965a74180e140fbf1acaf77920e6814d4bee23715`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e765f9104d488baefed27a632f77947aa964a46dd9fa433b0e1f8775135c2`  
		Last Modified: Tue, 16 May 2023 01:48:20 GMT  
		Size: 239.1 MB (239074877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3a534b843be989ab6bcffda10cab7a25d9e89e372b418982beed4a5bd53e8d`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7a6b5a08e51594b5b48996514c854e0f9962e92af84647500c01e694a1a37f`  
		Last Modified: Tue, 16 May 2023 01:48:39 GMT  
		Size: 55.0 MB (55033552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e353beb4991a434beec1fc72cbb1bf5fbc88d61b103943cbd7edbaff3adf4e`  
		Last Modified: Tue, 16 May 2023 01:48:32 GMT  
		Size: 282.3 KB (282293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927d2ccabcebe45f8c2eaef683482295a9b01cd8ab7221cbc6b6234fceaae72e`  
		Last Modified: Tue, 16 May 2023 01:48:43 GMT  
		Size: 64.8 MB (64750073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:598eef934e9a0771c770be071bd381472cc667fbdd566290db95cf6d1448656d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.3 MB (412347336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a267fa349af659c76cdfb1f050f322f0584799eddf7902aa2bf7b22944db4a82`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:26:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:27:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:31:25 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:31:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:31:25 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:32:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:32:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:33:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac2eb781401fa2e4b052e397dc9f928e12a514dc36ae819c2a7abbade3a2ac0`  
		Last Modified: Tue, 16 May 2023 01:41:23 GMT  
		Size: 820.0 KB (819997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cee73a0939d3c0134856984b0f59e574b09845f42141f0e51a3ad7d3aa952b`  
		Last Modified: Tue, 16 May 2023 01:41:22 GMT  
		Size: 4.5 MB (4462716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bc25c9e9a20886e1895f9865c0ab6c367804dcf7d1fa93c4db637031e63b24`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600aba81d478ae55b4e43692c01f6987669b31e0770674637eeadca7daa54ce8`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c8797a2596b236b679b23d44b862b8b31161d06f60c4be964bb68508bad8`  
		Last Modified: Tue, 16 May 2023 01:41:46 GMT  
		Size: 252.5 MB (252523134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aa5b2cfcaaee2696bef62d280da0a68b762aa0c0eae563b386d61d563effb4`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101d4df18e2c0c39b90e2ddfb1834e3a24830c29592bd99b0a67138423030d1`  
		Last Modified: Tue, 16 May 2023 01:42:03 GMT  
		Size: 63.3 MB (63280661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776ca8ab0bde6eb881ce4739f6c994fc6ae802b5b51684190027fec142d14c7`  
		Last Modified: Tue, 16 May 2023 01:41:56 GMT  
		Size: 282.3 KB (282297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8c936e17cc88e7625757bb4c92076a187e149b9ccf4482a396d2a314b5ca6f`  
		Last Modified: Tue, 16 May 2023 01:42:04 GMT  
		Size: 67.2 MB (67235761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:4c16420fc4f1f71dd59278ea8f881eef389cb3d9417faaa12edc6553615d767d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:21bb4ad490af560bb44192eed50c1c493358c59c01d70171814c9afbec151bbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.7 MB (437749392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77f179e2e80523fb74868ca6cc6d867b9fc5131cdeb36db2e4e9f1fc9ea0e2f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:04:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:05:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:05:05 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:08:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:08:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:08:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:08:45 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:09:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:09:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:10:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8112c7660661f5d395aac99b0d2403ccaaf47cfce01b40167688a866847d540`  
		Last Modified: Tue, 16 May 2023 01:17:48 GMT  
		Size: 819.1 KB (819098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64664c88569b54e7b2cace7a7eff36f63ca10a75b05e5c1ddceb69bbff1d387b`  
		Last Modified: Tue, 16 May 2023 01:17:47 GMT  
		Size: 4.9 MB (4878519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20548c67c76407d9f268011684621401f1bb204c67b556072a06759d86b2cd82`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96bc2cae0fba817ecce5d15aafad4eee15610dfe2178708ed47f732f7f71bd`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60000963f8bb247e6b22511e73ce54d4b3fefb24047ab49992acd24f8272aab5`  
		Last Modified: Tue, 16 May 2023 01:18:20 GMT  
		Size: 259.6 MB (259592143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af96a47a2aa7f522fcdf38f50ca1ff4abda4c7efd140a1d960f59b90f47d7788`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b12ba5acbea014d663262f916b8adc37a9271199290d917abd458538df9cb70`  
		Last Modified: Tue, 16 May 2023 01:18:38 GMT  
		Size: 70.5 MB (70459679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41bbf0250a9904f7b67e9257aa660ab936db8911b99cd58d9350b109b920e31`  
		Last Modified: Tue, 16 May 2023 01:18:29 GMT  
		Size: 282.3 KB (282294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f25d5aeddde8c1ec7ab0e2e9b51e8c30c5e7d69ad7cb00cb679682e3a47b3`  
		Last Modified: Tue, 16 May 2023 01:18:40 GMT  
		Size: 75.0 MB (75000304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:0deb73ef8cdb24db1b6e38252bdcd582b97c120df9883c5e2d92c29503d1080a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.4 MB (386361722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce96880b22806db09af180be813a22b103b113db2f5cb686151ae7b771b0c4a5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:36:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:36:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:36:36 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:39:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:39:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:39:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:39:46 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:40:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:40:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:41:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:104619cc05a86891fa549978d70aed0cbcdf1e0a3f254eaa4f6c74fd7986232a`  
		Last Modified: Tue, 16 May 2023 01:34:52 GMT  
		Size: 22.3 MB (22308796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7662c0a09033f259cfefea66bfc47c3b9bbb307562a6b6998fc3a682c979fd`  
		Last Modified: Tue, 16 May 2023 01:47:49 GMT  
		Size: 819.9 KB (819940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde6eeba47f86346580f9fa91a059b60c0bb4cf3e5f6ed1e3679d9e2f39334`  
		Last Modified: Tue, 16 May 2023 01:47:48 GMT  
		Size: 4.1 MB (4090344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe51f70da36d055f10883024bfa76e76dcac9b4a97f98f52e77f33d0f99750b`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93559bbce6b99ec39b7cebb965a74180e140fbf1acaf77920e6814d4bee23715`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e765f9104d488baefed27a632f77947aa964a46dd9fa433b0e1f8775135c2`  
		Last Modified: Tue, 16 May 2023 01:48:20 GMT  
		Size: 239.1 MB (239074877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3a534b843be989ab6bcffda10cab7a25d9e89e372b418982beed4a5bd53e8d`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7a6b5a08e51594b5b48996514c854e0f9962e92af84647500c01e694a1a37f`  
		Last Modified: Tue, 16 May 2023 01:48:39 GMT  
		Size: 55.0 MB (55033552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e353beb4991a434beec1fc72cbb1bf5fbc88d61b103943cbd7edbaff3adf4e`  
		Last Modified: Tue, 16 May 2023 01:48:32 GMT  
		Size: 282.3 KB (282293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927d2ccabcebe45f8c2eaef683482295a9b01cd8ab7221cbc6b6234fceaae72e`  
		Last Modified: Tue, 16 May 2023 01:48:43 GMT  
		Size: 64.8 MB (64750073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:598eef934e9a0771c770be071bd381472cc667fbdd566290db95cf6d1448656d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.3 MB (412347336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a267fa349af659c76cdfb1f050f322f0584799eddf7902aa2bf7b22944db4a82`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:26:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:27:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:31:25 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:31:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:31:25 GMT
CMD ["bash"]
# Tue, 16 May 2023 01:32:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:32:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 16 May 2023 01:33:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac2eb781401fa2e4b052e397dc9f928e12a514dc36ae819c2a7abbade3a2ac0`  
		Last Modified: Tue, 16 May 2023 01:41:23 GMT  
		Size: 820.0 KB (819997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cee73a0939d3c0134856984b0f59e574b09845f42141f0e51a3ad7d3aa952b`  
		Last Modified: Tue, 16 May 2023 01:41:22 GMT  
		Size: 4.5 MB (4462716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bc25c9e9a20886e1895f9865c0ab6c367804dcf7d1fa93c4db637031e63b24`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600aba81d478ae55b4e43692c01f6987669b31e0770674637eeadca7daa54ce8`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c8797a2596b236b679b23d44b862b8b31161d06f60c4be964bb68508bad8`  
		Last Modified: Tue, 16 May 2023 01:41:46 GMT  
		Size: 252.5 MB (252523134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aa5b2cfcaaee2696bef62d280da0a68b762aa0c0eae563b386d61d563effb4`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101d4df18e2c0c39b90e2ddfb1834e3a24830c29592bd99b0a67138423030d1`  
		Last Modified: Tue, 16 May 2023 01:42:03 GMT  
		Size: 63.3 MB (63280661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776ca8ab0bde6eb881ce4739f6c994fc6ae802b5b51684190027fec142d14c7`  
		Last Modified: Tue, 16 May 2023 01:41:56 GMT  
		Size: 282.3 KB (282297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8c936e17cc88e7625757bb4c92076a187e149b9ccf4482a396d2a314b5ca6f`  
		Last Modified: Tue, 16 May 2023 01:42:04 GMT  
		Size: 67.2 MB (67235761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:526d64c285d5dc79374ee66b464e4edfe02c63664753ae3c415d90e1396a3865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:88b0627eb45b2ebb315020c66ce2d451b7cb2f868828521804e918a34f80ba53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (292007115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6bffb25cf6397d48c101b92a5aece01446c9eb246b958d6b248eada283416a8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:04:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:05:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:05:05 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:08:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:08:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:08:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:08:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8112c7660661f5d395aac99b0d2403ccaaf47cfce01b40167688a866847d540`  
		Last Modified: Tue, 16 May 2023 01:17:48 GMT  
		Size: 819.1 KB (819098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64664c88569b54e7b2cace7a7eff36f63ca10a75b05e5c1ddceb69bbff1d387b`  
		Last Modified: Tue, 16 May 2023 01:17:47 GMT  
		Size: 4.9 MB (4878519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20548c67c76407d9f268011684621401f1bb204c67b556072a06759d86b2cd82`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96bc2cae0fba817ecce5d15aafad4eee15610dfe2178708ed47f732f7f71bd`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60000963f8bb247e6b22511e73ce54d4b3fefb24047ab49992acd24f8272aab5`  
		Last Modified: Tue, 16 May 2023 01:18:20 GMT  
		Size: 259.6 MB (259592143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af96a47a2aa7f522fcdf38f50ca1ff4abda4c7efd140a1d960f59b90f47d7788`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:3bdca4d506f1847bbe0547a73ee8bc4f6bd394c8d2832b6edbb0b527e34bea79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266295804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bcde6af57fbad9bea421ac870138412418f08dd0de83f61e3c0d5baad1e3d0f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:36:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:36:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:36:36 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:39:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:39:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:39:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:39:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:104619cc05a86891fa549978d70aed0cbcdf1e0a3f254eaa4f6c74fd7986232a`  
		Last Modified: Tue, 16 May 2023 01:34:52 GMT  
		Size: 22.3 MB (22308796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7662c0a09033f259cfefea66bfc47c3b9bbb307562a6b6998fc3a682c979fd`  
		Last Modified: Tue, 16 May 2023 01:47:49 GMT  
		Size: 819.9 KB (819940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde6eeba47f86346580f9fa91a059b60c0bb4cf3e5f6ed1e3679d9e2f39334`  
		Last Modified: Tue, 16 May 2023 01:47:48 GMT  
		Size: 4.1 MB (4090344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe51f70da36d055f10883024bfa76e76dcac9b4a97f98f52e77f33d0f99750b`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93559bbce6b99ec39b7cebb965a74180e140fbf1acaf77920e6814d4bee23715`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e765f9104d488baefed27a632f77947aa964a46dd9fa433b0e1f8775135c2`  
		Last Modified: Tue, 16 May 2023 01:48:20 GMT  
		Size: 239.1 MB (239074877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3a534b843be989ab6bcffda10cab7a25d9e89e372b418982beed4a5bd53e8d`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1d718e4d40ae335a28d1a06991e095c0b854b4362c600372f7a89c48c81b97f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.5 MB (281548617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d01af3854384e5145f6c136312f7b25b347c5b41022811a51bc258de17f3bd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:26:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:27:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:31:25 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:31:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:31:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac2eb781401fa2e4b052e397dc9f928e12a514dc36ae819c2a7abbade3a2ac0`  
		Last Modified: Tue, 16 May 2023 01:41:23 GMT  
		Size: 820.0 KB (819997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cee73a0939d3c0134856984b0f59e574b09845f42141f0e51a3ad7d3aa952b`  
		Last Modified: Tue, 16 May 2023 01:41:22 GMT  
		Size: 4.5 MB (4462716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bc25c9e9a20886e1895f9865c0ab6c367804dcf7d1fa93c4db637031e63b24`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600aba81d478ae55b4e43692c01f6987669b31e0770674637eeadca7daa54ce8`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c8797a2596b236b679b23d44b862b8b31161d06f60c4be964bb68508bad8`  
		Last Modified: Tue, 16 May 2023 01:41:46 GMT  
		Size: 252.5 MB (252523134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aa5b2cfcaaee2696bef62d280da0a68b762aa0c0eae563b386d61d563effb4`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:526d64c285d5dc79374ee66b464e4edfe02c63664753ae3c415d90e1396a3865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:88b0627eb45b2ebb315020c66ce2d451b7cb2f868828521804e918a34f80ba53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (292007115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6bffb25cf6397d48c101b92a5aece01446c9eb246b958d6b248eada283416a8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:04:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:05:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:05:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:05:05 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:05:05 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:08:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:08:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:08:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:08:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8112c7660661f5d395aac99b0d2403ccaaf47cfce01b40167688a866847d540`  
		Last Modified: Tue, 16 May 2023 01:17:48 GMT  
		Size: 819.1 KB (819098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64664c88569b54e7b2cace7a7eff36f63ca10a75b05e5c1ddceb69bbff1d387b`  
		Last Modified: Tue, 16 May 2023 01:17:47 GMT  
		Size: 4.9 MB (4878519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20548c67c76407d9f268011684621401f1bb204c67b556072a06759d86b2cd82`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96bc2cae0fba817ecce5d15aafad4eee15610dfe2178708ed47f732f7f71bd`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60000963f8bb247e6b22511e73ce54d4b3fefb24047ab49992acd24f8272aab5`  
		Last Modified: Tue, 16 May 2023 01:18:20 GMT  
		Size: 259.6 MB (259592143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af96a47a2aa7f522fcdf38f50ca1ff4abda4c7efd140a1d960f59b90f47d7788`  
		Last Modified: Tue, 16 May 2023 01:17:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:3bdca4d506f1847bbe0547a73ee8bc4f6bd394c8d2832b6edbb0b527e34bea79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266295804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bcde6af57fbad9bea421ac870138412418f08dd0de83f61e3c0d5baad1e3d0f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:26:37 GMT
ARG RELEASE
# Fri, 12 May 2023 09:26:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:26:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:26:38 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:26:40 GMT
ADD file:c66513453620aaf35bbe377c693bac11a921cf12b7c0990cde7a0d5d113b93e0 in / 
# Fri, 12 May 2023 09:26:40 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:36:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:36:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:36:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:36:36 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:36:36 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:39:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:39:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:39:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:39:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:104619cc05a86891fa549978d70aed0cbcdf1e0a3f254eaa4f6c74fd7986232a`  
		Last Modified: Tue, 16 May 2023 01:34:52 GMT  
		Size: 22.3 MB (22308796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7662c0a09033f259cfefea66bfc47c3b9bbb307562a6b6998fc3a682c979fd`  
		Last Modified: Tue, 16 May 2023 01:47:49 GMT  
		Size: 819.9 KB (819940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde6eeba47f86346580f9fa91a059b60c0bb4cf3e5f6ed1e3679d9e2f39334`  
		Last Modified: Tue, 16 May 2023 01:47:48 GMT  
		Size: 4.1 MB (4090344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe51f70da36d055f10883024bfa76e76dcac9b4a97f98f52e77f33d0f99750b`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93559bbce6b99ec39b7cebb965a74180e140fbf1acaf77920e6814d4bee23715`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e765f9104d488baefed27a632f77947aa964a46dd9fa433b0e1f8775135c2`  
		Last Modified: Tue, 16 May 2023 01:48:20 GMT  
		Size: 239.1 MB (239074877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3a534b843be989ab6bcffda10cab7a25d9e89e372b418982beed4a5bd53e8d`  
		Last Modified: Tue, 16 May 2023 01:47:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1d718e4d40ae335a28d1a06991e095c0b854b4362c600372f7a89c48c81b97f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.5 MB (281548617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d01af3854384e5145f6c136312f7b25b347c5b41022811a51bc258de17f3bd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:26:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:27:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 16 May 2023 01:27:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 16 May 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 16 May 2023 01:27:04 GMT
ENV ROS_DISTRO=melodic
# Tue, 16 May 2023 01:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:31:25 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 16 May 2023 01:31:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 16 May 2023 01:31:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac2eb781401fa2e4b052e397dc9f928e12a514dc36ae819c2a7abbade3a2ac0`  
		Last Modified: Tue, 16 May 2023 01:41:23 GMT  
		Size: 820.0 KB (819997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cee73a0939d3c0134856984b0f59e574b09845f42141f0e51a3ad7d3aa952b`  
		Last Modified: Tue, 16 May 2023 01:41:22 GMT  
		Size: 4.5 MB (4462716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bc25c9e9a20886e1895f9865c0ab6c367804dcf7d1fa93c4db637031e63b24`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600aba81d478ae55b4e43692c01f6987669b31e0770674637eeadca7daa54ce8`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c8797a2596b236b679b23d44b862b8b31161d06f60c4be964bb68508bad8`  
		Last Modified: Tue, 16 May 2023 01:41:46 GMT  
		Size: 252.5 MB (252523134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aa5b2cfcaaee2696bef62d280da0a68b762aa0c0eae563b386d61d563effb4`  
		Last Modified: Tue, 16 May 2023 01:41:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:2a6a1279dbefe704c75455ab745cee108d76d9a2928b59b1fb2f46dfaf0b1b6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:f10dcf5c7de2ebdf90dc2fe1c0c17359ad44d184c307c37945dbf6868c74c1bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343151242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d932427105199181dca9d9ad90a855f7e395ad62ca98042928922c4b4c833dbf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:00:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 01:02:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:02:29 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:02:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b009b5adbd509635590b8ca3f676b6641b7bb66ab0512ccd4066db76ca60f5`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b0f9dac5dfd8149acea5db9be04cf12e33419619851a19de0dc33268bc543`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b823ac6a3ceddc3171904f453472228f5ce941332ae1c4c3a97b62399cb8`  
		Last Modified: Tue, 18 Apr 2023 01:15:25 GMT  
		Size: 177.0 MB (177015888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d72917faacc696317190bddb87cec63b461b7bbb280990ed04a1ab40b01565a`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616856e05b972b9a1860c701a649c8178c883e876e7555fd8d7c2ffb639a3a82`  
		Last Modified: Tue, 18 Apr 2023 01:15:42 GMT  
		Size: 50.9 MB (50939692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d27b2bae79f36c6b903ae1427cbaf54e4dce26b1dfb7325ba73541b10d1525a`  
		Last Modified: Tue, 18 Apr 2023 01:15:34 GMT  
		Size: 297.1 KB (297147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d72adfba67c09bba7be116aa4cd34b1519f68648b3fa6f0afc7e5a92979a76c`  
		Last Modified: Tue, 18 Apr 2023 01:15:46 GMT  
		Size: 79.6 MB (79606798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:e67e92cb18c95bba379dfc18c80f8c0a74fd5fcca4a46385857196e5346af8ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289226398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ca36166d90654bd251fd79f47436a0366dfddb369712dd9d6245bf6f34d118`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:03:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:03:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:06:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:06:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:06:05 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:07:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ecaa4a720ffd8b3f56038a2d5f616807fa7485f551442c1f40ea8fd3981476`  
		Last Modified: Tue, 18 Apr 2023 02:16:19 GMT  
		Size: 1.2 MB (1157196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7945fb40cca95a4e5c72309573289c0784fb110e1606688d25f64849ca28139`  
		Last Modified: Tue, 18 Apr 2023 02:16:18 GMT  
		Size: 4.7 MB (4679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c069a57904ca9856ac4e9d5b220c3c4b98c50fded7cdd74e670f2338c3fb330`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b1cc4dc29f69e7392b245372d8097dcecebafe0667c8f2726299a4de8874fb`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dd47d037bb6cd6982d83524e76328da32499ff9d59f265b0ec7756a8a52072`  
		Last Modified: Tue, 18 Apr 2023 02:16:46 GMT  
		Size: 157.5 MB (157503873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f3aa8b76ccbcd8b349669fc88b8205c0cd0f8a4d1c858519ae07119f9e4879`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefc606d3dd23a8815fd1e238d5fdfe32080b4795073ba61cee804527816162a`  
		Last Modified: Tue, 18 Apr 2023 02:16:59 GMT  
		Size: 40.5 MB (40503298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc1f052e8af8e9f8ce3488131b6e3db7f4c91846dfc84d2f75688b69a04961`  
		Last Modified: Tue, 18 Apr 2023 02:16:54 GMT  
		Size: 297.1 KB (297142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb40216b8c1d941c1be2d7ab0be0dd7b2c40485ff30f2d5693e2c7bf59ee3f`  
		Last Modified: Tue, 18 Apr 2023 02:17:03 GMT  
		Size: 60.5 MB (60496479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d5ea21ddeb3a8263b55ff73a81ba0a53954362e89dbb5bc3070f7c55b5e8c6e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322836771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc8c46b2872805b8ba64f84218bf3b7ff59ec0c72e34a2e11a8be1df5048b440`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:06:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:09:00 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:09:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:09:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89011a19d825c31dd1ecdacfff5418ea066cc6c3d8b16aa5495409bae017b1f1`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf18013b664813b5e2ac52cbfde90f06a51486a530223919716ad97cb24c2a`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1809be61e23432d56e45874bfae781cc545d2889cf2d4a4ec837bbe62c12ae`  
		Last Modified: Tue, 18 Apr 2023 02:22:22 GMT  
		Size: 171.5 MB (171472211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29476e1a64f98957516be750445e8fe8dab41029f42b326871dad7c15a5002f4`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9778a01d5ceece6c4f0c2c0c02cc6f090ecb6a15e4ae5b1ae330ee94589a570`  
		Last Modified: Tue, 18 Apr 2023 02:22:36 GMT  
		Size: 45.2 MB (45203703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdd76f4f02f17a00aaef729800e659e052bf15f73a3a5e03cdb8c835a754761`  
		Last Modified: Tue, 18 Apr 2023 02:22:31 GMT  
		Size: 297.1 KB (297141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f09767fc16c06e81dd2dc318f6e7d1bb01562aefaaed477349db702168210`  
		Last Modified: Tue, 18 Apr 2023 02:22:38 GMT  
		Size: 72.0 MB (71974377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:4b97a026887ae7d73fc7e4103c2faef87668049746fedc35937b3b002aea9a27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:b2837b4b7e3f2989f814e7e6195088beb1a79dc1b3803991b8a9c6f9d6997407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.1 MB (835124849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a0ee0caaa8aa9a1db06fa9667d78d02c49ba07c23bc6dc0acbd574f25134e4a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:00:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 01:02:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:02:29 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:02:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:11:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b009b5adbd509635590b8ca3f676b6641b7bb66ab0512ccd4066db76ca60f5`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b0f9dac5dfd8149acea5db9be04cf12e33419619851a19de0dc33268bc543`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b823ac6a3ceddc3171904f453472228f5ce941332ae1c4c3a97b62399cb8`  
		Last Modified: Tue, 18 Apr 2023 01:15:25 GMT  
		Size: 177.0 MB (177015888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d72917faacc696317190bddb87cec63b461b7bbb280990ed04a1ab40b01565a`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616856e05b972b9a1860c701a649c8178c883e876e7555fd8d7c2ffb639a3a82`  
		Last Modified: Tue, 18 Apr 2023 01:15:42 GMT  
		Size: 50.9 MB (50939692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d27b2bae79f36c6b903ae1427cbaf54e4dce26b1dfb7325ba73541b10d1525a`  
		Last Modified: Tue, 18 Apr 2023 01:15:34 GMT  
		Size: 297.1 KB (297147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d72adfba67c09bba7be116aa4cd34b1519f68648b3fa6f0afc7e5a92979a76c`  
		Last Modified: Tue, 18 Apr 2023 01:15:46 GMT  
		Size: 79.6 MB (79606798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaa5a976970713e8541e12005180f8af73fca53a6bb8b427c8ef2e4e00bc81f`  
		Last Modified: Tue, 18 Apr 2023 01:17:16 GMT  
		Size: 492.0 MB (491973607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:f037e3e47c85b4fc8bb442b3c526d0b530e84dfc8eb4ff5900134ecd357c356e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.1 MB (726148964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e100fff8a6f92597a6ca93c3147e48f94276a436caf60f08e0805c4a4a0243`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:03:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:03:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:06:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:06:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:06:05 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:07:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:15:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ecaa4a720ffd8b3f56038a2d5f616807fa7485f551442c1f40ea8fd3981476`  
		Last Modified: Tue, 18 Apr 2023 02:16:19 GMT  
		Size: 1.2 MB (1157196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7945fb40cca95a4e5c72309573289c0784fb110e1606688d25f64849ca28139`  
		Last Modified: Tue, 18 Apr 2023 02:16:18 GMT  
		Size: 4.7 MB (4679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c069a57904ca9856ac4e9d5b220c3c4b98c50fded7cdd74e670f2338c3fb330`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b1cc4dc29f69e7392b245372d8097dcecebafe0667c8f2726299a4de8874fb`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dd47d037bb6cd6982d83524e76328da32499ff9d59f265b0ec7756a8a52072`  
		Last Modified: Tue, 18 Apr 2023 02:16:46 GMT  
		Size: 157.5 MB (157503873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f3aa8b76ccbcd8b349669fc88b8205c0cd0f8a4d1c858519ae07119f9e4879`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefc606d3dd23a8815fd1e238d5fdfe32080b4795073ba61cee804527816162a`  
		Last Modified: Tue, 18 Apr 2023 02:16:59 GMT  
		Size: 40.5 MB (40503298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc1f052e8af8e9f8ce3488131b6e3db7f4c91846dfc84d2f75688b69a04961`  
		Last Modified: Tue, 18 Apr 2023 02:16:54 GMT  
		Size: 297.1 KB (297142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb40216b8c1d941c1be2d7ab0be0dd7b2c40485ff30f2d5693e2c7bf59ee3f`  
		Last Modified: Tue, 18 Apr 2023 02:17:03 GMT  
		Size: 60.5 MB (60496479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f579db257587db087e82f98bae2bb40f55c3dc4005abb9d1e04d028bb83b9ed6`  
		Last Modified: Tue, 18 Apr 2023 02:18:21 GMT  
		Size: 436.9 MB (436922566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c3fc83f5e275c2110f57fb743ec1e4a13e7c31a58fd3f7c3453f28fccf94a5cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.4 MB (785400867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a3b0bdf0c4b2ba33d8bdd6837d2b95a127ca755c58352a2debdc4fc6bdcc610`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:06:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:09:00 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:09:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:09:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:18:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89011a19d825c31dd1ecdacfff5418ea066cc6c3d8b16aa5495409bae017b1f1`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf18013b664813b5e2ac52cbfde90f06a51486a530223919716ad97cb24c2a`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1809be61e23432d56e45874bfae781cc545d2889cf2d4a4ec837bbe62c12ae`  
		Last Modified: Tue, 18 Apr 2023 02:22:22 GMT  
		Size: 171.5 MB (171472211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29476e1a64f98957516be750445e8fe8dab41029f42b326871dad7c15a5002f4`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9778a01d5ceece6c4f0c2c0c02cc6f090ecb6a15e4ae5b1ae330ee94589a570`  
		Last Modified: Tue, 18 Apr 2023 02:22:36 GMT  
		Size: 45.2 MB (45203703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdd76f4f02f17a00aaef729800e659e052bf15f73a3a5e03cdb8c835a754761`  
		Last Modified: Tue, 18 Apr 2023 02:22:31 GMT  
		Size: 297.1 KB (297141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f09767fc16c06e81dd2dc318f6e7d1bb01562aefaaed477349db702168210`  
		Last Modified: Tue, 18 Apr 2023 02:22:38 GMT  
		Size: 72.0 MB (71974377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c74524ff9156cda41dfa59395623696ff70464d7d9ec721daa3a8370dfa20c`  
		Last Modified: Tue, 18 Apr 2023 02:23:47 GMT  
		Size: 462.6 MB (462564096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:f1ebbbe44b9c6c6ee1a5654b615bf057fa4af00fc876718e0299bb57f27be137
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:c7c280f7e68de331b55ddf821c5e3ce79b37c32fdb12677369b96c178f02319f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.3 MB (951330146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfeac76fe61436b0e1249188946fc7ddfbf07df3bd35d9fc74ef90088f7c5f28`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:07 GMT
ADD file:d176a72312205fc75b2950df98f4ed25abadd4b053b9d85bea67466a5b30220f in / 
# Tue, 02 May 2023 23:47:08 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:38:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:38:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 May 2023 21:38:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:38:39 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:38:39 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:38:39 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 May 2023 21:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:39:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 May 2023 21:39:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:40:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:40:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:40:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:41:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a94073ab46f8d565f5938cc345d32f7adda10a2585e39555079da9d4ee595974`  
		Last Modified: Tue, 02 May 2023 23:50:40 GMT  
		Size: 50.4 MB (50448697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6a520b96cab6be544c3de79dfbd2e79a43648778ff5ffc9cea03b9afea1a8a`  
		Last Modified: Wed, 03 May 2023 22:02:33 GMT  
		Size: 10.9 MB (10897025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b18fd569bd474fa851fd78f1d3bf2e9678d8423061fdd217c621a34a0e1a18`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b96262d8a19c986620307e5e5f5bc87d241ebddd343a22e317096193e83ca7`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba9b33e9316a950f2ca0db084e17331cca39064c3a3d10175a5732482915e1c`  
		Last Modified: Wed, 03 May 2023 22:03:02 GMT  
		Size: 239.3 MB (239262397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f679b704b1a974ebf77923991309e3935a8e4e5950043f8e8df9817cb566018`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0114f4c6a2082f6e76098833ebdf4262123ac4a571969bf9e9e38f3b7160e730`  
		Last Modified: Wed, 03 May 2023 22:03:20 GMT  
		Size: 86.6 MB (86625207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1570d96e90fa78b5cc55358c3d0cce3f912d1c9ce9118a0c94901ba67a8a2ab`  
		Last Modified: Wed, 03 May 2023 22:03:09 GMT  
		Size: 293.2 KB (293249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f61e4fbe9210080b697fa8cf61250a48a94b4b6784227406fff9b625ad3878`  
		Last Modified: Wed, 03 May 2023 22:03:18 GMT  
		Size: 76.0 MB (75978108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcbf959d17ccd4828027535976e0f0a26d465b40373f851ca0ac7326eec0090`  
		Last Modified: Wed, 03 May 2023 22:04:41 GMT  
		Size: 487.8 MB (487823052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ec23922d0787f090589e69579d1d3088d1774da7fe2f86fade0da06b70d72878
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **868.1 MB (868118719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812361257ce265e2135af64173d0f1644277c0776e06fcc1fdeff4454a1c617e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:22:56 GMT
ADD file:6042e29dcf5e22439cd69873d8960f8d3977abe915ef462aaa84368a7186a3bf in / 
# Wed, 03 May 2023 00:22:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:32:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:32:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 May 2023 18:32:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:32:32 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:32:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:32:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 May 2023 18:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:33:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 May 2023 18:33:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:33:54 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:34:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:34:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:35:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:39:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7c5fe8e0ac53c77142bf16686fc01d0d2b1fb2da7be5414cdf2f224ec485592`  
		Last Modified: Wed, 03 May 2023 00:26:10 GMT  
		Size: 49.2 MB (49238630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f4b1b3aff79daeba459c24d6625912443a9c4b6e072fd443df8cf1fe609a3b`  
		Last Modified: Wed, 03 May 2023 18:59:14 GMT  
		Size: 10.9 MB (10902746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bd0f1f3ef8032558026a60ca367a9d7b0a28a5d5656befe67922b145ce30bf`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ffa192fc268fe17d966f4b3cea0d44a2889b03c6266a5d26e16c239241f65e`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66412823f7f9778ca86e89b006f993392e02d4dcf6d72bececff2961ab62e97`  
		Last Modified: Wed, 03 May 2023 18:59:49 GMT  
		Size: 184.5 MB (184456335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220fcae6736a0fef7e49e980a9743d78ac71f0793d181838e243ca8df2e17b7`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb95d7c1cbf0d06fe344363abab7d53bcf3e9530c86b6b5d15445e3456dc5f`  
		Last Modified: Wed, 03 May 2023 19:00:03 GMT  
		Size: 84.4 MB (84396518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35bfb55f24afd444091072d43309bdde850dfe001b51461b00b1341cd892783`  
		Last Modified: Wed, 03 May 2023 18:59:55 GMT  
		Size: 292.5 KB (292488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9887f28731774c4b067f23703dec47affd41340f5bf051055b087050dff54a`  
		Last Modified: Wed, 03 May 2023 19:00:04 GMT  
		Size: 74.1 MB (74090649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8217fb14e9a1c962bf9d63368d2bb4367d0bc08df13d48652aeb6ba86dbf83`  
		Last Modified: Wed, 03 May 2023 19:01:14 GMT  
		Size: 464.7 MB (464738941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:4b97a026887ae7d73fc7e4103c2faef87668049746fedc35937b3b002aea9a27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:b2837b4b7e3f2989f814e7e6195088beb1a79dc1b3803991b8a9c6f9d6997407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.1 MB (835124849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a0ee0caaa8aa9a1db06fa9667d78d02c49ba07c23bc6dc0acbd574f25134e4a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:00:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 01:02:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:02:29 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:02:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:11:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b009b5adbd509635590b8ca3f676b6641b7bb66ab0512ccd4066db76ca60f5`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b0f9dac5dfd8149acea5db9be04cf12e33419619851a19de0dc33268bc543`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b823ac6a3ceddc3171904f453472228f5ce941332ae1c4c3a97b62399cb8`  
		Last Modified: Tue, 18 Apr 2023 01:15:25 GMT  
		Size: 177.0 MB (177015888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d72917faacc696317190bddb87cec63b461b7bbb280990ed04a1ab40b01565a`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616856e05b972b9a1860c701a649c8178c883e876e7555fd8d7c2ffb639a3a82`  
		Last Modified: Tue, 18 Apr 2023 01:15:42 GMT  
		Size: 50.9 MB (50939692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d27b2bae79f36c6b903ae1427cbaf54e4dce26b1dfb7325ba73541b10d1525a`  
		Last Modified: Tue, 18 Apr 2023 01:15:34 GMT  
		Size: 297.1 KB (297147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d72adfba67c09bba7be116aa4cd34b1519f68648b3fa6f0afc7e5a92979a76c`  
		Last Modified: Tue, 18 Apr 2023 01:15:46 GMT  
		Size: 79.6 MB (79606798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaa5a976970713e8541e12005180f8af73fca53a6bb8b427c8ef2e4e00bc81f`  
		Last Modified: Tue, 18 Apr 2023 01:17:16 GMT  
		Size: 492.0 MB (491973607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:f037e3e47c85b4fc8bb442b3c526d0b530e84dfc8eb4ff5900134ecd357c356e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.1 MB (726148964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e100fff8a6f92597a6ca93c3147e48f94276a436caf60f08e0805c4a4a0243`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:03:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:03:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:06:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:06:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:06:05 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:07:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:15:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ecaa4a720ffd8b3f56038a2d5f616807fa7485f551442c1f40ea8fd3981476`  
		Last Modified: Tue, 18 Apr 2023 02:16:19 GMT  
		Size: 1.2 MB (1157196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7945fb40cca95a4e5c72309573289c0784fb110e1606688d25f64849ca28139`  
		Last Modified: Tue, 18 Apr 2023 02:16:18 GMT  
		Size: 4.7 MB (4679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c069a57904ca9856ac4e9d5b220c3c4b98c50fded7cdd74e670f2338c3fb330`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b1cc4dc29f69e7392b245372d8097dcecebafe0667c8f2726299a4de8874fb`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dd47d037bb6cd6982d83524e76328da32499ff9d59f265b0ec7756a8a52072`  
		Last Modified: Tue, 18 Apr 2023 02:16:46 GMT  
		Size: 157.5 MB (157503873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f3aa8b76ccbcd8b349669fc88b8205c0cd0f8a4d1c858519ae07119f9e4879`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefc606d3dd23a8815fd1e238d5fdfe32080b4795073ba61cee804527816162a`  
		Last Modified: Tue, 18 Apr 2023 02:16:59 GMT  
		Size: 40.5 MB (40503298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc1f052e8af8e9f8ce3488131b6e3db7f4c91846dfc84d2f75688b69a04961`  
		Last Modified: Tue, 18 Apr 2023 02:16:54 GMT  
		Size: 297.1 KB (297142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb40216b8c1d941c1be2d7ab0be0dd7b2c40485ff30f2d5693e2c7bf59ee3f`  
		Last Modified: Tue, 18 Apr 2023 02:17:03 GMT  
		Size: 60.5 MB (60496479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f579db257587db087e82f98bae2bb40f55c3dc4005abb9d1e04d028bb83b9ed6`  
		Last Modified: Tue, 18 Apr 2023 02:18:21 GMT  
		Size: 436.9 MB (436922566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c3fc83f5e275c2110f57fb743ec1e4a13e7c31a58fd3f7c3453f28fccf94a5cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.4 MB (785400867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a3b0bdf0c4b2ba33d8bdd6837d2b95a127ca755c58352a2debdc4fc6bdcc610`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:06:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:09:00 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:09:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:09:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:18:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89011a19d825c31dd1ecdacfff5418ea066cc6c3d8b16aa5495409bae017b1f1`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf18013b664813b5e2ac52cbfde90f06a51486a530223919716ad97cb24c2a`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1809be61e23432d56e45874bfae781cc545d2889cf2d4a4ec837bbe62c12ae`  
		Last Modified: Tue, 18 Apr 2023 02:22:22 GMT  
		Size: 171.5 MB (171472211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29476e1a64f98957516be750445e8fe8dab41029f42b326871dad7c15a5002f4`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9778a01d5ceece6c4f0c2c0c02cc6f090ecb6a15e4ae5b1ae330ee94589a570`  
		Last Modified: Tue, 18 Apr 2023 02:22:36 GMT  
		Size: 45.2 MB (45203703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdd76f4f02f17a00aaef729800e659e052bf15f73a3a5e03cdb8c835a754761`  
		Last Modified: Tue, 18 Apr 2023 02:22:31 GMT  
		Size: 297.1 KB (297141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f09767fc16c06e81dd2dc318f6e7d1bb01562aefaaed477349db702168210`  
		Last Modified: Tue, 18 Apr 2023 02:22:38 GMT  
		Size: 72.0 MB (71974377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c74524ff9156cda41dfa59395623696ff70464d7d9ec721daa3a8370dfa20c`  
		Last Modified: Tue, 18 Apr 2023 02:23:47 GMT  
		Size: 462.6 MB (462564096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:d6151a7afe8a57524b5cec40f482f543c2c7849b66546f55adebc0d469daa740
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:b870378b8c25331554c06f288ae4fba67daf1f000430925e54236f2a567a95c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359013481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4154fe3a7c025c85bc3b7a5aff2f57b233f928cbbb1c40e1a24f8c459c5e28cc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:00:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 01:02:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:02:29 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:02:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:05:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b009b5adbd509635590b8ca3f676b6641b7bb66ab0512ccd4066db76ca60f5`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b0f9dac5dfd8149acea5db9be04cf12e33419619851a19de0dc33268bc543`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b823ac6a3ceddc3171904f453472228f5ce941332ae1c4c3a97b62399cb8`  
		Last Modified: Tue, 18 Apr 2023 01:15:25 GMT  
		Size: 177.0 MB (177015888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d72917faacc696317190bddb87cec63b461b7bbb280990ed04a1ab40b01565a`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616856e05b972b9a1860c701a649c8178c883e876e7555fd8d7c2ffb639a3a82`  
		Last Modified: Tue, 18 Apr 2023 01:15:42 GMT  
		Size: 50.9 MB (50939692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d27b2bae79f36c6b903ae1427cbaf54e4dce26b1dfb7325ba73541b10d1525a`  
		Last Modified: Tue, 18 Apr 2023 01:15:34 GMT  
		Size: 297.1 KB (297147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d72adfba67c09bba7be116aa4cd34b1519f68648b3fa6f0afc7e5a92979a76c`  
		Last Modified: Tue, 18 Apr 2023 01:15:46 GMT  
		Size: 79.6 MB (79606798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4a7a8934c82957b2c04f5902cf859844e400249d00c9c7e16ef710f21a96ee`  
		Last Modified: Tue, 18 Apr 2023 01:15:59 GMT  
		Size: 15.9 MB (15862239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:9afe7fd54704e4fab8c74675eee8266f47da3c843cf6590848db581c33c67fc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303293268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d25a309160b3642cc318ef185b2c1caa75ae3f205e2f294a26faae78aabbc0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:03:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:03:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:06:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:06:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:06:05 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:07:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ecaa4a720ffd8b3f56038a2d5f616807fa7485f551442c1f40ea8fd3981476`  
		Last Modified: Tue, 18 Apr 2023 02:16:19 GMT  
		Size: 1.2 MB (1157196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7945fb40cca95a4e5c72309573289c0784fb110e1606688d25f64849ca28139`  
		Last Modified: Tue, 18 Apr 2023 02:16:18 GMT  
		Size: 4.7 MB (4679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c069a57904ca9856ac4e9d5b220c3c4b98c50fded7cdd74e670f2338c3fb330`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b1cc4dc29f69e7392b245372d8097dcecebafe0667c8f2726299a4de8874fb`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dd47d037bb6cd6982d83524e76328da32499ff9d59f265b0ec7756a8a52072`  
		Last Modified: Tue, 18 Apr 2023 02:16:46 GMT  
		Size: 157.5 MB (157503873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f3aa8b76ccbcd8b349669fc88b8205c0cd0f8a4d1c858519ae07119f9e4879`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefc606d3dd23a8815fd1e238d5fdfe32080b4795073ba61cee804527816162a`  
		Last Modified: Tue, 18 Apr 2023 02:16:59 GMT  
		Size: 40.5 MB (40503298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc1f052e8af8e9f8ce3488131b6e3db7f4c91846dfc84d2f75688b69a04961`  
		Last Modified: Tue, 18 Apr 2023 02:16:54 GMT  
		Size: 297.1 KB (297142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb40216b8c1d941c1be2d7ab0be0dd7b2c40485ff30f2d5693e2c7bf59ee3f`  
		Last Modified: Tue, 18 Apr 2023 02:17:03 GMT  
		Size: 60.5 MB (60496479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bed6a6252a7416a7ffbfa6b7387dddc1c4388e44497b0806437a326a6295d87`  
		Last Modified: Tue, 18 Apr 2023 02:17:15 GMT  
		Size: 14.1 MB (14066870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2533f69247833764ddf7afe4f4b5770c9971b5019b470c911984e636b0eb80f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338295210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c9e708cb7b236b8280bc2e38de11314a901ffc5f631038fc3baa6b87df7d70`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:06:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:09:00 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:09:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:09:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:11:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89011a19d825c31dd1ecdacfff5418ea066cc6c3d8b16aa5495409bae017b1f1`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf18013b664813b5e2ac52cbfde90f06a51486a530223919716ad97cb24c2a`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1809be61e23432d56e45874bfae781cc545d2889cf2d4a4ec837bbe62c12ae`  
		Last Modified: Tue, 18 Apr 2023 02:22:22 GMT  
		Size: 171.5 MB (171472211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29476e1a64f98957516be750445e8fe8dab41029f42b326871dad7c15a5002f4`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9778a01d5ceece6c4f0c2c0c02cc6f090ecb6a15e4ae5b1ae330ee94589a570`  
		Last Modified: Tue, 18 Apr 2023 02:22:36 GMT  
		Size: 45.2 MB (45203703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdd76f4f02f17a00aaef729800e659e052bf15f73a3a5e03cdb8c835a754761`  
		Last Modified: Tue, 18 Apr 2023 02:22:31 GMT  
		Size: 297.1 KB (297141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f09767fc16c06e81dd2dc318f6e7d1bb01562aefaaed477349db702168210`  
		Last Modified: Tue, 18 Apr 2023 02:22:38 GMT  
		Size: 72.0 MB (71974377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aca94dfd1aa81009c8bae0863333e2be4a9b32f240850a23ccb3a28917a43d`  
		Last Modified: Tue, 18 Apr 2023 02:22:52 GMT  
		Size: 15.5 MB (15458439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:d0d68d43cbeb429719e95cff034f0fb27a23fdd8025b28cf530de55e5c9e77f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:b1db5de3c20d2e22ead61a7bf5d3c7a2e0bd17c3a51dfb3ad5e79abb064237e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.7 MB (484664045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e7c8b36b79c9686088bb1bb19f60151e21b53fd8dd31676eb5537c06fe5071`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:07 GMT
ADD file:d176a72312205fc75b2950df98f4ed25abadd4b053b9d85bea67466a5b30220f in / 
# Tue, 02 May 2023 23:47:08 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:38:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:38:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 May 2023 21:38:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:38:39 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:38:39 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:38:39 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 May 2023 21:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:39:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 May 2023 21:39:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:40:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:40:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:40:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:41:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:41:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a94073ab46f8d565f5938cc345d32f7adda10a2585e39555079da9d4ee595974`  
		Last Modified: Tue, 02 May 2023 23:50:40 GMT  
		Size: 50.4 MB (50448697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6a520b96cab6be544c3de79dfbd2e79a43648778ff5ffc9cea03b9afea1a8a`  
		Last Modified: Wed, 03 May 2023 22:02:33 GMT  
		Size: 10.9 MB (10897025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b18fd569bd474fa851fd78f1d3bf2e9678d8423061fdd217c621a34a0e1a18`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b96262d8a19c986620307e5e5f5bc87d241ebddd343a22e317096193e83ca7`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba9b33e9316a950f2ca0db084e17331cca39064c3a3d10175a5732482915e1c`  
		Last Modified: Wed, 03 May 2023 22:03:02 GMT  
		Size: 239.3 MB (239262397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f679b704b1a974ebf77923991309e3935a8e4e5950043f8e8df9817cb566018`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0114f4c6a2082f6e76098833ebdf4262123ac4a571969bf9e9e38f3b7160e730`  
		Last Modified: Wed, 03 May 2023 22:03:20 GMT  
		Size: 86.6 MB (86625207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1570d96e90fa78b5cc55358c3d0cce3f912d1c9ce9118a0c94901ba67a8a2ab`  
		Last Modified: Wed, 03 May 2023 22:03:09 GMT  
		Size: 293.2 KB (293249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f61e4fbe9210080b697fa8cf61250a48a94b4b6784227406fff9b625ad3878`  
		Last Modified: Wed, 03 May 2023 22:03:18 GMT  
		Size: 76.0 MB (75978108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970cf90ffb56b90e32ca3b5e62c8d081c47000f6ef2addf1ff37158692e7438c`  
		Last Modified: Wed, 03 May 2023 22:03:28 GMT  
		Size: 21.2 MB (21156951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:62b331583d881703aa3722cb01832e369827a54ed42d0f5644eeb624ed7bfadd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.2 MB (424200671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:384665c219d79e6d596ff456bd49b0074781ec6579ff636272c9b64aac094356`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:22:56 GMT
ADD file:6042e29dcf5e22439cd69873d8960f8d3977abe915ef462aaa84368a7186a3bf in / 
# Wed, 03 May 2023 00:22:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:32:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:32:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 May 2023 18:32:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:32:32 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:32:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:32:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 May 2023 18:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:33:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 May 2023 18:33:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:33:54 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:34:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:34:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:35:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:35:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7c5fe8e0ac53c77142bf16686fc01d0d2b1fb2da7be5414cdf2f224ec485592`  
		Last Modified: Wed, 03 May 2023 00:26:10 GMT  
		Size: 49.2 MB (49238630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f4b1b3aff79daeba459c24d6625912443a9c4b6e072fd443df8cf1fe609a3b`  
		Last Modified: Wed, 03 May 2023 18:59:14 GMT  
		Size: 10.9 MB (10902746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bd0f1f3ef8032558026a60ca367a9d7b0a28a5d5656befe67922b145ce30bf`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ffa192fc268fe17d966f4b3cea0d44a2889b03c6266a5d26e16c239241f65e`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66412823f7f9778ca86e89b006f993392e02d4dcf6d72bececff2961ab62e97`  
		Last Modified: Wed, 03 May 2023 18:59:49 GMT  
		Size: 184.5 MB (184456335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220fcae6736a0fef7e49e980a9743d78ac71f0793d181838e243ca8df2e17b7`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb95d7c1cbf0d06fe344363abab7d53bcf3e9530c86b6b5d15445e3456dc5f`  
		Last Modified: Wed, 03 May 2023 19:00:03 GMT  
		Size: 84.4 MB (84396518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35bfb55f24afd444091072d43309bdde850dfe001b51461b00b1341cd892783`  
		Last Modified: Wed, 03 May 2023 18:59:55 GMT  
		Size: 292.5 KB (292488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9887f28731774c4b067f23703dec47affd41340f5bf051055b087050dff54a`  
		Last Modified: Wed, 03 May 2023 19:00:04 GMT  
		Size: 74.1 MB (74090649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b56d67b24627b9c34d7c74e4216c7df0077cb8e6fddbee61d2b611db7cc6652`  
		Last Modified: Wed, 03 May 2023 19:00:16 GMT  
		Size: 20.8 MB (20820893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:d6151a7afe8a57524b5cec40f482f543c2c7849b66546f55adebc0d469daa740
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:b870378b8c25331554c06f288ae4fba67daf1f000430925e54236f2a567a95c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359013481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4154fe3a7c025c85bc3b7a5aff2f57b233f928cbbb1c40e1a24f8c459c5e28cc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:00:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 01:02:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:02:29 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:02:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:05:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b009b5adbd509635590b8ca3f676b6641b7bb66ab0512ccd4066db76ca60f5`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b0f9dac5dfd8149acea5db9be04cf12e33419619851a19de0dc33268bc543`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b823ac6a3ceddc3171904f453472228f5ce941332ae1c4c3a97b62399cb8`  
		Last Modified: Tue, 18 Apr 2023 01:15:25 GMT  
		Size: 177.0 MB (177015888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d72917faacc696317190bddb87cec63b461b7bbb280990ed04a1ab40b01565a`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616856e05b972b9a1860c701a649c8178c883e876e7555fd8d7c2ffb639a3a82`  
		Last Modified: Tue, 18 Apr 2023 01:15:42 GMT  
		Size: 50.9 MB (50939692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d27b2bae79f36c6b903ae1427cbaf54e4dce26b1dfb7325ba73541b10d1525a`  
		Last Modified: Tue, 18 Apr 2023 01:15:34 GMT  
		Size: 297.1 KB (297147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d72adfba67c09bba7be116aa4cd34b1519f68648b3fa6f0afc7e5a92979a76c`  
		Last Modified: Tue, 18 Apr 2023 01:15:46 GMT  
		Size: 79.6 MB (79606798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4a7a8934c82957b2c04f5902cf859844e400249d00c9c7e16ef710f21a96ee`  
		Last Modified: Tue, 18 Apr 2023 01:15:59 GMT  
		Size: 15.9 MB (15862239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:9afe7fd54704e4fab8c74675eee8266f47da3c843cf6590848db581c33c67fc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303293268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d25a309160b3642cc318ef185b2c1caa75ae3f205e2f294a26faae78aabbc0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:03:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:03:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:06:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:06:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:06:05 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:07:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ecaa4a720ffd8b3f56038a2d5f616807fa7485f551442c1f40ea8fd3981476`  
		Last Modified: Tue, 18 Apr 2023 02:16:19 GMT  
		Size: 1.2 MB (1157196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7945fb40cca95a4e5c72309573289c0784fb110e1606688d25f64849ca28139`  
		Last Modified: Tue, 18 Apr 2023 02:16:18 GMT  
		Size: 4.7 MB (4679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c069a57904ca9856ac4e9d5b220c3c4b98c50fded7cdd74e670f2338c3fb330`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b1cc4dc29f69e7392b245372d8097dcecebafe0667c8f2726299a4de8874fb`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dd47d037bb6cd6982d83524e76328da32499ff9d59f265b0ec7756a8a52072`  
		Last Modified: Tue, 18 Apr 2023 02:16:46 GMT  
		Size: 157.5 MB (157503873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f3aa8b76ccbcd8b349669fc88b8205c0cd0f8a4d1c858519ae07119f9e4879`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefc606d3dd23a8815fd1e238d5fdfe32080b4795073ba61cee804527816162a`  
		Last Modified: Tue, 18 Apr 2023 02:16:59 GMT  
		Size: 40.5 MB (40503298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc1f052e8af8e9f8ce3488131b6e3db7f4c91846dfc84d2f75688b69a04961`  
		Last Modified: Tue, 18 Apr 2023 02:16:54 GMT  
		Size: 297.1 KB (297142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb40216b8c1d941c1be2d7ab0be0dd7b2c40485ff30f2d5693e2c7bf59ee3f`  
		Last Modified: Tue, 18 Apr 2023 02:17:03 GMT  
		Size: 60.5 MB (60496479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bed6a6252a7416a7ffbfa6b7387dddc1c4388e44497b0806437a326a6295d87`  
		Last Modified: Tue, 18 Apr 2023 02:17:15 GMT  
		Size: 14.1 MB (14066870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2533f69247833764ddf7afe4f4b5770c9971b5019b470c911984e636b0eb80f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338295210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c9e708cb7b236b8280bc2e38de11314a901ffc5f631038fc3baa6b87df7d70`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:06:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:09:00 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:09:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:09:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:11:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89011a19d825c31dd1ecdacfff5418ea066cc6c3d8b16aa5495409bae017b1f1`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf18013b664813b5e2ac52cbfde90f06a51486a530223919716ad97cb24c2a`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1809be61e23432d56e45874bfae781cc545d2889cf2d4a4ec837bbe62c12ae`  
		Last Modified: Tue, 18 Apr 2023 02:22:22 GMT  
		Size: 171.5 MB (171472211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29476e1a64f98957516be750445e8fe8dab41029f42b326871dad7c15a5002f4`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9778a01d5ceece6c4f0c2c0c02cc6f090ecb6a15e4ae5b1ae330ee94589a570`  
		Last Modified: Tue, 18 Apr 2023 02:22:36 GMT  
		Size: 45.2 MB (45203703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdd76f4f02f17a00aaef729800e659e052bf15f73a3a5e03cdb8c835a754761`  
		Last Modified: Tue, 18 Apr 2023 02:22:31 GMT  
		Size: 297.1 KB (297141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f09767fc16c06e81dd2dc318f6e7d1bb01562aefaaed477349db702168210`  
		Last Modified: Tue, 18 Apr 2023 02:22:38 GMT  
		Size: 72.0 MB (71974377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aca94dfd1aa81009c8bae0863333e2be4a9b32f240850a23ccb3a28917a43d`  
		Last Modified: Tue, 18 Apr 2023 02:22:52 GMT  
		Size: 15.5 MB (15458439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:2a6a1279dbefe704c75455ab745cee108d76d9a2928b59b1fb2f46dfaf0b1b6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:f10dcf5c7de2ebdf90dc2fe1c0c17359ad44d184c307c37945dbf6868c74c1bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343151242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d932427105199181dca9d9ad90a855f7e395ad62ca98042928922c4b4c833dbf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:00:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 01:02:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:02:29 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:02:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b009b5adbd509635590b8ca3f676b6641b7bb66ab0512ccd4066db76ca60f5`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b0f9dac5dfd8149acea5db9be04cf12e33419619851a19de0dc33268bc543`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b823ac6a3ceddc3171904f453472228f5ce941332ae1c4c3a97b62399cb8`  
		Last Modified: Tue, 18 Apr 2023 01:15:25 GMT  
		Size: 177.0 MB (177015888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d72917faacc696317190bddb87cec63b461b7bbb280990ed04a1ab40b01565a`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616856e05b972b9a1860c701a649c8178c883e876e7555fd8d7c2ffb639a3a82`  
		Last Modified: Tue, 18 Apr 2023 01:15:42 GMT  
		Size: 50.9 MB (50939692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d27b2bae79f36c6b903ae1427cbaf54e4dce26b1dfb7325ba73541b10d1525a`  
		Last Modified: Tue, 18 Apr 2023 01:15:34 GMT  
		Size: 297.1 KB (297147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d72adfba67c09bba7be116aa4cd34b1519f68648b3fa6f0afc7e5a92979a76c`  
		Last Modified: Tue, 18 Apr 2023 01:15:46 GMT  
		Size: 79.6 MB (79606798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:e67e92cb18c95bba379dfc18c80f8c0a74fd5fcca4a46385857196e5346af8ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289226398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ca36166d90654bd251fd79f47436a0366dfddb369712dd9d6245bf6f34d118`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:03:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:03:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:06:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:06:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:06:05 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:07:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ecaa4a720ffd8b3f56038a2d5f616807fa7485f551442c1f40ea8fd3981476`  
		Last Modified: Tue, 18 Apr 2023 02:16:19 GMT  
		Size: 1.2 MB (1157196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7945fb40cca95a4e5c72309573289c0784fb110e1606688d25f64849ca28139`  
		Last Modified: Tue, 18 Apr 2023 02:16:18 GMT  
		Size: 4.7 MB (4679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c069a57904ca9856ac4e9d5b220c3c4b98c50fded7cdd74e670f2338c3fb330`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b1cc4dc29f69e7392b245372d8097dcecebafe0667c8f2726299a4de8874fb`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dd47d037bb6cd6982d83524e76328da32499ff9d59f265b0ec7756a8a52072`  
		Last Modified: Tue, 18 Apr 2023 02:16:46 GMT  
		Size: 157.5 MB (157503873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f3aa8b76ccbcd8b349669fc88b8205c0cd0f8a4d1c858519ae07119f9e4879`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefc606d3dd23a8815fd1e238d5fdfe32080b4795073ba61cee804527816162a`  
		Last Modified: Tue, 18 Apr 2023 02:16:59 GMT  
		Size: 40.5 MB (40503298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc1f052e8af8e9f8ce3488131b6e3db7f4c91846dfc84d2f75688b69a04961`  
		Last Modified: Tue, 18 Apr 2023 02:16:54 GMT  
		Size: 297.1 KB (297142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb40216b8c1d941c1be2d7ab0be0dd7b2c40485ff30f2d5693e2c7bf59ee3f`  
		Last Modified: Tue, 18 Apr 2023 02:17:03 GMT  
		Size: 60.5 MB (60496479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d5ea21ddeb3a8263b55ff73a81ba0a53954362e89dbb5bc3070f7c55b5e8c6e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322836771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc8c46b2872805b8ba64f84218bf3b7ff59ec0c72e34a2e11a8be1df5048b440`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:06:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:09:00 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:09:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:09:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89011a19d825c31dd1ecdacfff5418ea066cc6c3d8b16aa5495409bae017b1f1`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf18013b664813b5e2ac52cbfde90f06a51486a530223919716ad97cb24c2a`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1809be61e23432d56e45874bfae781cc545d2889cf2d4a4ec837bbe62c12ae`  
		Last Modified: Tue, 18 Apr 2023 02:22:22 GMT  
		Size: 171.5 MB (171472211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29476e1a64f98957516be750445e8fe8dab41029f42b326871dad7c15a5002f4`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9778a01d5ceece6c4f0c2c0c02cc6f090ecb6a15e4ae5b1ae330ee94589a570`  
		Last Modified: Tue, 18 Apr 2023 02:22:36 GMT  
		Size: 45.2 MB (45203703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdd76f4f02f17a00aaef729800e659e052bf15f73a3a5e03cdb8c835a754761`  
		Last Modified: Tue, 18 Apr 2023 02:22:31 GMT  
		Size: 297.1 KB (297141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f09767fc16c06e81dd2dc318f6e7d1bb01562aefaaed477349db702168210`  
		Last Modified: Tue, 18 Apr 2023 02:22:38 GMT  
		Size: 72.0 MB (71974377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:823d6b83834d90f32dd2babe4f4216b8d40f41248337aff393e7087a78d84d26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:de19486f3039e22310211e49c6beda02acbf917c1b3e0bf729ae7e6890dd3ea7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.5 MB (463507094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:073a64a265c273c9567378fdd9d9d48177b572100f49fa09faa2aae504f12156`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:07 GMT
ADD file:d176a72312205fc75b2950df98f4ed25abadd4b053b9d85bea67466a5b30220f in / 
# Tue, 02 May 2023 23:47:08 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:38:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:38:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 May 2023 21:38:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:38:39 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:38:39 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:38:39 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 May 2023 21:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:39:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 May 2023 21:39:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:40:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:40:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:40:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:41:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a94073ab46f8d565f5938cc345d32f7adda10a2585e39555079da9d4ee595974`  
		Last Modified: Tue, 02 May 2023 23:50:40 GMT  
		Size: 50.4 MB (50448697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6a520b96cab6be544c3de79dfbd2e79a43648778ff5ffc9cea03b9afea1a8a`  
		Last Modified: Wed, 03 May 2023 22:02:33 GMT  
		Size: 10.9 MB (10897025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b18fd569bd474fa851fd78f1d3bf2e9678d8423061fdd217c621a34a0e1a18`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b96262d8a19c986620307e5e5f5bc87d241ebddd343a22e317096193e83ca7`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba9b33e9316a950f2ca0db084e17331cca39064c3a3d10175a5732482915e1c`  
		Last Modified: Wed, 03 May 2023 22:03:02 GMT  
		Size: 239.3 MB (239262397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f679b704b1a974ebf77923991309e3935a8e4e5950043f8e8df9817cb566018`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0114f4c6a2082f6e76098833ebdf4262123ac4a571969bf9e9e38f3b7160e730`  
		Last Modified: Wed, 03 May 2023 22:03:20 GMT  
		Size: 86.6 MB (86625207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1570d96e90fa78b5cc55358c3d0cce3f912d1c9ce9118a0c94901ba67a8a2ab`  
		Last Modified: Wed, 03 May 2023 22:03:09 GMT  
		Size: 293.2 KB (293249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f61e4fbe9210080b697fa8cf61250a48a94b4b6784227406fff9b625ad3878`  
		Last Modified: Wed, 03 May 2023 22:03:18 GMT  
		Size: 76.0 MB (75978108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d2495f169f9a49c28103ae740395c5a9ede13a65dfb1e0ff3739fd144d4afa4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.4 MB (403379778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83f24aa8b579c354d9947b9b827b33bfe3b392b0fbe3b825dce53b692072e775`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:22:56 GMT
ADD file:6042e29dcf5e22439cd69873d8960f8d3977abe915ef462aaa84368a7186a3bf in / 
# Wed, 03 May 2023 00:22:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:32:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:32:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 May 2023 18:32:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:32:32 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:32:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:32:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 May 2023 18:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:33:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 May 2023 18:33:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:33:54 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:34:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:34:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:35:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7c5fe8e0ac53c77142bf16686fc01d0d2b1fb2da7be5414cdf2f224ec485592`  
		Last Modified: Wed, 03 May 2023 00:26:10 GMT  
		Size: 49.2 MB (49238630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f4b1b3aff79daeba459c24d6625912443a9c4b6e072fd443df8cf1fe609a3b`  
		Last Modified: Wed, 03 May 2023 18:59:14 GMT  
		Size: 10.9 MB (10902746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bd0f1f3ef8032558026a60ca367a9d7b0a28a5d5656befe67922b145ce30bf`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ffa192fc268fe17d966f4b3cea0d44a2889b03c6266a5d26e16c239241f65e`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66412823f7f9778ca86e89b006f993392e02d4dcf6d72bececff2961ab62e97`  
		Last Modified: Wed, 03 May 2023 18:59:49 GMT  
		Size: 184.5 MB (184456335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220fcae6736a0fef7e49e980a9743d78ac71f0793d181838e243ca8df2e17b7`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb95d7c1cbf0d06fe344363abab7d53bcf3e9530c86b6b5d15445e3456dc5f`  
		Last Modified: Wed, 03 May 2023 19:00:03 GMT  
		Size: 84.4 MB (84396518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35bfb55f24afd444091072d43309bdde850dfe001b51461b00b1341cd892783`  
		Last Modified: Wed, 03 May 2023 18:59:55 GMT  
		Size: 292.5 KB (292488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9887f28731774c4b067f23703dec47affd41340f5bf051055b087050dff54a`  
		Last Modified: Wed, 03 May 2023 19:00:04 GMT  
		Size: 74.1 MB (74090649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:2a6a1279dbefe704c75455ab745cee108d76d9a2928b59b1fb2f46dfaf0b1b6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:f10dcf5c7de2ebdf90dc2fe1c0c17359ad44d184c307c37945dbf6868c74c1bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343151242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d932427105199181dca9d9ad90a855f7e395ad62ca98042928922c4b4c833dbf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:00:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 01:02:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:02:29 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:02:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b009b5adbd509635590b8ca3f676b6641b7bb66ab0512ccd4066db76ca60f5`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b0f9dac5dfd8149acea5db9be04cf12e33419619851a19de0dc33268bc543`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b823ac6a3ceddc3171904f453472228f5ce941332ae1c4c3a97b62399cb8`  
		Last Modified: Tue, 18 Apr 2023 01:15:25 GMT  
		Size: 177.0 MB (177015888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d72917faacc696317190bddb87cec63b461b7bbb280990ed04a1ab40b01565a`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616856e05b972b9a1860c701a649c8178c883e876e7555fd8d7c2ffb639a3a82`  
		Last Modified: Tue, 18 Apr 2023 01:15:42 GMT  
		Size: 50.9 MB (50939692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d27b2bae79f36c6b903ae1427cbaf54e4dce26b1dfb7325ba73541b10d1525a`  
		Last Modified: Tue, 18 Apr 2023 01:15:34 GMT  
		Size: 297.1 KB (297147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d72adfba67c09bba7be116aa4cd34b1519f68648b3fa6f0afc7e5a92979a76c`  
		Last Modified: Tue, 18 Apr 2023 01:15:46 GMT  
		Size: 79.6 MB (79606798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:e67e92cb18c95bba379dfc18c80f8c0a74fd5fcca4a46385857196e5346af8ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289226398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ca36166d90654bd251fd79f47436a0366dfddb369712dd9d6245bf6f34d118`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:03:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:03:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:06:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:06:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:06:05 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:07:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ecaa4a720ffd8b3f56038a2d5f616807fa7485f551442c1f40ea8fd3981476`  
		Last Modified: Tue, 18 Apr 2023 02:16:19 GMT  
		Size: 1.2 MB (1157196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7945fb40cca95a4e5c72309573289c0784fb110e1606688d25f64849ca28139`  
		Last Modified: Tue, 18 Apr 2023 02:16:18 GMT  
		Size: 4.7 MB (4679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c069a57904ca9856ac4e9d5b220c3c4b98c50fded7cdd74e670f2338c3fb330`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b1cc4dc29f69e7392b245372d8097dcecebafe0667c8f2726299a4de8874fb`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dd47d037bb6cd6982d83524e76328da32499ff9d59f265b0ec7756a8a52072`  
		Last Modified: Tue, 18 Apr 2023 02:16:46 GMT  
		Size: 157.5 MB (157503873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f3aa8b76ccbcd8b349669fc88b8205c0cd0f8a4d1c858519ae07119f9e4879`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefc606d3dd23a8815fd1e238d5fdfe32080b4795073ba61cee804527816162a`  
		Last Modified: Tue, 18 Apr 2023 02:16:59 GMT  
		Size: 40.5 MB (40503298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc1f052e8af8e9f8ce3488131b6e3db7f4c91846dfc84d2f75688b69a04961`  
		Last Modified: Tue, 18 Apr 2023 02:16:54 GMT  
		Size: 297.1 KB (297142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb40216b8c1d941c1be2d7ab0be0dd7b2c40485ff30f2d5693e2c7bf59ee3f`  
		Last Modified: Tue, 18 Apr 2023 02:17:03 GMT  
		Size: 60.5 MB (60496479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d5ea21ddeb3a8263b55ff73a81ba0a53954362e89dbb5bc3070f7c55b5e8c6e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322836771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc8c46b2872805b8ba64f84218bf3b7ff59ec0c72e34a2e11a8be1df5048b440`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:06:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:09:00 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:09:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:09:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89011a19d825c31dd1ecdacfff5418ea066cc6c3d8b16aa5495409bae017b1f1`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf18013b664813b5e2ac52cbfde90f06a51486a530223919716ad97cb24c2a`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1809be61e23432d56e45874bfae781cc545d2889cf2d4a4ec837bbe62c12ae`  
		Last Modified: Tue, 18 Apr 2023 02:22:22 GMT  
		Size: 171.5 MB (171472211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29476e1a64f98957516be750445e8fe8dab41029f42b326871dad7c15a5002f4`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9778a01d5ceece6c4f0c2c0c02cc6f090ecb6a15e4ae5b1ae330ee94589a570`  
		Last Modified: Tue, 18 Apr 2023 02:22:36 GMT  
		Size: 45.2 MB (45203703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdd76f4f02f17a00aaef729800e659e052bf15f73a3a5e03cdb8c835a754761`  
		Last Modified: Tue, 18 Apr 2023 02:22:31 GMT  
		Size: 297.1 KB (297141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f09767fc16c06e81dd2dc318f6e7d1bb01562aefaaed477349db702168210`  
		Last Modified: Tue, 18 Apr 2023 02:22:38 GMT  
		Size: 72.0 MB (71974377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:d336bfe2faebcedd09483963baa0c5d1692831fe7cfb85510091b45f59765da1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:f311687f0e07d308f5edac5894f615aceaf0dc23178f4f99a18e65617d258aeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212307605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c825e8b4e5aa43d757c04d62d6c3062572b0d55d3dca486b4650f03cb84526aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:00:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 01:02:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:02:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b009b5adbd509635590b8ca3f676b6641b7bb66ab0512ccd4066db76ca60f5`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b0f9dac5dfd8149acea5db9be04cf12e33419619851a19de0dc33268bc543`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b823ac6a3ceddc3171904f453472228f5ce941332ae1c4c3a97b62399cb8`  
		Last Modified: Tue, 18 Apr 2023 01:15:25 GMT  
		Size: 177.0 MB (177015888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d72917faacc696317190bddb87cec63b461b7bbb280990ed04a1ab40b01565a`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:c1ed5a9386ee61130e008915dc3466c1f73e5bbf5ace73efd82da96667bc09e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187929479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22b36005d9a1b0c3904ed1bb3c0e53cc775327bc3cd0afafcc48a8ce37dd04f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:03:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:03:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:06:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:06:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:06:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ecaa4a720ffd8b3f56038a2d5f616807fa7485f551442c1f40ea8fd3981476`  
		Last Modified: Tue, 18 Apr 2023 02:16:19 GMT  
		Size: 1.2 MB (1157196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7945fb40cca95a4e5c72309573289c0784fb110e1606688d25f64849ca28139`  
		Last Modified: Tue, 18 Apr 2023 02:16:18 GMT  
		Size: 4.7 MB (4679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c069a57904ca9856ac4e9d5b220c3c4b98c50fded7cdd74e670f2338c3fb330`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b1cc4dc29f69e7392b245372d8097dcecebafe0667c8f2726299a4de8874fb`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dd47d037bb6cd6982d83524e76328da32499ff9d59f265b0ec7756a8a52072`  
		Last Modified: Tue, 18 Apr 2023 02:16:46 GMT  
		Size: 157.5 MB (157503873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f3aa8b76ccbcd8b349669fc88b8205c0cd0f8a4d1c858519ae07119f9e4879`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a34bb855c8275f00f8cbdc389aad3700c9a534f957e980432f2e1274dfb7c855
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205361550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38d280d269fb18b9baaf4981a834070ac1995f922470c9b6d3c58acbe3e6bc48`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:06:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:09:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89011a19d825c31dd1ecdacfff5418ea066cc6c3d8b16aa5495409bae017b1f1`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf18013b664813b5e2ac52cbfde90f06a51486a530223919716ad97cb24c2a`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1809be61e23432d56e45874bfae781cc545d2889cf2d4a4ec837bbe62c12ae`  
		Last Modified: Tue, 18 Apr 2023 02:22:22 GMT  
		Size: 171.5 MB (171472211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29476e1a64f98957516be750445e8fe8dab41029f42b326871dad7c15a5002f4`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:a4a811bb0506fd730247101c9095e391520714c7e163db4b78349aa63e9f7fd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:953dfc6c66e60b0106ef4cbc304baef2155861ecbba69d13bd1db5433bdf5c7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300610530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43f4b3df3a420ffe44998a06fbcdfd1f2a73251645b24ba5dc015a0ef05158a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:07 GMT
ADD file:d176a72312205fc75b2950df98f4ed25abadd4b053b9d85bea67466a5b30220f in / 
# Tue, 02 May 2023 23:47:08 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:38:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:38:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 May 2023 21:38:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:38:39 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:38:39 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:38:39 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 May 2023 21:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:39:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 May 2023 21:39:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:40:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a94073ab46f8d565f5938cc345d32f7adda10a2585e39555079da9d4ee595974`  
		Last Modified: Tue, 02 May 2023 23:50:40 GMT  
		Size: 50.4 MB (50448697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6a520b96cab6be544c3de79dfbd2e79a43648778ff5ffc9cea03b9afea1a8a`  
		Last Modified: Wed, 03 May 2023 22:02:33 GMT  
		Size: 10.9 MB (10897025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b18fd569bd474fa851fd78f1d3bf2e9678d8423061fdd217c621a34a0e1a18`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b96262d8a19c986620307e5e5f5bc87d241ebddd343a22e317096193e83ca7`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba9b33e9316a950f2ca0db084e17331cca39064c3a3d10175a5732482915e1c`  
		Last Modified: Wed, 03 May 2023 22:03:02 GMT  
		Size: 239.3 MB (239262397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f679b704b1a974ebf77923991309e3935a8e4e5950043f8e8df9817cb566018`  
		Last Modified: Wed, 03 May 2023 22:02:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1e368f04c44fb0167ff47d43b10fd721c254e2e52f39cf02a2f8e1c9d20bc3ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244600123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0841f2fb87cc10cf6793954ab95d56fde855f4a16509c5a9e94ae9ed297fc522`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:22:56 GMT
ADD file:6042e29dcf5e22439cd69873d8960f8d3977abe915ef462aaa84368a7186a3bf in / 
# Wed, 03 May 2023 00:22:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:32:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:32:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 May 2023 18:32:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:32:32 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:32:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:32:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 May 2023 18:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:33:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 May 2023 18:33:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:33:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b7c5fe8e0ac53c77142bf16686fc01d0d2b1fb2da7be5414cdf2f224ec485592`  
		Last Modified: Wed, 03 May 2023 00:26:10 GMT  
		Size: 49.2 MB (49238630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f4b1b3aff79daeba459c24d6625912443a9c4b6e072fd443df8cf1fe609a3b`  
		Last Modified: Wed, 03 May 2023 18:59:14 GMT  
		Size: 10.9 MB (10902746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bd0f1f3ef8032558026a60ca367a9d7b0a28a5d5656befe67922b145ce30bf`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ffa192fc268fe17d966f4b3cea0d44a2889b03c6266a5d26e16c239241f65e`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66412823f7f9778ca86e89b006f993392e02d4dcf6d72bececff2961ab62e97`  
		Last Modified: Wed, 03 May 2023 18:59:49 GMT  
		Size: 184.5 MB (184456335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220fcae6736a0fef7e49e980a9743d78ac71f0793d181838e243ca8df2e17b7`  
		Last Modified: Wed, 03 May 2023 18:59:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:d336bfe2faebcedd09483963baa0c5d1692831fe7cfb85510091b45f59765da1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:f311687f0e07d308f5edac5894f615aceaf0dc23178f4f99a18e65617d258aeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212307605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c825e8b4e5aa43d757c04d62d6c3062572b0d55d3dca486b4650f03cb84526aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:00:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 01:02:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:02:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b009b5adbd509635590b8ca3f676b6641b7bb66ab0512ccd4066db76ca60f5`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b0f9dac5dfd8149acea5db9be04cf12e33419619851a19de0dc33268bc543`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b823ac6a3ceddc3171904f453472228f5ce941332ae1c4c3a97b62399cb8`  
		Last Modified: Tue, 18 Apr 2023 01:15:25 GMT  
		Size: 177.0 MB (177015888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d72917faacc696317190bddb87cec63b461b7bbb280990ed04a1ab40b01565a`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:c1ed5a9386ee61130e008915dc3466c1f73e5bbf5ace73efd82da96667bc09e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187929479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22b36005d9a1b0c3904ed1bb3c0e53cc775327bc3cd0afafcc48a8ce37dd04f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:03:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:03:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:06:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:06:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:06:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ecaa4a720ffd8b3f56038a2d5f616807fa7485f551442c1f40ea8fd3981476`  
		Last Modified: Tue, 18 Apr 2023 02:16:19 GMT  
		Size: 1.2 MB (1157196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7945fb40cca95a4e5c72309573289c0784fb110e1606688d25f64849ca28139`  
		Last Modified: Tue, 18 Apr 2023 02:16:18 GMT  
		Size: 4.7 MB (4679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c069a57904ca9856ac4e9d5b220c3c4b98c50fded7cdd74e670f2338c3fb330`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b1cc4dc29f69e7392b245372d8097dcecebafe0667c8f2726299a4de8874fb`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dd47d037bb6cd6982d83524e76328da32499ff9d59f265b0ec7756a8a52072`  
		Last Modified: Tue, 18 Apr 2023 02:16:46 GMT  
		Size: 157.5 MB (157503873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f3aa8b76ccbcd8b349669fc88b8205c0cd0f8a4d1c858519ae07119f9e4879`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a34bb855c8275f00f8cbdc389aad3700c9a534f957e980432f2e1274dfb7c855
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205361550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38d280d269fb18b9baaf4981a834070ac1995f922470c9b6d3c58acbe3e6bc48`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:06:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:09:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89011a19d825c31dd1ecdacfff5418ea066cc6c3d8b16aa5495409bae017b1f1`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf18013b664813b5e2ac52cbfde90f06a51486a530223919716ad97cb24c2a`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1809be61e23432d56e45874bfae781cc545d2889cf2d4a4ec837bbe62c12ae`  
		Last Modified: Tue, 18 Apr 2023 02:22:22 GMT  
		Size: 171.5 MB (171472211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29476e1a64f98957516be750445e8fe8dab41029f42b326871dad7c15a5002f4`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:abc58cb199df89a4ebb91e59f87d0413c7e23b3f527c4fe498e35843a593ceaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:0b8d4b1d363a67cf3c95eb289f00a428230aa794032ef06e274235f1ec22a904
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268601984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a591daad46f014598854c581bde6d5327ea870515c178f9525d9fd4813a8e3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:57:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 21:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:58:29 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:58:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:58:29 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:59:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:59:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:59:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 21:59:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285dfa96f611fd7adc01ba69ac7e4a2f1908b2e0789b6af59c697d81ef586ac`  
		Last Modified: Wed, 03 May 2023 22:07:39 GMT  
		Size: 124.1 MB (124111474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6607aaf2a2bb9ae2485f009f0e839192b6a1e5a9236fef31b92e88e11da8412`  
		Last Modified: Wed, 03 May 2023 22:07:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d7c154e1b997c1b21c7505dfb66305a3062256015ec7a7890e1b6ef3eacd3f`  
		Last Modified: Wed, 03 May 2023 22:07:57 GMT  
		Size: 85.0 MB (84998074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c86a7baccad3d6c956fc7871ccfb6668dd150271b737949ff71f9c1c4b91ad3`  
		Last Modified: Wed, 03 May 2023 22:07:47 GMT  
		Size: 283.9 KB (283944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1c84c738f9e7df26ff7d69e76c60b208ac7bf7b078a0ef362fd027cb97710f`  
		Last Modified: Wed, 03 May 2023 22:07:47 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b11880a7eca1765742848615c1ab9d3c6452d148e5be64bddbfe47e82b7e497`  
		Last Modified: Wed, 03 May 2023 22:07:50 GMT  
		Size: 23.7 MB (23705240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8513d4373b2cef3549372258bbbdad4a3cb57d7d207393a698fefcc0a3609df1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261137250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89897cd876660e5cb45a197371d5c5c788539e2d8d7288ab373b4a4ff00d561a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:55:25 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 18:56:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:56:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:56:10 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:56:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:56:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 18:56:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344fd0345199b732007d1fd801848c7f86eaadf910174213af53e56be4d95dea`  
		Last Modified: Wed, 03 May 2023 19:03:41 GMT  
		Size: 121.6 MB (121590308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b879cb6b4af64e18cfa7544975f71141f8047683cf7dbfbfd66f5f2b7a64d26`  
		Last Modified: Wed, 03 May 2023 19:03:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a93d68ae5e043a209fd1fa65f157ad74e5ae2c2cf3b758f03a8dc91247ab2f`  
		Last Modified: Wed, 03 May 2023 19:03:57 GMT  
		Size: 82.7 MB (82733194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0ee7cfe91dbc7e58d5ffb7818cb066caf355b4f689e1f470cb0a7936f6dc9b`  
		Last Modified: Wed, 03 May 2023 19:03:49 GMT  
		Size: 283.8 KB (283764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7d206a3ad557445769cd5038bb2eafeb117b95d2e9872a6abb12935476535`  
		Last Modified: Wed, 03 May 2023 19:03:49 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75019cce8ecc252b25bcfef4182b738a310040c946fcb237ad1c66637a84a72f`  
		Last Modified: Wed, 03 May 2023 19:03:52 GMT  
		Size: 23.1 MB (23094522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:82a9630fdadb5d397c1dcf27e31f8b1dbe3fab7e66dcad28991676b17e67300f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:f0e7a2952fcc117d4969ee49dc0ef07e2fa79d077b8b33712e2d1e06373cb1c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1098255707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:959c377c3ce152f7b74058a68fbba2bae5705cae7ea0c21bdc2182db2e018dc5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:57:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 21:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:58:29 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:58:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:58:29 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:59:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:59:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:59:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 21:59:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:01:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285dfa96f611fd7adc01ba69ac7e4a2f1908b2e0789b6af59c697d81ef586ac`  
		Last Modified: Wed, 03 May 2023 22:07:39 GMT  
		Size: 124.1 MB (124111474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6607aaf2a2bb9ae2485f009f0e839192b6a1e5a9236fef31b92e88e11da8412`  
		Last Modified: Wed, 03 May 2023 22:07:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d7c154e1b997c1b21c7505dfb66305a3062256015ec7a7890e1b6ef3eacd3f`  
		Last Modified: Wed, 03 May 2023 22:07:57 GMT  
		Size: 85.0 MB (84998074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c86a7baccad3d6c956fc7871ccfb6668dd150271b737949ff71f9c1c4b91ad3`  
		Last Modified: Wed, 03 May 2023 22:07:47 GMT  
		Size: 283.9 KB (283944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1c84c738f9e7df26ff7d69e76c60b208ac7bf7b078a0ef362fd027cb97710f`  
		Last Modified: Wed, 03 May 2023 22:07:47 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b11880a7eca1765742848615c1ab9d3c6452d148e5be64bddbfe47e82b7e497`  
		Last Modified: Wed, 03 May 2023 22:07:50 GMT  
		Size: 23.7 MB (23705240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735251ae525982faf2e4ecf876a86d9a427118a8fe81f5d1ebb29a1e9798602`  
		Last Modified: Wed, 03 May 2023 22:09:39 GMT  
		Size: 829.7 MB (829653723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f7dba83cb53ae9266523c053b08e988f6efaee740ba6fd2dda171c2ae8004415
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1049564633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed682eb40d73fdfb78a87225de5dafd43c81846a05b95e871bbe31a3b9b1fbd6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:55:25 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 18:56:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:56:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:56:10 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:56:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:56:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 18:56:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:58:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344fd0345199b732007d1fd801848c7f86eaadf910174213af53e56be4d95dea`  
		Last Modified: Wed, 03 May 2023 19:03:41 GMT  
		Size: 121.6 MB (121590308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b879cb6b4af64e18cfa7544975f71141f8047683cf7dbfbfd66f5f2b7a64d26`  
		Last Modified: Wed, 03 May 2023 19:03:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a93d68ae5e043a209fd1fa65f157ad74e5ae2c2cf3b758f03a8dc91247ab2f`  
		Last Modified: Wed, 03 May 2023 19:03:57 GMT  
		Size: 82.7 MB (82733194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0ee7cfe91dbc7e58d5ffb7818cb066caf355b4f689e1f470cb0a7936f6dc9b`  
		Last Modified: Wed, 03 May 2023 19:03:49 GMT  
		Size: 283.8 KB (283764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7d206a3ad557445769cd5038bb2eafeb117b95d2e9872a6abb12935476535`  
		Last Modified: Wed, 03 May 2023 19:03:49 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75019cce8ecc252b25bcfef4182b738a310040c946fcb237ad1c66637a84a72f`  
		Last Modified: Wed, 03 May 2023 19:03:52 GMT  
		Size: 23.1 MB (23094522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f880d8bf7b1b579ee784f5120a704942d1807ad7c570400fae434c9772ab9ac`  
		Last Modified: Wed, 03 May 2023 19:05:12 GMT  
		Size: 788.4 MB (788427383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:82a9630fdadb5d397c1dcf27e31f8b1dbe3fab7e66dcad28991676b17e67300f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:f0e7a2952fcc117d4969ee49dc0ef07e2fa79d077b8b33712e2d1e06373cb1c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1098255707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:959c377c3ce152f7b74058a68fbba2bae5705cae7ea0c21bdc2182db2e018dc5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:57:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 21:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:58:29 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:58:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:58:29 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:59:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:59:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:59:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 21:59:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:01:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285dfa96f611fd7adc01ba69ac7e4a2f1908b2e0789b6af59c697d81ef586ac`  
		Last Modified: Wed, 03 May 2023 22:07:39 GMT  
		Size: 124.1 MB (124111474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6607aaf2a2bb9ae2485f009f0e839192b6a1e5a9236fef31b92e88e11da8412`  
		Last Modified: Wed, 03 May 2023 22:07:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d7c154e1b997c1b21c7505dfb66305a3062256015ec7a7890e1b6ef3eacd3f`  
		Last Modified: Wed, 03 May 2023 22:07:57 GMT  
		Size: 85.0 MB (84998074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c86a7baccad3d6c956fc7871ccfb6668dd150271b737949ff71f9c1c4b91ad3`  
		Last Modified: Wed, 03 May 2023 22:07:47 GMT  
		Size: 283.9 KB (283944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1c84c738f9e7df26ff7d69e76c60b208ac7bf7b078a0ef362fd027cb97710f`  
		Last Modified: Wed, 03 May 2023 22:07:47 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b11880a7eca1765742848615c1ab9d3c6452d148e5be64bddbfe47e82b7e497`  
		Last Modified: Wed, 03 May 2023 22:07:50 GMT  
		Size: 23.7 MB (23705240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735251ae525982faf2e4ecf876a86d9a427118a8fe81f5d1ebb29a1e9798602`  
		Last Modified: Wed, 03 May 2023 22:09:39 GMT  
		Size: 829.7 MB (829653723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f7dba83cb53ae9266523c053b08e988f6efaee740ba6fd2dda171c2ae8004415
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1049564633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed682eb40d73fdfb78a87225de5dafd43c81846a05b95e871bbe31a3b9b1fbd6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:55:25 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 18:56:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:56:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:56:10 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:56:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:56:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 18:56:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:58:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344fd0345199b732007d1fd801848c7f86eaadf910174213af53e56be4d95dea`  
		Last Modified: Wed, 03 May 2023 19:03:41 GMT  
		Size: 121.6 MB (121590308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b879cb6b4af64e18cfa7544975f71141f8047683cf7dbfbfd66f5f2b7a64d26`  
		Last Modified: Wed, 03 May 2023 19:03:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a93d68ae5e043a209fd1fa65f157ad74e5ae2c2cf3b758f03a8dc91247ab2f`  
		Last Modified: Wed, 03 May 2023 19:03:57 GMT  
		Size: 82.7 MB (82733194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0ee7cfe91dbc7e58d5ffb7818cb066caf355b4f689e1f470cb0a7936f6dc9b`  
		Last Modified: Wed, 03 May 2023 19:03:49 GMT  
		Size: 283.8 KB (283764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7d206a3ad557445769cd5038bb2eafeb117b95d2e9872a6abb12935476535`  
		Last Modified: Wed, 03 May 2023 19:03:49 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75019cce8ecc252b25bcfef4182b738a310040c946fcb237ad1c66637a84a72f`  
		Last Modified: Wed, 03 May 2023 19:03:52 GMT  
		Size: 23.1 MB (23094522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f880d8bf7b1b579ee784f5120a704942d1807ad7c570400fae434c9772ab9ac`  
		Last Modified: Wed, 03 May 2023 19:05:12 GMT  
		Size: 788.4 MB (788427383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:abc58cb199df89a4ebb91e59f87d0413c7e23b3f527c4fe498e35843a593ceaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:0b8d4b1d363a67cf3c95eb289f00a428230aa794032ef06e274235f1ec22a904
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268601984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a591daad46f014598854c581bde6d5327ea870515c178f9525d9fd4813a8e3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:57:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 21:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:58:29 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:58:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:58:29 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:59:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:59:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:59:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 21:59:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285dfa96f611fd7adc01ba69ac7e4a2f1908b2e0789b6af59c697d81ef586ac`  
		Last Modified: Wed, 03 May 2023 22:07:39 GMT  
		Size: 124.1 MB (124111474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6607aaf2a2bb9ae2485f009f0e839192b6a1e5a9236fef31b92e88e11da8412`  
		Last Modified: Wed, 03 May 2023 22:07:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d7c154e1b997c1b21c7505dfb66305a3062256015ec7a7890e1b6ef3eacd3f`  
		Last Modified: Wed, 03 May 2023 22:07:57 GMT  
		Size: 85.0 MB (84998074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c86a7baccad3d6c956fc7871ccfb6668dd150271b737949ff71f9c1c4b91ad3`  
		Last Modified: Wed, 03 May 2023 22:07:47 GMT  
		Size: 283.9 KB (283944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1c84c738f9e7df26ff7d69e76c60b208ac7bf7b078a0ef362fd027cb97710f`  
		Last Modified: Wed, 03 May 2023 22:07:47 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b11880a7eca1765742848615c1ab9d3c6452d148e5be64bddbfe47e82b7e497`  
		Last Modified: Wed, 03 May 2023 22:07:50 GMT  
		Size: 23.7 MB (23705240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8513d4373b2cef3549372258bbbdad4a3cb57d7d207393a698fefcc0a3609df1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261137250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89897cd876660e5cb45a197371d5c5c788539e2d8d7288ab373b4a4ff00d561a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:55:25 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 18:56:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:56:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:56:10 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:56:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:56:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 18:56:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344fd0345199b732007d1fd801848c7f86eaadf910174213af53e56be4d95dea`  
		Last Modified: Wed, 03 May 2023 19:03:41 GMT  
		Size: 121.6 MB (121590308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b879cb6b4af64e18cfa7544975f71141f8047683cf7dbfbfd66f5f2b7a64d26`  
		Last Modified: Wed, 03 May 2023 19:03:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a93d68ae5e043a209fd1fa65f157ad74e5ae2c2cf3b758f03a8dc91247ab2f`  
		Last Modified: Wed, 03 May 2023 19:03:57 GMT  
		Size: 82.7 MB (82733194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0ee7cfe91dbc7e58d5ffb7818cb066caf355b4f689e1f470cb0a7936f6dc9b`  
		Last Modified: Wed, 03 May 2023 19:03:49 GMT  
		Size: 283.8 KB (283764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7d206a3ad557445769cd5038bb2eafeb117b95d2e9872a6abb12935476535`  
		Last Modified: Wed, 03 May 2023 19:03:49 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75019cce8ecc252b25bcfef4182b738a310040c946fcb237ad1c66637a84a72f`  
		Last Modified: Wed, 03 May 2023 19:03:52 GMT  
		Size: 23.1 MB (23094522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:abc58cb199df89a4ebb91e59f87d0413c7e23b3f527c4fe498e35843a593ceaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:0b8d4b1d363a67cf3c95eb289f00a428230aa794032ef06e274235f1ec22a904
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268601984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a591daad46f014598854c581bde6d5327ea870515c178f9525d9fd4813a8e3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:57:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 21:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:58:29 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:58:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:58:29 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:59:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:59:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 21:59:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 21:59:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285dfa96f611fd7adc01ba69ac7e4a2f1908b2e0789b6af59c697d81ef586ac`  
		Last Modified: Wed, 03 May 2023 22:07:39 GMT  
		Size: 124.1 MB (124111474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6607aaf2a2bb9ae2485f009f0e839192b6a1e5a9236fef31b92e88e11da8412`  
		Last Modified: Wed, 03 May 2023 22:07:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d7c154e1b997c1b21c7505dfb66305a3062256015ec7a7890e1b6ef3eacd3f`  
		Last Modified: Wed, 03 May 2023 22:07:57 GMT  
		Size: 85.0 MB (84998074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c86a7baccad3d6c956fc7871ccfb6668dd150271b737949ff71f9c1c4b91ad3`  
		Last Modified: Wed, 03 May 2023 22:07:47 GMT  
		Size: 283.9 KB (283944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1c84c738f9e7df26ff7d69e76c60b208ac7bf7b078a0ef362fd027cb97710f`  
		Last Modified: Wed, 03 May 2023 22:07:47 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b11880a7eca1765742848615c1ab9d3c6452d148e5be64bddbfe47e82b7e497`  
		Last Modified: Wed, 03 May 2023 22:07:50 GMT  
		Size: 23.7 MB (23705240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8513d4373b2cef3549372258bbbdad4a3cb57d7d207393a698fefcc0a3609df1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261137250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89897cd876660e5cb45a197371d5c5c788539e2d8d7288ab373b4a4ff00d561a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:55:25 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 18:56:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:56:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:56:10 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:56:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 May 2023 18:56:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 03 May 2023 18:56:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344fd0345199b732007d1fd801848c7f86eaadf910174213af53e56be4d95dea`  
		Last Modified: Wed, 03 May 2023 19:03:41 GMT  
		Size: 121.6 MB (121590308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b879cb6b4af64e18cfa7544975f71141f8047683cf7dbfbfd66f5f2b7a64d26`  
		Last Modified: Wed, 03 May 2023 19:03:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a93d68ae5e043a209fd1fa65f157ad74e5ae2c2cf3b758f03a8dc91247ab2f`  
		Last Modified: Wed, 03 May 2023 19:03:57 GMT  
		Size: 82.7 MB (82733194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0ee7cfe91dbc7e58d5ffb7818cb066caf355b4f689e1f470cb0a7936f6dc9b`  
		Last Modified: Wed, 03 May 2023 19:03:49 GMT  
		Size: 283.8 KB (283764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7d206a3ad557445769cd5038bb2eafeb117b95d2e9872a6abb12935476535`  
		Last Modified: Wed, 03 May 2023 19:03:49 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75019cce8ecc252b25bcfef4182b738a310040c946fcb237ad1c66637a84a72f`  
		Last Modified: Wed, 03 May 2023 19:03:52 GMT  
		Size: 23.1 MB (23094522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:7c6fd91f22885515a1c752ada9d7a81f845f0eba2f5ac3117a82bc7d89708e4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:c8883575234d14f42663ff77882ec52883957690345f9e4df96593a4c8ea3088
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159612306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec246e630b1cfb45a280935f5077489eda8a4dcb63fc872418715e5bf684d3d1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:57:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 21:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:58:29 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:58:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:58:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285dfa96f611fd7adc01ba69ac7e4a2f1908b2e0789b6af59c697d81ef586ac`  
		Last Modified: Wed, 03 May 2023 22:07:39 GMT  
		Size: 124.1 MB (124111474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6607aaf2a2bb9ae2485f009f0e839192b6a1e5a9236fef31b92e88e11da8412`  
		Last Modified: Wed, 03 May 2023 22:07:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:663e17236101e1d8f141ac251ca5e046c605f691ba727fb74a709a26beadac90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155023347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44b58fb0655b5f92256fd045d234b0538c79618c46802a2f44fa90d7aa45a0c1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:55:25 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 18:56:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:56:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:56:10 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344fd0345199b732007d1fd801848c7f86eaadf910174213af53e56be4d95dea`  
		Last Modified: Wed, 03 May 2023 19:03:41 GMT  
		Size: 121.6 MB (121590308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b879cb6b4af64e18cfa7544975f71141f8047683cf7dbfbfd66f5f2b7a64d26`  
		Last Modified: Wed, 03 May 2023 19:03:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:7c6fd91f22885515a1c752ada9d7a81f845f0eba2f5ac3117a82bc7d89708e4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:c8883575234d14f42663ff77882ec52883957690345f9e4df96593a4c8ea3088
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159612306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec246e630b1cfb45a280935f5077489eda8a4dcb63fc872418715e5bf684d3d1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:45:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:45:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 21:45:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 21:45:41 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:45:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 21:57:22 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 21:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:58:29 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 21:58:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 21:58:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d709c34b032e9c25f3ef7dbc9cc5be0ab87d014082e04d1f4a5d20e2970446b`  
		Last Modified: Wed, 03 May 2023 22:04:52 GMT  
		Size: 1.2 MB (1239802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a8c29b4dfa9054fe01f5590245b9ad2e27c309027d00b628451f55bfde59c`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c946d99b6f2ae4da84c6c0af0b3204f17c5371e0ef1e1968fc20d3c812123`  
		Last Modified: Wed, 03 May 2023 22:04:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89451566146a587c0f7bde9c5bd208af5e73072fa556ff6ad6ac85c213406cb6`  
		Last Modified: Wed, 03 May 2023 22:04:49 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285dfa96f611fd7adc01ba69ac7e4a2f1908b2e0789b6af59c697d81ef586ac`  
		Last Modified: Wed, 03 May 2023 22:07:39 GMT  
		Size: 124.1 MB (124111474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6607aaf2a2bb9ae2485f009f0e839192b6a1e5a9236fef31b92e88e11da8412`  
		Last Modified: Wed, 03 May 2023 22:07:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:663e17236101e1d8f141ac251ca5e046c605f691ba727fb74a709a26beadac90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155023347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44b58fb0655b5f92256fd045d234b0538c79618c46802a2f44fa90d7aa45a0c1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:55:25 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 18:56:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:56:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:56:10 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344fd0345199b732007d1fd801848c7f86eaadf910174213af53e56be4d95dea`  
		Last Modified: Wed, 03 May 2023 19:03:41 GMT  
		Size: 121.6 MB (121590308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b879cb6b4af64e18cfa7544975f71141f8047683cf7dbfbfd66f5f2b7a64d26`  
		Last Modified: Wed, 03 May 2023 19:03:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
