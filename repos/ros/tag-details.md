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
$ docker pull ros@sha256:86d41b25c789aec0f9f99517c763d566a2072e64d9a40ad7bf62e4496b99ef84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:c4da6b64514e027f09106cab7acaa3746284d0d087fc2aa5f9d388834bdace2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.1 MB (263050019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83850d460372907bedba817705c89514b0e188eaeb3c00d70817a6418018f6a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 04:25:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:25:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:25:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:25:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:26:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:26:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:26:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 04:27:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62e2d9c70cd1fb5cfb879150c7d04b63ab2922e154e11b0fd47031a52c16a5a`  
		Last Modified: Thu, 16 Mar 2023 04:47:31 GMT  
		Size: 106.3 MB (106343939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273cc0c60a3141d6e964d07b9ac39f9126b3d3ca36a70493cc8496448375fd55`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0800e2c533d39c10eda1c33c4cc5e7d8c164ae5d620b68a5674ec6ff18427d`  
		Last Modified: Thu, 16 Mar 2023 04:47:54 GMT  
		Size: 97.9 MB (97887694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130e7a70d397d234ae4137584d1d00a5ddf4d23b258ecf856deeefab1fe664f5`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 314.1 KB (314072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a79070b854f777682eb1cc3a62e2cf75029fdd5105fe7ed8e85a993ea5226c`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cfb85e0aafffb281729a9c1323877d16e594d6ccd10b8d798b53c0925247c4`  
		Last Modified: Thu, 16 Mar 2023 04:47:45 GMT  
		Size: 23.1 MB (23071520 bytes)  
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
$ docker pull ros@sha256:43a8695cab914cd14f66f821f9f2454fbf9ec576db67259babd6b8b3c147c936
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:c7f1bedcb4a74ab19a42f5ab1ef0dea81c60cc4a881f1f4268ba06486503512c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1092111378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b02b667be811572dc804347a6aa91d2722570580ca0ed2ae5127139a0354fca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 04:25:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:25:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:25:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:25:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:26:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:26:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:26:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 04:27:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62e2d9c70cd1fb5cfb879150c7d04b63ab2922e154e11b0fd47031a52c16a5a`  
		Last Modified: Thu, 16 Mar 2023 04:47:31 GMT  
		Size: 106.3 MB (106343939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273cc0c60a3141d6e964d07b9ac39f9126b3d3ca36a70493cc8496448375fd55`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0800e2c533d39c10eda1c33c4cc5e7d8c164ae5d620b68a5674ec6ff18427d`  
		Last Modified: Thu, 16 Mar 2023 04:47:54 GMT  
		Size: 97.9 MB (97887694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130e7a70d397d234ae4137584d1d00a5ddf4d23b258ecf856deeefab1fe664f5`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 314.1 KB (314072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a79070b854f777682eb1cc3a62e2cf75029fdd5105fe7ed8e85a993ea5226c`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cfb85e0aafffb281729a9c1323877d16e594d6ccd10b8d798b53c0925247c4`  
		Last Modified: Thu, 16 Mar 2023 04:47:45 GMT  
		Size: 23.1 MB (23071520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163aa40880ff6addd2ed1bde56b1b1a48bdc6f9d076de22fbd661d8291799dea`  
		Last Modified: Thu, 16 Mar 2023 04:49:44 GMT  
		Size: 829.1 MB (829061359 bytes)  
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
$ docker pull ros@sha256:43a8695cab914cd14f66f821f9f2454fbf9ec576db67259babd6b8b3c147c936
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:c7f1bedcb4a74ab19a42f5ab1ef0dea81c60cc4a881f1f4268ba06486503512c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1092111378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b02b667be811572dc804347a6aa91d2722570580ca0ed2ae5127139a0354fca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 04:25:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:25:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:25:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:25:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:26:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:26:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:26:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 04:27:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62e2d9c70cd1fb5cfb879150c7d04b63ab2922e154e11b0fd47031a52c16a5a`  
		Last Modified: Thu, 16 Mar 2023 04:47:31 GMT  
		Size: 106.3 MB (106343939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273cc0c60a3141d6e964d07b9ac39f9126b3d3ca36a70493cc8496448375fd55`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0800e2c533d39c10eda1c33c4cc5e7d8c164ae5d620b68a5674ec6ff18427d`  
		Last Modified: Thu, 16 Mar 2023 04:47:54 GMT  
		Size: 97.9 MB (97887694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130e7a70d397d234ae4137584d1d00a5ddf4d23b258ecf856deeefab1fe664f5`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 314.1 KB (314072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a79070b854f777682eb1cc3a62e2cf75029fdd5105fe7ed8e85a993ea5226c`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cfb85e0aafffb281729a9c1323877d16e594d6ccd10b8d798b53c0925247c4`  
		Last Modified: Thu, 16 Mar 2023 04:47:45 GMT  
		Size: 23.1 MB (23071520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163aa40880ff6addd2ed1bde56b1b1a48bdc6f9d076de22fbd661d8291799dea`  
		Last Modified: Thu, 16 Mar 2023 04:49:44 GMT  
		Size: 829.1 MB (829061359 bytes)  
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
$ docker pull ros@sha256:86d41b25c789aec0f9f99517c763d566a2072e64d9a40ad7bf62e4496b99ef84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:c4da6b64514e027f09106cab7acaa3746284d0d087fc2aa5f9d388834bdace2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.1 MB (263050019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83850d460372907bedba817705c89514b0e188eaeb3c00d70817a6418018f6a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 04:25:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:25:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:25:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:25:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:26:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:26:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:26:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 04:27:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62e2d9c70cd1fb5cfb879150c7d04b63ab2922e154e11b0fd47031a52c16a5a`  
		Last Modified: Thu, 16 Mar 2023 04:47:31 GMT  
		Size: 106.3 MB (106343939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273cc0c60a3141d6e964d07b9ac39f9126b3d3ca36a70493cc8496448375fd55`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0800e2c533d39c10eda1c33c4cc5e7d8c164ae5d620b68a5674ec6ff18427d`  
		Last Modified: Thu, 16 Mar 2023 04:47:54 GMT  
		Size: 97.9 MB (97887694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130e7a70d397d234ae4137584d1d00a5ddf4d23b258ecf856deeefab1fe664f5`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 314.1 KB (314072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a79070b854f777682eb1cc3a62e2cf75029fdd5105fe7ed8e85a993ea5226c`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cfb85e0aafffb281729a9c1323877d16e594d6ccd10b8d798b53c0925247c4`  
		Last Modified: Thu, 16 Mar 2023 04:47:45 GMT  
		Size: 23.1 MB (23071520 bytes)  
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
$ docker pull ros@sha256:86d41b25c789aec0f9f99517c763d566a2072e64d9a40ad7bf62e4496b99ef84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:c4da6b64514e027f09106cab7acaa3746284d0d087fc2aa5f9d388834bdace2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.1 MB (263050019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83850d460372907bedba817705c89514b0e188eaeb3c00d70817a6418018f6a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 04:25:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:25:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:25:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:25:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:26:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:26:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:26:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 04:27:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62e2d9c70cd1fb5cfb879150c7d04b63ab2922e154e11b0fd47031a52c16a5a`  
		Last Modified: Thu, 16 Mar 2023 04:47:31 GMT  
		Size: 106.3 MB (106343939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273cc0c60a3141d6e964d07b9ac39f9126b3d3ca36a70493cc8496448375fd55`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0800e2c533d39c10eda1c33c4cc5e7d8c164ae5d620b68a5674ec6ff18427d`  
		Last Modified: Thu, 16 Mar 2023 04:47:54 GMT  
		Size: 97.9 MB (97887694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130e7a70d397d234ae4137584d1d00a5ddf4d23b258ecf856deeefab1fe664f5`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 314.1 KB (314072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a79070b854f777682eb1cc3a62e2cf75029fdd5105fe7ed8e85a993ea5226c`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cfb85e0aafffb281729a9c1323877d16e594d6ccd10b8d798b53c0925247c4`  
		Last Modified: Thu, 16 Mar 2023 04:47:45 GMT  
		Size: 23.1 MB (23071520 bytes)  
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
$ docker pull ros@sha256:8f0a4fecd0bef8feca63d6df7ed22b8bade5385a19801ee62e55eb4d7f2f7ca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:4dc54da7afb688b0861c8a20d824f8b6a58898a88533efb316d2f98dd1de7483
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141774328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f4e1460dcf48492e08836c26bfb4538f18d0aaa8ab4cd5aab828a613d901ef`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 04:25:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:25:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:25:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:25:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62e2d9c70cd1fb5cfb879150c7d04b63ab2922e154e11b0fd47031a52c16a5a`  
		Last Modified: Thu, 16 Mar 2023 04:47:31 GMT  
		Size: 106.3 MB (106343939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273cc0c60a3141d6e964d07b9ac39f9126b3d3ca36a70493cc8496448375fd55`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
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
$ docker pull ros@sha256:8f0a4fecd0bef8feca63d6df7ed22b8bade5385a19801ee62e55eb4d7f2f7ca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:4dc54da7afb688b0861c8a20d824f8b6a58898a88533efb316d2f98dd1de7483
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141774328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f4e1460dcf48492e08836c26bfb4538f18d0aaa8ab4cd5aab828a613d901ef`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 04:25:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:25:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:25:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:25:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62e2d9c70cd1fb5cfb879150c7d04b63ab2922e154e11b0fd47031a52c16a5a`  
		Last Modified: Thu, 16 Mar 2023 04:47:31 GMT  
		Size: 106.3 MB (106343939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273cc0c60a3141d6e964d07b9ac39f9126b3d3ca36a70493cc8496448375fd55`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
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
$ docker pull ros@sha256:86d41b25c789aec0f9f99517c763d566a2072e64d9a40ad7bf62e4496b99ef84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:c4da6b64514e027f09106cab7acaa3746284d0d087fc2aa5f9d388834bdace2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.1 MB (263050019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83850d460372907bedba817705c89514b0e188eaeb3c00d70817a6418018f6a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 04:25:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:25:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:25:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:25:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:26:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:26:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:26:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 04:27:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62e2d9c70cd1fb5cfb879150c7d04b63ab2922e154e11b0fd47031a52c16a5a`  
		Last Modified: Thu, 16 Mar 2023 04:47:31 GMT  
		Size: 106.3 MB (106343939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273cc0c60a3141d6e964d07b9ac39f9126b3d3ca36a70493cc8496448375fd55`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0800e2c533d39c10eda1c33c4cc5e7d8c164ae5d620b68a5674ec6ff18427d`  
		Last Modified: Thu, 16 Mar 2023 04:47:54 GMT  
		Size: 97.9 MB (97887694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130e7a70d397d234ae4137584d1d00a5ddf4d23b258ecf856deeefab1fe664f5`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 314.1 KB (314072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a79070b854f777682eb1cc3a62e2cf75029fdd5105fe7ed8e85a993ea5226c`  
		Last Modified: Thu, 16 Mar 2023 04:47:41 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cfb85e0aafffb281729a9c1323877d16e594d6ccd10b8d798b53c0925247c4`  
		Last Modified: Thu, 16 Mar 2023 04:47:45 GMT  
		Size: 23.1 MB (23071520 bytes)  
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
$ docker pull ros@sha256:45e9441e2496f7ac90aa11d3a132fe5feaac7c5a42d7ff8ad6f3268a6e9f5526
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:8cfd2b761f6398ff60cc52321cb275c7f4619d88007315bdbcdbe348d309c433
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.6 MB (437565428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ffed69de06cc91173726d899c430f78440e25b31702da04ba83af365fa684`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:58:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 04:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:00:33 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:00:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:01:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73b43b50fc9056c1213c61cfa3193cd15f8faa751905b21e0e9019473426a74`  
		Last Modified: Thu, 16 Mar 2023 03:11:48 GMT  
		Size: 819.0 KB (818997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6111169e4c0857f4eaf38437fa0beb5e0f66979105b8fdfd3c85c5c5e1544992`  
		Last Modified: Thu, 16 Mar 2023 04:41:15 GMT  
		Size: 4.9 MB (4878581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280739d0ef2f7bb759ccb3b3bb8a5f15a3d1ee562afe99609a493c65039b87a6`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d189808242488a25bc31490cfec5360bcb99b6a965f8782e6af80cf69e81ad79`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc74d1ea892a60a383eaee3d39a2f94fcd19fa347ee48e940f7152e5a8d6bccb`  
		Last Modified: Thu, 16 Mar 2023 04:41:48 GMT  
		Size: 259.6 MB (259588669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43567d3a1b9a70a0e7ec7a689892a144345cf9bcb6eb4151afba22b1eab2d47e`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc128d1e3275f672a35efb8cc6d100ff910f036dc6bbfdb5d0beea7ba5a48370`  
		Last Modified: Thu, 16 Mar 2023 04:42:06 GMT  
		Size: 70.3 MB (70268059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3dceb46441b9a8de4be3a53517c7cf44efe430d819993027ffd084b6dc13b`  
		Last Modified: Thu, 16 Mar 2023 04:41:57 GMT  
		Size: 297.9 KB (297878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1901e3f6c09a6bb1a3a48da8fb1162deb79e4a57ae416e9ca5b86ec2e21cab3d`  
		Last Modified: Thu, 16 Mar 2023 04:42:08 GMT  
		Size: 75.0 MB (75000651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:3687a2a597d4cbbad7b97d9d1c8d002ebc4529d1774ff414ce9b75e6ea5824b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386045599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2efceac15694febc23a6a434c28d41da0ef1606d59325eb677cbaca9514e4529`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:11:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:11:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:16:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:16:15 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:16:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:17:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7fca3839c8bd4903e2ee5f523935fb729f15724615fd9f77ce0d6cc2adbfa6`  
		Last Modified: Thu, 16 Mar 2023 03:39:00 GMT  
		Size: 820.1 KB (820097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3f218bb6743682d83611cfd2ae16145e67489129eccf76d1236a70b3a5bcac`  
		Last Modified: Thu, 16 Mar 2023 03:38:59 GMT  
		Size: 4.1 MB (4090687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1bf44a1167e1c920f67efd944ec51807eb500e2fea8c0103e3a0d46a52fc32`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ed9b280b6ac98a36e5f3f6a1cdeba5961c20493eddf18a97a0b9db954fa6e`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cea9e95a56ecce8cbb02ffdcdcb3059f16577e473b546648bf64fd56a319a1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:32 GMT  
		Size: 239.0 MB (239044585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9735bdd7bdcf6fcc5f9450057e43d66daabf09facf6269f79ba9fabe328adba`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dac314ffbb6434ef884f3647e224f3b30f1018f02b797077c272e6e18bf8339`  
		Last Modified: Thu, 16 Mar 2023 03:39:49 GMT  
		Size: 54.7 MB (54734178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54e23bfe2054492ace7dfe9733463a7ec3acdb0fde54945898eb6183e0dc9`  
		Last Modified: Thu, 16 Mar 2023 03:39:42 GMT  
		Size: 297.9 KB (297866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec2cdeae69a7086e37719ef96fc503992f0d4b2d60728205ec438444deda1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:53 GMT  
		Size: 64.8 MB (64750962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2ab5dc9b90d0595d56f9c237a7f3dc6486fb1f55ead2821374f62af860643cce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412182292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55011a93bd285ce6f41688a9ece2ac5baa2706064aa4762eaf70c4212d94b8f6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 02:56:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:00:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:50 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:00:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:00:50 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:01:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:01:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d56daf02ac303e7c230365644aca63ed850ebf40d29e81a5814308c13562239`  
		Last Modified: Thu, 16 Mar 2023 03:44:18 GMT  
		Size: 819.9 KB (819945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b83e85404464664e50669adc31927b351faa0e1bf21c647f66d7f27782fdb61`  
		Last Modified: Thu, 16 Mar 2023 03:44:16 GMT  
		Size: 4.5 MB (4462823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a184771f70aafd7d78ff51d90244556b28011bac2d29106066a25ba9e96dc089`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074f6bcd0b3bae9f4c581397d152b553279dd7184769c00f73e89f9ae5a2d1a`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4bc60dd1e1c3f4aaade0438967ef0ad4f929678ad0595f68c97aa6802e3508`  
		Last Modified: Thu, 16 Mar 2023 03:44:48 GMT  
		Size: 252.5 MB (252534995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f4fb4d9a35efa338820eac3e26a8095ab5dee1791a6486ba31cb576260bca`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fde270ea5c1652055c01f32fcccb425820da092a3595a17a1b46328120b1aff`  
		Last Modified: Thu, 16 Mar 2023 03:45:04 GMT  
		Size: 63.1 MB (63094293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b8e237fc97a182dc544c752d16ac1ce2e83c4d08538a122d43f03c33340a7e`  
		Last Modified: Thu, 16 Mar 2023 03:44:57 GMT  
		Size: 297.9 KB (297879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab7b64ecca2bb014b31a49a16d2dcd2856db7487d4967731df87dcc2c2b990d`  
		Last Modified: Thu, 16 Mar 2023 03:45:07 GMT  
		Size: 67.2 MB (67235800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:46d9cd2287d09d74a01c576064ecb03aafe56c91fbb9e5372022e787ac1b5428
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:6ebcac686524dae60060f7934db8334f5ff22418d2de833c3893b8af4bf5fd26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **743.3 MB (743270868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11c6649f5fc3cdcd4cfbce033238df0943655944c1732d1b9766ed9d7bb3a645`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:58:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 04:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:00:33 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:00:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:01:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:08:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73b43b50fc9056c1213c61cfa3193cd15f8faa751905b21e0e9019473426a74`  
		Last Modified: Thu, 16 Mar 2023 03:11:48 GMT  
		Size: 819.0 KB (818997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6111169e4c0857f4eaf38437fa0beb5e0f66979105b8fdfd3c85c5c5e1544992`  
		Last Modified: Thu, 16 Mar 2023 04:41:15 GMT  
		Size: 4.9 MB (4878581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280739d0ef2f7bb759ccb3b3bb8a5f15a3d1ee562afe99609a493c65039b87a6`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d189808242488a25bc31490cfec5360bcb99b6a965f8782e6af80cf69e81ad79`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc74d1ea892a60a383eaee3d39a2f94fcd19fa347ee48e940f7152e5a8d6bccb`  
		Last Modified: Thu, 16 Mar 2023 04:41:48 GMT  
		Size: 259.6 MB (259588669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43567d3a1b9a70a0e7ec7a689892a144345cf9bcb6eb4151afba22b1eab2d47e`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc128d1e3275f672a35efb8cc6d100ff910f036dc6bbfdb5d0beea7ba5a48370`  
		Last Modified: Thu, 16 Mar 2023 04:42:06 GMT  
		Size: 70.3 MB (70268059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3dceb46441b9a8de4be3a53517c7cf44efe430d819993027ffd084b6dc13b`  
		Last Modified: Thu, 16 Mar 2023 04:41:57 GMT  
		Size: 297.9 KB (297878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1901e3f6c09a6bb1a3a48da8fb1162deb79e4a57ae416e9ca5b86ec2e21cab3d`  
		Last Modified: Thu, 16 Mar 2023 04:42:08 GMT  
		Size: 75.0 MB (75000651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f76ac290ed6dbc97a801a28b1443aadd357409d21fc2e785e19d38432442de1`  
		Last Modified: Thu, 16 Mar 2023 04:43:16 GMT  
		Size: 305.7 MB (305705440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:39561d0b6ec44c224c00f1b16c57f348f311bc567d36d05875a14448d863483a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.4 MB (646369319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b433cb583adbfb375a1ca5f8b50fc6abf1241337355042752855124ae4db84dd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:11:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:11:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:16:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:16:15 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:16:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:17:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7fca3839c8bd4903e2ee5f523935fb729f15724615fd9f77ce0d6cc2adbfa6`  
		Last Modified: Thu, 16 Mar 2023 03:39:00 GMT  
		Size: 820.1 KB (820097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3f218bb6743682d83611cfd2ae16145e67489129eccf76d1236a70b3a5bcac`  
		Last Modified: Thu, 16 Mar 2023 03:38:59 GMT  
		Size: 4.1 MB (4090687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1bf44a1167e1c920f67efd944ec51807eb500e2fea8c0103e3a0d46a52fc32`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ed9b280b6ac98a36e5f3f6a1cdeba5961c20493eddf18a97a0b9db954fa6e`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cea9e95a56ecce8cbb02ffdcdcb3059f16577e473b546648bf64fd56a319a1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:32 GMT  
		Size: 239.0 MB (239044585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9735bdd7bdcf6fcc5f9450057e43d66daabf09facf6269f79ba9fabe328adba`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dac314ffbb6434ef884f3647e224f3b30f1018f02b797077c272e6e18bf8339`  
		Last Modified: Thu, 16 Mar 2023 03:39:49 GMT  
		Size: 54.7 MB (54734178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54e23bfe2054492ace7dfe9733463a7ec3acdb0fde54945898eb6183e0dc9`  
		Last Modified: Thu, 16 Mar 2023 03:39:42 GMT  
		Size: 297.9 KB (297866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec2cdeae69a7086e37719ef96fc503992f0d4b2d60728205ec438444deda1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:53 GMT  
		Size: 64.8 MB (64750962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25453f1f7d77cde07001a7e016b416aaf6637503b5cab1f7988a543de5b4628e`  
		Last Modified: Thu, 16 Mar 2023 03:40:55 GMT  
		Size: 260.3 MB (260323720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3d617c256b88392d689fcdc2194574e311ca9be80a0332969ccfff511647b733
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.2 MB (704189335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8771c555c6c72adef44ae8792d23e66479fab63afaba617621924c1f030e3c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 02:56:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:00:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:50 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:00:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:00:50 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:01:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:01:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:09:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d56daf02ac303e7c230365644aca63ed850ebf40d29e81a5814308c13562239`  
		Last Modified: Thu, 16 Mar 2023 03:44:18 GMT  
		Size: 819.9 KB (819945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b83e85404464664e50669adc31927b351faa0e1bf21c647f66d7f27782fdb61`  
		Last Modified: Thu, 16 Mar 2023 03:44:16 GMT  
		Size: 4.5 MB (4462823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a184771f70aafd7d78ff51d90244556b28011bac2d29106066a25ba9e96dc089`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074f6bcd0b3bae9f4c581397d152b553279dd7184769c00f73e89f9ae5a2d1a`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4bc60dd1e1c3f4aaade0438967ef0ad4f929678ad0595f68c97aa6802e3508`  
		Last Modified: Thu, 16 Mar 2023 03:44:48 GMT  
		Size: 252.5 MB (252534995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f4fb4d9a35efa338820eac3e26a8095ab5dee1791a6486ba31cb576260bca`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fde270ea5c1652055c01f32fcccb425820da092a3595a17a1b46328120b1aff`  
		Last Modified: Thu, 16 Mar 2023 03:45:04 GMT  
		Size: 63.1 MB (63094293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b8e237fc97a182dc544c752d16ac1ce2e83c4d08538a122d43f03c33340a7e`  
		Last Modified: Thu, 16 Mar 2023 03:44:57 GMT  
		Size: 297.9 KB (297879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab7b64ecca2bb014b31a49a16d2dcd2856db7487d4967731df87dcc2c2b990d`  
		Last Modified: Thu, 16 Mar 2023 03:45:07 GMT  
		Size: 67.2 MB (67235800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbf4b10d8dd4c11a655da224aa3a248e1ecbec6989f61e629628fb42120b997`  
		Last Modified: Thu, 16 Mar 2023 03:46:05 GMT  
		Size: 292.0 MB (292007043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:46d9cd2287d09d74a01c576064ecb03aafe56c91fbb9e5372022e787ac1b5428
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:6ebcac686524dae60060f7934db8334f5ff22418d2de833c3893b8af4bf5fd26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **743.3 MB (743270868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11c6649f5fc3cdcd4cfbce033238df0943655944c1732d1b9766ed9d7bb3a645`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:58:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 04:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:00:33 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:00:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:01:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:08:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73b43b50fc9056c1213c61cfa3193cd15f8faa751905b21e0e9019473426a74`  
		Last Modified: Thu, 16 Mar 2023 03:11:48 GMT  
		Size: 819.0 KB (818997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6111169e4c0857f4eaf38437fa0beb5e0f66979105b8fdfd3c85c5c5e1544992`  
		Last Modified: Thu, 16 Mar 2023 04:41:15 GMT  
		Size: 4.9 MB (4878581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280739d0ef2f7bb759ccb3b3bb8a5f15a3d1ee562afe99609a493c65039b87a6`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d189808242488a25bc31490cfec5360bcb99b6a965f8782e6af80cf69e81ad79`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc74d1ea892a60a383eaee3d39a2f94fcd19fa347ee48e940f7152e5a8d6bccb`  
		Last Modified: Thu, 16 Mar 2023 04:41:48 GMT  
		Size: 259.6 MB (259588669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43567d3a1b9a70a0e7ec7a689892a144345cf9bcb6eb4151afba22b1eab2d47e`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc128d1e3275f672a35efb8cc6d100ff910f036dc6bbfdb5d0beea7ba5a48370`  
		Last Modified: Thu, 16 Mar 2023 04:42:06 GMT  
		Size: 70.3 MB (70268059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3dceb46441b9a8de4be3a53517c7cf44efe430d819993027ffd084b6dc13b`  
		Last Modified: Thu, 16 Mar 2023 04:41:57 GMT  
		Size: 297.9 KB (297878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1901e3f6c09a6bb1a3a48da8fb1162deb79e4a57ae416e9ca5b86ec2e21cab3d`  
		Last Modified: Thu, 16 Mar 2023 04:42:08 GMT  
		Size: 75.0 MB (75000651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f76ac290ed6dbc97a801a28b1443aadd357409d21fc2e785e19d38432442de1`  
		Last Modified: Thu, 16 Mar 2023 04:43:16 GMT  
		Size: 305.7 MB (305705440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:39561d0b6ec44c224c00f1b16c57f348f311bc567d36d05875a14448d863483a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.4 MB (646369319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b433cb583adbfb375a1ca5f8b50fc6abf1241337355042752855124ae4db84dd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:11:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:11:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:16:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:16:15 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:16:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:17:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7fca3839c8bd4903e2ee5f523935fb729f15724615fd9f77ce0d6cc2adbfa6`  
		Last Modified: Thu, 16 Mar 2023 03:39:00 GMT  
		Size: 820.1 KB (820097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3f218bb6743682d83611cfd2ae16145e67489129eccf76d1236a70b3a5bcac`  
		Last Modified: Thu, 16 Mar 2023 03:38:59 GMT  
		Size: 4.1 MB (4090687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1bf44a1167e1c920f67efd944ec51807eb500e2fea8c0103e3a0d46a52fc32`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ed9b280b6ac98a36e5f3f6a1cdeba5961c20493eddf18a97a0b9db954fa6e`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cea9e95a56ecce8cbb02ffdcdcb3059f16577e473b546648bf64fd56a319a1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:32 GMT  
		Size: 239.0 MB (239044585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9735bdd7bdcf6fcc5f9450057e43d66daabf09facf6269f79ba9fabe328adba`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dac314ffbb6434ef884f3647e224f3b30f1018f02b797077c272e6e18bf8339`  
		Last Modified: Thu, 16 Mar 2023 03:39:49 GMT  
		Size: 54.7 MB (54734178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54e23bfe2054492ace7dfe9733463a7ec3acdb0fde54945898eb6183e0dc9`  
		Last Modified: Thu, 16 Mar 2023 03:39:42 GMT  
		Size: 297.9 KB (297866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec2cdeae69a7086e37719ef96fc503992f0d4b2d60728205ec438444deda1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:53 GMT  
		Size: 64.8 MB (64750962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25453f1f7d77cde07001a7e016b416aaf6637503b5cab1f7988a543de5b4628e`  
		Last Modified: Thu, 16 Mar 2023 03:40:55 GMT  
		Size: 260.3 MB (260323720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3d617c256b88392d689fcdc2194574e311ca9be80a0332969ccfff511647b733
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.2 MB (704189335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8771c555c6c72adef44ae8792d23e66479fab63afaba617621924c1f030e3c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 02:56:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:00:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:50 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:00:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:00:50 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:01:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:01:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:09:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d56daf02ac303e7c230365644aca63ed850ebf40d29e81a5814308c13562239`  
		Last Modified: Thu, 16 Mar 2023 03:44:18 GMT  
		Size: 819.9 KB (819945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b83e85404464664e50669adc31927b351faa0e1bf21c647f66d7f27782fdb61`  
		Last Modified: Thu, 16 Mar 2023 03:44:16 GMT  
		Size: 4.5 MB (4462823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a184771f70aafd7d78ff51d90244556b28011bac2d29106066a25ba9e96dc089`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074f6bcd0b3bae9f4c581397d152b553279dd7184769c00f73e89f9ae5a2d1a`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4bc60dd1e1c3f4aaade0438967ef0ad4f929678ad0595f68c97aa6802e3508`  
		Last Modified: Thu, 16 Mar 2023 03:44:48 GMT  
		Size: 252.5 MB (252534995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f4fb4d9a35efa338820eac3e26a8095ab5dee1791a6486ba31cb576260bca`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fde270ea5c1652055c01f32fcccb425820da092a3595a17a1b46328120b1aff`  
		Last Modified: Thu, 16 Mar 2023 03:45:04 GMT  
		Size: 63.1 MB (63094293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b8e237fc97a182dc544c752d16ac1ce2e83c4d08538a122d43f03c33340a7e`  
		Last Modified: Thu, 16 Mar 2023 03:44:57 GMT  
		Size: 297.9 KB (297879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab7b64ecca2bb014b31a49a16d2dcd2856db7487d4967731df87dcc2c2b990d`  
		Last Modified: Thu, 16 Mar 2023 03:45:07 GMT  
		Size: 67.2 MB (67235800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbf4b10d8dd4c11a655da224aa3a248e1ecbec6989f61e629628fb42120b997`  
		Last Modified: Thu, 16 Mar 2023 03:46:05 GMT  
		Size: 292.0 MB (292007043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:d16b38b062ff41bb9a5f9ecca69a5c84e72d3cb0322e4aab4a422cc9ed1f1d42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:23d8dbab51038f248d2d19a1777a731af2b53008955e098cf5b0b9a7c9ec10b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.7 MB (448652161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f043259d2a2626442c70c295a13dfe775b25fd522ffdbb6eddf514edbfcc4b60`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:58:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 04:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:00:33 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:00:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:01:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:03:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73b43b50fc9056c1213c61cfa3193cd15f8faa751905b21e0e9019473426a74`  
		Last Modified: Thu, 16 Mar 2023 03:11:48 GMT  
		Size: 819.0 KB (818997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6111169e4c0857f4eaf38437fa0beb5e0f66979105b8fdfd3c85c5c5e1544992`  
		Last Modified: Thu, 16 Mar 2023 04:41:15 GMT  
		Size: 4.9 MB (4878581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280739d0ef2f7bb759ccb3b3bb8a5f15a3d1ee562afe99609a493c65039b87a6`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d189808242488a25bc31490cfec5360bcb99b6a965f8782e6af80cf69e81ad79`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc74d1ea892a60a383eaee3d39a2f94fcd19fa347ee48e940f7152e5a8d6bccb`  
		Last Modified: Thu, 16 Mar 2023 04:41:48 GMT  
		Size: 259.6 MB (259588669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43567d3a1b9a70a0e7ec7a689892a144345cf9bcb6eb4151afba22b1eab2d47e`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc128d1e3275f672a35efb8cc6d100ff910f036dc6bbfdb5d0beea7ba5a48370`  
		Last Modified: Thu, 16 Mar 2023 04:42:06 GMT  
		Size: 70.3 MB (70268059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3dceb46441b9a8de4be3a53517c7cf44efe430d819993027ffd084b6dc13b`  
		Last Modified: Thu, 16 Mar 2023 04:41:57 GMT  
		Size: 297.9 KB (297878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1901e3f6c09a6bb1a3a48da8fb1162deb79e4a57ae416e9ca5b86ec2e21cab3d`  
		Last Modified: Thu, 16 Mar 2023 04:42:08 GMT  
		Size: 75.0 MB (75000651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2931bcf3ec12937e9d6e316229b002c7515d449faaafafa0db8522e959dbde94`  
		Last Modified: Thu, 16 Mar 2023 04:42:22 GMT  
		Size: 11.1 MB (11086733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:289b5773ca6f48c9b33f6e78d3927d5f8ce82e30caa4f1796bedace63ec7062c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396169033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8fe266a72b185cf1431c8a4d377037aaa4b7bbcbe8656658935c11696fd107d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:11:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:11:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:16:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:16:15 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:16:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:17:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7fca3839c8bd4903e2ee5f523935fb729f15724615fd9f77ce0d6cc2adbfa6`  
		Last Modified: Thu, 16 Mar 2023 03:39:00 GMT  
		Size: 820.1 KB (820097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3f218bb6743682d83611cfd2ae16145e67489129eccf76d1236a70b3a5bcac`  
		Last Modified: Thu, 16 Mar 2023 03:38:59 GMT  
		Size: 4.1 MB (4090687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1bf44a1167e1c920f67efd944ec51807eb500e2fea8c0103e3a0d46a52fc32`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ed9b280b6ac98a36e5f3f6a1cdeba5961c20493eddf18a97a0b9db954fa6e`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cea9e95a56ecce8cbb02ffdcdcb3059f16577e473b546648bf64fd56a319a1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:32 GMT  
		Size: 239.0 MB (239044585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9735bdd7bdcf6fcc5f9450057e43d66daabf09facf6269f79ba9fabe328adba`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dac314ffbb6434ef884f3647e224f3b30f1018f02b797077c272e6e18bf8339`  
		Last Modified: Thu, 16 Mar 2023 03:39:49 GMT  
		Size: 54.7 MB (54734178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54e23bfe2054492ace7dfe9733463a7ec3acdb0fde54945898eb6183e0dc9`  
		Last Modified: Thu, 16 Mar 2023 03:39:42 GMT  
		Size: 297.9 KB (297866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec2cdeae69a7086e37719ef96fc503992f0d4b2d60728205ec438444deda1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:53 GMT  
		Size: 64.8 MB (64750962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7634457b9c881ce425d9d01bdff94fd83b012daa031b020cabb98af51b26e5ef`  
		Last Modified: Thu, 16 Mar 2023 03:40:09 GMT  
		Size: 10.1 MB (10123434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c0a0a8a25dc822ea48b40c45d74b267ddf4dbe22b8accc9fd66bb146c34eb974
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422923396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916440a18deb3d20ae03381c36c2693e05070e1e703b8b2f66e74168127dce44`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 02:56:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:00:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:50 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:00:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:00:50 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:01:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:01:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d56daf02ac303e7c230365644aca63ed850ebf40d29e81a5814308c13562239`  
		Last Modified: Thu, 16 Mar 2023 03:44:18 GMT  
		Size: 819.9 KB (819945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b83e85404464664e50669adc31927b351faa0e1bf21c647f66d7f27782fdb61`  
		Last Modified: Thu, 16 Mar 2023 03:44:16 GMT  
		Size: 4.5 MB (4462823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a184771f70aafd7d78ff51d90244556b28011bac2d29106066a25ba9e96dc089`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074f6bcd0b3bae9f4c581397d152b553279dd7184769c00f73e89f9ae5a2d1a`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4bc60dd1e1c3f4aaade0438967ef0ad4f929678ad0595f68c97aa6802e3508`  
		Last Modified: Thu, 16 Mar 2023 03:44:48 GMT  
		Size: 252.5 MB (252534995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f4fb4d9a35efa338820eac3e26a8095ab5dee1791a6486ba31cb576260bca`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fde270ea5c1652055c01f32fcccb425820da092a3595a17a1b46328120b1aff`  
		Last Modified: Thu, 16 Mar 2023 03:45:04 GMT  
		Size: 63.1 MB (63094293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b8e237fc97a182dc544c752d16ac1ce2e83c4d08538a122d43f03c33340a7e`  
		Last Modified: Thu, 16 Mar 2023 03:44:57 GMT  
		Size: 297.9 KB (297879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab7b64ecca2bb014b31a49a16d2dcd2856db7487d4967731df87dcc2c2b990d`  
		Last Modified: Thu, 16 Mar 2023 03:45:07 GMT  
		Size: 67.2 MB (67235800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1391b68cbd182ee0c5bb36c626732e1b8182df4ec25d7ad2c636d92cd8428df`  
		Last Modified: Thu, 16 Mar 2023 03:45:21 GMT  
		Size: 10.7 MB (10741104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:d16b38b062ff41bb9a5f9ecca69a5c84e72d3cb0322e4aab4a422cc9ed1f1d42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:23d8dbab51038f248d2d19a1777a731af2b53008955e098cf5b0b9a7c9ec10b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.7 MB (448652161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f043259d2a2626442c70c295a13dfe775b25fd522ffdbb6eddf514edbfcc4b60`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:58:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 04:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:00:33 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:00:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:01:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:03:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73b43b50fc9056c1213c61cfa3193cd15f8faa751905b21e0e9019473426a74`  
		Last Modified: Thu, 16 Mar 2023 03:11:48 GMT  
		Size: 819.0 KB (818997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6111169e4c0857f4eaf38437fa0beb5e0f66979105b8fdfd3c85c5c5e1544992`  
		Last Modified: Thu, 16 Mar 2023 04:41:15 GMT  
		Size: 4.9 MB (4878581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280739d0ef2f7bb759ccb3b3bb8a5f15a3d1ee562afe99609a493c65039b87a6`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d189808242488a25bc31490cfec5360bcb99b6a965f8782e6af80cf69e81ad79`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc74d1ea892a60a383eaee3d39a2f94fcd19fa347ee48e940f7152e5a8d6bccb`  
		Last Modified: Thu, 16 Mar 2023 04:41:48 GMT  
		Size: 259.6 MB (259588669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43567d3a1b9a70a0e7ec7a689892a144345cf9bcb6eb4151afba22b1eab2d47e`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc128d1e3275f672a35efb8cc6d100ff910f036dc6bbfdb5d0beea7ba5a48370`  
		Last Modified: Thu, 16 Mar 2023 04:42:06 GMT  
		Size: 70.3 MB (70268059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3dceb46441b9a8de4be3a53517c7cf44efe430d819993027ffd084b6dc13b`  
		Last Modified: Thu, 16 Mar 2023 04:41:57 GMT  
		Size: 297.9 KB (297878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1901e3f6c09a6bb1a3a48da8fb1162deb79e4a57ae416e9ca5b86ec2e21cab3d`  
		Last Modified: Thu, 16 Mar 2023 04:42:08 GMT  
		Size: 75.0 MB (75000651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2931bcf3ec12937e9d6e316229b002c7515d449faaafafa0db8522e959dbde94`  
		Last Modified: Thu, 16 Mar 2023 04:42:22 GMT  
		Size: 11.1 MB (11086733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:289b5773ca6f48c9b33f6e78d3927d5f8ce82e30caa4f1796bedace63ec7062c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396169033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8fe266a72b185cf1431c8a4d377037aaa4b7bbcbe8656658935c11696fd107d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:11:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:11:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:16:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:16:15 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:16:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:17:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7fca3839c8bd4903e2ee5f523935fb729f15724615fd9f77ce0d6cc2adbfa6`  
		Last Modified: Thu, 16 Mar 2023 03:39:00 GMT  
		Size: 820.1 KB (820097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3f218bb6743682d83611cfd2ae16145e67489129eccf76d1236a70b3a5bcac`  
		Last Modified: Thu, 16 Mar 2023 03:38:59 GMT  
		Size: 4.1 MB (4090687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1bf44a1167e1c920f67efd944ec51807eb500e2fea8c0103e3a0d46a52fc32`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ed9b280b6ac98a36e5f3f6a1cdeba5961c20493eddf18a97a0b9db954fa6e`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cea9e95a56ecce8cbb02ffdcdcb3059f16577e473b546648bf64fd56a319a1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:32 GMT  
		Size: 239.0 MB (239044585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9735bdd7bdcf6fcc5f9450057e43d66daabf09facf6269f79ba9fabe328adba`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dac314ffbb6434ef884f3647e224f3b30f1018f02b797077c272e6e18bf8339`  
		Last Modified: Thu, 16 Mar 2023 03:39:49 GMT  
		Size: 54.7 MB (54734178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54e23bfe2054492ace7dfe9733463a7ec3acdb0fde54945898eb6183e0dc9`  
		Last Modified: Thu, 16 Mar 2023 03:39:42 GMT  
		Size: 297.9 KB (297866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec2cdeae69a7086e37719ef96fc503992f0d4b2d60728205ec438444deda1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:53 GMT  
		Size: 64.8 MB (64750962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7634457b9c881ce425d9d01bdff94fd83b012daa031b020cabb98af51b26e5ef`  
		Last Modified: Thu, 16 Mar 2023 03:40:09 GMT  
		Size: 10.1 MB (10123434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c0a0a8a25dc822ea48b40c45d74b267ddf4dbe22b8accc9fd66bb146c34eb974
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422923396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916440a18deb3d20ae03381c36c2693e05070e1e703b8b2f66e74168127dce44`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 02:56:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:00:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:50 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:00:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:00:50 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:01:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:01:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d56daf02ac303e7c230365644aca63ed850ebf40d29e81a5814308c13562239`  
		Last Modified: Thu, 16 Mar 2023 03:44:18 GMT  
		Size: 819.9 KB (819945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b83e85404464664e50669adc31927b351faa0e1bf21c647f66d7f27782fdb61`  
		Last Modified: Thu, 16 Mar 2023 03:44:16 GMT  
		Size: 4.5 MB (4462823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a184771f70aafd7d78ff51d90244556b28011bac2d29106066a25ba9e96dc089`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074f6bcd0b3bae9f4c581397d152b553279dd7184769c00f73e89f9ae5a2d1a`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4bc60dd1e1c3f4aaade0438967ef0ad4f929678ad0595f68c97aa6802e3508`  
		Last Modified: Thu, 16 Mar 2023 03:44:48 GMT  
		Size: 252.5 MB (252534995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f4fb4d9a35efa338820eac3e26a8095ab5dee1791a6486ba31cb576260bca`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fde270ea5c1652055c01f32fcccb425820da092a3595a17a1b46328120b1aff`  
		Last Modified: Thu, 16 Mar 2023 03:45:04 GMT  
		Size: 63.1 MB (63094293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b8e237fc97a182dc544c752d16ac1ce2e83c4d08538a122d43f03c33340a7e`  
		Last Modified: Thu, 16 Mar 2023 03:44:57 GMT  
		Size: 297.9 KB (297879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab7b64ecca2bb014b31a49a16d2dcd2856db7487d4967731df87dcc2c2b990d`  
		Last Modified: Thu, 16 Mar 2023 03:45:07 GMT  
		Size: 67.2 MB (67235800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1391b68cbd182ee0c5bb36c626732e1b8182df4ec25d7ad2c636d92cd8428df`  
		Last Modified: Thu, 16 Mar 2023 03:45:21 GMT  
		Size: 10.7 MB (10741104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:45e9441e2496f7ac90aa11d3a132fe5feaac7c5a42d7ff8ad6f3268a6e9f5526
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:8cfd2b761f6398ff60cc52321cb275c7f4619d88007315bdbcdbe348d309c433
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.6 MB (437565428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ffed69de06cc91173726d899c430f78440e25b31702da04ba83af365fa684`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:58:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 04:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:00:33 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:00:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:01:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73b43b50fc9056c1213c61cfa3193cd15f8faa751905b21e0e9019473426a74`  
		Last Modified: Thu, 16 Mar 2023 03:11:48 GMT  
		Size: 819.0 KB (818997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6111169e4c0857f4eaf38437fa0beb5e0f66979105b8fdfd3c85c5c5e1544992`  
		Last Modified: Thu, 16 Mar 2023 04:41:15 GMT  
		Size: 4.9 MB (4878581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280739d0ef2f7bb759ccb3b3bb8a5f15a3d1ee562afe99609a493c65039b87a6`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d189808242488a25bc31490cfec5360bcb99b6a965f8782e6af80cf69e81ad79`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc74d1ea892a60a383eaee3d39a2f94fcd19fa347ee48e940f7152e5a8d6bccb`  
		Last Modified: Thu, 16 Mar 2023 04:41:48 GMT  
		Size: 259.6 MB (259588669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43567d3a1b9a70a0e7ec7a689892a144345cf9bcb6eb4151afba22b1eab2d47e`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc128d1e3275f672a35efb8cc6d100ff910f036dc6bbfdb5d0beea7ba5a48370`  
		Last Modified: Thu, 16 Mar 2023 04:42:06 GMT  
		Size: 70.3 MB (70268059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3dceb46441b9a8de4be3a53517c7cf44efe430d819993027ffd084b6dc13b`  
		Last Modified: Thu, 16 Mar 2023 04:41:57 GMT  
		Size: 297.9 KB (297878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1901e3f6c09a6bb1a3a48da8fb1162deb79e4a57ae416e9ca5b86ec2e21cab3d`  
		Last Modified: Thu, 16 Mar 2023 04:42:08 GMT  
		Size: 75.0 MB (75000651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:3687a2a597d4cbbad7b97d9d1c8d002ebc4529d1774ff414ce9b75e6ea5824b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386045599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2efceac15694febc23a6a434c28d41da0ef1606d59325eb677cbaca9514e4529`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:11:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:11:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:16:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:16:15 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:16:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:17:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7fca3839c8bd4903e2ee5f523935fb729f15724615fd9f77ce0d6cc2adbfa6`  
		Last Modified: Thu, 16 Mar 2023 03:39:00 GMT  
		Size: 820.1 KB (820097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3f218bb6743682d83611cfd2ae16145e67489129eccf76d1236a70b3a5bcac`  
		Last Modified: Thu, 16 Mar 2023 03:38:59 GMT  
		Size: 4.1 MB (4090687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1bf44a1167e1c920f67efd944ec51807eb500e2fea8c0103e3a0d46a52fc32`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ed9b280b6ac98a36e5f3f6a1cdeba5961c20493eddf18a97a0b9db954fa6e`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cea9e95a56ecce8cbb02ffdcdcb3059f16577e473b546648bf64fd56a319a1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:32 GMT  
		Size: 239.0 MB (239044585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9735bdd7bdcf6fcc5f9450057e43d66daabf09facf6269f79ba9fabe328adba`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dac314ffbb6434ef884f3647e224f3b30f1018f02b797077c272e6e18bf8339`  
		Last Modified: Thu, 16 Mar 2023 03:39:49 GMT  
		Size: 54.7 MB (54734178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54e23bfe2054492ace7dfe9733463a7ec3acdb0fde54945898eb6183e0dc9`  
		Last Modified: Thu, 16 Mar 2023 03:39:42 GMT  
		Size: 297.9 KB (297866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec2cdeae69a7086e37719ef96fc503992f0d4b2d60728205ec438444deda1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:53 GMT  
		Size: 64.8 MB (64750962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2ab5dc9b90d0595d56f9c237a7f3dc6486fb1f55ead2821374f62af860643cce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412182292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55011a93bd285ce6f41688a9ece2ac5baa2706064aa4762eaf70c4212d94b8f6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 02:56:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:00:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:50 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:00:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:00:50 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:01:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:01:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d56daf02ac303e7c230365644aca63ed850ebf40d29e81a5814308c13562239`  
		Last Modified: Thu, 16 Mar 2023 03:44:18 GMT  
		Size: 819.9 KB (819945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b83e85404464664e50669adc31927b351faa0e1bf21c647f66d7f27782fdb61`  
		Last Modified: Thu, 16 Mar 2023 03:44:16 GMT  
		Size: 4.5 MB (4462823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a184771f70aafd7d78ff51d90244556b28011bac2d29106066a25ba9e96dc089`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074f6bcd0b3bae9f4c581397d152b553279dd7184769c00f73e89f9ae5a2d1a`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4bc60dd1e1c3f4aaade0438967ef0ad4f929678ad0595f68c97aa6802e3508`  
		Last Modified: Thu, 16 Mar 2023 03:44:48 GMT  
		Size: 252.5 MB (252534995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f4fb4d9a35efa338820eac3e26a8095ab5dee1791a6486ba31cb576260bca`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fde270ea5c1652055c01f32fcccb425820da092a3595a17a1b46328120b1aff`  
		Last Modified: Thu, 16 Mar 2023 03:45:04 GMT  
		Size: 63.1 MB (63094293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b8e237fc97a182dc544c752d16ac1ce2e83c4d08538a122d43f03c33340a7e`  
		Last Modified: Thu, 16 Mar 2023 03:44:57 GMT  
		Size: 297.9 KB (297879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab7b64ecca2bb014b31a49a16d2dcd2856db7487d4967731df87dcc2c2b990d`  
		Last Modified: Thu, 16 Mar 2023 03:45:07 GMT  
		Size: 67.2 MB (67235800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:45e9441e2496f7ac90aa11d3a132fe5feaac7c5a42d7ff8ad6f3268a6e9f5526
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:8cfd2b761f6398ff60cc52321cb275c7f4619d88007315bdbcdbe348d309c433
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.6 MB (437565428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ffed69de06cc91173726d899c430f78440e25b31702da04ba83af365fa684`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:58:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 04:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:00:33 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:00:34 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:01:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73b43b50fc9056c1213c61cfa3193cd15f8faa751905b21e0e9019473426a74`  
		Last Modified: Thu, 16 Mar 2023 03:11:48 GMT  
		Size: 819.0 KB (818997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6111169e4c0857f4eaf38437fa0beb5e0f66979105b8fdfd3c85c5c5e1544992`  
		Last Modified: Thu, 16 Mar 2023 04:41:15 GMT  
		Size: 4.9 MB (4878581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280739d0ef2f7bb759ccb3b3bb8a5f15a3d1ee562afe99609a493c65039b87a6`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d189808242488a25bc31490cfec5360bcb99b6a965f8782e6af80cf69e81ad79`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc74d1ea892a60a383eaee3d39a2f94fcd19fa347ee48e940f7152e5a8d6bccb`  
		Last Modified: Thu, 16 Mar 2023 04:41:48 GMT  
		Size: 259.6 MB (259588669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43567d3a1b9a70a0e7ec7a689892a144345cf9bcb6eb4151afba22b1eab2d47e`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc128d1e3275f672a35efb8cc6d100ff910f036dc6bbfdb5d0beea7ba5a48370`  
		Last Modified: Thu, 16 Mar 2023 04:42:06 GMT  
		Size: 70.3 MB (70268059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3dceb46441b9a8de4be3a53517c7cf44efe430d819993027ffd084b6dc13b`  
		Last Modified: Thu, 16 Mar 2023 04:41:57 GMT  
		Size: 297.9 KB (297878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1901e3f6c09a6bb1a3a48da8fb1162deb79e4a57ae416e9ca5b86ec2e21cab3d`  
		Last Modified: Thu, 16 Mar 2023 04:42:08 GMT  
		Size: 75.0 MB (75000651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:3687a2a597d4cbbad7b97d9d1c8d002ebc4529d1774ff414ce9b75e6ea5824b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386045599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2efceac15694febc23a6a434c28d41da0ef1606d59325eb677cbaca9514e4529`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:11:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:11:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:16:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:16:15 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:16:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:17:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7fca3839c8bd4903e2ee5f523935fb729f15724615fd9f77ce0d6cc2adbfa6`  
		Last Modified: Thu, 16 Mar 2023 03:39:00 GMT  
		Size: 820.1 KB (820097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3f218bb6743682d83611cfd2ae16145e67489129eccf76d1236a70b3a5bcac`  
		Last Modified: Thu, 16 Mar 2023 03:38:59 GMT  
		Size: 4.1 MB (4090687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1bf44a1167e1c920f67efd944ec51807eb500e2fea8c0103e3a0d46a52fc32`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ed9b280b6ac98a36e5f3f6a1cdeba5961c20493eddf18a97a0b9db954fa6e`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cea9e95a56ecce8cbb02ffdcdcb3059f16577e473b546648bf64fd56a319a1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:32 GMT  
		Size: 239.0 MB (239044585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9735bdd7bdcf6fcc5f9450057e43d66daabf09facf6269f79ba9fabe328adba`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dac314ffbb6434ef884f3647e224f3b30f1018f02b797077c272e6e18bf8339`  
		Last Modified: Thu, 16 Mar 2023 03:39:49 GMT  
		Size: 54.7 MB (54734178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54e23bfe2054492ace7dfe9733463a7ec3acdb0fde54945898eb6183e0dc9`  
		Last Modified: Thu, 16 Mar 2023 03:39:42 GMT  
		Size: 297.9 KB (297866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec2cdeae69a7086e37719ef96fc503992f0d4b2d60728205ec438444deda1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:53 GMT  
		Size: 64.8 MB (64750962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2ab5dc9b90d0595d56f9c237a7f3dc6486fb1f55ead2821374f62af860643cce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412182292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55011a93bd285ce6f41688a9ece2ac5baa2706064aa4762eaf70c4212d94b8f6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 02:56:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:00:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:50 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:00:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:00:50 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:01:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:01:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d56daf02ac303e7c230365644aca63ed850ebf40d29e81a5814308c13562239`  
		Last Modified: Thu, 16 Mar 2023 03:44:18 GMT  
		Size: 819.9 KB (819945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b83e85404464664e50669adc31927b351faa0e1bf21c647f66d7f27782fdb61`  
		Last Modified: Thu, 16 Mar 2023 03:44:16 GMT  
		Size: 4.5 MB (4462823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a184771f70aafd7d78ff51d90244556b28011bac2d29106066a25ba9e96dc089`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074f6bcd0b3bae9f4c581397d152b553279dd7184769c00f73e89f9ae5a2d1a`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4bc60dd1e1c3f4aaade0438967ef0ad4f929678ad0595f68c97aa6802e3508`  
		Last Modified: Thu, 16 Mar 2023 03:44:48 GMT  
		Size: 252.5 MB (252534995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f4fb4d9a35efa338820eac3e26a8095ab5dee1791a6486ba31cb576260bca`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fde270ea5c1652055c01f32fcccb425820da092a3595a17a1b46328120b1aff`  
		Last Modified: Thu, 16 Mar 2023 03:45:04 GMT  
		Size: 63.1 MB (63094293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b8e237fc97a182dc544c752d16ac1ce2e83c4d08538a122d43f03c33340a7e`  
		Last Modified: Thu, 16 Mar 2023 03:44:57 GMT  
		Size: 297.9 KB (297879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab7b64ecca2bb014b31a49a16d2dcd2856db7487d4967731df87dcc2c2b990d`  
		Last Modified: Thu, 16 Mar 2023 03:45:07 GMT  
		Size: 67.2 MB (67235800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:fc9434ebd6ccdea0e90015ea59922478328648a6f1379463bf5e56e1faf9791d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:cc6d92ce3909dc28ed5ac2e82dd33d26c740e389509d90d582b74b9aae768810
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291998840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c261729c13141b33151a8b81bc59100969b2336ac3c7bc6978ab4e11627f9aff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:58:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 04:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:00:33 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:00:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73b43b50fc9056c1213c61cfa3193cd15f8faa751905b21e0e9019473426a74`  
		Last Modified: Thu, 16 Mar 2023 03:11:48 GMT  
		Size: 819.0 KB (818997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6111169e4c0857f4eaf38437fa0beb5e0f66979105b8fdfd3c85c5c5e1544992`  
		Last Modified: Thu, 16 Mar 2023 04:41:15 GMT  
		Size: 4.9 MB (4878581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280739d0ef2f7bb759ccb3b3bb8a5f15a3d1ee562afe99609a493c65039b87a6`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d189808242488a25bc31490cfec5360bcb99b6a965f8782e6af80cf69e81ad79`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc74d1ea892a60a383eaee3d39a2f94fcd19fa347ee48e940f7152e5a8d6bccb`  
		Last Modified: Thu, 16 Mar 2023 04:41:48 GMT  
		Size: 259.6 MB (259588669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43567d3a1b9a70a0e7ec7a689892a144345cf9bcb6eb4151afba22b1eab2d47e`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:6a39f77cf6bf0f42476c1806341a8fd3fc96d58f760633a4c8797139b20b751e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266262593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c617789c637e9584ae7023324d318dacb6b4328e8259de95fb092f7e1ce7d71`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:11:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:11:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:16:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:16:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7fca3839c8bd4903e2ee5f523935fb729f15724615fd9f77ce0d6cc2adbfa6`  
		Last Modified: Thu, 16 Mar 2023 03:39:00 GMT  
		Size: 820.1 KB (820097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3f218bb6743682d83611cfd2ae16145e67489129eccf76d1236a70b3a5bcac`  
		Last Modified: Thu, 16 Mar 2023 03:38:59 GMT  
		Size: 4.1 MB (4090687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1bf44a1167e1c920f67efd944ec51807eb500e2fea8c0103e3a0d46a52fc32`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ed9b280b6ac98a36e5f3f6a1cdeba5961c20493eddf18a97a0b9db954fa6e`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cea9e95a56ecce8cbb02ffdcdcb3059f16577e473b546648bf64fd56a319a1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:32 GMT  
		Size: 239.0 MB (239044585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9735bdd7bdcf6fcc5f9450057e43d66daabf09facf6269f79ba9fabe328adba`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d8ee9421e769f2c97f2687c736b9c296b212efe91c2763b39daf951cc016ba6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281554320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:976c1ec086190504a9967a1b399cc2a7f6664473429137a04cbd5cd272bceaa1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 02:56:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:00:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:50 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:00:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:00:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d56daf02ac303e7c230365644aca63ed850ebf40d29e81a5814308c13562239`  
		Last Modified: Thu, 16 Mar 2023 03:44:18 GMT  
		Size: 819.9 KB (819945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b83e85404464664e50669adc31927b351faa0e1bf21c647f66d7f27782fdb61`  
		Last Modified: Thu, 16 Mar 2023 03:44:16 GMT  
		Size: 4.5 MB (4462823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a184771f70aafd7d78ff51d90244556b28011bac2d29106066a25ba9e96dc089`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074f6bcd0b3bae9f4c581397d152b553279dd7184769c00f73e89f9ae5a2d1a`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4bc60dd1e1c3f4aaade0438967ef0ad4f929678ad0595f68c97aa6802e3508`  
		Last Modified: Thu, 16 Mar 2023 03:44:48 GMT  
		Size: 252.5 MB (252534995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f4fb4d9a35efa338820eac3e26a8095ab5dee1791a6486ba31cb576260bca`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:fc9434ebd6ccdea0e90015ea59922478328648a6f1379463bf5e56e1faf9791d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:cc6d92ce3909dc28ed5ac2e82dd33d26c740e389509d90d582b74b9aae768810
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291998840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c261729c13141b33151a8b81bc59100969b2336ac3c7bc6978ab4e11627f9aff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:58:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:58:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:58:28 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 04:00:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:00:33 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:00:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73b43b50fc9056c1213c61cfa3193cd15f8faa751905b21e0e9019473426a74`  
		Last Modified: Thu, 16 Mar 2023 03:11:48 GMT  
		Size: 819.0 KB (818997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6111169e4c0857f4eaf38437fa0beb5e0f66979105b8fdfd3c85c5c5e1544992`  
		Last Modified: Thu, 16 Mar 2023 04:41:15 GMT  
		Size: 4.9 MB (4878581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280739d0ef2f7bb759ccb3b3bb8a5f15a3d1ee562afe99609a493c65039b87a6`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d189808242488a25bc31490cfec5360bcb99b6a965f8782e6af80cf69e81ad79`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc74d1ea892a60a383eaee3d39a2f94fcd19fa347ee48e940f7152e5a8d6bccb`  
		Last Modified: Thu, 16 Mar 2023 04:41:48 GMT  
		Size: 259.6 MB (259588669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43567d3a1b9a70a0e7ec7a689892a144345cf9bcb6eb4151afba22b1eab2d47e`  
		Last Modified: Thu, 16 Mar 2023 04:41:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:6a39f77cf6bf0f42476c1806341a8fd3fc96d58f760633a4c8797139b20b751e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266262593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c617789c637e9584ae7023324d318dacb6b4328e8259de95fb092f7e1ce7d71`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:11:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:11:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:11:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:11:55 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:16:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:16:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:16:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9fb42489e9f507aa183ef669baec25f94b8c4c22159a4ccc23a1977cedd0d1fa`  
		Last Modified: Thu, 16 Mar 2023 03:39:03 GMT  
		Size: 22.3 MB (22305374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7fca3839c8bd4903e2ee5f523935fb729f15724615fd9f77ce0d6cc2adbfa6`  
		Last Modified: Thu, 16 Mar 2023 03:39:00 GMT  
		Size: 820.1 KB (820097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3f218bb6743682d83611cfd2ae16145e67489129eccf76d1236a70b3a5bcac`  
		Last Modified: Thu, 16 Mar 2023 03:38:59 GMT  
		Size: 4.1 MB (4090687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1bf44a1167e1c920f67efd944ec51807eb500e2fea8c0103e3a0d46a52fc32`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ed9b280b6ac98a36e5f3f6a1cdeba5961c20493eddf18a97a0b9db954fa6e`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cea9e95a56ecce8cbb02ffdcdcb3059f16577e473b546648bf64fd56a319a1b`  
		Last Modified: Thu, 16 Mar 2023 03:39:32 GMT  
		Size: 239.0 MB (239044585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9735bdd7bdcf6fcc5f9450057e43d66daabf09facf6269f79ba9fabe328adba`  
		Last Modified: Thu, 16 Mar 2023 03:38:58 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d8ee9421e769f2c97f2687c736b9c296b212efe91c2763b39daf951cc016ba6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281554320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:976c1ec086190504a9967a1b399cc2a7f6664473429137a04cbd5cd272bceaa1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:56:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:56:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 02:56:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 02:56:48 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Mar 2023 03:00:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:00:50 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:00:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:00:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d56daf02ac303e7c230365644aca63ed850ebf40d29e81a5814308c13562239`  
		Last Modified: Thu, 16 Mar 2023 03:44:18 GMT  
		Size: 819.9 KB (819945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b83e85404464664e50669adc31927b351faa0e1bf21c647f66d7f27782fdb61`  
		Last Modified: Thu, 16 Mar 2023 03:44:16 GMT  
		Size: 4.5 MB (4462823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a184771f70aafd7d78ff51d90244556b28011bac2d29106066a25ba9e96dc089`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074f6bcd0b3bae9f4c581397d152b553279dd7184769c00f73e89f9ae5a2d1a`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4bc60dd1e1c3f4aaade0438967ef0ad4f929678ad0595f68c97aa6802e3508`  
		Last Modified: Thu, 16 Mar 2023 03:44:48 GMT  
		Size: 252.5 MB (252534995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f4fb4d9a35efa338820eac3e26a8095ab5dee1791a6486ba31cb576260bca`  
		Last Modified: Thu, 16 Mar 2023 03:44:15 GMT  
		Size: 196.0 B  
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
$ docker pull ros@sha256:bd5fc4b295512c7fa8dce4efa1c978b3d628d6d6af698c788665ddd137c995cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:2d40d32907926aaefb11b4c7dcbaeebf52103d598cbd394c12ec86b40c97e692
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.3 MB (951320221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46af7519e58644cbc3d57322cc816d396b8bda1ddf41c1b712fb5e975537ab4a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:42:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:42:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 Apr 2023 09:42:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 Apr 2023 09:42:36 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 09:42:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 Apr 2023 09:42:36 GMT
ENV ROS_DISTRO=noetic
# Wed, 12 Apr 2023 09:43:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:43:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 12 Apr 2023 09:43:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 Apr 2023 09:43:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:44:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:44:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 12 Apr 2023 09:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:49:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b00ed65624414cebfd59eb932346275e83df42e1422d20a7b14c8c9edeb48a`  
		Last Modified: Wed, 12 Apr 2023 09:50:13 GMT  
		Size: 10.9 MB (10897019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b3f5b658f43273d64d1a1aeea2487b1b9970a33e08f5a29563764943265a0d`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb716cf3c7952570768bfd3fc5fccb036e9a0beb781e9291a6e11d3f460c93cb`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95e1cb6890794f51bf3e91eae05d0594612953151193fce93420de5a9145f71`  
		Last Modified: Wed, 12 Apr 2023 09:50:42 GMT  
		Size: 239.2 MB (239239058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2534899cbc0a30e85913561bf4af251fd949395ba14ff3352a4afcc7dcf4e8`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0454600fb4adeb722ace480ea8933b040d3b48fdd7d28c7082eced41a81434f5`  
		Last Modified: Wed, 12 Apr 2023 09:51:00 GMT  
		Size: 86.6 MB (86624654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4401a00ee0597bf328d3f44d15501ac656165b052d153dcbd298a69c447af0`  
		Last Modified: Wed, 12 Apr 2023 09:50:48 GMT  
		Size: 313.0 KB (312981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e121b0feeb32a176d80b2d8ee992747b9c8498669bc20d20b92eedf867ec8890`  
		Last Modified: Wed, 12 Apr 2023 09:50:57 GMT  
		Size: 76.0 MB (75978107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4260926addb6a4d57ccf566574df11b0c4c215a725f15d5b8fb228241f92f3f2`  
		Last Modified: Wed, 12 Apr 2023 09:52:23 GMT  
		Size: 487.8 MB (487817262 bytes)  
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
$ docker pull ros@sha256:f6333591ef1ba3acac19ff94cafe99632293efcf87c7c903656da513bb1c6cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:8be6a4017ab924705d204b5543bc735d6f2b24ae7aa0218b075df7dc7be56a9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.7 MB (484659940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:037652e029b16ee89f1f44c33ae00f3c5372c84d731d01eba0a41dd42349f6c2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:42:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:42:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 Apr 2023 09:42:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 Apr 2023 09:42:36 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 09:42:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 Apr 2023 09:42:36 GMT
ENV ROS_DISTRO=noetic
# Wed, 12 Apr 2023 09:43:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:43:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 12 Apr 2023 09:43:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 Apr 2023 09:43:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:44:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:44:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 12 Apr 2023 09:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:45:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b00ed65624414cebfd59eb932346275e83df42e1422d20a7b14c8c9edeb48a`  
		Last Modified: Wed, 12 Apr 2023 09:50:13 GMT  
		Size: 10.9 MB (10897019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b3f5b658f43273d64d1a1aeea2487b1b9970a33e08f5a29563764943265a0d`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb716cf3c7952570768bfd3fc5fccb036e9a0beb781e9291a6e11d3f460c93cb`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95e1cb6890794f51bf3e91eae05d0594612953151193fce93420de5a9145f71`  
		Last Modified: Wed, 12 Apr 2023 09:50:42 GMT  
		Size: 239.2 MB (239239058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2534899cbc0a30e85913561bf4af251fd949395ba14ff3352a4afcc7dcf4e8`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0454600fb4adeb722ace480ea8933b040d3b48fdd7d28c7082eced41a81434f5`  
		Last Modified: Wed, 12 Apr 2023 09:51:00 GMT  
		Size: 86.6 MB (86624654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4401a00ee0597bf328d3f44d15501ac656165b052d153dcbd298a69c447af0`  
		Last Modified: Wed, 12 Apr 2023 09:50:48 GMT  
		Size: 313.0 KB (312981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e121b0feeb32a176d80b2d8ee992747b9c8498669bc20d20b92eedf867ec8890`  
		Last Modified: Wed, 12 Apr 2023 09:50:57 GMT  
		Size: 76.0 MB (75978107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e0ecca7cd4d691fe5a4de7b009310f1e21326d187c068f6347d3cebcc4ed35`  
		Last Modified: Wed, 12 Apr 2023 09:51:09 GMT  
		Size: 21.2 MB (21156981 bytes)  
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
$ docker pull ros@sha256:e4a44510cbbaff8c99ba6e2592910366bc367df7af8ba3153386d123946ec1d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:634113cfb1c3d673ab0f868889ede070899c0d58176fc3be883511e986804434
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.5 MB (463502959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa631feb74bf3416192ad8f2098cd9d258e9c8013bc1c5cdd52b914f9c6c50f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:42:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:42:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 Apr 2023 09:42:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 Apr 2023 09:42:36 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 09:42:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 Apr 2023 09:42:36 GMT
ENV ROS_DISTRO=noetic
# Wed, 12 Apr 2023 09:43:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:43:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 12 Apr 2023 09:43:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 Apr 2023 09:43:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:44:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:44:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 12 Apr 2023 09:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b00ed65624414cebfd59eb932346275e83df42e1422d20a7b14c8c9edeb48a`  
		Last Modified: Wed, 12 Apr 2023 09:50:13 GMT  
		Size: 10.9 MB (10897019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b3f5b658f43273d64d1a1aeea2487b1b9970a33e08f5a29563764943265a0d`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb716cf3c7952570768bfd3fc5fccb036e9a0beb781e9291a6e11d3f460c93cb`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95e1cb6890794f51bf3e91eae05d0594612953151193fce93420de5a9145f71`  
		Last Modified: Wed, 12 Apr 2023 09:50:42 GMT  
		Size: 239.2 MB (239239058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2534899cbc0a30e85913561bf4af251fd949395ba14ff3352a4afcc7dcf4e8`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0454600fb4adeb722ace480ea8933b040d3b48fdd7d28c7082eced41a81434f5`  
		Last Modified: Wed, 12 Apr 2023 09:51:00 GMT  
		Size: 86.6 MB (86624654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4401a00ee0597bf328d3f44d15501ac656165b052d153dcbd298a69c447af0`  
		Last Modified: Wed, 12 Apr 2023 09:50:48 GMT  
		Size: 313.0 KB (312981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e121b0feeb32a176d80b2d8ee992747b9c8498669bc20d20b92eedf867ec8890`  
		Last Modified: Wed, 12 Apr 2023 09:50:57 GMT  
		Size: 76.0 MB (75978107 bytes)  
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
$ docker pull ros@sha256:06cf4c09a8ee2373792157f32ec540ea08f39a989720f0eedf3c0c50dad1dae1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:2863415dfb26f22f0b6318820ccbb6dc7118363e8358a2459d7f6b0862a4805e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300587217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9924f12806821bd9bc09843e0f9f4c5315966616b0631dcd6617687e24f564b7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:42:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:42:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 Apr 2023 09:42:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 Apr 2023 09:42:36 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 09:42:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 Apr 2023 09:42:36 GMT
ENV ROS_DISTRO=noetic
# Wed, 12 Apr 2023 09:43:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:43:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 12 Apr 2023 09:43:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 Apr 2023 09:43:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b00ed65624414cebfd59eb932346275e83df42e1422d20a7b14c8c9edeb48a`  
		Last Modified: Wed, 12 Apr 2023 09:50:13 GMT  
		Size: 10.9 MB (10897019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b3f5b658f43273d64d1a1aeea2487b1b9970a33e08f5a29563764943265a0d`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb716cf3c7952570768bfd3fc5fccb036e9a0beb781e9291a6e11d3f460c93cb`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95e1cb6890794f51bf3e91eae05d0594612953151193fce93420de5a9145f71`  
		Last Modified: Wed, 12 Apr 2023 09:50:42 GMT  
		Size: 239.2 MB (239239058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2534899cbc0a30e85913561bf4af251fd949395ba14ff3352a4afcc7dcf4e8`  
		Last Modified: Wed, 12 Apr 2023 09:50:11 GMT  
		Size: 195.0 B  
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
$ docker pull ros@sha256:165af6c427873d718bc79cf8b407f519077e210ae0b9e62295a12a32681313bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:bea2dd71803129ff4287c6f4d4cf9725db4ec6c4f9851a6092e3aa2930e1ee4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.4 MB (264395896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1f345177240421e71c5853cbe2799356ba5c4c5abb287e1664058d96ff6f36`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:35:49 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:22:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:12 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:22:12 GMT
CMD ["bash"]
# Mon, 03 Apr 2023 23:22:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Apr 2023 23:23:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 03 Apr 2023 23:23:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406973cc1afb21645698bc7cf99d59709094c778a695225530393d37f1efd4ef`  
		Last Modified: Mon, 03 Apr 2023 23:32:42 GMT  
		Size: 120.2 MB (120235298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287f7cbea03df781b97c2e3b15b36c82aa25f249e4db3d062359ee77adda9aed`  
		Last Modified: Mon, 03 Apr 2023 23:32:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0031f4343f597c7dc81a01519206af6b00095949bb89d81ddb4063f1b5ddb681`  
		Last Modified: Mon, 03 Apr 2023 23:33:00 GMT  
		Size: 84.9 MB (84917407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c311a022e201d3be7e11783d7a6aae4fb7821e3ddd40a4e8aa1a10ace208bcc`  
		Last Modified: Mon, 03 Apr 2023 23:32:50 GMT  
		Size: 303.1 KB (303121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2be757f329eba861f5e82aa755adac3a5b61547fd9ae337ffac40320085926c`  
		Last Modified: Mon, 03 Apr 2023 23:32:49 GMT  
		Size: 2.4 KB (2443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533a72e10cd8870d2cafedff062b7d3a84fcb8237923930ce5252434cc3fa585`  
		Last Modified: Mon, 03 Apr 2023 23:32:53 GMT  
		Size: 23.5 MB (23507237 bytes)  
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
$ docker pull ros@sha256:bd7810c2e55e802baedfc6ebca564508a8c7be12b7d19938757b2e19a45bae4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:fd6b3e63184eca87cf3ed86ac42dfb6cd75d1b4533a9920e16725101f11260c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1093958182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b466fd0980596647b40a560d9ee3f4acb1dadd9e30cc198721e8da801b54e32`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:35:49 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:22:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:12 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:22:12 GMT
CMD ["bash"]
# Mon, 03 Apr 2023 23:22:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Apr 2023 23:23:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 03 Apr 2023 23:23:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:31:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406973cc1afb21645698bc7cf99d59709094c778a695225530393d37f1efd4ef`  
		Last Modified: Mon, 03 Apr 2023 23:32:42 GMT  
		Size: 120.2 MB (120235298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287f7cbea03df781b97c2e3b15b36c82aa25f249e4db3d062359ee77adda9aed`  
		Last Modified: Mon, 03 Apr 2023 23:32:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0031f4343f597c7dc81a01519206af6b00095949bb89d81ddb4063f1b5ddb681`  
		Last Modified: Mon, 03 Apr 2023 23:33:00 GMT  
		Size: 84.9 MB (84917407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c311a022e201d3be7e11783d7a6aae4fb7821e3ddd40a4e8aa1a10ace208bcc`  
		Last Modified: Mon, 03 Apr 2023 23:32:50 GMT  
		Size: 303.1 KB (303121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2be757f329eba861f5e82aa755adac3a5b61547fd9ae337ffac40320085926c`  
		Last Modified: Mon, 03 Apr 2023 23:32:49 GMT  
		Size: 2.4 KB (2443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533a72e10cd8870d2cafedff062b7d3a84fcb8237923930ce5252434cc3fa585`  
		Last Modified: Mon, 03 Apr 2023 23:32:53 GMT  
		Size: 23.5 MB (23507237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d3cc26cd9214fbf157625a1a049e0c87c03f6d18c5a23b24e08fe3761c8075`  
		Last Modified: Mon, 03 Apr 2023 23:34:42 GMT  
		Size: 829.6 MB (829562286 bytes)  
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
$ docker pull ros@sha256:bd7810c2e55e802baedfc6ebca564508a8c7be12b7d19938757b2e19a45bae4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:fd6b3e63184eca87cf3ed86ac42dfb6cd75d1b4533a9920e16725101f11260c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1093958182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b466fd0980596647b40a560d9ee3f4acb1dadd9e30cc198721e8da801b54e32`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:35:49 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:22:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:12 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:22:12 GMT
CMD ["bash"]
# Mon, 03 Apr 2023 23:22:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Apr 2023 23:23:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 03 Apr 2023 23:23:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:31:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406973cc1afb21645698bc7cf99d59709094c778a695225530393d37f1efd4ef`  
		Last Modified: Mon, 03 Apr 2023 23:32:42 GMT  
		Size: 120.2 MB (120235298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287f7cbea03df781b97c2e3b15b36c82aa25f249e4db3d062359ee77adda9aed`  
		Last Modified: Mon, 03 Apr 2023 23:32:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0031f4343f597c7dc81a01519206af6b00095949bb89d81ddb4063f1b5ddb681`  
		Last Modified: Mon, 03 Apr 2023 23:33:00 GMT  
		Size: 84.9 MB (84917407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c311a022e201d3be7e11783d7a6aae4fb7821e3ddd40a4e8aa1a10ace208bcc`  
		Last Modified: Mon, 03 Apr 2023 23:32:50 GMT  
		Size: 303.1 KB (303121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2be757f329eba861f5e82aa755adac3a5b61547fd9ae337ffac40320085926c`  
		Last Modified: Mon, 03 Apr 2023 23:32:49 GMT  
		Size: 2.4 KB (2443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533a72e10cd8870d2cafedff062b7d3a84fcb8237923930ce5252434cc3fa585`  
		Last Modified: Mon, 03 Apr 2023 23:32:53 GMT  
		Size: 23.5 MB (23507237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d3cc26cd9214fbf157625a1a049e0c87c03f6d18c5a23b24e08fe3761c8075`  
		Last Modified: Mon, 03 Apr 2023 23:34:42 GMT  
		Size: 829.6 MB (829562286 bytes)  
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
$ docker pull ros@sha256:165af6c427873d718bc79cf8b407f519077e210ae0b9e62295a12a32681313bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:bea2dd71803129ff4287c6f4d4cf9725db4ec6c4f9851a6092e3aa2930e1ee4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.4 MB (264395896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1f345177240421e71c5853cbe2799356ba5c4c5abb287e1664058d96ff6f36`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:35:49 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:22:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:12 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:22:12 GMT
CMD ["bash"]
# Mon, 03 Apr 2023 23:22:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Apr 2023 23:23:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 03 Apr 2023 23:23:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406973cc1afb21645698bc7cf99d59709094c778a695225530393d37f1efd4ef`  
		Last Modified: Mon, 03 Apr 2023 23:32:42 GMT  
		Size: 120.2 MB (120235298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287f7cbea03df781b97c2e3b15b36c82aa25f249e4db3d062359ee77adda9aed`  
		Last Modified: Mon, 03 Apr 2023 23:32:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0031f4343f597c7dc81a01519206af6b00095949bb89d81ddb4063f1b5ddb681`  
		Last Modified: Mon, 03 Apr 2023 23:33:00 GMT  
		Size: 84.9 MB (84917407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c311a022e201d3be7e11783d7a6aae4fb7821e3ddd40a4e8aa1a10ace208bcc`  
		Last Modified: Mon, 03 Apr 2023 23:32:50 GMT  
		Size: 303.1 KB (303121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2be757f329eba861f5e82aa755adac3a5b61547fd9ae337ffac40320085926c`  
		Last Modified: Mon, 03 Apr 2023 23:32:49 GMT  
		Size: 2.4 KB (2443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533a72e10cd8870d2cafedff062b7d3a84fcb8237923930ce5252434cc3fa585`  
		Last Modified: Mon, 03 Apr 2023 23:32:53 GMT  
		Size: 23.5 MB (23507237 bytes)  
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
$ docker pull ros@sha256:165af6c427873d718bc79cf8b407f519077e210ae0b9e62295a12a32681313bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:bea2dd71803129ff4287c6f4d4cf9725db4ec6c4f9851a6092e3aa2930e1ee4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.4 MB (264395896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1f345177240421e71c5853cbe2799356ba5c4c5abb287e1664058d96ff6f36`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:35:49 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:22:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:12 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:22:12 GMT
CMD ["bash"]
# Mon, 03 Apr 2023 23:22:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Apr 2023 23:23:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 03 Apr 2023 23:23:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406973cc1afb21645698bc7cf99d59709094c778a695225530393d37f1efd4ef`  
		Last Modified: Mon, 03 Apr 2023 23:32:42 GMT  
		Size: 120.2 MB (120235298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287f7cbea03df781b97c2e3b15b36c82aa25f249e4db3d062359ee77adda9aed`  
		Last Modified: Mon, 03 Apr 2023 23:32:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0031f4343f597c7dc81a01519206af6b00095949bb89d81ddb4063f1b5ddb681`  
		Last Modified: Mon, 03 Apr 2023 23:33:00 GMT  
		Size: 84.9 MB (84917407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c311a022e201d3be7e11783d7a6aae4fb7821e3ddd40a4e8aa1a10ace208bcc`  
		Last Modified: Mon, 03 Apr 2023 23:32:50 GMT  
		Size: 303.1 KB (303121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2be757f329eba861f5e82aa755adac3a5b61547fd9ae337ffac40320085926c`  
		Last Modified: Mon, 03 Apr 2023 23:32:49 GMT  
		Size: 2.4 KB (2443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533a72e10cd8870d2cafedff062b7d3a84fcb8237923930ce5252434cc3fa585`  
		Last Modified: Mon, 03 Apr 2023 23:32:53 GMT  
		Size: 23.5 MB (23507237 bytes)  
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
$ docker pull ros@sha256:2adbd236585a2b254fbef29dc4b788157ce3d4c2af8511f14b883215453183c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:c9921f9a67468c9f71bea0ea8bae126f4cf407ab367adcaa37cca8e8cb438c4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155665688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26eb1d55ea08d3da76bccaf3a8a5ae07b8a8732340dbdc3ec44a22f87ffd7b29`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:35:49 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:22:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:12 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:22:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406973cc1afb21645698bc7cf99d59709094c778a695225530393d37f1efd4ef`  
		Last Modified: Mon, 03 Apr 2023 23:32:42 GMT  
		Size: 120.2 MB (120235298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287f7cbea03df781b97c2e3b15b36c82aa25f249e4db3d062359ee77adda9aed`  
		Last Modified: Mon, 03 Apr 2023 23:32:23 GMT  
		Size: 197.0 B  
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
$ docker pull ros@sha256:2adbd236585a2b254fbef29dc4b788157ce3d4c2af8511f14b883215453183c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:c9921f9a67468c9f71bea0ea8bae126f4cf407ab367adcaa37cca8e8cb438c4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155665688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26eb1d55ea08d3da76bccaf3a8a5ae07b8a8732340dbdc3ec44a22f87ffd7b29`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:35:49 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:22:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:12 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:22:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406973cc1afb21645698bc7cf99d59709094c778a695225530393d37f1efd4ef`  
		Last Modified: Mon, 03 Apr 2023 23:32:42 GMT  
		Size: 120.2 MB (120235298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287f7cbea03df781b97c2e3b15b36c82aa25f249e4db3d062359ee77adda9aed`  
		Last Modified: Mon, 03 Apr 2023 23:32:23 GMT  
		Size: 197.0 B  
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
