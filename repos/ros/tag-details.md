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
$ docker pull ros@sha256:a3a3f407b3fa69ad3bda20f822f913e3fe8d06a2616dbbcb5e8336a3ce026a51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:e7778d84e91917cfd94d5b4c6b13abc1aedf88541bdf475a976d06ee75787478
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250944809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77d2094447e8ddda98319527b05a93263af8524d1819505c5b903d0797bb4d41`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:20:26 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:20:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 04:21:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:21:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:21:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:21:25 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:21:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:22:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:22:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 04:22:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b6c60e4af795544c6d1c364ed29a2ed8c498f2e5da5a57dea651d7c7a523b5`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eed6591731f4cd0e89ff07e515fd42f1466e54d5fc27307ce4f3b8ae3afb141`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0523ba22e09bf736f80bd994abe837c7b137f287b8eea0f5e7bdbd00da85176c`  
		Last Modified: Thu, 16 Mar 2023 04:46:21 GMT  
		Size: 120.4 MB (120370671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d32eb5055c7800fac72e3cac723ba624a400884ebf5f5a9500ee754097b1e3`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9d766c59781e81fe431a83896cad4f0713dbabebe97aed5147ad1b93882ff`  
		Last Modified: Thu, 16 Mar 2023 04:46:40 GMT  
		Size: 73.3 MB (73340719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3213fb9cdb02761d0f1588aafdd6d1aea86527d98ac336b4990038700eafd6`  
		Last Modified: Thu, 16 Mar 2023 04:46:30 GMT  
		Size: 279.9 KB (279912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850f044353a9cd5a3393fdcb430d07b7ed8b8ebdf18fc92426f230eff57e4f9`  
		Last Modified: Thu, 16 Mar 2023 04:46:30 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aabf876615ac9c2be0dd9f801770504d13fde42076b0b2f95e4f68dd0c57216`  
		Last Modified: Thu, 16 Mar 2023 04:46:33 GMT  
		Size: 21.7 MB (21662435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:faf71017f30cd4a71e27447d574207fc5e10da8cc6546b983c3fff6ec6a84477
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226807812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c72845950c710d7c343b5e65337dd70242701e34b0340a3d4ee9324c22d69c7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:12 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:23:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 03:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:06 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:24:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:24:06 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:24:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 03:24:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42860775fce781d98f8f21abfafa48660e634182b69b05266851498055971a82`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7191287fc71fa37ace07c3fb721fe8b0df2516866da1e7b98f48aa71b8bdb94e`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e24d2145f0cc2cf9a85047ab49b1f2f4b457e7b81b534c1bfc25642cd3a10fd`  
		Last Modified: Thu, 16 Mar 2023 03:48:43 GMT  
		Size: 104.6 MB (104568150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27f4054f4fcc5c1a7c641b6a19891c7fe042a2d4ba353b8eb7d094b1ccde304`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b61acdd97d95df9976326ba8a1dc79a739c367e9d0232e2ae3560909a891af4`  
		Last Modified: Thu, 16 Mar 2023 03:48:59 GMT  
		Size: 67.7 MB (67684730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11b685a5e9052a6bd9772d42b4900972bc1037ca8648eae13801e200578820`  
		Last Modified: Thu, 16 Mar 2023 03:48:52 GMT  
		Size: 279.9 KB (279917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8d4285dfe20611b685fe67cf842b70a9e8b6409de0e9d12bcc27174be70897`  
		Last Modified: Thu, 16 Mar 2023 03:48:51 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab10b5ea657202d97bef2d89bc8b1d0d91f7b99e5f04ee9ef87100edfc1dccd`  
		Last Modified: Thu, 16 Mar 2023 03:48:54 GMT  
		Size: 20.4 MB (20385758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:a3a3f407b3fa69ad3bda20f822f913e3fe8d06a2616dbbcb5e8336a3ce026a51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:e7778d84e91917cfd94d5b4c6b13abc1aedf88541bdf475a976d06ee75787478
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250944809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77d2094447e8ddda98319527b05a93263af8524d1819505c5b903d0797bb4d41`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:20:26 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:20:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 04:21:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:21:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:21:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:21:25 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:21:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:22:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:22:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 04:22:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b6c60e4af795544c6d1c364ed29a2ed8c498f2e5da5a57dea651d7c7a523b5`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eed6591731f4cd0e89ff07e515fd42f1466e54d5fc27307ce4f3b8ae3afb141`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0523ba22e09bf736f80bd994abe837c7b137f287b8eea0f5e7bdbd00da85176c`  
		Last Modified: Thu, 16 Mar 2023 04:46:21 GMT  
		Size: 120.4 MB (120370671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d32eb5055c7800fac72e3cac723ba624a400884ebf5f5a9500ee754097b1e3`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9d766c59781e81fe431a83896cad4f0713dbabebe97aed5147ad1b93882ff`  
		Last Modified: Thu, 16 Mar 2023 04:46:40 GMT  
		Size: 73.3 MB (73340719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3213fb9cdb02761d0f1588aafdd6d1aea86527d98ac336b4990038700eafd6`  
		Last Modified: Thu, 16 Mar 2023 04:46:30 GMT  
		Size: 279.9 KB (279912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850f044353a9cd5a3393fdcb430d07b7ed8b8ebdf18fc92426f230eff57e4f9`  
		Last Modified: Thu, 16 Mar 2023 04:46:30 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aabf876615ac9c2be0dd9f801770504d13fde42076b0b2f95e4f68dd0c57216`  
		Last Modified: Thu, 16 Mar 2023 04:46:33 GMT  
		Size: 21.7 MB (21662435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:faf71017f30cd4a71e27447d574207fc5e10da8cc6546b983c3fff6ec6a84477
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226807812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c72845950c710d7c343b5e65337dd70242701e34b0340a3d4ee9324c22d69c7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:12 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:23:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 03:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:06 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:24:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:24:06 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:24:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 03:24:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42860775fce781d98f8f21abfafa48660e634182b69b05266851498055971a82`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7191287fc71fa37ace07c3fb721fe8b0df2516866da1e7b98f48aa71b8bdb94e`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e24d2145f0cc2cf9a85047ab49b1f2f4b457e7b81b534c1bfc25642cd3a10fd`  
		Last Modified: Thu, 16 Mar 2023 03:48:43 GMT  
		Size: 104.6 MB (104568150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27f4054f4fcc5c1a7c641b6a19891c7fe042a2d4ba353b8eb7d094b1ccde304`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b61acdd97d95df9976326ba8a1dc79a739c367e9d0232e2ae3560909a891af4`  
		Last Modified: Thu, 16 Mar 2023 03:48:59 GMT  
		Size: 67.7 MB (67684730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11b685a5e9052a6bd9772d42b4900972bc1037ca8648eae13801e200578820`  
		Last Modified: Thu, 16 Mar 2023 03:48:52 GMT  
		Size: 279.9 KB (279917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8d4285dfe20611b685fe67cf842b70a9e8b6409de0e9d12bcc27174be70897`  
		Last Modified: Thu, 16 Mar 2023 03:48:51 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab10b5ea657202d97bef2d89bc8b1d0d91f7b99e5f04ee9ef87100edfc1dccd`  
		Last Modified: Thu, 16 Mar 2023 03:48:54 GMT  
		Size: 20.4 MB (20385758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:a3a3f407b3fa69ad3bda20f822f913e3fe8d06a2616dbbcb5e8336a3ce026a51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:e7778d84e91917cfd94d5b4c6b13abc1aedf88541bdf475a976d06ee75787478
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250944809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77d2094447e8ddda98319527b05a93263af8524d1819505c5b903d0797bb4d41`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:20:26 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:20:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 04:21:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:21:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:21:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:21:25 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:21:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:22:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:22:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 04:22:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b6c60e4af795544c6d1c364ed29a2ed8c498f2e5da5a57dea651d7c7a523b5`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eed6591731f4cd0e89ff07e515fd42f1466e54d5fc27307ce4f3b8ae3afb141`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0523ba22e09bf736f80bd994abe837c7b137f287b8eea0f5e7bdbd00da85176c`  
		Last Modified: Thu, 16 Mar 2023 04:46:21 GMT  
		Size: 120.4 MB (120370671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d32eb5055c7800fac72e3cac723ba624a400884ebf5f5a9500ee754097b1e3`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9d766c59781e81fe431a83896cad4f0713dbabebe97aed5147ad1b93882ff`  
		Last Modified: Thu, 16 Mar 2023 04:46:40 GMT  
		Size: 73.3 MB (73340719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3213fb9cdb02761d0f1588aafdd6d1aea86527d98ac336b4990038700eafd6`  
		Last Modified: Thu, 16 Mar 2023 04:46:30 GMT  
		Size: 279.9 KB (279912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850f044353a9cd5a3393fdcb430d07b7ed8b8ebdf18fc92426f230eff57e4f9`  
		Last Modified: Thu, 16 Mar 2023 04:46:30 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aabf876615ac9c2be0dd9f801770504d13fde42076b0b2f95e4f68dd0c57216`  
		Last Modified: Thu, 16 Mar 2023 04:46:33 GMT  
		Size: 21.7 MB (21662435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:faf71017f30cd4a71e27447d574207fc5e10da8cc6546b983c3fff6ec6a84477
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226807812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c72845950c710d7c343b5e65337dd70242701e34b0340a3d4ee9324c22d69c7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:12 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:23:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 03:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:06 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:24:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:24:06 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:24:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 03:24:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42860775fce781d98f8f21abfafa48660e634182b69b05266851498055971a82`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7191287fc71fa37ace07c3fb721fe8b0df2516866da1e7b98f48aa71b8bdb94e`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e24d2145f0cc2cf9a85047ab49b1f2f4b457e7b81b534c1bfc25642cd3a10fd`  
		Last Modified: Thu, 16 Mar 2023 03:48:43 GMT  
		Size: 104.6 MB (104568150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27f4054f4fcc5c1a7c641b6a19891c7fe042a2d4ba353b8eb7d094b1ccde304`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b61acdd97d95df9976326ba8a1dc79a739c367e9d0232e2ae3560909a891af4`  
		Last Modified: Thu, 16 Mar 2023 03:48:59 GMT  
		Size: 67.7 MB (67684730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11b685a5e9052a6bd9772d42b4900972bc1037ca8648eae13801e200578820`  
		Last Modified: Thu, 16 Mar 2023 03:48:52 GMT  
		Size: 279.9 KB (279917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8d4285dfe20611b685fe67cf842b70a9e8b6409de0e9d12bcc27174be70897`  
		Last Modified: Thu, 16 Mar 2023 03:48:51 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab10b5ea657202d97bef2d89bc8b1d0d91f7b99e5f04ee9ef87100edfc1dccd`  
		Last Modified: Thu, 16 Mar 2023 03:48:54 GMT  
		Size: 20.4 MB (20385758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:8ff3fa733933011a9316a5d4481d570594d1642e36bcc1e3d54c990b41d7b391
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:12663f4a72e14f75b9b899130531a4156f277f602a051735431a9450ec198bdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155659289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f873c76184120a0c518af4c8718488e3ced4b3cf4b6ee293174c6591e923f6f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:20:26 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:20:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 04:21:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:21:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:21:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:21:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b6c60e4af795544c6d1c364ed29a2ed8c498f2e5da5a57dea651d7c7a523b5`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eed6591731f4cd0e89ff07e515fd42f1466e54d5fc27307ce4f3b8ae3afb141`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0523ba22e09bf736f80bd994abe837c7b137f287b8eea0f5e7bdbd00da85176c`  
		Last Modified: Thu, 16 Mar 2023 04:46:21 GMT  
		Size: 120.4 MB (120370671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d32eb5055c7800fac72e3cac723ba624a400884ebf5f5a9500ee754097b1e3`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2a1467ed2272139d4e04c1dd4501272a37ae159f9c10bccf37aacc7ccd0aafc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138454995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981a435d018f0a748e447262b9f99f1b5a9febc6024f82e4e08ad90b4f9213d0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:12 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:23:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 03:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:06 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:24:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:24:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42860775fce781d98f8f21abfafa48660e634182b69b05266851498055971a82`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7191287fc71fa37ace07c3fb721fe8b0df2516866da1e7b98f48aa71b8bdb94e`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e24d2145f0cc2cf9a85047ab49b1f2f4b457e7b81b534c1bfc25642cd3a10fd`  
		Last Modified: Thu, 16 Mar 2023 03:48:43 GMT  
		Size: 104.6 MB (104568150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27f4054f4fcc5c1a7c641b6a19891c7fe042a2d4ba353b8eb7d094b1ccde304`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:8ff3fa733933011a9316a5d4481d570594d1642e36bcc1e3d54c990b41d7b391
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:12663f4a72e14f75b9b899130531a4156f277f602a051735431a9450ec198bdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155659289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f873c76184120a0c518af4c8718488e3ced4b3cf4b6ee293174c6591e923f6f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:20:26 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:20:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 04:21:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:21:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:21:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:21:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b6c60e4af795544c6d1c364ed29a2ed8c498f2e5da5a57dea651d7c7a523b5`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eed6591731f4cd0e89ff07e515fd42f1466e54d5fc27307ce4f3b8ae3afb141`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0523ba22e09bf736f80bd994abe837c7b137f287b8eea0f5e7bdbd00da85176c`  
		Last Modified: Thu, 16 Mar 2023 04:46:21 GMT  
		Size: 120.4 MB (120370671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d32eb5055c7800fac72e3cac723ba624a400884ebf5f5a9500ee754097b1e3`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2a1467ed2272139d4e04c1dd4501272a37ae159f9c10bccf37aacc7ccd0aafc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138454995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981a435d018f0a748e447262b9f99f1b5a9febc6024f82e4e08ad90b4f9213d0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:12 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:23:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 03:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:06 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:24:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:24:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42860775fce781d98f8f21abfafa48660e634182b69b05266851498055971a82`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7191287fc71fa37ace07c3fb721fe8b0df2516866da1e7b98f48aa71b8bdb94e`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e24d2145f0cc2cf9a85047ab49b1f2f4b457e7b81b534c1bfc25642cd3a10fd`  
		Last Modified: Thu, 16 Mar 2023 03:48:43 GMT  
		Size: 104.6 MB (104568150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27f4054f4fcc5c1a7c641b6a19891c7fe042a2d4ba353b8eb7d094b1ccde304`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:85e6616e9a877d362a59861821b66f37c19a20389506955a71060f8c9915a45b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:9da2e17fdcbde4b6c85e683288c16318aeb1abd725f4b8e338b79aa5913e4e8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349048873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5754690238d8794729825bfa477f6b5705e179fbd80c81f41180bb945d7646`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:20:26 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:20:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 04:21:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:21:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:21:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:21:25 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:21:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:22:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:22:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 04:22:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:22:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 04:22:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:22:35 GMT
ENV ROS1_DISTRO=noetic
# Thu, 16 Mar 2023 04:22:36 GMT
ENV ROS2_DISTRO=foxy
# Thu, 16 Mar 2023 04:23:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:14 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b6c60e4af795544c6d1c364ed29a2ed8c498f2e5da5a57dea651d7c7a523b5`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eed6591731f4cd0e89ff07e515fd42f1466e54d5fc27307ce4f3b8ae3afb141`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0523ba22e09bf736f80bd994abe837c7b137f287b8eea0f5e7bdbd00da85176c`  
		Last Modified: Thu, 16 Mar 2023 04:46:21 GMT  
		Size: 120.4 MB (120370671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d32eb5055c7800fac72e3cac723ba624a400884ebf5f5a9500ee754097b1e3`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9d766c59781e81fe431a83896cad4f0713dbabebe97aed5147ad1b93882ff`  
		Last Modified: Thu, 16 Mar 2023 04:46:40 GMT  
		Size: 73.3 MB (73340719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3213fb9cdb02761d0f1588aafdd6d1aea86527d98ac336b4990038700eafd6`  
		Last Modified: Thu, 16 Mar 2023 04:46:30 GMT  
		Size: 279.9 KB (279912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850f044353a9cd5a3393fdcb430d07b7ed8b8ebdf18fc92426f230eff57e4f9`  
		Last Modified: Thu, 16 Mar 2023 04:46:30 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aabf876615ac9c2be0dd9f801770504d13fde42076b0b2f95e4f68dd0c57216`  
		Last Modified: Thu, 16 Mar 2023 04:46:33 GMT  
		Size: 21.7 MB (21662435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c55c6a35c527c80ba41ab57cfc0aeecbcaf03a8e21d52d510181da679bfac6`  
		Last Modified: Thu, 16 Mar 2023 04:46:51 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f20b731e283d25346685de83f1440763ca136e6cc0a35cbe21422d043b972dd`  
		Last Modified: Thu, 16 Mar 2023 04:46:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20660b50a185f3eeb1a43d67bdaeb11a64c73fe6f4e32197642c8408848c6b18`  
		Last Modified: Thu, 16 Mar 2023 04:47:05 GMT  
		Size: 76.4 MB (76429157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad40a10a98c57a7eb642b09195ade82c9548952e17c9fcf1240770d671c7103`  
		Last Modified: Thu, 16 Mar 2023 04:46:56 GMT  
		Size: 21.7 MB (21674281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13756eb5e96bd40ce7f9ad35d1c2b643de10c62455af3309904258c67215e74`  
		Last Modified: Thu, 16 Mar 2023 04:46:51 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ae4f7591eae21b9f0abb07cf02221b942789d6336423f1f0b891f77a40ed9e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317630108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5d55ffb232c17b5db88aa6e0b5cd1d38dd1c0c8c450ffe7bc57137086dd187`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:12 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:23:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 03:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:06 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:24:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:24:06 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:24:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 03:24:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:24:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:24:59 GMT
ENV ROS1_DISTRO=noetic
# Thu, 16 Mar 2023 03:24:59 GMT
ENV ROS2_DISTRO=foxy
# Thu, 16 Mar 2023 03:25:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:30 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42860775fce781d98f8f21abfafa48660e634182b69b05266851498055971a82`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7191287fc71fa37ace07c3fb721fe8b0df2516866da1e7b98f48aa71b8bdb94e`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e24d2145f0cc2cf9a85047ab49b1f2f4b457e7b81b534c1bfc25642cd3a10fd`  
		Last Modified: Thu, 16 Mar 2023 03:48:43 GMT  
		Size: 104.6 MB (104568150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27f4054f4fcc5c1a7c641b6a19891c7fe042a2d4ba353b8eb7d094b1ccde304`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b61acdd97d95df9976326ba8a1dc79a739c367e9d0232e2ae3560909a891af4`  
		Last Modified: Thu, 16 Mar 2023 03:48:59 GMT  
		Size: 67.7 MB (67684730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11b685a5e9052a6bd9772d42b4900972bc1037ca8648eae13801e200578820`  
		Last Modified: Thu, 16 Mar 2023 03:48:52 GMT  
		Size: 279.9 KB (279917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8d4285dfe20611b685fe67cf842b70a9e8b6409de0e9d12bcc27174be70897`  
		Last Modified: Thu, 16 Mar 2023 03:48:51 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab10b5ea657202d97bef2d89bc8b1d0d91f7b99e5f04ee9ef87100edfc1dccd`  
		Last Modified: Thu, 16 Mar 2023 03:48:54 GMT  
		Size: 20.4 MB (20385758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9da9850fbdebec3cf3685151e664e038e2628dd8c09bca753e13b538675fcd`  
		Last Modified: Thu, 16 Mar 2023 03:49:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a82cab40cfa91b60ba64a899790a39b77200d232069659d5aaeaf10ee1dbf92`  
		Last Modified: Thu, 16 Mar 2023 03:49:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf248e08c595e13904d0d40d28e22b9f0f5e586c0f55ceba204e34c55b2d334`  
		Last Modified: Thu, 16 Mar 2023 03:49:23 GMT  
		Size: 76.5 MB (76495934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7713413d61c87cbf93543d08a3a476192cbdf1db9eb33cc0dee39d37f60de8f2`  
		Last Modified: Thu, 16 Mar 2023 03:49:12 GMT  
		Size: 14.3 MB (14325733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ee2466e3b53232367b496f7990dd5a5594945dfa09301dd087beee9b2ce3e8`  
		Last Modified: Thu, 16 Mar 2023 03:49:10 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:85e6616e9a877d362a59861821b66f37c19a20389506955a71060f8c9915a45b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:9da2e17fdcbde4b6c85e683288c16318aeb1abd725f4b8e338b79aa5913e4e8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349048873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5754690238d8794729825bfa477f6b5705e179fbd80c81f41180bb945d7646`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:20:26 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:20:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:20:27 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 04:21:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:21:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 04:21:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:21:25 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:21:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:22:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:22:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 04:22:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:22:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 04:22:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:22:35 GMT
ENV ROS1_DISTRO=noetic
# Thu, 16 Mar 2023 04:22:36 GMT
ENV ROS2_DISTRO=foxy
# Thu, 16 Mar 2023 04:23:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:14 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b6c60e4af795544c6d1c364ed29a2ed8c498f2e5da5a57dea651d7c7a523b5`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eed6591731f4cd0e89ff07e515fd42f1466e54d5fc27307ce4f3b8ae3afb141`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0523ba22e09bf736f80bd994abe837c7b137f287b8eea0f5e7bdbd00da85176c`  
		Last Modified: Thu, 16 Mar 2023 04:46:21 GMT  
		Size: 120.4 MB (120370671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d32eb5055c7800fac72e3cac723ba624a400884ebf5f5a9500ee754097b1e3`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f9d766c59781e81fe431a83896cad4f0713dbabebe97aed5147ad1b93882ff`  
		Last Modified: Thu, 16 Mar 2023 04:46:40 GMT  
		Size: 73.3 MB (73340719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3213fb9cdb02761d0f1588aafdd6d1aea86527d98ac336b4990038700eafd6`  
		Last Modified: Thu, 16 Mar 2023 04:46:30 GMT  
		Size: 279.9 KB (279912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850f044353a9cd5a3393fdcb430d07b7ed8b8ebdf18fc92426f230eff57e4f9`  
		Last Modified: Thu, 16 Mar 2023 04:46:30 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aabf876615ac9c2be0dd9f801770504d13fde42076b0b2f95e4f68dd0c57216`  
		Last Modified: Thu, 16 Mar 2023 04:46:33 GMT  
		Size: 21.7 MB (21662435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c55c6a35c527c80ba41ab57cfc0aeecbcaf03a8e21d52d510181da679bfac6`  
		Last Modified: Thu, 16 Mar 2023 04:46:51 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f20b731e283d25346685de83f1440763ca136e6cc0a35cbe21422d043b972dd`  
		Last Modified: Thu, 16 Mar 2023 04:46:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20660b50a185f3eeb1a43d67bdaeb11a64c73fe6f4e32197642c8408848c6b18`  
		Last Modified: Thu, 16 Mar 2023 04:47:05 GMT  
		Size: 76.4 MB (76429157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad40a10a98c57a7eb642b09195ade82c9548952e17c9fcf1240770d671c7103`  
		Last Modified: Thu, 16 Mar 2023 04:46:56 GMT  
		Size: 21.7 MB (21674281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13756eb5e96bd40ce7f9ad35d1c2b643de10c62455af3309904258c67215e74`  
		Last Modified: Thu, 16 Mar 2023 04:46:51 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ae4f7591eae21b9f0abb07cf02221b942789d6336423f1f0b891f77a40ed9e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317630108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5d55ffb232c17b5db88aa6e0b5cd1d38dd1c0c8c450ffe7bc57137086dd187`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:23:12 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:23:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:23:13 GMT
ENV ROS_DISTRO=foxy
# Thu, 16 Mar 2023 03:24:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:06 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:24:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:24:06 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:24:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:24:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 03:24:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:24:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:24:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:24:59 GMT
ENV ROS1_DISTRO=noetic
# Thu, 16 Mar 2023 03:24:59 GMT
ENV ROS2_DISTRO=foxy
# Thu, 16 Mar 2023 03:25:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.16.0-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:30 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42860775fce781d98f8f21abfafa48660e634182b69b05266851498055971a82`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7191287fc71fa37ace07c3fb721fe8b0df2516866da1e7b98f48aa71b8bdb94e`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e24d2145f0cc2cf9a85047ab49b1f2f4b457e7b81b534c1bfc25642cd3a10fd`  
		Last Modified: Thu, 16 Mar 2023 03:48:43 GMT  
		Size: 104.6 MB (104568150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27f4054f4fcc5c1a7c641b6a19891c7fe042a2d4ba353b8eb7d094b1ccde304`  
		Last Modified: Thu, 16 Mar 2023 03:48:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b61acdd97d95df9976326ba8a1dc79a739c367e9d0232e2ae3560909a891af4`  
		Last Modified: Thu, 16 Mar 2023 03:48:59 GMT  
		Size: 67.7 MB (67684730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11b685a5e9052a6bd9772d42b4900972bc1037ca8648eae13801e200578820`  
		Last Modified: Thu, 16 Mar 2023 03:48:52 GMT  
		Size: 279.9 KB (279917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8d4285dfe20611b685fe67cf842b70a9e8b6409de0e9d12bcc27174be70897`  
		Last Modified: Thu, 16 Mar 2023 03:48:51 GMT  
		Size: 2.4 KB (2412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab10b5ea657202d97bef2d89bc8b1d0d91f7b99e5f04ee9ef87100edfc1dccd`  
		Last Modified: Thu, 16 Mar 2023 03:48:54 GMT  
		Size: 20.4 MB (20385758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9da9850fbdebec3cf3685151e664e038e2628dd8c09bca753e13b538675fcd`  
		Last Modified: Thu, 16 Mar 2023 03:49:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a82cab40cfa91b60ba64a899790a39b77200d232069659d5aaeaf10ee1dbf92`  
		Last Modified: Thu, 16 Mar 2023 03:49:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf248e08c595e13904d0d40d28e22b9f0f5e586c0f55ceba204e34c55b2d334`  
		Last Modified: Thu, 16 Mar 2023 03:49:23 GMT  
		Size: 76.5 MB (76495934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7713413d61c87cbf93543d08a3a476192cbdf1db9eb33cc0dee39d37f60de8f2`  
		Last Modified: Thu, 16 Mar 2023 03:49:12 GMT  
		Size: 14.3 MB (14325733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ee2466e3b53232367b496f7990dd5a5594945dfa09301dd087beee9b2ce3e8`  
		Last Modified: Thu, 16 Mar 2023 03:49:10 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble`

```console
$ docker pull ros@sha256:2337605c48a6ea19b9d569b3d4bc85bbbbecac1127043bcdfef8a413f2509abf
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
$ docker pull ros@sha256:13ae2d3f3fa2154db958fc4c4532d4eee94ad5d1032bcb774ef1fc7d368c4715
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255710392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71fb575afde737ff6d46340ec65ce6e4e2d3c7f1ebfcfd6a664737d25684d802`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 03:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:28:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:28:11 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:29:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:29:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 03:30:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6453cb94f5370ccc175e0beb4b452635a97dfef6eaef28404383ac68f1f1c853`  
		Last Modified: Thu, 16 Mar 2023 03:49:48 GMT  
		Size: 104.1 MB (104059541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36e33dee97e6c3aeef467124304049cb4ac734784ca6a719d90245fdfc3941`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8eae9dc476ad24b977f846a349417e676ed533c003e58f7ee95949832a7602`  
		Last Modified: Thu, 16 Mar 2023 03:50:08 GMT  
		Size: 95.5 MB (95477291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666fc157dbdee31a004f825aa48bbd562084d77e3c4f6af8224ebf3454372bd9`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 314.1 KB (314059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d637ed46ef3f6193062806be0d5578e4896c4814956f0b3430a6df02a081a9f`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eba6bb0da5c90df9800c7413610aa12a00f284a53b94640965b45315cc062f1`  
		Last Modified: Thu, 16 Mar 2023 03:50:01 GMT  
		Size: 22.5 MB (22497013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:3eaa7fd66e074d5a2efd5623c0280fe0e55cad7eef7cb91bc94ad5923121d02d
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
$ docker pull ros@sha256:ef2993e9f537d0b03802fcd6530c9c1f27eb00c0793b48224d87fe6ef35e1dee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1043611616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8d8df5ba19b1b337e12f7a32f280f5463b231bbb4a0d9d084c061e1a7b133f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 03:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:28:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:28:11 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:29:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:29:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 03:30:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:40:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6453cb94f5370ccc175e0beb4b452635a97dfef6eaef28404383ac68f1f1c853`  
		Last Modified: Thu, 16 Mar 2023 03:49:48 GMT  
		Size: 104.1 MB (104059541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36e33dee97e6c3aeef467124304049cb4ac734784ca6a719d90245fdfc3941`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8eae9dc476ad24b977f846a349417e676ed533c003e58f7ee95949832a7602`  
		Last Modified: Thu, 16 Mar 2023 03:50:08 GMT  
		Size: 95.5 MB (95477291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666fc157dbdee31a004f825aa48bbd562084d77e3c4f6af8224ebf3454372bd9`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 314.1 KB (314059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d637ed46ef3f6193062806be0d5578e4896c4814956f0b3430a6df02a081a9f`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eba6bb0da5c90df9800c7413610aa12a00f284a53b94640965b45315cc062f1`  
		Last Modified: Thu, 16 Mar 2023 03:50:01 GMT  
		Size: 22.5 MB (22497013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486b0eb7f86078079369662798d4483c6cffc6565e40357306335b470a254982`  
		Last Modified: Thu, 16 Mar 2023 03:51:39 GMT  
		Size: 787.9 MB (787901224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:3eaa7fd66e074d5a2efd5623c0280fe0e55cad7eef7cb91bc94ad5923121d02d
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
$ docker pull ros@sha256:ef2993e9f537d0b03802fcd6530c9c1f27eb00c0793b48224d87fe6ef35e1dee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1043611616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8d8df5ba19b1b337e12f7a32f280f5463b231bbb4a0d9d084c061e1a7b133f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 03:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:28:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:28:11 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:29:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:29:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 03:30:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:40:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6453cb94f5370ccc175e0beb4b452635a97dfef6eaef28404383ac68f1f1c853`  
		Last Modified: Thu, 16 Mar 2023 03:49:48 GMT  
		Size: 104.1 MB (104059541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36e33dee97e6c3aeef467124304049cb4ac734784ca6a719d90245fdfc3941`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8eae9dc476ad24b977f846a349417e676ed533c003e58f7ee95949832a7602`  
		Last Modified: Thu, 16 Mar 2023 03:50:08 GMT  
		Size: 95.5 MB (95477291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666fc157dbdee31a004f825aa48bbd562084d77e3c4f6af8224ebf3454372bd9`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 314.1 KB (314059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d637ed46ef3f6193062806be0d5578e4896c4814956f0b3430a6df02a081a9f`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eba6bb0da5c90df9800c7413610aa12a00f284a53b94640965b45315cc062f1`  
		Last Modified: Thu, 16 Mar 2023 03:50:01 GMT  
		Size: 22.5 MB (22497013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486b0eb7f86078079369662798d4483c6cffc6565e40357306335b470a254982`  
		Last Modified: Thu, 16 Mar 2023 03:51:39 GMT  
		Size: 787.9 MB (787901224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:2337605c48a6ea19b9d569b3d4bc85bbbbecac1127043bcdfef8a413f2509abf
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
$ docker pull ros@sha256:13ae2d3f3fa2154db958fc4c4532d4eee94ad5d1032bcb774ef1fc7d368c4715
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255710392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71fb575afde737ff6d46340ec65ce6e4e2d3c7f1ebfcfd6a664737d25684d802`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 03:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:28:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:28:11 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:29:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:29:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 03:30:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6453cb94f5370ccc175e0beb4b452635a97dfef6eaef28404383ac68f1f1c853`  
		Last Modified: Thu, 16 Mar 2023 03:49:48 GMT  
		Size: 104.1 MB (104059541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36e33dee97e6c3aeef467124304049cb4ac734784ca6a719d90245fdfc3941`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8eae9dc476ad24b977f846a349417e676ed533c003e58f7ee95949832a7602`  
		Last Modified: Thu, 16 Mar 2023 03:50:08 GMT  
		Size: 95.5 MB (95477291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666fc157dbdee31a004f825aa48bbd562084d77e3c4f6af8224ebf3454372bd9`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 314.1 KB (314059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d637ed46ef3f6193062806be0d5578e4896c4814956f0b3430a6df02a081a9f`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eba6bb0da5c90df9800c7413610aa12a00f284a53b94640965b45315cc062f1`  
		Last Modified: Thu, 16 Mar 2023 03:50:01 GMT  
		Size: 22.5 MB (22497013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:2337605c48a6ea19b9d569b3d4bc85bbbbecac1127043bcdfef8a413f2509abf
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
$ docker pull ros@sha256:13ae2d3f3fa2154db958fc4c4532d4eee94ad5d1032bcb774ef1fc7d368c4715
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255710392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71fb575afde737ff6d46340ec65ce6e4e2d3c7f1ebfcfd6a664737d25684d802`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 03:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:28:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:28:11 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:29:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:29:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 03:30:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6453cb94f5370ccc175e0beb4b452635a97dfef6eaef28404383ac68f1f1c853`  
		Last Modified: Thu, 16 Mar 2023 03:49:48 GMT  
		Size: 104.1 MB (104059541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36e33dee97e6c3aeef467124304049cb4ac734784ca6a719d90245fdfc3941`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8eae9dc476ad24b977f846a349417e676ed533c003e58f7ee95949832a7602`  
		Last Modified: Thu, 16 Mar 2023 03:50:08 GMT  
		Size: 95.5 MB (95477291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666fc157dbdee31a004f825aa48bbd562084d77e3c4f6af8224ebf3454372bd9`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 314.1 KB (314059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d637ed46ef3f6193062806be0d5578e4896c4814956f0b3430a6df02a081a9f`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eba6bb0da5c90df9800c7413610aa12a00f284a53b94640965b45315cc062f1`  
		Last Modified: Thu, 16 Mar 2023 03:50:01 GMT  
		Size: 22.5 MB (22497013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:f6f18fb541500f5d9b4ddae4bef789595dcec7e0b8411036dafd170856d9497c
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
$ docker pull ros@sha256:3c5d133eed60ceb975b905fa43dd55476743f4f4205bae3c5676b830991c11e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137419603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35184dcc5eb48b22a05a63cc0c0d28ad23824a84bf0c74e532d818ea647b1c7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 03:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:28:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:28:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6453cb94f5370ccc175e0beb4b452635a97dfef6eaef28404383ac68f1f1c853`  
		Last Modified: Thu, 16 Mar 2023 03:49:48 GMT  
		Size: 104.1 MB (104059541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36e33dee97e6c3aeef467124304049cb4ac734784ca6a719d90245fdfc3941`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:f6f18fb541500f5d9b4ddae4bef789595dcec7e0b8411036dafd170856d9497c
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
$ docker pull ros@sha256:3c5d133eed60ceb975b905fa43dd55476743f4f4205bae3c5676b830991c11e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137419603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35184dcc5eb48b22a05a63cc0c0d28ad23824a84bf0c74e532d818ea647b1c7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 03:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:28:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:28:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6453cb94f5370ccc175e0beb4b452635a97dfef6eaef28404383ac68f1f1c853`  
		Last Modified: Thu, 16 Mar 2023 03:49:48 GMT  
		Size: 104.1 MB (104059541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36e33dee97e6c3aeef467124304049cb4ac734784ca6a719d90245fdfc3941`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:2337605c48a6ea19b9d569b3d4bc85bbbbecac1127043bcdfef8a413f2509abf
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
$ docker pull ros@sha256:13ae2d3f3fa2154db958fc4c4532d4eee94ad5d1032bcb774ef1fc7d368c4715
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255710392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71fb575afde737ff6d46340ec65ce6e4e2d3c7f1ebfcfd6a664737d25684d802`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV ROS_DISTRO=humble
# Thu, 16 Mar 2023 03:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 16 Mar 2023 03:28:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:28:11 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:29:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:29:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Mar 2023 03:30:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6453cb94f5370ccc175e0beb4b452635a97dfef6eaef28404383ac68f1f1c853`  
		Last Modified: Thu, 16 Mar 2023 03:49:48 GMT  
		Size: 104.1 MB (104059541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36e33dee97e6c3aeef467124304049cb4ac734784ca6a719d90245fdfc3941`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8eae9dc476ad24b977f846a349417e676ed533c003e58f7ee95949832a7602`  
		Last Modified: Thu, 16 Mar 2023 03:50:08 GMT  
		Size: 95.5 MB (95477291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666fc157dbdee31a004f825aa48bbd562084d77e3c4f6af8224ebf3454372bd9`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 314.1 KB (314059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d637ed46ef3f6193062806be0d5578e4896c4814956f0b3430a6df02a081a9f`  
		Last Modified: Thu, 16 Mar 2023 03:49:58 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eba6bb0da5c90df9800c7413610aa12a00f284a53b94640965b45315cc062f1`  
		Last Modified: Thu, 16 Mar 2023 03:50:01 GMT  
		Size: 22.5 MB (22497013 bytes)  
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
$ docker pull ros@sha256:be96e3bf51930fa25d98ca9631a79a11e5262529687ca2afd291d5baca5e4845
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:f8f42074222bd00a9b089d9f34036abf91b68a35c03e423398a3e64d59dfe62f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343164665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b56a2c6b724820ee06e125c51e8e704a6b4ba61bbfebcf16af198e602cb642f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 04:09:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:09:06 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:04 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:11:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:11:04 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:11:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:13:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adae176e5cd2a30cf1122ee112b4b721b01ea9b4c0ac5e541d66c07aaaec48`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adccda1b6439c0a801a24fa60738b89782e4c7193200f6f27ce29713715eb56`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82508576a99a0a8d8797589d2c709fa671510864b5270428799fc45a75007041`  
		Last Modified: Thu, 16 Mar 2023 04:43:53 GMT  
		Size: 177.0 MB (177011633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581df5fa2a83d010d48e7b47f737a951bda847f9ee5c724e9ccc3856cf28ee08`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32822115c02183cc93979e5eb6530d84df2e5871996db9b7dc7c65443966bf1`  
		Last Modified: Thu, 16 Mar 2023 04:44:11 GMT  
		Size: 50.9 MB (50940109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d2b3f91c40b14acd615fbc7eb23e2ae46a9e339e795fc221fdc21561270f58`  
		Last Modified: Thu, 16 Mar 2023 04:44:03 GMT  
		Size: 317.4 KB (317353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304ec1393d4ab6577989c766d2b4172d18d06a2d05bc1685889432e70a066f40`  
		Last Modified: Thu, 16 Mar 2023 04:44:15 GMT  
		Size: 79.6 MB (79606953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:f69b4e9d767e0f5ea05e053e59c7683f87cea0d6d42ee8fa0abd2cd6cc674eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289247972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60b6d51cdc636dd5e3e07574122c2df344fdf9002803cca05876ffc5e08153b2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:25:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:27:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:27:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:27:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:27:55 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:28:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07a04d14911f425c252acad00ad16f68336179fdb2bd057ecbc008654d4a9dc`  
		Last Modified: Thu, 16 Mar 2023 03:41:09 GMT  
		Size: 1.2 MB (1154620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3bf1f4e2e473ac685bd824bf2830576a48ab98791369a09fea2d0dbd4a929f`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 4.7 MB (4679050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6ed9de687ca448ae7407bb48c22de4deda7d30a973cef11a4b6d8d8fb38e7`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa126a480cce3f126ceba011ffee67346db673365bb738950073ba2ba74783`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0c85b3c21b15d3eb1f9e6b0b89b695ba25d60a4591c501019a1276bc0fd1e5`  
		Last Modified: Thu, 16 Mar 2023 03:41:35 GMT  
		Size: 157.5 MB (157508946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015ee579e11221f21424f6a032081a7ccc05e90c3115b747cd39125644bd52f`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502398c5b962c956411f0c9bb61dc5d8cb53a75a822beab1a67338a6040844da`  
		Last Modified: Thu, 16 Mar 2023 03:41:51 GMT  
		Size: 40.5 MB (40502661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4016c5932fe61d99fdb58e6cc4986e20a201b4c0ebac799059f2dd4d5f430ab`  
		Last Modified: Thu, 16 Mar 2023 03:41:46 GMT  
		Size: 317.3 KB (317345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5a37a447e1f58827e4f91f66e94e8e7a186d73e26aed5bd96060931f145801`  
		Last Modified: Thu, 16 Mar 2023 03:41:55 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b576d3034caf213b58905fae455fcdcde299046f2f53f1801f032c876e25e6ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322875712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdc6ebcdb919385e49b76876c7c7b36a8b277493a63efdaa1e0f53241e0478ed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:10:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:12:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:12:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:12:47 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:13:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:14:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b33d380951389d9d1ce91514fb73e120ca3b974c248cd2f314992c3465b2b9`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfba233f21202f1db01a89b8102baef60e3122f36c4d66830892d50d49066`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e709008824e0a6b98c808a5f0f85b444a3e58e2c5b46f6addc72a67e87ae918`  
		Last Modified: Thu, 16 Mar 2023 03:46:40 GMT  
		Size: 171.5 MB (171493131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111abfb9fbc2b0549a5f36a5dfe15229955477056115fe93d5630e6dcbf67970`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2d073551834d896f537facf3e35341eb2ab136a5aaf7fb5c935c3bb5c7126e`  
		Last Modified: Thu, 16 Mar 2023 03:46:55 GMT  
		Size: 45.2 MB (45203778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518a989d6dba523fd6a7f2604b03c29146262b03f347c30dfd5e306f8de1c10c`  
		Last Modified: Thu, 16 Mar 2023 03:46:50 GMT  
		Size: 317.4 KB (317350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17de9a769b38ea53a05082bc632c3a08673f269fff61bb683575c1ef260f8862`  
		Last Modified: Thu, 16 Mar 2023 03:47:00 GMT  
		Size: 72.0 MB (71974610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:7a2a28827571d9b99ccae998d72566029852f2107abf1c152029885bee8c6e7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:96fd163c12a7b98719686f7e2bd2254c72b8113f23c563f305a92e01cffdc4c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.1 MB (835137037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a90707807cb54af5c80b8e1afcaa6d3dde3e7b431af07f0be2cf5fd44597483`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 04:09:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:09:06 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:04 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:11:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:11:04 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:11:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:13:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:19:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adae176e5cd2a30cf1122ee112b4b721b01ea9b4c0ac5e541d66c07aaaec48`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adccda1b6439c0a801a24fa60738b89782e4c7193200f6f27ce29713715eb56`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82508576a99a0a8d8797589d2c709fa671510864b5270428799fc45a75007041`  
		Last Modified: Thu, 16 Mar 2023 04:43:53 GMT  
		Size: 177.0 MB (177011633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581df5fa2a83d010d48e7b47f737a951bda847f9ee5c724e9ccc3856cf28ee08`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32822115c02183cc93979e5eb6530d84df2e5871996db9b7dc7c65443966bf1`  
		Last Modified: Thu, 16 Mar 2023 04:44:11 GMT  
		Size: 50.9 MB (50940109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d2b3f91c40b14acd615fbc7eb23e2ae46a9e339e795fc221fdc21561270f58`  
		Last Modified: Thu, 16 Mar 2023 04:44:03 GMT  
		Size: 317.4 KB (317353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304ec1393d4ab6577989c766d2b4172d18d06a2d05bc1685889432e70a066f40`  
		Last Modified: Thu, 16 Mar 2023 04:44:15 GMT  
		Size: 79.6 MB (79606953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa602089cfc9a551e4c6c4314ef7fd36039fd36229a50dfd4a220a9ea30d5d`  
		Last Modified: Thu, 16 Mar 2023 04:45:49 GMT  
		Size: 492.0 MB (491972372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:5d712eee029d47a123de2fe7bcec5f7c0e875c3025bc80b7d54a80112df0f2d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726168090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5512c37a43ed1d0f691ed805b8439660ea4acb411e6a500894893f74530f589e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:25:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:27:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:27:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:27:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:27:55 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:28:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:38:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07a04d14911f425c252acad00ad16f68336179fdb2bd057ecbc008654d4a9dc`  
		Last Modified: Thu, 16 Mar 2023 03:41:09 GMT  
		Size: 1.2 MB (1154620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3bf1f4e2e473ac685bd824bf2830576a48ab98791369a09fea2d0dbd4a929f`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 4.7 MB (4679050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6ed9de687ca448ae7407bb48c22de4deda7d30a973cef11a4b6d8d8fb38e7`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa126a480cce3f126ceba011ffee67346db673365bb738950073ba2ba74783`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0c85b3c21b15d3eb1f9e6b0b89b695ba25d60a4591c501019a1276bc0fd1e5`  
		Last Modified: Thu, 16 Mar 2023 03:41:35 GMT  
		Size: 157.5 MB (157508946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015ee579e11221f21424f6a032081a7ccc05e90c3115b747cd39125644bd52f`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502398c5b962c956411f0c9bb61dc5d8cb53a75a822beab1a67338a6040844da`  
		Last Modified: Thu, 16 Mar 2023 03:41:51 GMT  
		Size: 40.5 MB (40502661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4016c5932fe61d99fdb58e6cc4986e20a201b4c0ebac799059f2dd4d5f430ab`  
		Last Modified: Thu, 16 Mar 2023 03:41:46 GMT  
		Size: 317.3 KB (317345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5a37a447e1f58827e4f91f66e94e8e7a186d73e26aed5bd96060931f145801`  
		Last Modified: Thu, 16 Mar 2023 03:41:55 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b343405c024c81c76c2c966618c8481c0c72a9e06d4e2224ce21057a8d82adf`  
		Last Modified: Thu, 16 Mar 2023 03:43:21 GMT  
		Size: 436.9 MB (436920118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:aed092d7100de07fd7543975f1ad590fec1fcb887b86dbf59943d5cecb560ab7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.4 MB (785439188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d27e47e27f2d7226090a303ab88411198eaf7d451074be86bccec15bfc4e7d77`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:10:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:12:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:12:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:12:47 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:13:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:14:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b33d380951389d9d1ce91514fb73e120ca3b974c248cd2f314992c3465b2b9`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfba233f21202f1db01a89b8102baef60e3122f36c4d66830892d50d49066`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e709008824e0a6b98c808a5f0f85b444a3e58e2c5b46f6addc72a67e87ae918`  
		Last Modified: Thu, 16 Mar 2023 03:46:40 GMT  
		Size: 171.5 MB (171493131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111abfb9fbc2b0549a5f36a5dfe15229955477056115fe93d5630e6dcbf67970`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2d073551834d896f537facf3e35341eb2ab136a5aaf7fb5c935c3bb5c7126e`  
		Last Modified: Thu, 16 Mar 2023 03:46:55 GMT  
		Size: 45.2 MB (45203778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518a989d6dba523fd6a7f2604b03c29146262b03f347c30dfd5e306f8de1c10c`  
		Last Modified: Thu, 16 Mar 2023 03:46:50 GMT  
		Size: 317.4 KB (317350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17de9a769b38ea53a05082bc632c3a08673f269fff61bb683575c1ef260f8862`  
		Last Modified: Thu, 16 Mar 2023 03:47:00 GMT  
		Size: 72.0 MB (71974610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c222849614ae4a8fe5d83b4fe2e00757edc0d9d8c21a6d2b2500dff1c7d1bddb`  
		Last Modified: Thu, 16 Mar 2023 03:48:17 GMT  
		Size: 462.6 MB (462563476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:a16987d5d6729ea57d120332059ed56e1eb7612a7f9aaccafa83a55c00c4c790
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
$ docker pull ros@sha256:980152242b671d03db9a26efee4daf2633661b4247037bbd3acc946f3ac4444b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **868.1 MB (868115447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e8b5202e5fb2faaf4a1dee3bd47c886e64dc7f1589ca5a6b67bb2579e11c30`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:17:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:17:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 Apr 2023 03:17:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 Apr 2023 03:17:50 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 03:17:50 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 Apr 2023 03:17:50 GMT
ENV ROS_DISTRO=noetic
# Wed, 12 Apr 2023 03:19:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:19:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 12 Apr 2023 03:19:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 Apr 2023 03:19:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:19:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 12 Apr 2023 03:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:24:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926daaa3f39d210833d9a3a75b2e33aafd38f4adcda623bb40686f5480d8eda7`  
		Last Modified: Wed, 12 Apr 2023 03:25:46 GMT  
		Size: 10.9 MB (10902667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ef889428a3c0c2686a4bb8d4e5af08778a1b25251d4873a4635b0b2af721d8`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b211d556fba373cffc4c30d24942793ca6d51c78179037897e5f465fc65e4408`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161bac3145a70b13a85c49796d22151dc27a76ea04b256183b318cc9efc8686d`  
		Last Modified: Wed, 12 Apr 2023 03:26:06 GMT  
		Size: 184.4 MB (184427087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91b09fc5f446950a1e8e392c05737de9820b95e50745e93232b6ff4dba0617`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d31bfc2a7fad06ba1563ddcf7f96daf937621936041ba76fb2e42b45d9f327`  
		Last Modified: Wed, 12 Apr 2023 03:26:21 GMT  
		Size: 84.4 MB (84395801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ec420fccc4bc3cf3805910ff22f8789cd48387fcefed5829785ab9279e8e9f`  
		Last Modified: Wed, 12 Apr 2023 03:26:13 GMT  
		Size: 313.0 KB (312977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e8033e5e52d2e2310af7d82b5846e3f1900897dee49ceb23bf0721dac3353e`  
		Last Modified: Wed, 12 Apr 2023 03:26:20 GMT  
		Size: 74.1 MB (74090563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c366ae282bf50e572d970fd7d54011aaa06faca583dc1548110f0865cdc3809`  
		Last Modified: Wed, 12 Apr 2023 03:27:22 GMT  
		Size: 464.7 MB (464745308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:7a2a28827571d9b99ccae998d72566029852f2107abf1c152029885bee8c6e7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:96fd163c12a7b98719686f7e2bd2254c72b8113f23c563f305a92e01cffdc4c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.1 MB (835137037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a90707807cb54af5c80b8e1afcaa6d3dde3e7b431af07f0be2cf5fd44597483`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 04:09:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:09:06 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:04 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:11:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:11:04 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:11:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:13:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:19:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adae176e5cd2a30cf1122ee112b4b721b01ea9b4c0ac5e541d66c07aaaec48`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adccda1b6439c0a801a24fa60738b89782e4c7193200f6f27ce29713715eb56`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82508576a99a0a8d8797589d2c709fa671510864b5270428799fc45a75007041`  
		Last Modified: Thu, 16 Mar 2023 04:43:53 GMT  
		Size: 177.0 MB (177011633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581df5fa2a83d010d48e7b47f737a951bda847f9ee5c724e9ccc3856cf28ee08`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32822115c02183cc93979e5eb6530d84df2e5871996db9b7dc7c65443966bf1`  
		Last Modified: Thu, 16 Mar 2023 04:44:11 GMT  
		Size: 50.9 MB (50940109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d2b3f91c40b14acd615fbc7eb23e2ae46a9e339e795fc221fdc21561270f58`  
		Last Modified: Thu, 16 Mar 2023 04:44:03 GMT  
		Size: 317.4 KB (317353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304ec1393d4ab6577989c766d2b4172d18d06a2d05bc1685889432e70a066f40`  
		Last Modified: Thu, 16 Mar 2023 04:44:15 GMT  
		Size: 79.6 MB (79606953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa602089cfc9a551e4c6c4314ef7fd36039fd36229a50dfd4a220a9ea30d5d`  
		Last Modified: Thu, 16 Mar 2023 04:45:49 GMT  
		Size: 492.0 MB (491972372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:5d712eee029d47a123de2fe7bcec5f7c0e875c3025bc80b7d54a80112df0f2d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726168090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5512c37a43ed1d0f691ed805b8439660ea4acb411e6a500894893f74530f589e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:25:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:27:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:27:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:27:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:27:55 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:28:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:38:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07a04d14911f425c252acad00ad16f68336179fdb2bd057ecbc008654d4a9dc`  
		Last Modified: Thu, 16 Mar 2023 03:41:09 GMT  
		Size: 1.2 MB (1154620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3bf1f4e2e473ac685bd824bf2830576a48ab98791369a09fea2d0dbd4a929f`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 4.7 MB (4679050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6ed9de687ca448ae7407bb48c22de4deda7d30a973cef11a4b6d8d8fb38e7`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa126a480cce3f126ceba011ffee67346db673365bb738950073ba2ba74783`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0c85b3c21b15d3eb1f9e6b0b89b695ba25d60a4591c501019a1276bc0fd1e5`  
		Last Modified: Thu, 16 Mar 2023 03:41:35 GMT  
		Size: 157.5 MB (157508946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015ee579e11221f21424f6a032081a7ccc05e90c3115b747cd39125644bd52f`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502398c5b962c956411f0c9bb61dc5d8cb53a75a822beab1a67338a6040844da`  
		Last Modified: Thu, 16 Mar 2023 03:41:51 GMT  
		Size: 40.5 MB (40502661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4016c5932fe61d99fdb58e6cc4986e20a201b4c0ebac799059f2dd4d5f430ab`  
		Last Modified: Thu, 16 Mar 2023 03:41:46 GMT  
		Size: 317.3 KB (317345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5a37a447e1f58827e4f91f66e94e8e7a186d73e26aed5bd96060931f145801`  
		Last Modified: Thu, 16 Mar 2023 03:41:55 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b343405c024c81c76c2c966618c8481c0c72a9e06d4e2224ce21057a8d82adf`  
		Last Modified: Thu, 16 Mar 2023 03:43:21 GMT  
		Size: 436.9 MB (436920118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:aed092d7100de07fd7543975f1ad590fec1fcb887b86dbf59943d5cecb560ab7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.4 MB (785439188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d27e47e27f2d7226090a303ab88411198eaf7d451074be86bccec15bfc4e7d77`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:10:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:12:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:12:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:12:47 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:13:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:14:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:22:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b33d380951389d9d1ce91514fb73e120ca3b974c248cd2f314992c3465b2b9`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfba233f21202f1db01a89b8102baef60e3122f36c4d66830892d50d49066`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e709008824e0a6b98c808a5f0f85b444a3e58e2c5b46f6addc72a67e87ae918`  
		Last Modified: Thu, 16 Mar 2023 03:46:40 GMT  
		Size: 171.5 MB (171493131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111abfb9fbc2b0549a5f36a5dfe15229955477056115fe93d5630e6dcbf67970`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2d073551834d896f537facf3e35341eb2ab136a5aaf7fb5c935c3bb5c7126e`  
		Last Modified: Thu, 16 Mar 2023 03:46:55 GMT  
		Size: 45.2 MB (45203778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518a989d6dba523fd6a7f2604b03c29146262b03f347c30dfd5e306f8de1c10c`  
		Last Modified: Thu, 16 Mar 2023 03:46:50 GMT  
		Size: 317.4 KB (317350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17de9a769b38ea53a05082bc632c3a08673f269fff61bb683575c1ef260f8862`  
		Last Modified: Thu, 16 Mar 2023 03:47:00 GMT  
		Size: 72.0 MB (71974610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c222849614ae4a8fe5d83b4fe2e00757edc0d9d8c21a6d2b2500dff1c7d1bddb`  
		Last Modified: Thu, 16 Mar 2023 03:48:17 GMT  
		Size: 462.6 MB (462563476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:b4f75a1493e450e2bec6a0f054c38bfe7ef4fac1611486cc4d13d6def1a8eb73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:574009f1d453ec8933f2778451c16cdfe517e40255e013eeb8504386efde77c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359026756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5871024add8b14999e293a94e8a751593359ded58c238016827e00884a7f1b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 04:09:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:09:06 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:04 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:11:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:11:04 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:11:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:13:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:13:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adae176e5cd2a30cf1122ee112b4b721b01ea9b4c0ac5e541d66c07aaaec48`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adccda1b6439c0a801a24fa60738b89782e4c7193200f6f27ce29713715eb56`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82508576a99a0a8d8797589d2c709fa671510864b5270428799fc45a75007041`  
		Last Modified: Thu, 16 Mar 2023 04:43:53 GMT  
		Size: 177.0 MB (177011633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581df5fa2a83d010d48e7b47f737a951bda847f9ee5c724e9ccc3856cf28ee08`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32822115c02183cc93979e5eb6530d84df2e5871996db9b7dc7c65443966bf1`  
		Last Modified: Thu, 16 Mar 2023 04:44:11 GMT  
		Size: 50.9 MB (50940109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d2b3f91c40b14acd615fbc7eb23e2ae46a9e339e795fc221fdc21561270f58`  
		Last Modified: Thu, 16 Mar 2023 04:44:03 GMT  
		Size: 317.4 KB (317353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304ec1393d4ab6577989c766d2b4172d18d06a2d05bc1685889432e70a066f40`  
		Last Modified: Thu, 16 Mar 2023 04:44:15 GMT  
		Size: 79.6 MB (79606953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52d1f5433523d03a1d3cf6639659a32287776c83897bc6065b762307771ebe6`  
		Last Modified: Thu, 16 Mar 2023 04:44:29 GMT  
		Size: 15.9 MB (15862091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:58d03ae5f07375ed708bf57ef870c9badee6c37d655580dc3c9c4d662b1f7b83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303314726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb179eeb6e4d9ea28a9de61c36783e599077fa519e4f623328b533e4acfc0b6c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:25:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:27:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:27:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:27:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:27:55 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:28:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:30:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07a04d14911f425c252acad00ad16f68336179fdb2bd057ecbc008654d4a9dc`  
		Last Modified: Thu, 16 Mar 2023 03:41:09 GMT  
		Size: 1.2 MB (1154620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3bf1f4e2e473ac685bd824bf2830576a48ab98791369a09fea2d0dbd4a929f`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 4.7 MB (4679050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6ed9de687ca448ae7407bb48c22de4deda7d30a973cef11a4b6d8d8fb38e7`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa126a480cce3f126ceba011ffee67346db673365bb738950073ba2ba74783`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0c85b3c21b15d3eb1f9e6b0b89b695ba25d60a4591c501019a1276bc0fd1e5`  
		Last Modified: Thu, 16 Mar 2023 03:41:35 GMT  
		Size: 157.5 MB (157508946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015ee579e11221f21424f6a032081a7ccc05e90c3115b747cd39125644bd52f`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502398c5b962c956411f0c9bb61dc5d8cb53a75a822beab1a67338a6040844da`  
		Last Modified: Thu, 16 Mar 2023 03:41:51 GMT  
		Size: 40.5 MB (40502661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4016c5932fe61d99fdb58e6cc4986e20a201b4c0ebac799059f2dd4d5f430ab`  
		Last Modified: Thu, 16 Mar 2023 03:41:46 GMT  
		Size: 317.3 KB (317345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5a37a447e1f58827e4f91f66e94e8e7a186d73e26aed5bd96060931f145801`  
		Last Modified: Thu, 16 Mar 2023 03:41:55 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d6fc98f11693bedefdd8353d4eedd821ce365a46b6151b40d79a9d3a4ccd37`  
		Last Modified: Thu, 16 Mar 2023 03:42:12 GMT  
		Size: 14.1 MB (14066754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d0e68cde141a45dd521a278286ce856ac5afc9c8258b5698e927ff51a8db0cdf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338334185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3849a5dac73709d6eb2ddbda097f48ef4c89ac11030b12573341cdbe465144b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:10:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:12:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:12:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:12:47 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:13:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:14:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:15:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b33d380951389d9d1ce91514fb73e120ca3b974c248cd2f314992c3465b2b9`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfba233f21202f1db01a89b8102baef60e3122f36c4d66830892d50d49066`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e709008824e0a6b98c808a5f0f85b444a3e58e2c5b46f6addc72a67e87ae918`  
		Last Modified: Thu, 16 Mar 2023 03:46:40 GMT  
		Size: 171.5 MB (171493131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111abfb9fbc2b0549a5f36a5dfe15229955477056115fe93d5630e6dcbf67970`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2d073551834d896f537facf3e35341eb2ab136a5aaf7fb5c935c3bb5c7126e`  
		Last Modified: Thu, 16 Mar 2023 03:46:55 GMT  
		Size: 45.2 MB (45203778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518a989d6dba523fd6a7f2604b03c29146262b03f347c30dfd5e306f8de1c10c`  
		Last Modified: Thu, 16 Mar 2023 03:46:50 GMT  
		Size: 317.4 KB (317350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17de9a769b38ea53a05082bc632c3a08673f269fff61bb683575c1ef260f8862`  
		Last Modified: Thu, 16 Mar 2023 03:47:00 GMT  
		Size: 72.0 MB (71974610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2078c240094ca97068561d642ba0cd83348ba779f215bb56ecebe305632e51`  
		Last Modified: Thu, 16 Mar 2023 03:47:13 GMT  
		Size: 15.5 MB (15458473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:3943c809ce16fde33fc81d33f181c658a9e9e730d4eaee03f82d73f5e27b83af
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
$ docker pull ros@sha256:e02060cddc00b5e7425b09f32d96167b94622b3f1eee50fc5098e674fc3c60bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.2 MB (424191041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:582ac484d974eb0b874fa8dbce396a268b8582220cdc2c68768393ace9d01a40`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:17:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:17:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 Apr 2023 03:17:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 Apr 2023 03:17:50 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 03:17:50 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 Apr 2023 03:17:50 GMT
ENV ROS_DISTRO=noetic
# Wed, 12 Apr 2023 03:19:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:19:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 12 Apr 2023 03:19:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 Apr 2023 03:19:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:19:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 12 Apr 2023 03:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:21:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926daaa3f39d210833d9a3a75b2e33aafd38f4adcda623bb40686f5480d8eda7`  
		Last Modified: Wed, 12 Apr 2023 03:25:46 GMT  
		Size: 10.9 MB (10902667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ef889428a3c0c2686a4bb8d4e5af08778a1b25251d4873a4635b0b2af721d8`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b211d556fba373cffc4c30d24942793ca6d51c78179037897e5f465fc65e4408`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161bac3145a70b13a85c49796d22151dc27a76ea04b256183b318cc9efc8686d`  
		Last Modified: Wed, 12 Apr 2023 03:26:06 GMT  
		Size: 184.4 MB (184427087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91b09fc5f446950a1e8e392c05737de9820b95e50745e93232b6ff4dba0617`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d31bfc2a7fad06ba1563ddcf7f96daf937621936041ba76fb2e42b45d9f327`  
		Last Modified: Wed, 12 Apr 2023 03:26:21 GMT  
		Size: 84.4 MB (84395801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ec420fccc4bc3cf3805910ff22f8789cd48387fcefed5829785ab9279e8e9f`  
		Last Modified: Wed, 12 Apr 2023 03:26:13 GMT  
		Size: 313.0 KB (312977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e8033e5e52d2e2310af7d82b5846e3f1900897dee49ceb23bf0721dac3353e`  
		Last Modified: Wed, 12 Apr 2023 03:26:20 GMT  
		Size: 74.1 MB (74090563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea9d228ccf7178e163cfc639dea467a73470e631550cd2c405a24752317598e`  
		Last Modified: Wed, 12 Apr 2023 03:26:29 GMT  
		Size: 20.8 MB (20820902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:b4f75a1493e450e2bec6a0f054c38bfe7ef4fac1611486cc4d13d6def1a8eb73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:574009f1d453ec8933f2778451c16cdfe517e40255e013eeb8504386efde77c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359026756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5871024add8b14999e293a94e8a751593359ded58c238016827e00884a7f1b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 04:09:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:09:06 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:04 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:11:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:11:04 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:11:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:13:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:13:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adae176e5cd2a30cf1122ee112b4b721b01ea9b4c0ac5e541d66c07aaaec48`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adccda1b6439c0a801a24fa60738b89782e4c7193200f6f27ce29713715eb56`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82508576a99a0a8d8797589d2c709fa671510864b5270428799fc45a75007041`  
		Last Modified: Thu, 16 Mar 2023 04:43:53 GMT  
		Size: 177.0 MB (177011633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581df5fa2a83d010d48e7b47f737a951bda847f9ee5c724e9ccc3856cf28ee08`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32822115c02183cc93979e5eb6530d84df2e5871996db9b7dc7c65443966bf1`  
		Last Modified: Thu, 16 Mar 2023 04:44:11 GMT  
		Size: 50.9 MB (50940109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d2b3f91c40b14acd615fbc7eb23e2ae46a9e339e795fc221fdc21561270f58`  
		Last Modified: Thu, 16 Mar 2023 04:44:03 GMT  
		Size: 317.4 KB (317353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304ec1393d4ab6577989c766d2b4172d18d06a2d05bc1685889432e70a066f40`  
		Last Modified: Thu, 16 Mar 2023 04:44:15 GMT  
		Size: 79.6 MB (79606953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52d1f5433523d03a1d3cf6639659a32287776c83897bc6065b762307771ebe6`  
		Last Modified: Thu, 16 Mar 2023 04:44:29 GMT  
		Size: 15.9 MB (15862091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:58d03ae5f07375ed708bf57ef870c9badee6c37d655580dc3c9c4d662b1f7b83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303314726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb179eeb6e4d9ea28a9de61c36783e599077fa519e4f623328b533e4acfc0b6c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:25:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:27:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:27:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:27:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:27:55 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:28:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:30:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07a04d14911f425c252acad00ad16f68336179fdb2bd057ecbc008654d4a9dc`  
		Last Modified: Thu, 16 Mar 2023 03:41:09 GMT  
		Size: 1.2 MB (1154620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3bf1f4e2e473ac685bd824bf2830576a48ab98791369a09fea2d0dbd4a929f`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 4.7 MB (4679050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6ed9de687ca448ae7407bb48c22de4deda7d30a973cef11a4b6d8d8fb38e7`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa126a480cce3f126ceba011ffee67346db673365bb738950073ba2ba74783`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0c85b3c21b15d3eb1f9e6b0b89b695ba25d60a4591c501019a1276bc0fd1e5`  
		Last Modified: Thu, 16 Mar 2023 03:41:35 GMT  
		Size: 157.5 MB (157508946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015ee579e11221f21424f6a032081a7ccc05e90c3115b747cd39125644bd52f`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502398c5b962c956411f0c9bb61dc5d8cb53a75a822beab1a67338a6040844da`  
		Last Modified: Thu, 16 Mar 2023 03:41:51 GMT  
		Size: 40.5 MB (40502661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4016c5932fe61d99fdb58e6cc4986e20a201b4c0ebac799059f2dd4d5f430ab`  
		Last Modified: Thu, 16 Mar 2023 03:41:46 GMT  
		Size: 317.3 KB (317345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5a37a447e1f58827e4f91f66e94e8e7a186d73e26aed5bd96060931f145801`  
		Last Modified: Thu, 16 Mar 2023 03:41:55 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d6fc98f11693bedefdd8353d4eedd821ce365a46b6151b40d79a9d3a4ccd37`  
		Last Modified: Thu, 16 Mar 2023 03:42:12 GMT  
		Size: 14.1 MB (14066754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d0e68cde141a45dd521a278286ce856ac5afc9c8258b5698e927ff51a8db0cdf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338334185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3849a5dac73709d6eb2ddbda097f48ef4c89ac11030b12573341cdbe465144b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:10:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:12:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:12:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:12:47 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:13:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:14:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:15:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b33d380951389d9d1ce91514fb73e120ca3b974c248cd2f314992c3465b2b9`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfba233f21202f1db01a89b8102baef60e3122f36c4d66830892d50d49066`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e709008824e0a6b98c808a5f0f85b444a3e58e2c5b46f6addc72a67e87ae918`  
		Last Modified: Thu, 16 Mar 2023 03:46:40 GMT  
		Size: 171.5 MB (171493131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111abfb9fbc2b0549a5f36a5dfe15229955477056115fe93d5630e6dcbf67970`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2d073551834d896f537facf3e35341eb2ab136a5aaf7fb5c935c3bb5c7126e`  
		Last Modified: Thu, 16 Mar 2023 03:46:55 GMT  
		Size: 45.2 MB (45203778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518a989d6dba523fd6a7f2604b03c29146262b03f347c30dfd5e306f8de1c10c`  
		Last Modified: Thu, 16 Mar 2023 03:46:50 GMT  
		Size: 317.4 KB (317350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17de9a769b38ea53a05082bc632c3a08673f269fff61bb683575c1ef260f8862`  
		Last Modified: Thu, 16 Mar 2023 03:47:00 GMT  
		Size: 72.0 MB (71974610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2078c240094ca97068561d642ba0cd83348ba779f215bb56ecebe305632e51`  
		Last Modified: Thu, 16 Mar 2023 03:47:13 GMT  
		Size: 15.5 MB (15458473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:be96e3bf51930fa25d98ca9631a79a11e5262529687ca2afd291d5baca5e4845
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:f8f42074222bd00a9b089d9f34036abf91b68a35c03e423398a3e64d59dfe62f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343164665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b56a2c6b724820ee06e125c51e8e704a6b4ba61bbfebcf16af198e602cb642f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 04:09:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:09:06 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:04 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:11:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:11:04 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:11:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:13:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adae176e5cd2a30cf1122ee112b4b721b01ea9b4c0ac5e541d66c07aaaec48`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adccda1b6439c0a801a24fa60738b89782e4c7193200f6f27ce29713715eb56`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82508576a99a0a8d8797589d2c709fa671510864b5270428799fc45a75007041`  
		Last Modified: Thu, 16 Mar 2023 04:43:53 GMT  
		Size: 177.0 MB (177011633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581df5fa2a83d010d48e7b47f737a951bda847f9ee5c724e9ccc3856cf28ee08`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32822115c02183cc93979e5eb6530d84df2e5871996db9b7dc7c65443966bf1`  
		Last Modified: Thu, 16 Mar 2023 04:44:11 GMT  
		Size: 50.9 MB (50940109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d2b3f91c40b14acd615fbc7eb23e2ae46a9e339e795fc221fdc21561270f58`  
		Last Modified: Thu, 16 Mar 2023 04:44:03 GMT  
		Size: 317.4 KB (317353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304ec1393d4ab6577989c766d2b4172d18d06a2d05bc1685889432e70a066f40`  
		Last Modified: Thu, 16 Mar 2023 04:44:15 GMT  
		Size: 79.6 MB (79606953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:f69b4e9d767e0f5ea05e053e59c7683f87cea0d6d42ee8fa0abd2cd6cc674eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289247972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60b6d51cdc636dd5e3e07574122c2df344fdf9002803cca05876ffc5e08153b2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:25:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:27:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:27:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:27:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:27:55 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:28:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07a04d14911f425c252acad00ad16f68336179fdb2bd057ecbc008654d4a9dc`  
		Last Modified: Thu, 16 Mar 2023 03:41:09 GMT  
		Size: 1.2 MB (1154620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3bf1f4e2e473ac685bd824bf2830576a48ab98791369a09fea2d0dbd4a929f`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 4.7 MB (4679050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6ed9de687ca448ae7407bb48c22de4deda7d30a973cef11a4b6d8d8fb38e7`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa126a480cce3f126ceba011ffee67346db673365bb738950073ba2ba74783`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0c85b3c21b15d3eb1f9e6b0b89b695ba25d60a4591c501019a1276bc0fd1e5`  
		Last Modified: Thu, 16 Mar 2023 03:41:35 GMT  
		Size: 157.5 MB (157508946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015ee579e11221f21424f6a032081a7ccc05e90c3115b747cd39125644bd52f`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502398c5b962c956411f0c9bb61dc5d8cb53a75a822beab1a67338a6040844da`  
		Last Modified: Thu, 16 Mar 2023 03:41:51 GMT  
		Size: 40.5 MB (40502661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4016c5932fe61d99fdb58e6cc4986e20a201b4c0ebac799059f2dd4d5f430ab`  
		Last Modified: Thu, 16 Mar 2023 03:41:46 GMT  
		Size: 317.3 KB (317345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5a37a447e1f58827e4f91f66e94e8e7a186d73e26aed5bd96060931f145801`  
		Last Modified: Thu, 16 Mar 2023 03:41:55 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b576d3034caf213b58905fae455fcdcde299046f2f53f1801f032c876e25e6ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322875712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdc6ebcdb919385e49b76876c7c7b36a8b277493a63efdaa1e0f53241e0478ed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:10:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:12:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:12:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:12:47 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:13:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:14:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b33d380951389d9d1ce91514fb73e120ca3b974c248cd2f314992c3465b2b9`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfba233f21202f1db01a89b8102baef60e3122f36c4d66830892d50d49066`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e709008824e0a6b98c808a5f0f85b444a3e58e2c5b46f6addc72a67e87ae918`  
		Last Modified: Thu, 16 Mar 2023 03:46:40 GMT  
		Size: 171.5 MB (171493131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111abfb9fbc2b0549a5f36a5dfe15229955477056115fe93d5630e6dcbf67970`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2d073551834d896f537facf3e35341eb2ab136a5aaf7fb5c935c3bb5c7126e`  
		Last Modified: Thu, 16 Mar 2023 03:46:55 GMT  
		Size: 45.2 MB (45203778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518a989d6dba523fd6a7f2604b03c29146262b03f347c30dfd5e306f8de1c10c`  
		Last Modified: Thu, 16 Mar 2023 03:46:50 GMT  
		Size: 317.4 KB (317350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17de9a769b38ea53a05082bc632c3a08673f269fff61bb683575c1ef260f8862`  
		Last Modified: Thu, 16 Mar 2023 03:47:00 GMT  
		Size: 72.0 MB (71974610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:86fd17b31e5877912a8feed0c2b23ea683ba437166b52f1b18924b18a63ec7ac
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
$ docker pull ros@sha256:5971dc7ec3ad49d24166c6819403649dbae3e8e84b59c386476c592a07d91f56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.4 MB (403370139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b600a194613fa00e767aab1f7badf050f32e978c0718e9d8a5aa982930c429e8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:17:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:17:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 Apr 2023 03:17:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 Apr 2023 03:17:50 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 03:17:50 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 Apr 2023 03:17:50 GMT
ENV ROS_DISTRO=noetic
# Wed, 12 Apr 2023 03:19:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:19:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 12 Apr 2023 03:19:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 Apr 2023 03:19:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:19:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 12 Apr 2023 03:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926daaa3f39d210833d9a3a75b2e33aafd38f4adcda623bb40686f5480d8eda7`  
		Last Modified: Wed, 12 Apr 2023 03:25:46 GMT  
		Size: 10.9 MB (10902667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ef889428a3c0c2686a4bb8d4e5af08778a1b25251d4873a4635b0b2af721d8`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b211d556fba373cffc4c30d24942793ca6d51c78179037897e5f465fc65e4408`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161bac3145a70b13a85c49796d22151dc27a76ea04b256183b318cc9efc8686d`  
		Last Modified: Wed, 12 Apr 2023 03:26:06 GMT  
		Size: 184.4 MB (184427087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91b09fc5f446950a1e8e392c05737de9820b95e50745e93232b6ff4dba0617`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d31bfc2a7fad06ba1563ddcf7f96daf937621936041ba76fb2e42b45d9f327`  
		Last Modified: Wed, 12 Apr 2023 03:26:21 GMT  
		Size: 84.4 MB (84395801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ec420fccc4bc3cf3805910ff22f8789cd48387fcefed5829785ab9279e8e9f`  
		Last Modified: Wed, 12 Apr 2023 03:26:13 GMT  
		Size: 313.0 KB (312977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e8033e5e52d2e2310af7d82b5846e3f1900897dee49ceb23bf0721dac3353e`  
		Last Modified: Wed, 12 Apr 2023 03:26:20 GMT  
		Size: 74.1 MB (74090563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:be96e3bf51930fa25d98ca9631a79a11e5262529687ca2afd291d5baca5e4845
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:f8f42074222bd00a9b089d9f34036abf91b68a35c03e423398a3e64d59dfe62f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343164665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b56a2c6b724820ee06e125c51e8e704a6b4ba61bbfebcf16af198e602cb642f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 04:09:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:09:06 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:04 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:11:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:11:04 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 04:11:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 04:13:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adae176e5cd2a30cf1122ee112b4b721b01ea9b4c0ac5e541d66c07aaaec48`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adccda1b6439c0a801a24fa60738b89782e4c7193200f6f27ce29713715eb56`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82508576a99a0a8d8797589d2c709fa671510864b5270428799fc45a75007041`  
		Last Modified: Thu, 16 Mar 2023 04:43:53 GMT  
		Size: 177.0 MB (177011633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581df5fa2a83d010d48e7b47f737a951bda847f9ee5c724e9ccc3856cf28ee08`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32822115c02183cc93979e5eb6530d84df2e5871996db9b7dc7c65443966bf1`  
		Last Modified: Thu, 16 Mar 2023 04:44:11 GMT  
		Size: 50.9 MB (50940109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d2b3f91c40b14acd615fbc7eb23e2ae46a9e339e795fc221fdc21561270f58`  
		Last Modified: Thu, 16 Mar 2023 04:44:03 GMT  
		Size: 317.4 KB (317353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304ec1393d4ab6577989c766d2b4172d18d06a2d05bc1685889432e70a066f40`  
		Last Modified: Thu, 16 Mar 2023 04:44:15 GMT  
		Size: 79.6 MB (79606953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:f69b4e9d767e0f5ea05e053e59c7683f87cea0d6d42ee8fa0abd2cd6cc674eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289247972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60b6d51cdc636dd5e3e07574122c2df344fdf9002803cca05876ffc5e08153b2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:25:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:27:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:27:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:27:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:27:55 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:28:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:28:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:29:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07a04d14911f425c252acad00ad16f68336179fdb2bd057ecbc008654d4a9dc`  
		Last Modified: Thu, 16 Mar 2023 03:41:09 GMT  
		Size: 1.2 MB (1154620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3bf1f4e2e473ac685bd824bf2830576a48ab98791369a09fea2d0dbd4a929f`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 4.7 MB (4679050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6ed9de687ca448ae7407bb48c22de4deda7d30a973cef11a4b6d8d8fb38e7`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa126a480cce3f126ceba011ffee67346db673365bb738950073ba2ba74783`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0c85b3c21b15d3eb1f9e6b0b89b695ba25d60a4591c501019a1276bc0fd1e5`  
		Last Modified: Thu, 16 Mar 2023 03:41:35 GMT  
		Size: 157.5 MB (157508946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015ee579e11221f21424f6a032081a7ccc05e90c3115b747cd39125644bd52f`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502398c5b962c956411f0c9bb61dc5d8cb53a75a822beab1a67338a6040844da`  
		Last Modified: Thu, 16 Mar 2023 03:41:51 GMT  
		Size: 40.5 MB (40502661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4016c5932fe61d99fdb58e6cc4986e20a201b4c0ebac799059f2dd4d5f430ab`  
		Last Modified: Thu, 16 Mar 2023 03:41:46 GMT  
		Size: 317.3 KB (317345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5a37a447e1f58827e4f91f66e94e8e7a186d73e26aed5bd96060931f145801`  
		Last Modified: Thu, 16 Mar 2023 03:41:55 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b576d3034caf213b58905fae455fcdcde299046f2f53f1801f032c876e25e6ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322875712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdc6ebcdb919385e49b76876c7c7b36a8b277493a63efdaa1e0f53241e0478ed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:10:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:12:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:12:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:12:47 GMT
CMD ["bash"]
# Thu, 16 Mar 2023 03:13:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:13:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 16 Mar 2023 03:14:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b33d380951389d9d1ce91514fb73e120ca3b974c248cd2f314992c3465b2b9`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfba233f21202f1db01a89b8102baef60e3122f36c4d66830892d50d49066`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e709008824e0a6b98c808a5f0f85b444a3e58e2c5b46f6addc72a67e87ae918`  
		Last Modified: Thu, 16 Mar 2023 03:46:40 GMT  
		Size: 171.5 MB (171493131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111abfb9fbc2b0549a5f36a5dfe15229955477056115fe93d5630e6dcbf67970`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2d073551834d896f537facf3e35341eb2ab136a5aaf7fb5c935c3bb5c7126e`  
		Last Modified: Thu, 16 Mar 2023 03:46:55 GMT  
		Size: 45.2 MB (45203778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518a989d6dba523fd6a7f2604b03c29146262b03f347c30dfd5e306f8de1c10c`  
		Last Modified: Thu, 16 Mar 2023 03:46:50 GMT  
		Size: 317.4 KB (317350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17de9a769b38ea53a05082bc632c3a08673f269fff61bb683575c1ef260f8862`  
		Last Modified: Thu, 16 Mar 2023 03:47:00 GMT  
		Size: 72.0 MB (71974610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:2a5404b7382088de5b76db33fe39cd35ecb7faf0815a7d1954fe63314d024b19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:a2bc1b65017a727bae0393c732ade294c60af4c0317c59f5e55d8fc164f180bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212300250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be68a0a2e35d7c67cccf17c6d75daf95a697a41debcdbe2b9bab7a084f21554a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 04:09:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:09:06 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:04 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:11:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:11:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adae176e5cd2a30cf1122ee112b4b721b01ea9b4c0ac5e541d66c07aaaec48`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adccda1b6439c0a801a24fa60738b89782e4c7193200f6f27ce29713715eb56`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82508576a99a0a8d8797589d2c709fa671510864b5270428799fc45a75007041`  
		Last Modified: Thu, 16 Mar 2023 04:43:53 GMT  
		Size: 177.0 MB (177011633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581df5fa2a83d010d48e7b47f737a951bda847f9ee5c724e9ccc3856cf28ee08`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:de3a9feacb51fc23cb5c31152c841cee1ba76c89329ac7f0c38b2e1768935c52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187931509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d272f3442d026f83833162e102a149050896dd37425a909f47a20d1207e48b6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:25:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:27:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:27:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:27:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:27:55 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07a04d14911f425c252acad00ad16f68336179fdb2bd057ecbc008654d4a9dc`  
		Last Modified: Thu, 16 Mar 2023 03:41:09 GMT  
		Size: 1.2 MB (1154620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3bf1f4e2e473ac685bd824bf2830576a48ab98791369a09fea2d0dbd4a929f`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 4.7 MB (4679050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6ed9de687ca448ae7407bb48c22de4deda7d30a973cef11a4b6d8d8fb38e7`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa126a480cce3f126ceba011ffee67346db673365bb738950073ba2ba74783`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0c85b3c21b15d3eb1f9e6b0b89b695ba25d60a4591c501019a1276bc0fd1e5`  
		Last Modified: Thu, 16 Mar 2023 03:41:35 GMT  
		Size: 157.5 MB (157508946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015ee579e11221f21424f6a032081a7ccc05e90c3115b747cd39125644bd52f`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:18cece770dbe8f635d2fa57d1f2f0e06a111dca641b05c37836dc6346890a2fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205379974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a79359d8f99cb131954b57206275ca705ada90ee88fcb8a0cb10b92f690db3bd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:10:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:12:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:12:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:12:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b33d380951389d9d1ce91514fb73e120ca3b974c248cd2f314992c3465b2b9`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfba233f21202f1db01a89b8102baef60e3122f36c4d66830892d50d49066`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e709008824e0a6b98c808a5f0f85b444a3e58e2c5b46f6addc72a67e87ae918`  
		Last Modified: Thu, 16 Mar 2023 03:46:40 GMT  
		Size: 171.5 MB (171493131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111abfb9fbc2b0549a5f36a5dfe15229955477056115fe93d5630e6dcbf67970`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:9aa31c313ff1713e0d88733a5f5d6f974360fecef9cc32898222af0a314647f9
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
$ docker pull ros@sha256:8598f8c64fe4997db9f88cd69309e62c5812f821aeabcce7081eccb943c0d984
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244570798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd04de286c4aa41a9b35ac5ed6f0f7dfcaec97e29a5d158ccb5dea5c690d9f5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:17:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:17:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 12 Apr 2023 03:17:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 12 Apr 2023 03:17:50 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 03:17:50 GMT
ENV LC_ALL=C.UTF-8
# Wed, 12 Apr 2023 03:17:50 GMT
ENV ROS_DISTRO=noetic
# Wed, 12 Apr 2023 03:19:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:19:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 12 Apr 2023 03:19:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 12 Apr 2023 03:19:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926daaa3f39d210833d9a3a75b2e33aafd38f4adcda623bb40686f5480d8eda7`  
		Last Modified: Wed, 12 Apr 2023 03:25:46 GMT  
		Size: 10.9 MB (10902667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ef889428a3c0c2686a4bb8d4e5af08778a1b25251d4873a4635b0b2af721d8`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b211d556fba373cffc4c30d24942793ca6d51c78179037897e5f465fc65e4408`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161bac3145a70b13a85c49796d22151dc27a76ea04b256183b318cc9efc8686d`  
		Last Modified: Wed, 12 Apr 2023 03:26:06 GMT  
		Size: 184.4 MB (184427087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91b09fc5f446950a1e8e392c05737de9820b95e50745e93232b6ff4dba0617`  
		Last Modified: Wed, 12 Apr 2023 03:25:45 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:2a5404b7382088de5b76db33fe39cd35ecb7faf0815a7d1954fe63314d024b19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:a2bc1b65017a727bae0393c732ade294c60af4c0317c59f5e55d8fc164f180bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212300250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be68a0a2e35d7c67cccf17c6d75daf95a697a41debcdbe2b9bab7a084f21554a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:03:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:09:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 04:09:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:09:05 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:09:06 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 04:11:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:11:04 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 04:11:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 04:11:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a3bf9c2e8661d0de58d4a85390b5a17d80f3abf64250efc0769650aa9ab69`  
		Last Modified: Thu, 16 Mar 2023 03:13:05 GMT  
		Size: 1.2 MB (1154522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd341efe0542b6414a62580c02a19287b22de0f35bfdd76fb24d84ae342511e`  
		Last Modified: Thu, 16 Mar 2023 04:43:26 GMT  
		Size: 5.6 MB (5553614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adae176e5cd2a30cf1122ee112b4b721b01ea9b4c0ac5e541d66c07aaaec48`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adccda1b6439c0a801a24fa60738b89782e4c7193200f6f27ce29713715eb56`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82508576a99a0a8d8797589d2c709fa671510864b5270428799fc45a75007041`  
		Last Modified: Thu, 16 Mar 2023 04:43:53 GMT  
		Size: 177.0 MB (177011633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581df5fa2a83d010d48e7b47f737a951bda847f9ee5c724e9ccc3856cf28ee08`  
		Last Modified: Thu, 16 Mar 2023 04:43:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:de3a9feacb51fc23cb5c31152c841cee1ba76c89329ac7f0c38b2e1768935c52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187931509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d272f3442d026f83833162e102a149050896dd37425a909f47a20d1207e48b6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:25:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:25:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:25:25 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:27:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:27:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:27:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:27:55 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07a04d14911f425c252acad00ad16f68336179fdb2bd057ecbc008654d4a9dc`  
		Last Modified: Thu, 16 Mar 2023 03:41:09 GMT  
		Size: 1.2 MB (1154620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3bf1f4e2e473ac685bd824bf2830576a48ab98791369a09fea2d0dbd4a929f`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 4.7 MB (4679050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6ed9de687ca448ae7407bb48c22de4deda7d30a973cef11a4b6d8d8fb38e7`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa126a480cce3f126ceba011ffee67346db673365bb738950073ba2ba74783`  
		Last Modified: Thu, 16 Mar 2023 03:41:07 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0c85b3c21b15d3eb1f9e6b0b89b695ba25d60a4591c501019a1276bc0fd1e5`  
		Last Modified: Thu, 16 Mar 2023 03:41:35 GMT  
		Size: 157.5 MB (157508946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015ee579e11221f21424f6a032081a7ccc05e90c3115b747cd39125644bd52f`  
		Last Modified: Thu, 16 Mar 2023 03:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:18cece770dbe8f635d2fa57d1f2f0e06a111dca641b05c37836dc6346890a2fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205379974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a79359d8f99cb131954b57206275ca705ada90ee88fcb8a0cb10b92f690db3bd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:10:11 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:10:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Mar 2023 03:10:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:10:22 GMT
ENV ROS_DISTRO=noetic
# Thu, 16 Mar 2023 03:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:12:47 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 16 Mar 2023 03:12:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Mar 2023 03:12:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c235c7a3c272479c47e3fdeef457877dd1bce12f4b4d8726aeb2b8e16d6acae4`  
		Last Modified: Thu, 16 Mar 2023 03:46:17 GMT  
		Size: 1.2 MB (1155462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25e62e51f71a010b6fdbdb16725b3bbfca6a13fca1e447d14e311d361db90f4`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 5.5 MB (5532807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b33d380951389d9d1ce91514fb73e120ca3b974c248cd2f314992c3465b2b9`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbfba233f21202f1db01a89b8102baef60e3122f36c4d66830892d50d49066`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e709008824e0a6b98c808a5f0f85b444a3e58e2c5b46f6addc72a67e87ae918`  
		Last Modified: Thu, 16 Mar 2023 03:46:40 GMT  
		Size: 171.5 MB (171493131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111abfb9fbc2b0549a5f36a5dfe15229955477056115fe93d5630e6dcbf67970`  
		Last Modified: Thu, 16 Mar 2023 03:46:15 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:215907da7f798e0e25fa3c4eadcd9e158eaa6bc6cef5e2e7e626562d8f67cd92
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
$ docker pull ros@sha256:03f73d299c4be78dcfe6ecb9a5f6cec36523c0b3621536196ee5e7597c9e154b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.0 MB (257005959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef467d9d43bbd390e65275d1c456ae20f51090c6abcde07eb03038db29a3f87`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:40:17 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:40:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:40:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:40:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:40:13 GMT
CMD ["bash"]
# Mon, 03 Apr 2023 23:40:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:41:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Apr 2023 23:41:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 03 Apr 2023 23:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81833bae8ba355ae6dab1ea01f0e77406295e21b17bbf496f3afcce7d6fad6f`  
		Last Modified: Mon, 03 Apr 2023 23:52:30 GMT  
		Size: 117.8 MB (117802804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f369ce2b8fdf47bc39a0b484bfd1353585a88e69ecaf4713bb0fdbd6477cd`  
		Last Modified: Mon, 03 Apr 2023 23:52:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e0cc2cdd9a83ed310ebdb6931dc2763a2988d2a1d34595b50c69bc1f400128`  
		Last Modified: Mon, 03 Apr 2023 23:52:46 GMT  
		Size: 82.6 MB (82628406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38758a0b6fd8b76288bf9545f0665f0e59eb59697fe3fbeff6e2b0666eabca31`  
		Last Modified: Mon, 03 Apr 2023 23:52:38 GMT  
		Size: 303.1 KB (303111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d81de00e57d0cd82fd74156e9b901ad3cb14fb7cd155aabbea09a951bc4d656`  
		Last Modified: Mon, 03 Apr 2023 23:52:38 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa623520a51349a085ce270b71a74a663b5e159f33942622ebd5a081b14a7fd`  
		Last Modified: Mon, 03 Apr 2023 23:52:40 GMT  
		Size: 22.9 MB (22909135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:6f7773d21944af5fea1c2b9cbb2c36c940bb6dd40aa1b3d53c8aac487a5a0059
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
$ docker pull ros@sha256:aebbe51e55547facd1fc7b725328b32c2bb559ee7c79d8642ac275d06205a46c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1045364911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3378198c698fd2095a7c5c0d1a47efbdb49f263dbaaf8e240199a73c81846b42`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:40:17 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:40:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:40:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:40:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:40:13 GMT
CMD ["bash"]
# Mon, 03 Apr 2023 23:40:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:41:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Apr 2023 23:41:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 03 Apr 2023 23:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:51:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81833bae8ba355ae6dab1ea01f0e77406295e21b17bbf496f3afcce7d6fad6f`  
		Last Modified: Mon, 03 Apr 2023 23:52:30 GMT  
		Size: 117.8 MB (117802804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f369ce2b8fdf47bc39a0b484bfd1353585a88e69ecaf4713bb0fdbd6477cd`  
		Last Modified: Mon, 03 Apr 2023 23:52:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e0cc2cdd9a83ed310ebdb6931dc2763a2988d2a1d34595b50c69bc1f400128`  
		Last Modified: Mon, 03 Apr 2023 23:52:46 GMT  
		Size: 82.6 MB (82628406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38758a0b6fd8b76288bf9545f0665f0e59eb59697fe3fbeff6e2b0666eabca31`  
		Last Modified: Mon, 03 Apr 2023 23:52:38 GMT  
		Size: 303.1 KB (303111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d81de00e57d0cd82fd74156e9b901ad3cb14fb7cd155aabbea09a951bc4d656`  
		Last Modified: Mon, 03 Apr 2023 23:52:38 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa623520a51349a085ce270b71a74a663b5e159f33942622ebd5a081b14a7fd`  
		Last Modified: Mon, 03 Apr 2023 23:52:40 GMT  
		Size: 22.9 MB (22909135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd07bb80a2b2c9e4f6257f3b970003bdaada1fb0ceba9611ab6e0435915084a0`  
		Last Modified: Mon, 03 Apr 2023 23:54:03 GMT  
		Size: 788.4 MB (788358952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:6f7773d21944af5fea1c2b9cbb2c36c940bb6dd40aa1b3d53c8aac487a5a0059
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
$ docker pull ros@sha256:aebbe51e55547facd1fc7b725328b32c2bb559ee7c79d8642ac275d06205a46c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1045364911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3378198c698fd2095a7c5c0d1a47efbdb49f263dbaaf8e240199a73c81846b42`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:40:17 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:40:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:40:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:40:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:40:13 GMT
CMD ["bash"]
# Mon, 03 Apr 2023 23:40:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:41:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Apr 2023 23:41:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 03 Apr 2023 23:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:51:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81833bae8ba355ae6dab1ea01f0e77406295e21b17bbf496f3afcce7d6fad6f`  
		Last Modified: Mon, 03 Apr 2023 23:52:30 GMT  
		Size: 117.8 MB (117802804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f369ce2b8fdf47bc39a0b484bfd1353585a88e69ecaf4713bb0fdbd6477cd`  
		Last Modified: Mon, 03 Apr 2023 23:52:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e0cc2cdd9a83ed310ebdb6931dc2763a2988d2a1d34595b50c69bc1f400128`  
		Last Modified: Mon, 03 Apr 2023 23:52:46 GMT  
		Size: 82.6 MB (82628406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38758a0b6fd8b76288bf9545f0665f0e59eb59697fe3fbeff6e2b0666eabca31`  
		Last Modified: Mon, 03 Apr 2023 23:52:38 GMT  
		Size: 303.1 KB (303111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d81de00e57d0cd82fd74156e9b901ad3cb14fb7cd155aabbea09a951bc4d656`  
		Last Modified: Mon, 03 Apr 2023 23:52:38 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa623520a51349a085ce270b71a74a663b5e159f33942622ebd5a081b14a7fd`  
		Last Modified: Mon, 03 Apr 2023 23:52:40 GMT  
		Size: 22.9 MB (22909135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd07bb80a2b2c9e4f6257f3b970003bdaada1fb0ceba9611ab6e0435915084a0`  
		Last Modified: Mon, 03 Apr 2023 23:54:03 GMT  
		Size: 788.4 MB (788358952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:215907da7f798e0e25fa3c4eadcd9e158eaa6bc6cef5e2e7e626562d8f67cd92
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
$ docker pull ros@sha256:03f73d299c4be78dcfe6ecb9a5f6cec36523c0b3621536196ee5e7597c9e154b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.0 MB (257005959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef467d9d43bbd390e65275d1c456ae20f51090c6abcde07eb03038db29a3f87`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:40:17 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:40:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:40:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:40:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:40:13 GMT
CMD ["bash"]
# Mon, 03 Apr 2023 23:40:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:41:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Apr 2023 23:41:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 03 Apr 2023 23:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81833bae8ba355ae6dab1ea01f0e77406295e21b17bbf496f3afcce7d6fad6f`  
		Last Modified: Mon, 03 Apr 2023 23:52:30 GMT  
		Size: 117.8 MB (117802804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f369ce2b8fdf47bc39a0b484bfd1353585a88e69ecaf4713bb0fdbd6477cd`  
		Last Modified: Mon, 03 Apr 2023 23:52:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e0cc2cdd9a83ed310ebdb6931dc2763a2988d2a1d34595b50c69bc1f400128`  
		Last Modified: Mon, 03 Apr 2023 23:52:46 GMT  
		Size: 82.6 MB (82628406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38758a0b6fd8b76288bf9545f0665f0e59eb59697fe3fbeff6e2b0666eabca31`  
		Last Modified: Mon, 03 Apr 2023 23:52:38 GMT  
		Size: 303.1 KB (303111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d81de00e57d0cd82fd74156e9b901ad3cb14fb7cd155aabbea09a951bc4d656`  
		Last Modified: Mon, 03 Apr 2023 23:52:38 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa623520a51349a085ce270b71a74a663b5e159f33942622ebd5a081b14a7fd`  
		Last Modified: Mon, 03 Apr 2023 23:52:40 GMT  
		Size: 22.9 MB (22909135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:215907da7f798e0e25fa3c4eadcd9e158eaa6bc6cef5e2e7e626562d8f67cd92
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
$ docker pull ros@sha256:03f73d299c4be78dcfe6ecb9a5f6cec36523c0b3621536196ee5e7597c9e154b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.0 MB (257005959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef467d9d43bbd390e65275d1c456ae20f51090c6abcde07eb03038db29a3f87`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:40:17 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:40:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:40:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:40:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:40:13 GMT
CMD ["bash"]
# Mon, 03 Apr 2023 23:40:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:41:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Apr 2023 23:41:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 03 Apr 2023 23:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81833bae8ba355ae6dab1ea01f0e77406295e21b17bbf496f3afcce7d6fad6f`  
		Last Modified: Mon, 03 Apr 2023 23:52:30 GMT  
		Size: 117.8 MB (117802804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f369ce2b8fdf47bc39a0b484bfd1353585a88e69ecaf4713bb0fdbd6477cd`  
		Last Modified: Mon, 03 Apr 2023 23:52:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e0cc2cdd9a83ed310ebdb6931dc2763a2988d2a1d34595b50c69bc1f400128`  
		Last Modified: Mon, 03 Apr 2023 23:52:46 GMT  
		Size: 82.6 MB (82628406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38758a0b6fd8b76288bf9545f0665f0e59eb59697fe3fbeff6e2b0666eabca31`  
		Last Modified: Mon, 03 Apr 2023 23:52:38 GMT  
		Size: 303.1 KB (303111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d81de00e57d0cd82fd74156e9b901ad3cb14fb7cd155aabbea09a951bc4d656`  
		Last Modified: Mon, 03 Apr 2023 23:52:38 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa623520a51349a085ce270b71a74a663b5e159f33942622ebd5a081b14a7fd`  
		Last Modified: Mon, 03 Apr 2023 23:52:40 GMT  
		Size: 22.9 MB (22909135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:3281de60f58217372a8821d4373d5c7a0648d4cfb270c36c3eec264d027f2aa8
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
$ docker pull ros@sha256:694df8293cd76b62392d84ddd62b5efb851f20d3b8a1f8fc285f97e7543ce54a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151162865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2506b0560036090677ea4e8ccf62443ce2301b69892173c7e941a4c51dabec1d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:40:17 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:40:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:40:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:40:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:40:13 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81833bae8ba355ae6dab1ea01f0e77406295e21b17bbf496f3afcce7d6fad6f`  
		Last Modified: Mon, 03 Apr 2023 23:52:30 GMT  
		Size: 117.8 MB (117802804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f369ce2b8fdf47bc39a0b484bfd1353585a88e69ecaf4713bb0fdbd6477cd`  
		Last Modified: Mon, 03 Apr 2023 23:52:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:3281de60f58217372a8821d4373d5c7a0648d4cfb270c36c3eec264d027f2aa8
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
$ docker pull ros@sha256:694df8293cd76b62392d84ddd62b5efb851f20d3b8a1f8fc285f97e7543ce54a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151162865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2506b0560036090677ea4e8ccf62443ce2301b69892173c7e941a4c51dabec1d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:25:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:26:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 03:26:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 03:26:18 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 03:40:17 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:40:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:40:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:40:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:40:13 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ebc1fa788322832bbed71ceadb3e11cb1a26969d4d664f7655a5b7c81c2b78`  
		Last Modified: Thu, 16 Mar 2023 03:49:34 GMT  
		Size: 1.2 MB (1169852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c0de312547c3fc66abbc624c4b248800ec78c0aab6b4fe6c072f35858664f`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 3.8 MB (3800241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8e2247bed14b878a035c112eb817cbee79740c938c0893cd55b231b58017e`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d086fdc5697b9365d08f5b9dd61a33e2547c5a22618ae5481f9d6041447223`  
		Last Modified: Thu, 16 Mar 2023 03:49:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81833bae8ba355ae6dab1ea01f0e77406295e21b17bbf496f3afcce7d6fad6f`  
		Last Modified: Mon, 03 Apr 2023 23:52:30 GMT  
		Size: 117.8 MB (117802804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f369ce2b8fdf47bc39a0b484bfd1353585a88e69ecaf4713bb0fdbd6477cd`  
		Last Modified: Mon, 03 Apr 2023 23:52:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
