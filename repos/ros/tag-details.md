<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ros`

-	[`ros:humble`](#roshumble)
-	[`ros:humble-perception`](#roshumble-perception)
-	[`ros:humble-perception-jammy`](#roshumble-perception-jammy)
-	[`ros:humble-ros-base`](#roshumble-ros-base)
-	[`ros:humble-ros-base-jammy`](#roshumble-ros-base-jammy)
-	[`ros:humble-ros-core`](#roshumble-ros-core)
-	[`ros:humble-ros-core-jammy`](#roshumble-ros-core-jammy)
-	[`ros:iron`](#rosiron)
-	[`ros:iron-perception`](#rosiron-perception)
-	[`ros:iron-perception-jammy`](#rosiron-perception-jammy)
-	[`ros:iron-ros-base`](#rosiron-ros-base)
-	[`ros:iron-ros-base-jammy`](#rosiron-ros-base-jammy)
-	[`ros:iron-ros-core`](#rosiron-ros-core)
-	[`ros:iron-ros-core-jammy`](#rosiron-ros-core-jammy)
-	[`ros:latest`](#roslatest)
-	[`ros:noetic`](#rosnoetic)
-	[`ros:noetic-perception`](#rosnoetic-perception)
-	[`ros:noetic-perception-focal`](#rosnoetic-perception-focal)
-	[`ros:noetic-robot`](#rosnoetic-robot)
-	[`ros:noetic-robot-focal`](#rosnoetic-robot-focal)
-	[`ros:noetic-ros-base`](#rosnoetic-ros-base)
-	[`ros:noetic-ros-base-focal`](#rosnoetic-ros-base-focal)
-	[`ros:noetic-ros-core`](#rosnoetic-ros-core)
-	[`ros:noetic-ros-core-focal`](#rosnoetic-ros-core-focal)
-	[`ros:rolling`](#rosrolling)
-	[`ros:rolling-perception`](#rosrolling-perception)
-	[`ros:rolling-perception-jammy`](#rosrolling-perception-jammy)
-	[`ros:rolling-ros-base`](#rosrolling-ros-base)
-	[`ros:rolling-ros-base-jammy`](#rosrolling-ros-base-jammy)
-	[`ros:rolling-ros-core`](#rosrolling-ros-core)
-	[`ros:rolling-ros-core-jammy`](#rosrolling-ros-core-jammy)

## `ros:humble`

```console
$ docker pull ros@sha256:74ca8a7e7292d618c51813fbae20abdd0495321bc5e51118a4366d4ede862729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:79355f8f337bde9a35328ba7420e384bce739fd7d7b5b7ade27b59b15c6334c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263166132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8dfee577ee17a0c0e4684c4ec3da6340c072da1c3969377404d15e3526aec12`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 19:50:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:50:04 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 19:50:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:50:04 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:51:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:51:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:51:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 19:52:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd524cf7754594d911fa06358015cf1327cb43355eb465f630a366e97dedef5b`  
		Last Modified: Tue, 04 Jul 2023 20:09:34 GMT  
		Size: 106.3 MB (106344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a0ac1a73dab9eca6d1d3cb5656032709291067b9f54a573c4a4730296d262b`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b3c2bf65a5f88854a4e9b3c40f16e67b119af543d6656867ff27174e1d8f45`  
		Last Modified: Tue, 04 Jul 2023 20:09:55 GMT  
		Size: 97.9 MB (97949653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fd7ea32c23c962d34cd70e32ac496fa75bc603430e4b70172a78380d217e5d`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 307.1 KB (307140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773f4fc51f45ba73bbf97b10b39b54b7e6b43063a0e37c48e847b48a62a4bf11`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dbf8cf19eabafc2081cdee9cc9873550fd53aac2bcdc52b1cccca47f3b7976`  
		Last Modified: Tue, 04 Jul 2023 20:09:46 GMT  
		Size: 23.1 MB (23086815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:51a3bacfaad84aee1b80cf73cb3588c4b535a8b35f1a75b8c6adb315039d85d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255898065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7d9e9fcdbbe0cebc229f6d9a9afa9d00b892ee62043ffcb18c240767923d81`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 14:41:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:41:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:41:06 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:41:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:41:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc99b708e63ea51d08155711080144b68401240806daf3d55ff31da8ce2e6e8`  
		Last Modified: Tue, 04 Jul 2023 15:02:14 GMT  
		Size: 104.1 MB (104091352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587e83797ba402344f156014188711bc267dad06b4fc07b9b76d84206961887`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4681cb50e4211cf1a6641009dd51e6330ee41ec7d56c69974b08bcad3e1eb97`  
		Last Modified: Tue, 04 Jul 2023 15:02:33 GMT  
		Size: 95.6 MB (95583335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64814832cf8516f200bd7dd874fa74752b972925ab9c3589cff205384d75de09`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 307.1 KB (307139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22ee3968485d390f331fe27b0544cdaa0341b0cf480ee4322c0dc756fe3160c`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 2.4 KB (2443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e450a263466aac0036b7b14cb06363d88c97575eb95b4d03e7cd1541305e43b6`  
		Last Modified: Tue, 04 Jul 2023 15:02:26 GMT  
		Size: 22.5 MB (22503697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:d73fcb8076b033239336e5f6e588f98dce2efbd652c85a2019c19d27411a8db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:82b41e780969c23f7d043aea43000a216f695037655a536543e40d0a1bc1f66f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **952.3 MB (952262558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58b69c3990c4c87abf41ddfb4115ee8099badca3699553369402ff1f1bc393fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 19:50:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:50:04 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 19:50:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:50:04 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:51:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:51:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:51:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 19:52:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:59:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd524cf7754594d911fa06358015cf1327cb43355eb465f630a366e97dedef5b`  
		Last Modified: Tue, 04 Jul 2023 20:09:34 GMT  
		Size: 106.3 MB (106344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a0ac1a73dab9eca6d1d3cb5656032709291067b9f54a573c4a4730296d262b`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b3c2bf65a5f88854a4e9b3c40f16e67b119af543d6656867ff27174e1d8f45`  
		Last Modified: Tue, 04 Jul 2023 20:09:55 GMT  
		Size: 97.9 MB (97949653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fd7ea32c23c962d34cd70e32ac496fa75bc603430e4b70172a78380d217e5d`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 307.1 KB (307140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773f4fc51f45ba73bbf97b10b39b54b7e6b43063a0e37c48e847b48a62a4bf11`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dbf8cf19eabafc2081cdee9cc9873550fd53aac2bcdc52b1cccca47f3b7976`  
		Last Modified: Tue, 04 Jul 2023 20:09:46 GMT  
		Size: 23.1 MB (23086815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a00e162c60da079b7e4481316e9401c7b4cf0675e2d028c8942809b3a61865c`  
		Last Modified: Tue, 04 Jul 2023 20:11:34 GMT  
		Size: 689.1 MB (689096426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4d8fb695550857c8570e04c0a51fcbda56719acb15180bb5f97cc33133fd1de4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **913.7 MB (913735876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0f1a5675115b29c71228e209141c46fd87b090a0b583f56e41b00f2c648e9b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 14:41:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:41:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:41:06 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:41:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:41:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:52:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc99b708e63ea51d08155711080144b68401240806daf3d55ff31da8ce2e6e8`  
		Last Modified: Tue, 04 Jul 2023 15:02:14 GMT  
		Size: 104.1 MB (104091352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587e83797ba402344f156014188711bc267dad06b4fc07b9b76d84206961887`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4681cb50e4211cf1a6641009dd51e6330ee41ec7d56c69974b08bcad3e1eb97`  
		Last Modified: Tue, 04 Jul 2023 15:02:33 GMT  
		Size: 95.6 MB (95583335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64814832cf8516f200bd7dd874fa74752b972925ab9c3589cff205384d75de09`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 307.1 KB (307139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22ee3968485d390f331fe27b0544cdaa0341b0cf480ee4322c0dc756fe3160c`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 2.4 KB (2443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e450a263466aac0036b7b14cb06363d88c97575eb95b4d03e7cd1541305e43b6`  
		Last Modified: Tue, 04 Jul 2023 15:02:26 GMT  
		Size: 22.5 MB (22503697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89358fb3d71856b83b2a7b91f147e47a9bd2f8d75266587d9a3063d4df9cc987`  
		Last Modified: Tue, 04 Jul 2023 15:04:07 GMT  
		Size: 657.8 MB (657837811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:d73fcb8076b033239336e5f6e588f98dce2efbd652c85a2019c19d27411a8db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:82b41e780969c23f7d043aea43000a216f695037655a536543e40d0a1bc1f66f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **952.3 MB (952262558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58b69c3990c4c87abf41ddfb4115ee8099badca3699553369402ff1f1bc393fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 19:50:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:50:04 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 19:50:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:50:04 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:51:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:51:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:51:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 19:52:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:59:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd524cf7754594d911fa06358015cf1327cb43355eb465f630a366e97dedef5b`  
		Last Modified: Tue, 04 Jul 2023 20:09:34 GMT  
		Size: 106.3 MB (106344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a0ac1a73dab9eca6d1d3cb5656032709291067b9f54a573c4a4730296d262b`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b3c2bf65a5f88854a4e9b3c40f16e67b119af543d6656867ff27174e1d8f45`  
		Last Modified: Tue, 04 Jul 2023 20:09:55 GMT  
		Size: 97.9 MB (97949653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fd7ea32c23c962d34cd70e32ac496fa75bc603430e4b70172a78380d217e5d`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 307.1 KB (307140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773f4fc51f45ba73bbf97b10b39b54b7e6b43063a0e37c48e847b48a62a4bf11`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dbf8cf19eabafc2081cdee9cc9873550fd53aac2bcdc52b1cccca47f3b7976`  
		Last Modified: Tue, 04 Jul 2023 20:09:46 GMT  
		Size: 23.1 MB (23086815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a00e162c60da079b7e4481316e9401c7b4cf0675e2d028c8942809b3a61865c`  
		Last Modified: Tue, 04 Jul 2023 20:11:34 GMT  
		Size: 689.1 MB (689096426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4d8fb695550857c8570e04c0a51fcbda56719acb15180bb5f97cc33133fd1de4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **913.7 MB (913735876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0f1a5675115b29c71228e209141c46fd87b090a0b583f56e41b00f2c648e9b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 14:41:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:41:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:41:06 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:41:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:41:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:52:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc99b708e63ea51d08155711080144b68401240806daf3d55ff31da8ce2e6e8`  
		Last Modified: Tue, 04 Jul 2023 15:02:14 GMT  
		Size: 104.1 MB (104091352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587e83797ba402344f156014188711bc267dad06b4fc07b9b76d84206961887`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4681cb50e4211cf1a6641009dd51e6330ee41ec7d56c69974b08bcad3e1eb97`  
		Last Modified: Tue, 04 Jul 2023 15:02:33 GMT  
		Size: 95.6 MB (95583335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64814832cf8516f200bd7dd874fa74752b972925ab9c3589cff205384d75de09`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 307.1 KB (307139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22ee3968485d390f331fe27b0544cdaa0341b0cf480ee4322c0dc756fe3160c`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 2.4 KB (2443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e450a263466aac0036b7b14cb06363d88c97575eb95b4d03e7cd1541305e43b6`  
		Last Modified: Tue, 04 Jul 2023 15:02:26 GMT  
		Size: 22.5 MB (22503697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89358fb3d71856b83b2a7b91f147e47a9bd2f8d75266587d9a3063d4df9cc987`  
		Last Modified: Tue, 04 Jul 2023 15:04:07 GMT  
		Size: 657.8 MB (657837811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:74ca8a7e7292d618c51813fbae20abdd0495321bc5e51118a4366d4ede862729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:79355f8f337bde9a35328ba7420e384bce739fd7d7b5b7ade27b59b15c6334c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263166132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8dfee577ee17a0c0e4684c4ec3da6340c072da1c3969377404d15e3526aec12`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 19:50:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:50:04 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 19:50:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:50:04 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:51:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:51:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:51:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 19:52:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd524cf7754594d911fa06358015cf1327cb43355eb465f630a366e97dedef5b`  
		Last Modified: Tue, 04 Jul 2023 20:09:34 GMT  
		Size: 106.3 MB (106344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a0ac1a73dab9eca6d1d3cb5656032709291067b9f54a573c4a4730296d262b`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b3c2bf65a5f88854a4e9b3c40f16e67b119af543d6656867ff27174e1d8f45`  
		Last Modified: Tue, 04 Jul 2023 20:09:55 GMT  
		Size: 97.9 MB (97949653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fd7ea32c23c962d34cd70e32ac496fa75bc603430e4b70172a78380d217e5d`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 307.1 KB (307140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773f4fc51f45ba73bbf97b10b39b54b7e6b43063a0e37c48e847b48a62a4bf11`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dbf8cf19eabafc2081cdee9cc9873550fd53aac2bcdc52b1cccca47f3b7976`  
		Last Modified: Tue, 04 Jul 2023 20:09:46 GMT  
		Size: 23.1 MB (23086815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:51a3bacfaad84aee1b80cf73cb3588c4b535a8b35f1a75b8c6adb315039d85d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255898065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7d9e9fcdbbe0cebc229f6d9a9afa9d00b892ee62043ffcb18c240767923d81`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 14:41:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:41:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:41:06 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:41:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:41:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc99b708e63ea51d08155711080144b68401240806daf3d55ff31da8ce2e6e8`  
		Last Modified: Tue, 04 Jul 2023 15:02:14 GMT  
		Size: 104.1 MB (104091352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587e83797ba402344f156014188711bc267dad06b4fc07b9b76d84206961887`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4681cb50e4211cf1a6641009dd51e6330ee41ec7d56c69974b08bcad3e1eb97`  
		Last Modified: Tue, 04 Jul 2023 15:02:33 GMT  
		Size: 95.6 MB (95583335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64814832cf8516f200bd7dd874fa74752b972925ab9c3589cff205384d75de09`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 307.1 KB (307139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22ee3968485d390f331fe27b0544cdaa0341b0cf480ee4322c0dc756fe3160c`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 2.4 KB (2443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e450a263466aac0036b7b14cb06363d88c97575eb95b4d03e7cd1541305e43b6`  
		Last Modified: Tue, 04 Jul 2023 15:02:26 GMT  
		Size: 22.5 MB (22503697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:74ca8a7e7292d618c51813fbae20abdd0495321bc5e51118a4366d4ede862729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:79355f8f337bde9a35328ba7420e384bce739fd7d7b5b7ade27b59b15c6334c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263166132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8dfee577ee17a0c0e4684c4ec3da6340c072da1c3969377404d15e3526aec12`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 19:50:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:50:04 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 19:50:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:50:04 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:51:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:51:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:51:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 19:52:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd524cf7754594d911fa06358015cf1327cb43355eb465f630a366e97dedef5b`  
		Last Modified: Tue, 04 Jul 2023 20:09:34 GMT  
		Size: 106.3 MB (106344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a0ac1a73dab9eca6d1d3cb5656032709291067b9f54a573c4a4730296d262b`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b3c2bf65a5f88854a4e9b3c40f16e67b119af543d6656867ff27174e1d8f45`  
		Last Modified: Tue, 04 Jul 2023 20:09:55 GMT  
		Size: 97.9 MB (97949653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fd7ea32c23c962d34cd70e32ac496fa75bc603430e4b70172a78380d217e5d`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 307.1 KB (307140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773f4fc51f45ba73bbf97b10b39b54b7e6b43063a0e37c48e847b48a62a4bf11`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dbf8cf19eabafc2081cdee9cc9873550fd53aac2bcdc52b1cccca47f3b7976`  
		Last Modified: Tue, 04 Jul 2023 20:09:46 GMT  
		Size: 23.1 MB (23086815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:51a3bacfaad84aee1b80cf73cb3588c4b535a8b35f1a75b8c6adb315039d85d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255898065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7d9e9fcdbbe0cebc229f6d9a9afa9d00b892ee62043ffcb18c240767923d81`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 14:41:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:41:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:41:06 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:41:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:41:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc99b708e63ea51d08155711080144b68401240806daf3d55ff31da8ce2e6e8`  
		Last Modified: Tue, 04 Jul 2023 15:02:14 GMT  
		Size: 104.1 MB (104091352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587e83797ba402344f156014188711bc267dad06b4fc07b9b76d84206961887`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4681cb50e4211cf1a6641009dd51e6330ee41ec7d56c69974b08bcad3e1eb97`  
		Last Modified: Tue, 04 Jul 2023 15:02:33 GMT  
		Size: 95.6 MB (95583335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64814832cf8516f200bd7dd874fa74752b972925ab9c3589cff205384d75de09`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 307.1 KB (307139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22ee3968485d390f331fe27b0544cdaa0341b0cf480ee4322c0dc756fe3160c`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 2.4 KB (2443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e450a263466aac0036b7b14cb06363d88c97575eb95b4d03e7cd1541305e43b6`  
		Last Modified: Tue, 04 Jul 2023 15:02:26 GMT  
		Size: 22.5 MB (22503697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:b744cb791c6dc3700a293f0065a55bc26a7662713648e9b609e96f88c4486eac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:00c01c2ee59af1b7cd0667332f1cc7c8ba5c9dda46a2812412544d086b51f1e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141820076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf8329c1fd5ff5cd43d44cfaa0fe95aa812fe452d280fdec75b035ffb8c7ba5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 19:50:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:50:04 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 19:50:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:50:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd524cf7754594d911fa06358015cf1327cb43355eb465f630a366e97dedef5b`  
		Last Modified: Tue, 04 Jul 2023 20:09:34 GMT  
		Size: 106.3 MB (106344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a0ac1a73dab9eca6d1d3cb5656032709291067b9f54a573c4a4730296d262b`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:268f0f924e3f57a839868e589d0872539266d91048c7eed6f6f17592bf768bb3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137501451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf4c9a915dd9277d29c5bb2fddd8d79eb15e3a6d9a7befef47f3ce5219f4e24`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 14:41:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:41:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:41:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc99b708e63ea51d08155711080144b68401240806daf3d55ff31da8ce2e6e8`  
		Last Modified: Tue, 04 Jul 2023 15:02:14 GMT  
		Size: 104.1 MB (104091352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587e83797ba402344f156014188711bc267dad06b4fc07b9b76d84206961887`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:b744cb791c6dc3700a293f0065a55bc26a7662713648e9b609e96f88c4486eac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:00c01c2ee59af1b7cd0667332f1cc7c8ba5c9dda46a2812412544d086b51f1e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141820076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf8329c1fd5ff5cd43d44cfaa0fe95aa812fe452d280fdec75b035ffb8c7ba5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 19:50:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:50:04 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 19:50:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:50:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd524cf7754594d911fa06358015cf1327cb43355eb465f630a366e97dedef5b`  
		Last Modified: Tue, 04 Jul 2023 20:09:34 GMT  
		Size: 106.3 MB (106344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a0ac1a73dab9eca6d1d3cb5656032709291067b9f54a573c4a4730296d262b`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:268f0f924e3f57a839868e589d0872539266d91048c7eed6f6f17592bf768bb3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137501451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf4c9a915dd9277d29c5bb2fddd8d79eb15e3a6d9a7befef47f3ce5219f4e24`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 14:41:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:41:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:41:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc99b708e63ea51d08155711080144b68401240806daf3d55ff31da8ce2e6e8`  
		Last Modified: Tue, 04 Jul 2023 15:02:14 GMT  
		Size: 104.1 MB (104091352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587e83797ba402344f156014188711bc267dad06b4fc07b9b76d84206961887`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron`

```console
$ docker pull ros@sha256:6a007e64bcd1b093c6ccd4f4cb66b75b1ed1471b60a53c70b7e45de35ebf9184
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron` - linux; amd64

```console
$ docker pull ros@sha256:c0d01ca752cc23ddddb389409680c54fb6c85949c79bc4a3bcdd2a266414a313
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.5 MB (268546213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4bee036752b69abd2271fb9ab494ff987a3923d00c355fc8651896a7dc9b00`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:59:50 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 20:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:00:34 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 20:00:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 20:01:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 20:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c215437d76e0aa23ad3ad77eacdff757fb515043d5fbc4aaab262edecf0f570`  
		Last Modified: Tue, 04 Jul 2023 20:12:05 GMT  
		Size: 124.1 MB (124106862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b7644717ba2f3371d754f83f5d74a18227dd0efa3552b47025bd2bb2e7e92`  
		Last Modified: Tue, 04 Jul 2023 20:11:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199be721033556b61121fd3dc17b7e99b7a7f82492d2272ba5b86f84a9ce7fc2`  
		Last Modified: Tue, 04 Jul 2023 20:12:24 GMT  
		Size: 85.0 MB (84994600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ff985aa05405f2f8956ec07b70eae3f30be79fec5c6d3c1617677f4c3696ac`  
		Last Modified: Tue, 04 Jul 2023 20:12:14 GMT  
		Size: 293.8 KB (293837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4dbbe640a7122ac20768a9e899cd6f765aca885c9d8f66066b241d69c62228`  
		Last Modified: Tue, 04 Jul 2023 20:12:14 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad8cd1c41ec878e1b4d38c0b86b45f871a82ec4c846bc1c940a726af567ffa9`  
		Last Modified: Tue, 04 Jul 2023 20:12:18 GMT  
		Size: 23.7 MB (23672931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c967043c1f4f9a590b5704a88b2992c665bbb07c9c9113c4aa3db0677336bc88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261105671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:298033ef439c73bc03b936628122d4211f2541f4d1e9b6dcb7aabc32fcea7500`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:52:30 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 14:53:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:15 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:53:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:53:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:53:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:53:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:53:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac60340acf4f8387c6b6179b8802a4d95c8a764c3275e4b40dcf43bbc18e7`  
		Last Modified: Tue, 04 Jul 2023 15:04:37 GMT  
		Size: 121.6 MB (121594149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bc2c0b5866181e7b667506bf7186bed428e235b1f57501f01c1523f2967c6f`  
		Last Modified: Tue, 04 Jul 2023 15:04:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2d048a238d45b0bb97de4679a5201642c788107f3fadc5dffab30584467e4`  
		Last Modified: Tue, 04 Jul 2023 15:04:54 GMT  
		Size: 82.7 MB (82736920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba4ee66a2fe7e8250e08ad5ef26eb39fd9302d05030d7d5b0e029ab68d0578`  
		Last Modified: Tue, 04 Jul 2023 15:04:46 GMT  
		Size: 293.8 KB (293838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe9b0009bf0e31d2aee3d80fa185f8d16b3f596a535639dabfcd6eb502f80fe`  
		Last Modified: Tue, 04 Jul 2023 15:04:46 GMT  
		Size: 2.4 KB (2418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3befa7d317c0c7dac526b38de97ecb51a996a3d9e49e1178cdebe3d2b225cd`  
		Last Modified: Tue, 04 Jul 2023 15:04:49 GMT  
		Size: 23.1 MB (23068245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-perception`

```console
$ docker pull ros@sha256:2f1c1ee744268e7b73319046c562e04f83f887936c215b52119d8c4e056dca5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-perception` - linux; amd64

```console
$ docker pull ros@sha256:7a1b415a873cdc2fed92f158280d30a77aae1483aa7306f48fd6e295990ad242
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **958.3 MB (958307590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d38ee7ef24d2408be7fd5721c1c92d6423c39d5d508f9f0f0732a40d730d727`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:59:50 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 20:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:00:34 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 20:00:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 20:01:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 20:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:02:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c215437d76e0aa23ad3ad77eacdff757fb515043d5fbc4aaab262edecf0f570`  
		Last Modified: Tue, 04 Jul 2023 20:12:05 GMT  
		Size: 124.1 MB (124106862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b7644717ba2f3371d754f83f5d74a18227dd0efa3552b47025bd2bb2e7e92`  
		Last Modified: Tue, 04 Jul 2023 20:11:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199be721033556b61121fd3dc17b7e99b7a7f82492d2272ba5b86f84a9ce7fc2`  
		Last Modified: Tue, 04 Jul 2023 20:12:24 GMT  
		Size: 85.0 MB (84994600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ff985aa05405f2f8956ec07b70eae3f30be79fec5c6d3c1617677f4c3696ac`  
		Last Modified: Tue, 04 Jul 2023 20:12:14 GMT  
		Size: 293.8 KB (293837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4dbbe640a7122ac20768a9e899cd6f765aca885c9d8f66066b241d69c62228`  
		Last Modified: Tue, 04 Jul 2023 20:12:14 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad8cd1c41ec878e1b4d38c0b86b45f871a82ec4c846bc1c940a726af567ffa9`  
		Last Modified: Tue, 04 Jul 2023 20:12:18 GMT  
		Size: 23.7 MB (23672931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6249bb59c709d10e886ff3cc6d5c5903cdda2650148c37b11f3d87a283223a`  
		Last Modified: Tue, 04 Jul 2023 20:14:03 GMT  
		Size: 689.8 MB (689761377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e23fbdf99473f486bf44b942d6aaf3128152d34273fc4c41dd7ea96bad29a7db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **919.6 MB (919580956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fdeab7306d1f14a0c7eccac9801825ddc08511f51299cb4b6c4f82fdc8cdaca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:52:30 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 14:53:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:15 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:53:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:53:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:53:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:53:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:53:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:55:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac60340acf4f8387c6b6179b8802a4d95c8a764c3275e4b40dcf43bbc18e7`  
		Last Modified: Tue, 04 Jul 2023 15:04:37 GMT  
		Size: 121.6 MB (121594149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bc2c0b5866181e7b667506bf7186bed428e235b1f57501f01c1523f2967c6f`  
		Last Modified: Tue, 04 Jul 2023 15:04:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2d048a238d45b0bb97de4679a5201642c788107f3fadc5dffab30584467e4`  
		Last Modified: Tue, 04 Jul 2023 15:04:54 GMT  
		Size: 82.7 MB (82736920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba4ee66a2fe7e8250e08ad5ef26eb39fd9302d05030d7d5b0e029ab68d0578`  
		Last Modified: Tue, 04 Jul 2023 15:04:46 GMT  
		Size: 293.8 KB (293838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe9b0009bf0e31d2aee3d80fa185f8d16b3f596a535639dabfcd6eb502f80fe`  
		Last Modified: Tue, 04 Jul 2023 15:04:46 GMT  
		Size: 2.4 KB (2418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3befa7d317c0c7dac526b38de97ecb51a996a3d9e49e1178cdebe3d2b225cd`  
		Last Modified: Tue, 04 Jul 2023 15:04:49 GMT  
		Size: 23.1 MB (23068245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036c38cd2ca44bd4b897a9e6a91bd6e2023be22797e17aaef8e6d6b3951c8bc1`  
		Last Modified: Tue, 04 Jul 2023 15:06:17 GMT  
		Size: 658.5 MB (658475285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-perception-jammy`

```console
$ docker pull ros@sha256:2f1c1ee744268e7b73319046c562e04f83f887936c215b52119d8c4e056dca5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:7a1b415a873cdc2fed92f158280d30a77aae1483aa7306f48fd6e295990ad242
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **958.3 MB (958307590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d38ee7ef24d2408be7fd5721c1c92d6423c39d5d508f9f0f0732a40d730d727`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:59:50 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 20:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:00:34 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 20:00:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 20:01:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 20:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:02:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c215437d76e0aa23ad3ad77eacdff757fb515043d5fbc4aaab262edecf0f570`  
		Last Modified: Tue, 04 Jul 2023 20:12:05 GMT  
		Size: 124.1 MB (124106862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b7644717ba2f3371d754f83f5d74a18227dd0efa3552b47025bd2bb2e7e92`  
		Last Modified: Tue, 04 Jul 2023 20:11:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199be721033556b61121fd3dc17b7e99b7a7f82492d2272ba5b86f84a9ce7fc2`  
		Last Modified: Tue, 04 Jul 2023 20:12:24 GMT  
		Size: 85.0 MB (84994600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ff985aa05405f2f8956ec07b70eae3f30be79fec5c6d3c1617677f4c3696ac`  
		Last Modified: Tue, 04 Jul 2023 20:12:14 GMT  
		Size: 293.8 KB (293837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4dbbe640a7122ac20768a9e899cd6f765aca885c9d8f66066b241d69c62228`  
		Last Modified: Tue, 04 Jul 2023 20:12:14 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad8cd1c41ec878e1b4d38c0b86b45f871a82ec4c846bc1c940a726af567ffa9`  
		Last Modified: Tue, 04 Jul 2023 20:12:18 GMT  
		Size: 23.7 MB (23672931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6249bb59c709d10e886ff3cc6d5c5903cdda2650148c37b11f3d87a283223a`  
		Last Modified: Tue, 04 Jul 2023 20:14:03 GMT  
		Size: 689.8 MB (689761377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e23fbdf99473f486bf44b942d6aaf3128152d34273fc4c41dd7ea96bad29a7db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **919.6 MB (919580956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fdeab7306d1f14a0c7eccac9801825ddc08511f51299cb4b6c4f82fdc8cdaca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:52:30 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 14:53:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:15 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:53:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:53:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:53:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:53:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:53:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:55:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac60340acf4f8387c6b6179b8802a4d95c8a764c3275e4b40dcf43bbc18e7`  
		Last Modified: Tue, 04 Jul 2023 15:04:37 GMT  
		Size: 121.6 MB (121594149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bc2c0b5866181e7b667506bf7186bed428e235b1f57501f01c1523f2967c6f`  
		Last Modified: Tue, 04 Jul 2023 15:04:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2d048a238d45b0bb97de4679a5201642c788107f3fadc5dffab30584467e4`  
		Last Modified: Tue, 04 Jul 2023 15:04:54 GMT  
		Size: 82.7 MB (82736920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba4ee66a2fe7e8250e08ad5ef26eb39fd9302d05030d7d5b0e029ab68d0578`  
		Last Modified: Tue, 04 Jul 2023 15:04:46 GMT  
		Size: 293.8 KB (293838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe9b0009bf0e31d2aee3d80fa185f8d16b3f596a535639dabfcd6eb502f80fe`  
		Last Modified: Tue, 04 Jul 2023 15:04:46 GMT  
		Size: 2.4 KB (2418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3befa7d317c0c7dac526b38de97ecb51a996a3d9e49e1178cdebe3d2b225cd`  
		Last Modified: Tue, 04 Jul 2023 15:04:49 GMT  
		Size: 23.1 MB (23068245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036c38cd2ca44bd4b897a9e6a91bd6e2023be22797e17aaef8e6d6b3951c8bc1`  
		Last Modified: Tue, 04 Jul 2023 15:06:17 GMT  
		Size: 658.5 MB (658475285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-base`

```console
$ docker pull ros@sha256:6a007e64bcd1b093c6ccd4f4cb66b75b1ed1471b60a53c70b7e45de35ebf9184
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:c0d01ca752cc23ddddb389409680c54fb6c85949c79bc4a3bcdd2a266414a313
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.5 MB (268546213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4bee036752b69abd2271fb9ab494ff987a3923d00c355fc8651896a7dc9b00`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:59:50 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 20:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:00:34 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 20:00:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 20:01:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 20:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c215437d76e0aa23ad3ad77eacdff757fb515043d5fbc4aaab262edecf0f570`  
		Last Modified: Tue, 04 Jul 2023 20:12:05 GMT  
		Size: 124.1 MB (124106862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b7644717ba2f3371d754f83f5d74a18227dd0efa3552b47025bd2bb2e7e92`  
		Last Modified: Tue, 04 Jul 2023 20:11:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199be721033556b61121fd3dc17b7e99b7a7f82492d2272ba5b86f84a9ce7fc2`  
		Last Modified: Tue, 04 Jul 2023 20:12:24 GMT  
		Size: 85.0 MB (84994600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ff985aa05405f2f8956ec07b70eae3f30be79fec5c6d3c1617677f4c3696ac`  
		Last Modified: Tue, 04 Jul 2023 20:12:14 GMT  
		Size: 293.8 KB (293837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4dbbe640a7122ac20768a9e899cd6f765aca885c9d8f66066b241d69c62228`  
		Last Modified: Tue, 04 Jul 2023 20:12:14 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad8cd1c41ec878e1b4d38c0b86b45f871a82ec4c846bc1c940a726af567ffa9`  
		Last Modified: Tue, 04 Jul 2023 20:12:18 GMT  
		Size: 23.7 MB (23672931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c967043c1f4f9a590b5704a88b2992c665bbb07c9c9113c4aa3db0677336bc88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261105671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:298033ef439c73bc03b936628122d4211f2541f4d1e9b6dcb7aabc32fcea7500`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:52:30 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 14:53:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:15 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:53:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:53:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:53:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:53:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:53:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac60340acf4f8387c6b6179b8802a4d95c8a764c3275e4b40dcf43bbc18e7`  
		Last Modified: Tue, 04 Jul 2023 15:04:37 GMT  
		Size: 121.6 MB (121594149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bc2c0b5866181e7b667506bf7186bed428e235b1f57501f01c1523f2967c6f`  
		Last Modified: Tue, 04 Jul 2023 15:04:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2d048a238d45b0bb97de4679a5201642c788107f3fadc5dffab30584467e4`  
		Last Modified: Tue, 04 Jul 2023 15:04:54 GMT  
		Size: 82.7 MB (82736920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba4ee66a2fe7e8250e08ad5ef26eb39fd9302d05030d7d5b0e029ab68d0578`  
		Last Modified: Tue, 04 Jul 2023 15:04:46 GMT  
		Size: 293.8 KB (293838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe9b0009bf0e31d2aee3d80fa185f8d16b3f596a535639dabfcd6eb502f80fe`  
		Last Modified: Tue, 04 Jul 2023 15:04:46 GMT  
		Size: 2.4 KB (2418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3befa7d317c0c7dac526b38de97ecb51a996a3d9e49e1178cdebe3d2b225cd`  
		Last Modified: Tue, 04 Jul 2023 15:04:49 GMT  
		Size: 23.1 MB (23068245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-base-jammy`

```console
$ docker pull ros@sha256:6a007e64bcd1b093c6ccd4f4cb66b75b1ed1471b60a53c70b7e45de35ebf9184
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:c0d01ca752cc23ddddb389409680c54fb6c85949c79bc4a3bcdd2a266414a313
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.5 MB (268546213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4bee036752b69abd2271fb9ab494ff987a3923d00c355fc8651896a7dc9b00`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:59:50 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 20:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:00:34 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 20:00:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 20:01:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 20:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c215437d76e0aa23ad3ad77eacdff757fb515043d5fbc4aaab262edecf0f570`  
		Last Modified: Tue, 04 Jul 2023 20:12:05 GMT  
		Size: 124.1 MB (124106862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b7644717ba2f3371d754f83f5d74a18227dd0efa3552b47025bd2bb2e7e92`  
		Last Modified: Tue, 04 Jul 2023 20:11:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199be721033556b61121fd3dc17b7e99b7a7f82492d2272ba5b86f84a9ce7fc2`  
		Last Modified: Tue, 04 Jul 2023 20:12:24 GMT  
		Size: 85.0 MB (84994600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ff985aa05405f2f8956ec07b70eae3f30be79fec5c6d3c1617677f4c3696ac`  
		Last Modified: Tue, 04 Jul 2023 20:12:14 GMT  
		Size: 293.8 KB (293837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4dbbe640a7122ac20768a9e899cd6f765aca885c9d8f66066b241d69c62228`  
		Last Modified: Tue, 04 Jul 2023 20:12:14 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad8cd1c41ec878e1b4d38c0b86b45f871a82ec4c846bc1c940a726af567ffa9`  
		Last Modified: Tue, 04 Jul 2023 20:12:18 GMT  
		Size: 23.7 MB (23672931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c967043c1f4f9a590b5704a88b2992c665bbb07c9c9113c4aa3db0677336bc88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261105671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:298033ef439c73bc03b936628122d4211f2541f4d1e9b6dcb7aabc32fcea7500`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:52:30 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 14:53:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:15 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:53:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:53:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:53:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:53:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:53:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac60340acf4f8387c6b6179b8802a4d95c8a764c3275e4b40dcf43bbc18e7`  
		Last Modified: Tue, 04 Jul 2023 15:04:37 GMT  
		Size: 121.6 MB (121594149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bc2c0b5866181e7b667506bf7186bed428e235b1f57501f01c1523f2967c6f`  
		Last Modified: Tue, 04 Jul 2023 15:04:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2d048a238d45b0bb97de4679a5201642c788107f3fadc5dffab30584467e4`  
		Last Modified: Tue, 04 Jul 2023 15:04:54 GMT  
		Size: 82.7 MB (82736920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba4ee66a2fe7e8250e08ad5ef26eb39fd9302d05030d7d5b0e029ab68d0578`  
		Last Modified: Tue, 04 Jul 2023 15:04:46 GMT  
		Size: 293.8 KB (293838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe9b0009bf0e31d2aee3d80fa185f8d16b3f596a535639dabfcd6eb502f80fe`  
		Last Modified: Tue, 04 Jul 2023 15:04:46 GMT  
		Size: 2.4 KB (2418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3befa7d317c0c7dac526b38de97ecb51a996a3d9e49e1178cdebe3d2b225cd`  
		Last Modified: Tue, 04 Jul 2023 15:04:49 GMT  
		Size: 23.1 MB (23068245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-core`

```console
$ docker pull ros@sha256:d8e19749270e3f7b67c8bf4f0bbcc5ad6fece27f8a00d38eaa5ba858efbfb1e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:18f05ac562c1ebb43ffa4ab507a15e9789fe492b198cd8541a78e01b61602223
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159582399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a5e6419d00ad0e5309de29c100ca93f7d87acfa6cdb966031b35b86181d721b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:59:50 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 20:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:00:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c215437d76e0aa23ad3ad77eacdff757fb515043d5fbc4aaab262edecf0f570`  
		Last Modified: Tue, 04 Jul 2023 20:12:05 GMT  
		Size: 124.1 MB (124106862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b7644717ba2f3371d754f83f5d74a18227dd0efa3552b47025bd2bb2e7e92`  
		Last Modified: Tue, 04 Jul 2023 20:11:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:617c5635903767febd251dbc88045fcf7d1f24554a9bf5f23639b8bba7e842c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155004250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baf436aa820ee55cc077b2bc31fb3eb397ec1a4644eaafb0833521e0c50f3d44`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:52:30 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 14:53:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:15 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:53:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:53:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac60340acf4f8387c6b6179b8802a4d95c8a764c3275e4b40dcf43bbc18e7`  
		Last Modified: Tue, 04 Jul 2023 15:04:37 GMT  
		Size: 121.6 MB (121594149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bc2c0b5866181e7b667506bf7186bed428e235b1f57501f01c1523f2967c6f`  
		Last Modified: Tue, 04 Jul 2023 15:04:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-core-jammy`

```console
$ docker pull ros@sha256:d8e19749270e3f7b67c8bf4f0bbcc5ad6fece27f8a00d38eaa5ba858efbfb1e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:18f05ac562c1ebb43ffa4ab507a15e9789fe492b198cd8541a78e01b61602223
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159582399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a5e6419d00ad0e5309de29c100ca93f7d87acfa6cdb966031b35b86181d721b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:59:50 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 20:00:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:00:34 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:00:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:00:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c215437d76e0aa23ad3ad77eacdff757fb515043d5fbc4aaab262edecf0f570`  
		Last Modified: Tue, 04 Jul 2023 20:12:05 GMT  
		Size: 124.1 MB (124106862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b7644717ba2f3371d754f83f5d74a18227dd0efa3552b47025bd2bb2e7e92`  
		Last Modified: Tue, 04 Jul 2023 20:11:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:617c5635903767febd251dbc88045fcf7d1f24554a9bf5f23639b8bba7e842c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155004250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baf436aa820ee55cc077b2bc31fb3eb397ec1a4644eaafb0833521e0c50f3d44`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:52:30 GMT
ENV ROS_DISTRO=iron
# Tue, 04 Jul 2023 14:53:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:53:15 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:53:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:53:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac60340acf4f8387c6b6179b8802a4d95c8a764c3275e4b40dcf43bbc18e7`  
		Last Modified: Tue, 04 Jul 2023 15:04:37 GMT  
		Size: 121.6 MB (121594149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bc2c0b5866181e7b667506bf7186bed428e235b1f57501f01c1523f2967c6f`  
		Last Modified: Tue, 04 Jul 2023 15:04:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:74ca8a7e7292d618c51813fbae20abdd0495321bc5e51118a4366d4ede862729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:79355f8f337bde9a35328ba7420e384bce739fd7d7b5b7ade27b59b15c6334c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263166132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8dfee577ee17a0c0e4684c4ec3da6340c072da1c3969377404d15e3526aec12`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 19:50:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:50:04 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 19:50:04 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:50:04 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:51:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:51:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:51:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 19:52:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd524cf7754594d911fa06358015cf1327cb43355eb465f630a366e97dedef5b`  
		Last Modified: Tue, 04 Jul 2023 20:09:34 GMT  
		Size: 106.3 MB (106344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a0ac1a73dab9eca6d1d3cb5656032709291067b9f54a573c4a4730296d262b`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b3c2bf65a5f88854a4e9b3c40f16e67b119af543d6656867ff27174e1d8f45`  
		Last Modified: Tue, 04 Jul 2023 20:09:55 GMT  
		Size: 97.9 MB (97949653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fd7ea32c23c962d34cd70e32ac496fa75bc603430e4b70172a78380d217e5d`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 307.1 KB (307140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773f4fc51f45ba73bbf97b10b39b54b7e6b43063a0e37c48e847b48a62a4bf11`  
		Last Modified: Tue, 04 Jul 2023 20:09:42 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dbf8cf19eabafc2081cdee9cc9873550fd53aac2bcdc52b1cccca47f3b7976`  
		Last Modified: Tue, 04 Jul 2023 20:09:46 GMT  
		Size: 23.1 MB (23086815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:51a3bacfaad84aee1b80cf73cb3588c4b535a8b35f1a75b8c6adb315039d85d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255898065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7d9e9fcdbbe0cebc229f6d9a9afa9d00b892ee62043ffcb18c240767923d81`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV ROS_DISTRO=humble
# Tue, 04 Jul 2023 14:41:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:05 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:41:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:41:06 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:41:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:41:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:41:47 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc99b708e63ea51d08155711080144b68401240806daf3d55ff31da8ce2e6e8`  
		Last Modified: Tue, 04 Jul 2023 15:02:14 GMT  
		Size: 104.1 MB (104091352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587e83797ba402344f156014188711bc267dad06b4fc07b9b76d84206961887`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4681cb50e4211cf1a6641009dd51e6330ee41ec7d56c69974b08bcad3e1eb97`  
		Last Modified: Tue, 04 Jul 2023 15:02:33 GMT  
		Size: 95.6 MB (95583335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64814832cf8516f200bd7dd874fa74752b972925ab9c3589cff205384d75de09`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 307.1 KB (307139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22ee3968485d390f331fe27b0544cdaa0341b0cf480ee4322c0dc756fe3160c`  
		Last Modified: Tue, 04 Jul 2023 15:02:23 GMT  
		Size: 2.4 KB (2443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e450a263466aac0036b7b14cb06363d88c97575eb95b4d03e7cd1541305e43b6`  
		Last Modified: Tue, 04 Jul 2023 15:02:26 GMT  
		Size: 22.5 MB (22503697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:b03f16f088bfe16a6b43bd7c7c8214b05699862024e59a594d9cee594441af43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:1f2a7d8e59ee5906b1f79b47f293d7458421a6e59561edfa0de0bb678caf0c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343210185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a98bb7bca647203e46bd29f1e0ab661837100a39f9c592d05459e376a040883`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:38:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:38:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:40:36 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:40:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:40:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:41:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:41:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:42:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff84dd75ab0363da2809c202391ffc2d59534b4888fb855bfd3e21fba17c6fc`  
		Last Modified: Tue, 04 Jul 2023 20:06:54 GMT  
		Size: 1.2 MB (1198708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564b5c67648727c462a4c2ba9d04cdbfa852b527efa36e4c6a859b58454f1c06`  
		Last Modified: Tue, 04 Jul 2023 20:06:53 GMT  
		Size: 5.6 MB (5553847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d18d779d6732554da8eb52855df2ccfe7921f00655dffb89550af33715f184`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5d180dd93ee0210935b93b72cc533ed3b35e05a47dc0b20fb5b5b9884e4c3`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac36e4a2604385d7a84264dc122ac61dd1af8f304d486fc983703238a0d02333`  
		Last Modified: Tue, 04 Jul 2023 20:07:19 GMT  
		Size: 177.0 MB (177027946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca272865f67e094abd7a450c446c31552297e72292785448cac9df1ac6bdcd1`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c2048f289191c959ae1bde0b76c4c37af804966f66c4599e4745a47810cad`  
		Last Modified: Tue, 04 Jul 2023 20:07:35 GMT  
		Size: 50.9 MB (50939858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ad18f9d687633622e84262935b3873354dcf6c1ce6c32d67568aa7f9c351f`  
		Last Modified: Tue, 04 Jul 2023 20:07:28 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9b129af37cdd180a7f4bb7fc69172d71d5bbc7c2e1eb95896ae3fa7a973fe`  
		Last Modified: Tue, 04 Jul 2023 20:07:39 GMT  
		Size: 79.6 MB (79604734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:44d4f5184dee8e1470cef26eb31aaca402a607f556ef3dcfd6695610f10c6d9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289311711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a824034ce70955715c5ad01653744c4c3a0330ad7419be72d21b1dbeb702391`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:51:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:52:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:55:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:55:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:55:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:57:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae4844234b1655ffcc66de6ff4d8fb9d8dc5b263579abf1c0f08fc45c10b`  
		Last Modified: Tue, 04 Jul 2023 20:06:37 GMT  
		Size: 1.2 MB (1198714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f870418e12b4135248455da61f5521096265e859ed7df1641c96d8052c1cd1ed`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 4.7 MB (4679197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37cb4cc4c6e905769f0ad1f740744e276e496b07b5efc7e4dcfd333e303892`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e584269a8e1f1afb39b1c87e053140430bf059f1a78c8091f862a0a6d7ce9d0`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f17c57312bea1c2c36a5f0b529de68ac63f57144e4e7911f2bfbdaa007f1cc2`  
		Last Modified: Tue, 04 Jul 2023 20:07:03 GMT  
		Size: 157.5 MB (157543123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb0493e0b9da981ce0cd0c9aeab054329b78efe17d28f3a208cfe95f617a1`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ec7ad778d705ac798c8c4e72ac5e0a3d97e71bf31fb07dc28dc1c7dbfde0b`  
		Last Modified: Tue, 04 Jul 2023 20:07:17 GMT  
		Size: 40.5 MB (40503772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4463c21fd1b24a56ceff0c21678439984b89244a4de1cebf2ca5d1e4fe6f6c`  
		Last Modified: Tue, 04 Jul 2023 20:07:12 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825a9d60f2d0bb1d7c24f20b6232803e0cae89bbd590ec88ddcddd9186193f1a`  
		Last Modified: Tue, 04 Jul 2023 20:07:21 GMT  
		Size: 60.5 MB (60493692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f131f36e81dbf42293146b1fa7d86be2ee41013c608e68efa1d355d1fc805f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322922029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f675169c509f89573c15272afd2e0826150be2d161f7dd7286baeab5042ef6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 14:25:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 14:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:28:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 14:28:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:28:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:29:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:29:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:30:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdd39b6ea2b9a0ce173cf2e1f26322497d5a9c7710030e37439ad5d4b2523`  
		Last Modified: Tue, 04 Jul 2023 14:59:38 GMT  
		Size: 1.2 MB (1199222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb204de59b70d94654e7760fc586c55bcd195218315dbf7589d66289510f275`  
		Last Modified: Tue, 04 Jul 2023 14:59:36 GMT  
		Size: 5.5 MB (5532648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74969841e6f58cb9e0f0a3c29463b5877ac9e57c3ce30bfcf3c1a6f5d74b6e`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed7a86bfb6803f03f9f877eab39ae2496795feb327436a44d9450ce2781b071`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d91c98424c5722a91cb12e54ca5c7af9f12c034b801df540e013a52df8e938`  
		Last Modified: Tue, 04 Jul 2023 15:00:09 GMT  
		Size: 171.5 MB (171511899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493841186da8cc28dcd3542f3c5e48f6853b465d5389b8a2e595292fe4acfa57`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656ccdb00e6c88095176998c459e8fbff2585a38ed2a7781a7812e457b3abe9a`  
		Last Modified: Tue, 04 Jul 2023 15:00:26 GMT  
		Size: 45.2 MB (45204441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cbde3a0d7e6e385474cc8f84e37c7ddb2ac72700849e7e7a586690a0a29efb`  
		Last Modified: Tue, 04 Jul 2023 15:00:21 GMT  
		Size: 302.7 KB (302677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a52ffd06935d7fffa1923572f179f9d9aa8e0661022b715746f72ad0673679`  
		Last Modified: Tue, 04 Jul 2023 15:00:30 GMT  
		Size: 72.0 MB (71970399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:ebe365d4e1b0b32e340c97a244396438efb4d371552eb2bdd90823eec6ef8483
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:17c20f8ed1eb9f78a84888c504ff6d817df0cad9639322203443d179a285030f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835187001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b06e83a64c3fe81d8797973d87f5889d6634bd1ad602d7afdea402b4c491aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:38:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:38:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:40:36 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:40:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:40:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:41:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:41:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:42:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:47:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff84dd75ab0363da2809c202391ffc2d59534b4888fb855bfd3e21fba17c6fc`  
		Last Modified: Tue, 04 Jul 2023 20:06:54 GMT  
		Size: 1.2 MB (1198708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564b5c67648727c462a4c2ba9d04cdbfa852b527efa36e4c6a859b58454f1c06`  
		Last Modified: Tue, 04 Jul 2023 20:06:53 GMT  
		Size: 5.6 MB (5553847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d18d779d6732554da8eb52855df2ccfe7921f00655dffb89550af33715f184`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5d180dd93ee0210935b93b72cc533ed3b35e05a47dc0b20fb5b5b9884e4c3`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac36e4a2604385d7a84264dc122ac61dd1af8f304d486fc983703238a0d02333`  
		Last Modified: Tue, 04 Jul 2023 20:07:19 GMT  
		Size: 177.0 MB (177027946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca272865f67e094abd7a450c446c31552297e72292785448cac9df1ac6bdcd1`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c2048f289191c959ae1bde0b76c4c37af804966f66c4599e4745a47810cad`  
		Last Modified: Tue, 04 Jul 2023 20:07:35 GMT  
		Size: 50.9 MB (50939858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ad18f9d687633622e84262935b3873354dcf6c1ce6c32d67568aa7f9c351f`  
		Last Modified: Tue, 04 Jul 2023 20:07:28 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9b129af37cdd180a7f4bb7fc69172d71d5bbc7c2e1eb95896ae3fa7a973fe`  
		Last Modified: Tue, 04 Jul 2023 20:07:39 GMT  
		Size: 79.6 MB (79604734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fb0bc20f4dc2d238bcb5f4d176ff43fb54f3b5a34458d48581516b9e84f6f1`  
		Last Modified: Tue, 04 Jul 2023 20:09:08 GMT  
		Size: 492.0 MB (491976816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:2e4ad716540593d1c21f58b35bf57b60b8b1425a8b2a1f36f8fe1b0d6ac45c2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726232769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f295e97a2f32d9cf7b131c884666f3f6efb35416466b359864f85227a14399`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:51:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:52:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:55:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:55:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:55:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:57:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:06:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae4844234b1655ffcc66de6ff4d8fb9d8dc5b263579abf1c0f08fc45c10b`  
		Last Modified: Tue, 04 Jul 2023 20:06:37 GMT  
		Size: 1.2 MB (1198714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f870418e12b4135248455da61f5521096265e859ed7df1641c96d8052c1cd1ed`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 4.7 MB (4679197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37cb4cc4c6e905769f0ad1f740744e276e496b07b5efc7e4dcfd333e303892`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e584269a8e1f1afb39b1c87e053140430bf059f1a78c8091f862a0a6d7ce9d0`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f17c57312bea1c2c36a5f0b529de68ac63f57144e4e7911f2bfbdaa007f1cc2`  
		Last Modified: Tue, 04 Jul 2023 20:07:03 GMT  
		Size: 157.5 MB (157543123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb0493e0b9da981ce0cd0c9aeab054329b78efe17d28f3a208cfe95f617a1`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ec7ad778d705ac798c8c4e72ac5e0a3d97e71bf31fb07dc28dc1c7dbfde0b`  
		Last Modified: Tue, 04 Jul 2023 20:07:17 GMT  
		Size: 40.5 MB (40503772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4463c21fd1b24a56ceff0c21678439984b89244a4de1cebf2ca5d1e4fe6f6c`  
		Last Modified: Tue, 04 Jul 2023 20:07:12 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825a9d60f2d0bb1d7c24f20b6232803e0cae89bbd590ec88ddcddd9186193f1a`  
		Last Modified: Tue, 04 Jul 2023 20:07:21 GMT  
		Size: 60.5 MB (60493692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9006a1bc48bc1a39846cdf688a533b775edb084b4f4cd75ab02bcc177fafa96d`  
		Last Modified: Tue, 04 Jul 2023 20:08:44 GMT  
		Size: 436.9 MB (436921058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fdbfb16fa302ffa99fa36abe4cde931930932b2eb5f3c4b19e2a62a05507dbd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.5 MB (785485223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e7ea58b109d590f4104b95cbc549cfede81b828eef5add2311188a7b44a9f5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 14:25:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 14:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:28:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 14:28:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:28:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:29:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:29:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:30:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdd39b6ea2b9a0ce173cf2e1f26322497d5a9c7710030e37439ad5d4b2523`  
		Last Modified: Tue, 04 Jul 2023 14:59:38 GMT  
		Size: 1.2 MB (1199222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb204de59b70d94654e7760fc586c55bcd195218315dbf7589d66289510f275`  
		Last Modified: Tue, 04 Jul 2023 14:59:36 GMT  
		Size: 5.5 MB (5532648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74969841e6f58cb9e0f0a3c29463b5877ac9e57c3ce30bfcf3c1a6f5d74b6e`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed7a86bfb6803f03f9f877eab39ae2496795feb327436a44d9450ce2781b071`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d91c98424c5722a91cb12e54ca5c7af9f12c034b801df540e013a52df8e938`  
		Last Modified: Tue, 04 Jul 2023 15:00:09 GMT  
		Size: 171.5 MB (171511899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493841186da8cc28dcd3542f3c5e48f6853b465d5389b8a2e595292fe4acfa57`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656ccdb00e6c88095176998c459e8fbff2585a38ed2a7781a7812e457b3abe9a`  
		Last Modified: Tue, 04 Jul 2023 15:00:26 GMT  
		Size: 45.2 MB (45204441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cbde3a0d7e6e385474cc8f84e37c7ddb2ac72700849e7e7a586690a0a29efb`  
		Last Modified: Tue, 04 Jul 2023 15:00:21 GMT  
		Size: 302.7 KB (302677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a52ffd06935d7fffa1923572f179f9d9aa8e0661022b715746f72ad0673679`  
		Last Modified: Tue, 04 Jul 2023 15:00:30 GMT  
		Size: 72.0 MB (71970399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37babbad7c4188821f3d9eeb838dc093838baf3b6f540e4baf0bda988f59c31b`  
		Last Modified: Tue, 04 Jul 2023 15:01:51 GMT  
		Size: 462.6 MB (462563194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:ebe365d4e1b0b32e340c97a244396438efb4d371552eb2bdd90823eec6ef8483
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:17c20f8ed1eb9f78a84888c504ff6d817df0cad9639322203443d179a285030f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835187001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b06e83a64c3fe81d8797973d87f5889d6634bd1ad602d7afdea402b4c491aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:38:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:38:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:40:36 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:40:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:40:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:41:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:41:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:42:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:47:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff84dd75ab0363da2809c202391ffc2d59534b4888fb855bfd3e21fba17c6fc`  
		Last Modified: Tue, 04 Jul 2023 20:06:54 GMT  
		Size: 1.2 MB (1198708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564b5c67648727c462a4c2ba9d04cdbfa852b527efa36e4c6a859b58454f1c06`  
		Last Modified: Tue, 04 Jul 2023 20:06:53 GMT  
		Size: 5.6 MB (5553847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d18d779d6732554da8eb52855df2ccfe7921f00655dffb89550af33715f184`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5d180dd93ee0210935b93b72cc533ed3b35e05a47dc0b20fb5b5b9884e4c3`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac36e4a2604385d7a84264dc122ac61dd1af8f304d486fc983703238a0d02333`  
		Last Modified: Tue, 04 Jul 2023 20:07:19 GMT  
		Size: 177.0 MB (177027946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca272865f67e094abd7a450c446c31552297e72292785448cac9df1ac6bdcd1`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c2048f289191c959ae1bde0b76c4c37af804966f66c4599e4745a47810cad`  
		Last Modified: Tue, 04 Jul 2023 20:07:35 GMT  
		Size: 50.9 MB (50939858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ad18f9d687633622e84262935b3873354dcf6c1ce6c32d67568aa7f9c351f`  
		Last Modified: Tue, 04 Jul 2023 20:07:28 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9b129af37cdd180a7f4bb7fc69172d71d5bbc7c2e1eb95896ae3fa7a973fe`  
		Last Modified: Tue, 04 Jul 2023 20:07:39 GMT  
		Size: 79.6 MB (79604734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fb0bc20f4dc2d238bcb5f4d176ff43fb54f3b5a34458d48581516b9e84f6f1`  
		Last Modified: Tue, 04 Jul 2023 20:09:08 GMT  
		Size: 492.0 MB (491976816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:2e4ad716540593d1c21f58b35bf57b60b8b1425a8b2a1f36f8fe1b0d6ac45c2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726232769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f295e97a2f32d9cf7b131c884666f3f6efb35416466b359864f85227a14399`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:51:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:52:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:55:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:55:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:55:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:57:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:06:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae4844234b1655ffcc66de6ff4d8fb9d8dc5b263579abf1c0f08fc45c10b`  
		Last Modified: Tue, 04 Jul 2023 20:06:37 GMT  
		Size: 1.2 MB (1198714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f870418e12b4135248455da61f5521096265e859ed7df1641c96d8052c1cd1ed`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 4.7 MB (4679197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37cb4cc4c6e905769f0ad1f740744e276e496b07b5efc7e4dcfd333e303892`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e584269a8e1f1afb39b1c87e053140430bf059f1a78c8091f862a0a6d7ce9d0`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f17c57312bea1c2c36a5f0b529de68ac63f57144e4e7911f2bfbdaa007f1cc2`  
		Last Modified: Tue, 04 Jul 2023 20:07:03 GMT  
		Size: 157.5 MB (157543123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb0493e0b9da981ce0cd0c9aeab054329b78efe17d28f3a208cfe95f617a1`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ec7ad778d705ac798c8c4e72ac5e0a3d97e71bf31fb07dc28dc1c7dbfde0b`  
		Last Modified: Tue, 04 Jul 2023 20:07:17 GMT  
		Size: 40.5 MB (40503772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4463c21fd1b24a56ceff0c21678439984b89244a4de1cebf2ca5d1e4fe6f6c`  
		Last Modified: Tue, 04 Jul 2023 20:07:12 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825a9d60f2d0bb1d7c24f20b6232803e0cae89bbd590ec88ddcddd9186193f1a`  
		Last Modified: Tue, 04 Jul 2023 20:07:21 GMT  
		Size: 60.5 MB (60493692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9006a1bc48bc1a39846cdf688a533b775edb084b4f4cd75ab02bcc177fafa96d`  
		Last Modified: Tue, 04 Jul 2023 20:08:44 GMT  
		Size: 436.9 MB (436921058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fdbfb16fa302ffa99fa36abe4cde931930932b2eb5f3c4b19e2a62a05507dbd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.5 MB (785485223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e7ea58b109d590f4104b95cbc549cfede81b828eef5add2311188a7b44a9f5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 14:25:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 14:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:28:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 14:28:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:28:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:29:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:29:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:30:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdd39b6ea2b9a0ce173cf2e1f26322497d5a9c7710030e37439ad5d4b2523`  
		Last Modified: Tue, 04 Jul 2023 14:59:38 GMT  
		Size: 1.2 MB (1199222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb204de59b70d94654e7760fc586c55bcd195218315dbf7589d66289510f275`  
		Last Modified: Tue, 04 Jul 2023 14:59:36 GMT  
		Size: 5.5 MB (5532648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74969841e6f58cb9e0f0a3c29463b5877ac9e57c3ce30bfcf3c1a6f5d74b6e`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed7a86bfb6803f03f9f877eab39ae2496795feb327436a44d9450ce2781b071`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d91c98424c5722a91cb12e54ca5c7af9f12c034b801df540e013a52df8e938`  
		Last Modified: Tue, 04 Jul 2023 15:00:09 GMT  
		Size: 171.5 MB (171511899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493841186da8cc28dcd3542f3c5e48f6853b465d5389b8a2e595292fe4acfa57`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656ccdb00e6c88095176998c459e8fbff2585a38ed2a7781a7812e457b3abe9a`  
		Last Modified: Tue, 04 Jul 2023 15:00:26 GMT  
		Size: 45.2 MB (45204441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cbde3a0d7e6e385474cc8f84e37c7ddb2ac72700849e7e7a586690a0a29efb`  
		Last Modified: Tue, 04 Jul 2023 15:00:21 GMT  
		Size: 302.7 KB (302677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a52ffd06935d7fffa1923572f179f9d9aa8e0661022b715746f72ad0673679`  
		Last Modified: Tue, 04 Jul 2023 15:00:30 GMT  
		Size: 72.0 MB (71970399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37babbad7c4188821f3d9eeb838dc093838baf3b6f540e4baf0bda988f59c31b`  
		Last Modified: Tue, 04 Jul 2023 15:01:51 GMT  
		Size: 462.6 MB (462563194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:99ad37a4b45de140c26d04dee130099124353535038d9a8dc53c46e19b50fb72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:74b585c00c52a11bc9ec0958cc34a2a5cc8e7095c64212e77683c08a3a5281d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359072544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e4b1ab66575af3b1bb37ec6aa0a39b517f644917f4a44bfb92ef5c30c0b5c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:38:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:38:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:40:36 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:40:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:40:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:41:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:41:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:42:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:43:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff84dd75ab0363da2809c202391ffc2d59534b4888fb855bfd3e21fba17c6fc`  
		Last Modified: Tue, 04 Jul 2023 20:06:54 GMT  
		Size: 1.2 MB (1198708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564b5c67648727c462a4c2ba9d04cdbfa852b527efa36e4c6a859b58454f1c06`  
		Last Modified: Tue, 04 Jul 2023 20:06:53 GMT  
		Size: 5.6 MB (5553847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d18d779d6732554da8eb52855df2ccfe7921f00655dffb89550af33715f184`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5d180dd93ee0210935b93b72cc533ed3b35e05a47dc0b20fb5b5b9884e4c3`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac36e4a2604385d7a84264dc122ac61dd1af8f304d486fc983703238a0d02333`  
		Last Modified: Tue, 04 Jul 2023 20:07:19 GMT  
		Size: 177.0 MB (177027946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca272865f67e094abd7a450c446c31552297e72292785448cac9df1ac6bdcd1`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c2048f289191c959ae1bde0b76c4c37af804966f66c4599e4745a47810cad`  
		Last Modified: Tue, 04 Jul 2023 20:07:35 GMT  
		Size: 50.9 MB (50939858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ad18f9d687633622e84262935b3873354dcf6c1ce6c32d67568aa7f9c351f`  
		Last Modified: Tue, 04 Jul 2023 20:07:28 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9b129af37cdd180a7f4bb7fc69172d71d5bbc7c2e1eb95896ae3fa7a973fe`  
		Last Modified: Tue, 04 Jul 2023 20:07:39 GMT  
		Size: 79.6 MB (79604734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c101713292cc95f42a217f6ed45522650943e3e1a114dec8b652fc43e710b2e`  
		Last Modified: Tue, 04 Jul 2023 20:07:52 GMT  
		Size: 15.9 MB (15862359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:9cd1b1ca2f064657e51e039dd1e8d3732503bd9e53154ec28d56e12e567bf580
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303379129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ca73e319f53dd262315677632c97c32581d5179f0b30d78bd374e983b43c9e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:51:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:52:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:55:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:55:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:55:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:57:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:58:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae4844234b1655ffcc66de6ff4d8fb9d8dc5b263579abf1c0f08fc45c10b`  
		Last Modified: Tue, 04 Jul 2023 20:06:37 GMT  
		Size: 1.2 MB (1198714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f870418e12b4135248455da61f5521096265e859ed7df1641c96d8052c1cd1ed`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 4.7 MB (4679197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37cb4cc4c6e905769f0ad1f740744e276e496b07b5efc7e4dcfd333e303892`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e584269a8e1f1afb39b1c87e053140430bf059f1a78c8091f862a0a6d7ce9d0`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f17c57312bea1c2c36a5f0b529de68ac63f57144e4e7911f2bfbdaa007f1cc2`  
		Last Modified: Tue, 04 Jul 2023 20:07:03 GMT  
		Size: 157.5 MB (157543123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb0493e0b9da981ce0cd0c9aeab054329b78efe17d28f3a208cfe95f617a1`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ec7ad778d705ac798c8c4e72ac5e0a3d97e71bf31fb07dc28dc1c7dbfde0b`  
		Last Modified: Tue, 04 Jul 2023 20:07:17 GMT  
		Size: 40.5 MB (40503772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4463c21fd1b24a56ceff0c21678439984b89244a4de1cebf2ca5d1e4fe6f6c`  
		Last Modified: Tue, 04 Jul 2023 20:07:12 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825a9d60f2d0bb1d7c24f20b6232803e0cae89bbd590ec88ddcddd9186193f1a`  
		Last Modified: Tue, 04 Jul 2023 20:07:21 GMT  
		Size: 60.5 MB (60493692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e70a84a8ae6597832e2577f2ea351fd41792040b5899b69b5057d9c0f51f2e`  
		Last Modified: Tue, 04 Jul 2023 20:07:35 GMT  
		Size: 14.1 MB (14067418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1e22313404c5ca312b67aa4f87c8eb00e8e9ac59e2a25732055b3b7dddc76db9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.4 MB (338380354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1f1af6ab834f1257ede11a3c92856f1389605c55fedefbd2504a62e28c74361`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 14:25:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 14:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:28:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 14:28:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:28:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:29:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:29:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:30:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:31:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdd39b6ea2b9a0ce173cf2e1f26322497d5a9c7710030e37439ad5d4b2523`  
		Last Modified: Tue, 04 Jul 2023 14:59:38 GMT  
		Size: 1.2 MB (1199222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb204de59b70d94654e7760fc586c55bcd195218315dbf7589d66289510f275`  
		Last Modified: Tue, 04 Jul 2023 14:59:36 GMT  
		Size: 5.5 MB (5532648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74969841e6f58cb9e0f0a3c29463b5877ac9e57c3ce30bfcf3c1a6f5d74b6e`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed7a86bfb6803f03f9f877eab39ae2496795feb327436a44d9450ce2781b071`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d91c98424c5722a91cb12e54ca5c7af9f12c034b801df540e013a52df8e938`  
		Last Modified: Tue, 04 Jul 2023 15:00:09 GMT  
		Size: 171.5 MB (171511899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493841186da8cc28dcd3542f3c5e48f6853b465d5389b8a2e595292fe4acfa57`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656ccdb00e6c88095176998c459e8fbff2585a38ed2a7781a7812e457b3abe9a`  
		Last Modified: Tue, 04 Jul 2023 15:00:26 GMT  
		Size: 45.2 MB (45204441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cbde3a0d7e6e385474cc8f84e37c7ddb2ac72700849e7e7a586690a0a29efb`  
		Last Modified: Tue, 04 Jul 2023 15:00:21 GMT  
		Size: 302.7 KB (302677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a52ffd06935d7fffa1923572f179f9d9aa8e0661022b715746f72ad0673679`  
		Last Modified: Tue, 04 Jul 2023 15:00:30 GMT  
		Size: 72.0 MB (71970399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a7976716fa1fb13821d8de1ed68e5a9f2ccf40cb3d3f3a7ced0a62d94bc635`  
		Last Modified: Tue, 04 Jul 2023 15:00:43 GMT  
		Size: 15.5 MB (15458325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:99ad37a4b45de140c26d04dee130099124353535038d9a8dc53c46e19b50fb72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:74b585c00c52a11bc9ec0958cc34a2a5cc8e7095c64212e77683c08a3a5281d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359072544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e4b1ab66575af3b1bb37ec6aa0a39b517f644917f4a44bfb92ef5c30c0b5c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:38:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:38:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:40:36 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:40:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:40:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:41:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:41:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:42:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:43:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff84dd75ab0363da2809c202391ffc2d59534b4888fb855bfd3e21fba17c6fc`  
		Last Modified: Tue, 04 Jul 2023 20:06:54 GMT  
		Size: 1.2 MB (1198708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564b5c67648727c462a4c2ba9d04cdbfa852b527efa36e4c6a859b58454f1c06`  
		Last Modified: Tue, 04 Jul 2023 20:06:53 GMT  
		Size: 5.6 MB (5553847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d18d779d6732554da8eb52855df2ccfe7921f00655dffb89550af33715f184`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5d180dd93ee0210935b93b72cc533ed3b35e05a47dc0b20fb5b5b9884e4c3`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac36e4a2604385d7a84264dc122ac61dd1af8f304d486fc983703238a0d02333`  
		Last Modified: Tue, 04 Jul 2023 20:07:19 GMT  
		Size: 177.0 MB (177027946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca272865f67e094abd7a450c446c31552297e72292785448cac9df1ac6bdcd1`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c2048f289191c959ae1bde0b76c4c37af804966f66c4599e4745a47810cad`  
		Last Modified: Tue, 04 Jul 2023 20:07:35 GMT  
		Size: 50.9 MB (50939858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ad18f9d687633622e84262935b3873354dcf6c1ce6c32d67568aa7f9c351f`  
		Last Modified: Tue, 04 Jul 2023 20:07:28 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9b129af37cdd180a7f4bb7fc69172d71d5bbc7c2e1eb95896ae3fa7a973fe`  
		Last Modified: Tue, 04 Jul 2023 20:07:39 GMT  
		Size: 79.6 MB (79604734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c101713292cc95f42a217f6ed45522650943e3e1a114dec8b652fc43e710b2e`  
		Last Modified: Tue, 04 Jul 2023 20:07:52 GMT  
		Size: 15.9 MB (15862359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:9cd1b1ca2f064657e51e039dd1e8d3732503bd9e53154ec28d56e12e567bf580
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303379129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ca73e319f53dd262315677632c97c32581d5179f0b30d78bd374e983b43c9e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:51:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:52:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:55:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:55:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:55:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:57:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:58:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae4844234b1655ffcc66de6ff4d8fb9d8dc5b263579abf1c0f08fc45c10b`  
		Last Modified: Tue, 04 Jul 2023 20:06:37 GMT  
		Size: 1.2 MB (1198714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f870418e12b4135248455da61f5521096265e859ed7df1641c96d8052c1cd1ed`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 4.7 MB (4679197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37cb4cc4c6e905769f0ad1f740744e276e496b07b5efc7e4dcfd333e303892`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e584269a8e1f1afb39b1c87e053140430bf059f1a78c8091f862a0a6d7ce9d0`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f17c57312bea1c2c36a5f0b529de68ac63f57144e4e7911f2bfbdaa007f1cc2`  
		Last Modified: Tue, 04 Jul 2023 20:07:03 GMT  
		Size: 157.5 MB (157543123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb0493e0b9da981ce0cd0c9aeab054329b78efe17d28f3a208cfe95f617a1`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ec7ad778d705ac798c8c4e72ac5e0a3d97e71bf31fb07dc28dc1c7dbfde0b`  
		Last Modified: Tue, 04 Jul 2023 20:07:17 GMT  
		Size: 40.5 MB (40503772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4463c21fd1b24a56ceff0c21678439984b89244a4de1cebf2ca5d1e4fe6f6c`  
		Last Modified: Tue, 04 Jul 2023 20:07:12 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825a9d60f2d0bb1d7c24f20b6232803e0cae89bbd590ec88ddcddd9186193f1a`  
		Last Modified: Tue, 04 Jul 2023 20:07:21 GMT  
		Size: 60.5 MB (60493692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e70a84a8ae6597832e2577f2ea351fd41792040b5899b69b5057d9c0f51f2e`  
		Last Modified: Tue, 04 Jul 2023 20:07:35 GMT  
		Size: 14.1 MB (14067418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1e22313404c5ca312b67aa4f87c8eb00e8e9ac59e2a25732055b3b7dddc76db9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.4 MB (338380354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1f1af6ab834f1257ede11a3c92856f1389605c55fedefbd2504a62e28c74361`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 14:25:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 14:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:28:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 14:28:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:28:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:29:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:29:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:30:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:31:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdd39b6ea2b9a0ce173cf2e1f26322497d5a9c7710030e37439ad5d4b2523`  
		Last Modified: Tue, 04 Jul 2023 14:59:38 GMT  
		Size: 1.2 MB (1199222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb204de59b70d94654e7760fc586c55bcd195218315dbf7589d66289510f275`  
		Last Modified: Tue, 04 Jul 2023 14:59:36 GMT  
		Size: 5.5 MB (5532648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74969841e6f58cb9e0f0a3c29463b5877ac9e57c3ce30bfcf3c1a6f5d74b6e`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed7a86bfb6803f03f9f877eab39ae2496795feb327436a44d9450ce2781b071`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d91c98424c5722a91cb12e54ca5c7af9f12c034b801df540e013a52df8e938`  
		Last Modified: Tue, 04 Jul 2023 15:00:09 GMT  
		Size: 171.5 MB (171511899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493841186da8cc28dcd3542f3c5e48f6853b465d5389b8a2e595292fe4acfa57`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656ccdb00e6c88095176998c459e8fbff2585a38ed2a7781a7812e457b3abe9a`  
		Last Modified: Tue, 04 Jul 2023 15:00:26 GMT  
		Size: 45.2 MB (45204441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cbde3a0d7e6e385474cc8f84e37c7ddb2ac72700849e7e7a586690a0a29efb`  
		Last Modified: Tue, 04 Jul 2023 15:00:21 GMT  
		Size: 302.7 KB (302677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a52ffd06935d7fffa1923572f179f9d9aa8e0661022b715746f72ad0673679`  
		Last Modified: Tue, 04 Jul 2023 15:00:30 GMT  
		Size: 72.0 MB (71970399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a7976716fa1fb13821d8de1ed68e5a9f2ccf40cb3d3f3a7ced0a62d94bc635`  
		Last Modified: Tue, 04 Jul 2023 15:00:43 GMT  
		Size: 15.5 MB (15458325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:b03f16f088bfe16a6b43bd7c7c8214b05699862024e59a594d9cee594441af43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:1f2a7d8e59ee5906b1f79b47f293d7458421a6e59561edfa0de0bb678caf0c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343210185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a98bb7bca647203e46bd29f1e0ab661837100a39f9c592d05459e376a040883`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:38:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:38:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:40:36 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:40:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:40:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:41:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:41:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:42:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff84dd75ab0363da2809c202391ffc2d59534b4888fb855bfd3e21fba17c6fc`  
		Last Modified: Tue, 04 Jul 2023 20:06:54 GMT  
		Size: 1.2 MB (1198708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564b5c67648727c462a4c2ba9d04cdbfa852b527efa36e4c6a859b58454f1c06`  
		Last Modified: Tue, 04 Jul 2023 20:06:53 GMT  
		Size: 5.6 MB (5553847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d18d779d6732554da8eb52855df2ccfe7921f00655dffb89550af33715f184`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5d180dd93ee0210935b93b72cc533ed3b35e05a47dc0b20fb5b5b9884e4c3`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac36e4a2604385d7a84264dc122ac61dd1af8f304d486fc983703238a0d02333`  
		Last Modified: Tue, 04 Jul 2023 20:07:19 GMT  
		Size: 177.0 MB (177027946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca272865f67e094abd7a450c446c31552297e72292785448cac9df1ac6bdcd1`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c2048f289191c959ae1bde0b76c4c37af804966f66c4599e4745a47810cad`  
		Last Modified: Tue, 04 Jul 2023 20:07:35 GMT  
		Size: 50.9 MB (50939858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ad18f9d687633622e84262935b3873354dcf6c1ce6c32d67568aa7f9c351f`  
		Last Modified: Tue, 04 Jul 2023 20:07:28 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9b129af37cdd180a7f4bb7fc69172d71d5bbc7c2e1eb95896ae3fa7a973fe`  
		Last Modified: Tue, 04 Jul 2023 20:07:39 GMT  
		Size: 79.6 MB (79604734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:44d4f5184dee8e1470cef26eb31aaca402a607f556ef3dcfd6695610f10c6d9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289311711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a824034ce70955715c5ad01653744c4c3a0330ad7419be72d21b1dbeb702391`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:51:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:52:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:55:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:55:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:55:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:57:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae4844234b1655ffcc66de6ff4d8fb9d8dc5b263579abf1c0f08fc45c10b`  
		Last Modified: Tue, 04 Jul 2023 20:06:37 GMT  
		Size: 1.2 MB (1198714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f870418e12b4135248455da61f5521096265e859ed7df1641c96d8052c1cd1ed`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 4.7 MB (4679197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37cb4cc4c6e905769f0ad1f740744e276e496b07b5efc7e4dcfd333e303892`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e584269a8e1f1afb39b1c87e053140430bf059f1a78c8091f862a0a6d7ce9d0`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f17c57312bea1c2c36a5f0b529de68ac63f57144e4e7911f2bfbdaa007f1cc2`  
		Last Modified: Tue, 04 Jul 2023 20:07:03 GMT  
		Size: 157.5 MB (157543123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb0493e0b9da981ce0cd0c9aeab054329b78efe17d28f3a208cfe95f617a1`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ec7ad778d705ac798c8c4e72ac5e0a3d97e71bf31fb07dc28dc1c7dbfde0b`  
		Last Modified: Tue, 04 Jul 2023 20:07:17 GMT  
		Size: 40.5 MB (40503772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4463c21fd1b24a56ceff0c21678439984b89244a4de1cebf2ca5d1e4fe6f6c`  
		Last Modified: Tue, 04 Jul 2023 20:07:12 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825a9d60f2d0bb1d7c24f20b6232803e0cae89bbd590ec88ddcddd9186193f1a`  
		Last Modified: Tue, 04 Jul 2023 20:07:21 GMT  
		Size: 60.5 MB (60493692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f131f36e81dbf42293146b1fa7d86be2ee41013c608e68efa1d355d1fc805f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322922029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f675169c509f89573c15272afd2e0826150be2d161f7dd7286baeab5042ef6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 14:25:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 14:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:28:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 14:28:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:28:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:29:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:29:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:30:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdd39b6ea2b9a0ce173cf2e1f26322497d5a9c7710030e37439ad5d4b2523`  
		Last Modified: Tue, 04 Jul 2023 14:59:38 GMT  
		Size: 1.2 MB (1199222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb204de59b70d94654e7760fc586c55bcd195218315dbf7589d66289510f275`  
		Last Modified: Tue, 04 Jul 2023 14:59:36 GMT  
		Size: 5.5 MB (5532648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74969841e6f58cb9e0f0a3c29463b5877ac9e57c3ce30bfcf3c1a6f5d74b6e`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed7a86bfb6803f03f9f877eab39ae2496795feb327436a44d9450ce2781b071`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d91c98424c5722a91cb12e54ca5c7af9f12c034b801df540e013a52df8e938`  
		Last Modified: Tue, 04 Jul 2023 15:00:09 GMT  
		Size: 171.5 MB (171511899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493841186da8cc28dcd3542f3c5e48f6853b465d5389b8a2e595292fe4acfa57`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656ccdb00e6c88095176998c459e8fbff2585a38ed2a7781a7812e457b3abe9a`  
		Last Modified: Tue, 04 Jul 2023 15:00:26 GMT  
		Size: 45.2 MB (45204441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cbde3a0d7e6e385474cc8f84e37c7ddb2ac72700849e7e7a586690a0a29efb`  
		Last Modified: Tue, 04 Jul 2023 15:00:21 GMT  
		Size: 302.7 KB (302677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a52ffd06935d7fffa1923572f179f9d9aa8e0661022b715746f72ad0673679`  
		Last Modified: Tue, 04 Jul 2023 15:00:30 GMT  
		Size: 72.0 MB (71970399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:b03f16f088bfe16a6b43bd7c7c8214b05699862024e59a594d9cee594441af43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:1f2a7d8e59ee5906b1f79b47f293d7458421a6e59561edfa0de0bb678caf0c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343210185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a98bb7bca647203e46bd29f1e0ab661837100a39f9c592d05459e376a040883`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:38:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:38:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:40:36 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:40:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:40:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:41:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:41:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:42:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff84dd75ab0363da2809c202391ffc2d59534b4888fb855bfd3e21fba17c6fc`  
		Last Modified: Tue, 04 Jul 2023 20:06:54 GMT  
		Size: 1.2 MB (1198708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564b5c67648727c462a4c2ba9d04cdbfa852b527efa36e4c6a859b58454f1c06`  
		Last Modified: Tue, 04 Jul 2023 20:06:53 GMT  
		Size: 5.6 MB (5553847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d18d779d6732554da8eb52855df2ccfe7921f00655dffb89550af33715f184`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5d180dd93ee0210935b93b72cc533ed3b35e05a47dc0b20fb5b5b9884e4c3`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac36e4a2604385d7a84264dc122ac61dd1af8f304d486fc983703238a0d02333`  
		Last Modified: Tue, 04 Jul 2023 20:07:19 GMT  
		Size: 177.0 MB (177027946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca272865f67e094abd7a450c446c31552297e72292785448cac9df1ac6bdcd1`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2c2048f289191c959ae1bde0b76c4c37af804966f66c4599e4745a47810cad`  
		Last Modified: Tue, 04 Jul 2023 20:07:35 GMT  
		Size: 50.9 MB (50939858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ad18f9d687633622e84262935b3873354dcf6c1ce6c32d67568aa7f9c351f`  
		Last Modified: Tue, 04 Jul 2023 20:07:28 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9b129af37cdd180a7f4bb7fc69172d71d5bbc7c2e1eb95896ae3fa7a973fe`  
		Last Modified: Tue, 04 Jul 2023 20:07:39 GMT  
		Size: 79.6 MB (79604734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:44d4f5184dee8e1470cef26eb31aaca402a607f556ef3dcfd6695610f10c6d9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289311711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a824034ce70955715c5ad01653744c4c3a0330ad7419be72d21b1dbeb702391`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:51:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:52:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:55:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:55:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:55:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 19:57:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae4844234b1655ffcc66de6ff4d8fb9d8dc5b263579abf1c0f08fc45c10b`  
		Last Modified: Tue, 04 Jul 2023 20:06:37 GMT  
		Size: 1.2 MB (1198714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f870418e12b4135248455da61f5521096265e859ed7df1641c96d8052c1cd1ed`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 4.7 MB (4679197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37cb4cc4c6e905769f0ad1f740744e276e496b07b5efc7e4dcfd333e303892`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e584269a8e1f1afb39b1c87e053140430bf059f1a78c8091f862a0a6d7ce9d0`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f17c57312bea1c2c36a5f0b529de68ac63f57144e4e7911f2bfbdaa007f1cc2`  
		Last Modified: Tue, 04 Jul 2023 20:07:03 GMT  
		Size: 157.5 MB (157543123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb0493e0b9da981ce0cd0c9aeab054329b78efe17d28f3a208cfe95f617a1`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ec7ad778d705ac798c8c4e72ac5e0a3d97e71bf31fb07dc28dc1c7dbfde0b`  
		Last Modified: Tue, 04 Jul 2023 20:07:17 GMT  
		Size: 40.5 MB (40503772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4463c21fd1b24a56ceff0c21678439984b89244a4de1cebf2ca5d1e4fe6f6c`  
		Last Modified: Tue, 04 Jul 2023 20:07:12 GMT  
		Size: 302.7 KB (302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825a9d60f2d0bb1d7c24f20b6232803e0cae89bbd590ec88ddcddd9186193f1a`  
		Last Modified: Tue, 04 Jul 2023 20:07:21 GMT  
		Size: 60.5 MB (60493692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f131f36e81dbf42293146b1fa7d86be2ee41013c608e68efa1d355d1fc805f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322922029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f675169c509f89573c15272afd2e0826150be2d161f7dd7286baeab5042ef6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 14:25:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 14:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:28:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 14:28:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:28:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:29:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:29:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:30:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdd39b6ea2b9a0ce173cf2e1f26322497d5a9c7710030e37439ad5d4b2523`  
		Last Modified: Tue, 04 Jul 2023 14:59:38 GMT  
		Size: 1.2 MB (1199222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb204de59b70d94654e7760fc586c55bcd195218315dbf7589d66289510f275`  
		Last Modified: Tue, 04 Jul 2023 14:59:36 GMT  
		Size: 5.5 MB (5532648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74969841e6f58cb9e0f0a3c29463b5877ac9e57c3ce30bfcf3c1a6f5d74b6e`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed7a86bfb6803f03f9f877eab39ae2496795feb327436a44d9450ce2781b071`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d91c98424c5722a91cb12e54ca5c7af9f12c034b801df540e013a52df8e938`  
		Last Modified: Tue, 04 Jul 2023 15:00:09 GMT  
		Size: 171.5 MB (171511899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493841186da8cc28dcd3542f3c5e48f6853b465d5389b8a2e595292fe4acfa57`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656ccdb00e6c88095176998c459e8fbff2585a38ed2a7781a7812e457b3abe9a`  
		Last Modified: Tue, 04 Jul 2023 15:00:26 GMT  
		Size: 45.2 MB (45204441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cbde3a0d7e6e385474cc8f84e37c7ddb2ac72700849e7e7a586690a0a29efb`  
		Last Modified: Tue, 04 Jul 2023 15:00:21 GMT  
		Size: 302.7 KB (302677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a52ffd06935d7fffa1923572f179f9d9aa8e0661022b715746f72ad0673679`  
		Last Modified: Tue, 04 Jul 2023 15:00:30 GMT  
		Size: 72.0 MB (71970399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:71e696e9c52fdd2c59491ec41255aef1bef838699c6785bc49fd3e481f15da5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:ba314e83e1140e38b730ded90897ff4abf9920a365aa66f67bf4442263ae7407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212362926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c8e3327cb9948f69b0783b7a885aed24c0a9895e05b7e7b560ef3a8d1e4d64`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:38:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:38:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:40:36 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:40:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:40:36 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff84dd75ab0363da2809c202391ffc2d59534b4888fb855bfd3e21fba17c6fc`  
		Last Modified: Tue, 04 Jul 2023 20:06:54 GMT  
		Size: 1.2 MB (1198708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564b5c67648727c462a4c2ba9d04cdbfa852b527efa36e4c6a859b58454f1c06`  
		Last Modified: Tue, 04 Jul 2023 20:06:53 GMT  
		Size: 5.6 MB (5553847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d18d779d6732554da8eb52855df2ccfe7921f00655dffb89550af33715f184`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5d180dd93ee0210935b93b72cc533ed3b35e05a47dc0b20fb5b5b9884e4c3`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac36e4a2604385d7a84264dc122ac61dd1af8f304d486fc983703238a0d02333`  
		Last Modified: Tue, 04 Jul 2023 20:07:19 GMT  
		Size: 177.0 MB (177027946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca272865f67e094abd7a450c446c31552297e72292785448cac9df1ac6bdcd1`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:8a5ac73d28a505b16a86f3e7185d0c1434c7dbf19ba486945d55d589316b5333
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (188011580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67480a9eb0025f587eae298a084f3ebb439aa33830002554ff9936d59bdc8b7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:51:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:52:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:55:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:55:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae4844234b1655ffcc66de6ff4d8fb9d8dc5b263579abf1c0f08fc45c10b`  
		Last Modified: Tue, 04 Jul 2023 20:06:37 GMT  
		Size: 1.2 MB (1198714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f870418e12b4135248455da61f5521096265e859ed7df1641c96d8052c1cd1ed`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 4.7 MB (4679197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37cb4cc4c6e905769f0ad1f740744e276e496b07b5efc7e4dcfd333e303892`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e584269a8e1f1afb39b1c87e053140430bf059f1a78c8091f862a0a6d7ce9d0`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f17c57312bea1c2c36a5f0b529de68ac63f57144e4e7911f2bfbdaa007f1cc2`  
		Last Modified: Tue, 04 Jul 2023 20:07:03 GMT  
		Size: 157.5 MB (157543123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb0493e0b9da981ce0cd0c9aeab054329b78efe17d28f3a208cfe95f617a1`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7ff2832f5f3e621f73dbcd5a6e456fff5357b32bf2fd4b34b4e787a916a64699
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205444512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80bbc889db53a10a59ced385cf734a2ce98caaddc375c3a77706af3c76283cf8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 14:25:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 14:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:28:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 14:28:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:28:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdd39b6ea2b9a0ce173cf2e1f26322497d5a9c7710030e37439ad5d4b2523`  
		Last Modified: Tue, 04 Jul 2023 14:59:38 GMT  
		Size: 1.2 MB (1199222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb204de59b70d94654e7760fc586c55bcd195218315dbf7589d66289510f275`  
		Last Modified: Tue, 04 Jul 2023 14:59:36 GMT  
		Size: 5.5 MB (5532648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74969841e6f58cb9e0f0a3c29463b5877ac9e57c3ce30bfcf3c1a6f5d74b6e`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed7a86bfb6803f03f9f877eab39ae2496795feb327436a44d9450ce2781b071`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d91c98424c5722a91cb12e54ca5c7af9f12c034b801df540e013a52df8e938`  
		Last Modified: Tue, 04 Jul 2023 15:00:09 GMT  
		Size: 171.5 MB (171511899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493841186da8cc28dcd3542f3c5e48f6853b465d5389b8a2e595292fe4acfa57`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:71e696e9c52fdd2c59491ec41255aef1bef838699c6785bc49fd3e481f15da5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:ba314e83e1140e38b730ded90897ff4abf9920a365aa66f67bf4442263ae7407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212362926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c8e3327cb9948f69b0783b7a885aed24c0a9895e05b7e7b560ef3a8d1e4d64`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:38:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:38:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:38:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:38:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:40:36 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:40:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:40:36 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff84dd75ab0363da2809c202391ffc2d59534b4888fb855bfd3e21fba17c6fc`  
		Last Modified: Tue, 04 Jul 2023 20:06:54 GMT  
		Size: 1.2 MB (1198708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564b5c67648727c462a4c2ba9d04cdbfa852b527efa36e4c6a859b58454f1c06`  
		Last Modified: Tue, 04 Jul 2023 20:06:53 GMT  
		Size: 5.6 MB (5553847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d18d779d6732554da8eb52855df2ccfe7921f00655dffb89550af33715f184`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5d180dd93ee0210935b93b72cc533ed3b35e05a47dc0b20fb5b5b9884e4c3`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac36e4a2604385d7a84264dc122ac61dd1af8f304d486fc983703238a0d02333`  
		Last Modified: Tue, 04 Jul 2023 20:07:19 GMT  
		Size: 177.0 MB (177027946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca272865f67e094abd7a450c446c31552297e72292785448cac9df1ac6bdcd1`  
		Last Modified: Tue, 04 Jul 2023 20:06:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:8a5ac73d28a505b16a86f3e7185d0c1434c7dbf19ba486945d55d589316b5333
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (188011580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67480a9eb0025f587eae298a084f3ebb439aa33830002554ff9936d59bdc8b7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:51:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:52:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 19:52:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 19:52:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 19:55:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 19:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 19:55:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae4844234b1655ffcc66de6ff4d8fb9d8dc5b263579abf1c0f08fc45c10b`  
		Last Modified: Tue, 04 Jul 2023 20:06:37 GMT  
		Size: 1.2 MB (1198714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f870418e12b4135248455da61f5521096265e859ed7df1641c96d8052c1cd1ed`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 4.7 MB (4679197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37cb4cc4c6e905769f0ad1f740744e276e496b07b5efc7e4dcfd333e303892`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e584269a8e1f1afb39b1c87e053140430bf059f1a78c8091f862a0a6d7ce9d0`  
		Last Modified: Tue, 04 Jul 2023 20:06:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f17c57312bea1c2c36a5f0b529de68ac63f57144e4e7911f2bfbdaa007f1cc2`  
		Last Modified: Tue, 04 Jul 2023 20:07:03 GMT  
		Size: 157.5 MB (157543123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb0493e0b9da981ce0cd0c9aeab054329b78efe17d28f3a208cfe95f617a1`  
		Last Modified: Tue, 04 Jul 2023 20:06:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7ff2832f5f3e621f73dbcd5a6e456fff5357b32bf2fd4b34b4e787a916a64699
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205444512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80bbc889db53a10a59ced385cf734a2ce98caaddc375c3a77706af3c76283cf8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:25:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Jul 2023 14:25:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:25:42 GMT
ENV ROS_DISTRO=noetic
# Tue, 04 Jul 2023 14:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:28:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 04 Jul 2023 14:28:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:28:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdd39b6ea2b9a0ce173cf2e1f26322497d5a9c7710030e37439ad5d4b2523`  
		Last Modified: Tue, 04 Jul 2023 14:59:38 GMT  
		Size: 1.2 MB (1199222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb204de59b70d94654e7760fc586c55bcd195218315dbf7589d66289510f275`  
		Last Modified: Tue, 04 Jul 2023 14:59:36 GMT  
		Size: 5.5 MB (5532648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74969841e6f58cb9e0f0a3c29463b5877ac9e57c3ce30bfcf3c1a6f5d74b6e`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed7a86bfb6803f03f9f877eab39ae2496795feb327436a44d9450ce2781b071`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d91c98424c5722a91cb12e54ca5c7af9f12c034b801df540e013a52df8e938`  
		Last Modified: Tue, 04 Jul 2023 15:00:09 GMT  
		Size: 171.5 MB (171511899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493841186da8cc28dcd3542f3c5e48f6853b465d5389b8a2e595292fe4acfa57`  
		Last Modified: Tue, 04 Jul 2023 14:59:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:7745519dae7786d284d0b3552837c30a0e9afd6768d827a0d93b37756dd6b56f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:10ba291dc0ba9e7d80bdd8dc2c6e5b75b9d3b7921a04cd9decc06fa24ae02481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268621992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06ecd9b25343291ebc10de5b11c044e8298b5d7caca26d6e99fc5f615705ea6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 20:02:59 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 20:03:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:03:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:03:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:03:41 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 20:04:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:04:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 20:04:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 20:04:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f56d27fecf4e210a05a82e8866e65c93e56a1c334d05dc920874efb491bc42`  
		Last Modified: Tue, 04 Jul 2023 20:14:32 GMT  
		Size: 124.2 MB (124153171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1dfb64b9fd9711f9b089a583e356a45f3db3501069df5009532484efb69ee77`  
		Last Modified: Tue, 04 Jul 2023 20:14:13 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecc8a7939fc2509dd255cb3900f371842f82522c2324050f42a217867f39fd2`  
		Last Modified: Tue, 04 Jul 2023 20:14:51 GMT  
		Size: 85.0 MB (84994763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34a0e75a6de1feb7201f461d07ea0bbbc2255a4efa547ab968d5b49fc018f6`  
		Last Modified: Tue, 04 Jul 2023 20:14:40 GMT  
		Size: 290.5 KB (290460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b8a9ac31ed4b14680802a41bf298d370d9a39a1f7942dcc8292beaaa4d200`  
		Last Modified: Tue, 04 Jul 2023 20:14:40 GMT  
		Size: 2.4 KB (2411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93d908b21c5425c4862d4f88c4cf270ae4c5b11118f7f286f07595d9e4b6ca`  
		Last Modified: Tue, 04 Jul 2023 20:14:44 GMT  
		Size: 23.7 MB (23705649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:92b6a5001e47ae5066362bce6cf0c75cdaaa1c17bea7f899d81fd829fb12c7f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261190693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba98e4afa86a5d08fa70e2208765b1d52e3da8f382a4fc0fdae491d3cc88d7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:55:51 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 14:56:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:56:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:56:31 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:56:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:56:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:57:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934fe752a2ee51b5ee65e779e62c11b4d010de2627c22aad530bf339442254a3`  
		Last Modified: Tue, 04 Jul 2023 15:06:40 GMT  
		Size: 121.6 MB (121646630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b74a8b78fc888acf5353ade379044a3c4401d9cfa1a8a627099e7abc5aeb5`  
		Last Modified: Tue, 04 Jul 2023 15:06:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e7693b7f950c38c41729372425390b0d1c18a939a4f7f8768692d2758b6595`  
		Last Modified: Tue, 04 Jul 2023 15:06:56 GMT  
		Size: 82.7 MB (82737126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe56d8305f1e6ac0120f77b665376bfd0ac33a7a7ade6224b2fe24a936488c1d`  
		Last Modified: Tue, 04 Jul 2023 15:06:49 GMT  
		Size: 290.5 KB (290464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42311ceca794a942ff2ced664bbdadeb8b91734e8c4cdc435ae480583b4a6701`  
		Last Modified: Tue, 04 Jul 2023 15:06:48 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f1ff2859eb8f182e0bac366d6ea3420a7f0f5201b0b28d1fb04ac1494fba49`  
		Last Modified: Tue, 04 Jul 2023 15:06:52 GMT  
		Size: 23.1 MB (23103969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:ade7c92eb6c387dc3ae3aed84296b18f2ce80864066ed6402d942a3cedc04d24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:753fb2d607a0957b322b96f7dae9e829e03fd653b6bbe21f9864cd197237df67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **958.4 MB (958400960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741e5b2b653e13ba8ec5903f9374a3275f0fcb99808da4279779ffd48dad008d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 20:02:59 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 20:03:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:03:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:03:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:03:41 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 20:04:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:04:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 20:04:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 20:04:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:05:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f56d27fecf4e210a05a82e8866e65c93e56a1c334d05dc920874efb491bc42`  
		Last Modified: Tue, 04 Jul 2023 20:14:32 GMT  
		Size: 124.2 MB (124153171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1dfb64b9fd9711f9b089a583e356a45f3db3501069df5009532484efb69ee77`  
		Last Modified: Tue, 04 Jul 2023 20:14:13 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecc8a7939fc2509dd255cb3900f371842f82522c2324050f42a217867f39fd2`  
		Last Modified: Tue, 04 Jul 2023 20:14:51 GMT  
		Size: 85.0 MB (84994763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34a0e75a6de1feb7201f461d07ea0bbbc2255a4efa547ab968d5b49fc018f6`  
		Last Modified: Tue, 04 Jul 2023 20:14:40 GMT  
		Size: 290.5 KB (290460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b8a9ac31ed4b14680802a41bf298d370d9a39a1f7942dcc8292beaaa4d200`  
		Last Modified: Tue, 04 Jul 2023 20:14:40 GMT  
		Size: 2.4 KB (2411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93d908b21c5425c4862d4f88c4cf270ae4c5b11118f7f286f07595d9e4b6ca`  
		Last Modified: Tue, 04 Jul 2023 20:14:44 GMT  
		Size: 23.7 MB (23705649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b042871bb7ac7cfd7dbeb91d80a45cc60535f75e42242d951d3659e04050a8`  
		Last Modified: Tue, 04 Jul 2023 20:16:28 GMT  
		Size: 689.8 MB (689778968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:440b2e1ae39e542f3dd2006379c5b79e0ab034a17f13295d454257a146b247ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **919.6 MB (919642068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a7dcd9962d3477e88c1e72280d545b984819889e98fcc34e449b96e13b49b96`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:55:51 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 14:56:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:56:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:56:31 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:56:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:56:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:57:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:58:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934fe752a2ee51b5ee65e779e62c11b4d010de2627c22aad530bf339442254a3`  
		Last Modified: Tue, 04 Jul 2023 15:06:40 GMT  
		Size: 121.6 MB (121646630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b74a8b78fc888acf5353ade379044a3c4401d9cfa1a8a627099e7abc5aeb5`  
		Last Modified: Tue, 04 Jul 2023 15:06:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e7693b7f950c38c41729372425390b0d1c18a939a4f7f8768692d2758b6595`  
		Last Modified: Tue, 04 Jul 2023 15:06:56 GMT  
		Size: 82.7 MB (82737126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe56d8305f1e6ac0120f77b665376bfd0ac33a7a7ade6224b2fe24a936488c1d`  
		Last Modified: Tue, 04 Jul 2023 15:06:49 GMT  
		Size: 290.5 KB (290464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42311ceca794a942ff2ced664bbdadeb8b91734e8c4cdc435ae480583b4a6701`  
		Last Modified: Tue, 04 Jul 2023 15:06:48 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f1ff2859eb8f182e0bac366d6ea3420a7f0f5201b0b28d1fb04ac1494fba49`  
		Last Modified: Tue, 04 Jul 2023 15:06:52 GMT  
		Size: 23.1 MB (23103969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729edef3394ea93bfc75ca193de39f3c96cbed3257052b3d7ded2f550c5cfd1c`  
		Last Modified: Tue, 04 Jul 2023 15:08:10 GMT  
		Size: 658.5 MB (658451375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:ade7c92eb6c387dc3ae3aed84296b18f2ce80864066ed6402d942a3cedc04d24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:753fb2d607a0957b322b96f7dae9e829e03fd653b6bbe21f9864cd197237df67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **958.4 MB (958400960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741e5b2b653e13ba8ec5903f9374a3275f0fcb99808da4279779ffd48dad008d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 20:02:59 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 20:03:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:03:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:03:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:03:41 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 20:04:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:04:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 20:04:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 20:04:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:05:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f56d27fecf4e210a05a82e8866e65c93e56a1c334d05dc920874efb491bc42`  
		Last Modified: Tue, 04 Jul 2023 20:14:32 GMT  
		Size: 124.2 MB (124153171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1dfb64b9fd9711f9b089a583e356a45f3db3501069df5009532484efb69ee77`  
		Last Modified: Tue, 04 Jul 2023 20:14:13 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecc8a7939fc2509dd255cb3900f371842f82522c2324050f42a217867f39fd2`  
		Last Modified: Tue, 04 Jul 2023 20:14:51 GMT  
		Size: 85.0 MB (84994763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34a0e75a6de1feb7201f461d07ea0bbbc2255a4efa547ab968d5b49fc018f6`  
		Last Modified: Tue, 04 Jul 2023 20:14:40 GMT  
		Size: 290.5 KB (290460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b8a9ac31ed4b14680802a41bf298d370d9a39a1f7942dcc8292beaaa4d200`  
		Last Modified: Tue, 04 Jul 2023 20:14:40 GMT  
		Size: 2.4 KB (2411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93d908b21c5425c4862d4f88c4cf270ae4c5b11118f7f286f07595d9e4b6ca`  
		Last Modified: Tue, 04 Jul 2023 20:14:44 GMT  
		Size: 23.7 MB (23705649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b042871bb7ac7cfd7dbeb91d80a45cc60535f75e42242d951d3659e04050a8`  
		Last Modified: Tue, 04 Jul 2023 20:16:28 GMT  
		Size: 689.8 MB (689778968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:440b2e1ae39e542f3dd2006379c5b79e0ab034a17f13295d454257a146b247ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **919.6 MB (919642068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a7dcd9962d3477e88c1e72280d545b984819889e98fcc34e449b96e13b49b96`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:55:51 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 14:56:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:56:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:56:31 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:56:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:56:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:57:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:58:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934fe752a2ee51b5ee65e779e62c11b4d010de2627c22aad530bf339442254a3`  
		Last Modified: Tue, 04 Jul 2023 15:06:40 GMT  
		Size: 121.6 MB (121646630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b74a8b78fc888acf5353ade379044a3c4401d9cfa1a8a627099e7abc5aeb5`  
		Last Modified: Tue, 04 Jul 2023 15:06:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e7693b7f950c38c41729372425390b0d1c18a939a4f7f8768692d2758b6595`  
		Last Modified: Tue, 04 Jul 2023 15:06:56 GMT  
		Size: 82.7 MB (82737126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe56d8305f1e6ac0120f77b665376bfd0ac33a7a7ade6224b2fe24a936488c1d`  
		Last Modified: Tue, 04 Jul 2023 15:06:49 GMT  
		Size: 290.5 KB (290464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42311ceca794a942ff2ced664bbdadeb8b91734e8c4cdc435ae480583b4a6701`  
		Last Modified: Tue, 04 Jul 2023 15:06:48 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f1ff2859eb8f182e0bac366d6ea3420a7f0f5201b0b28d1fb04ac1494fba49`  
		Last Modified: Tue, 04 Jul 2023 15:06:52 GMT  
		Size: 23.1 MB (23103969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729edef3394ea93bfc75ca193de39f3c96cbed3257052b3d7ded2f550c5cfd1c`  
		Last Modified: Tue, 04 Jul 2023 15:08:10 GMT  
		Size: 658.5 MB (658451375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:7745519dae7786d284d0b3552837c30a0e9afd6768d827a0d93b37756dd6b56f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:10ba291dc0ba9e7d80bdd8dc2c6e5b75b9d3b7921a04cd9decc06fa24ae02481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268621992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06ecd9b25343291ebc10de5b11c044e8298b5d7caca26d6e99fc5f615705ea6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 20:02:59 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 20:03:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:03:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:03:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:03:41 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 20:04:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:04:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 20:04:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 20:04:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f56d27fecf4e210a05a82e8866e65c93e56a1c334d05dc920874efb491bc42`  
		Last Modified: Tue, 04 Jul 2023 20:14:32 GMT  
		Size: 124.2 MB (124153171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1dfb64b9fd9711f9b089a583e356a45f3db3501069df5009532484efb69ee77`  
		Last Modified: Tue, 04 Jul 2023 20:14:13 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecc8a7939fc2509dd255cb3900f371842f82522c2324050f42a217867f39fd2`  
		Last Modified: Tue, 04 Jul 2023 20:14:51 GMT  
		Size: 85.0 MB (84994763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34a0e75a6de1feb7201f461d07ea0bbbc2255a4efa547ab968d5b49fc018f6`  
		Last Modified: Tue, 04 Jul 2023 20:14:40 GMT  
		Size: 290.5 KB (290460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b8a9ac31ed4b14680802a41bf298d370d9a39a1f7942dcc8292beaaa4d200`  
		Last Modified: Tue, 04 Jul 2023 20:14:40 GMT  
		Size: 2.4 KB (2411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93d908b21c5425c4862d4f88c4cf270ae4c5b11118f7f286f07595d9e4b6ca`  
		Last Modified: Tue, 04 Jul 2023 20:14:44 GMT  
		Size: 23.7 MB (23705649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:92b6a5001e47ae5066362bce6cf0c75cdaaa1c17bea7f899d81fd829fb12c7f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261190693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba98e4afa86a5d08fa70e2208765b1d52e3da8f382a4fc0fdae491d3cc88d7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:55:51 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 14:56:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:56:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:56:31 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:56:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:56:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:57:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934fe752a2ee51b5ee65e779e62c11b4d010de2627c22aad530bf339442254a3`  
		Last Modified: Tue, 04 Jul 2023 15:06:40 GMT  
		Size: 121.6 MB (121646630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b74a8b78fc888acf5353ade379044a3c4401d9cfa1a8a627099e7abc5aeb5`  
		Last Modified: Tue, 04 Jul 2023 15:06:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e7693b7f950c38c41729372425390b0d1c18a939a4f7f8768692d2758b6595`  
		Last Modified: Tue, 04 Jul 2023 15:06:56 GMT  
		Size: 82.7 MB (82737126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe56d8305f1e6ac0120f77b665376bfd0ac33a7a7ade6224b2fe24a936488c1d`  
		Last Modified: Tue, 04 Jul 2023 15:06:49 GMT  
		Size: 290.5 KB (290464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42311ceca794a942ff2ced664bbdadeb8b91734e8c4cdc435ae480583b4a6701`  
		Last Modified: Tue, 04 Jul 2023 15:06:48 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f1ff2859eb8f182e0bac366d6ea3420a7f0f5201b0b28d1fb04ac1494fba49`  
		Last Modified: Tue, 04 Jul 2023 15:06:52 GMT  
		Size: 23.1 MB (23103969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:7745519dae7786d284d0b3552837c30a0e9afd6768d827a0d93b37756dd6b56f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:10ba291dc0ba9e7d80bdd8dc2c6e5b75b9d3b7921a04cd9decc06fa24ae02481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268621992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06ecd9b25343291ebc10de5b11c044e8298b5d7caca26d6e99fc5f615705ea6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 20:02:59 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 20:03:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:03:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:03:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:03:41 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 20:04:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:04:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 20:04:10 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 20:04:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f56d27fecf4e210a05a82e8866e65c93e56a1c334d05dc920874efb491bc42`  
		Last Modified: Tue, 04 Jul 2023 20:14:32 GMT  
		Size: 124.2 MB (124153171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1dfb64b9fd9711f9b089a583e356a45f3db3501069df5009532484efb69ee77`  
		Last Modified: Tue, 04 Jul 2023 20:14:13 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecc8a7939fc2509dd255cb3900f371842f82522c2324050f42a217867f39fd2`  
		Last Modified: Tue, 04 Jul 2023 20:14:51 GMT  
		Size: 85.0 MB (84994763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34a0e75a6de1feb7201f461d07ea0bbbc2255a4efa547ab968d5b49fc018f6`  
		Last Modified: Tue, 04 Jul 2023 20:14:40 GMT  
		Size: 290.5 KB (290460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b8a9ac31ed4b14680802a41bf298d370d9a39a1f7942dcc8292beaaa4d200`  
		Last Modified: Tue, 04 Jul 2023 20:14:40 GMT  
		Size: 2.4 KB (2411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93d908b21c5425c4862d4f88c4cf270ae4c5b11118f7f286f07595d9e4b6ca`  
		Last Modified: Tue, 04 Jul 2023 20:14:44 GMT  
		Size: 23.7 MB (23705649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:92b6a5001e47ae5066362bce6cf0c75cdaaa1c17bea7f899d81fd829fb12c7f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261190693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba98e4afa86a5d08fa70e2208765b1d52e3da8f382a4fc0fdae491d3cc88d7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:55:51 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 14:56:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:56:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:56:31 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:56:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Jul 2023 14:56:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 04 Jul 2023 14:57:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934fe752a2ee51b5ee65e779e62c11b4d010de2627c22aad530bf339442254a3`  
		Last Modified: Tue, 04 Jul 2023 15:06:40 GMT  
		Size: 121.6 MB (121646630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b74a8b78fc888acf5353ade379044a3c4401d9cfa1a8a627099e7abc5aeb5`  
		Last Modified: Tue, 04 Jul 2023 15:06:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e7693b7f950c38c41729372425390b0d1c18a939a4f7f8768692d2758b6595`  
		Last Modified: Tue, 04 Jul 2023 15:06:56 GMT  
		Size: 82.7 MB (82737126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe56d8305f1e6ac0120f77b665376bfd0ac33a7a7ade6224b2fe24a936488c1d`  
		Last Modified: Tue, 04 Jul 2023 15:06:49 GMT  
		Size: 290.5 KB (290464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42311ceca794a942ff2ced664bbdadeb8b91734e8c4cdc435ae480583b4a6701`  
		Last Modified: Tue, 04 Jul 2023 15:06:48 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f1ff2859eb8f182e0bac366d6ea3420a7f0f5201b0b28d1fb04ac1494fba49`  
		Last Modified: Tue, 04 Jul 2023 15:06:52 GMT  
		Size: 23.1 MB (23103969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:91f0fc0f0fe28bfc385f3ed095584f969dbd87ecd6e38c1e95414765f457a819
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:39522d03bb05bfa53c0a19441acde188f907f622430592a2b05fd2c07df54403
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159628709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:761854bf5e6c928cb47d4c22abd10851d45873226e4a6b73f7e4902604c1cbf0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 20:02:59 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 20:03:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:03:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:03:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:03:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f56d27fecf4e210a05a82e8866e65c93e56a1c334d05dc920874efb491bc42`  
		Last Modified: Tue, 04 Jul 2023 20:14:32 GMT  
		Size: 124.2 MB (124153171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1dfb64b9fd9711f9b089a583e356a45f3db3501069df5009532484efb69ee77`  
		Last Modified: Tue, 04 Jul 2023 20:14:13 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3139be75c60244b5914fad42f4a5c55a1ac1ec10cb7f3ef6eee31b85a6e58010
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155056729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f2df171e0df624ebc39de30c178efe5227b50521936005e768e6a644542d64`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:55:51 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 14:56:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:56:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:56:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934fe752a2ee51b5ee65e779e62c11b4d010de2627c22aad530bf339442254a3`  
		Last Modified: Tue, 04 Jul 2023 15:06:40 GMT  
		Size: 121.6 MB (121646630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b74a8b78fc888acf5353ade379044a3c4401d9cfa1a8a627099e7abc5aeb5`  
		Last Modified: Tue, 04 Jul 2023 15:06:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:91f0fc0f0fe28bfc385f3ed095584f969dbd87ecd6e38c1e95414765f457a819
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:39522d03bb05bfa53c0a19441acde188f907f622430592a2b05fd2c07df54403
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159628709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:761854bf5e6c928cb47d4c22abd10851d45873226e4a6b73f7e4902604c1cbf0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 19:48:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:48:30 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 19:48:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 19:48:31 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 20:02:59 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 20:03:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:03:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 20:03:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 20:03:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96b181e03e7c00f9ff313a35cb309648ea7a63a12165e78d4298df8d842ef7`  
		Last Modified: Tue, 04 Jul 2023 20:09:20 GMT  
		Size: 1.2 MB (1213029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981b99f5f99f37d026fe791185912ef266fd67d841915968d7f58e1e21aa67dd`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 3.8 MB (3828864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457911032da59063f35f0ed9962d1f7235ab9b54c6a1b2434538945c43049d6d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca97964148324558ddeb21e9e1395cff5cbcb0443e2d4b59209fa6930ea226d`  
		Last Modified: Tue, 04 Jul 2023 20:09:18 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f56d27fecf4e210a05a82e8866e65c93e56a1c334d05dc920874efb491bc42`  
		Last Modified: Tue, 04 Jul 2023 20:14:32 GMT  
		Size: 124.2 MB (124153171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1dfb64b9fd9711f9b089a583e356a45f3db3501069df5009532484efb69ee77`  
		Last Modified: Tue, 04 Jul 2023 20:14:13 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3139be75c60244b5914fad42f4a5c55a1ac1ec10cb7f3ef6eee31b85a6e58010
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155056729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f2df171e0df624ebc39de30c178efe5227b50521936005e768e6a644542d64`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 14:39:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:39:32 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 04 Jul 2023 14:39:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 14:39:33 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Jul 2023 14:55:51 GMT
ENV ROS_DISTRO=rolling
# Tue, 04 Jul 2023 14:56:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:56:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 04 Jul 2023 14:56:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Jul 2023 14:56:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00229127f6e92c07e3d74389e863ed6853d2d18643b36b4305c0618bd0dde009`  
		Last Modified: Tue, 04 Jul 2023 15:02:02 GMT  
		Size: 1.2 MB (1214643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b203d955e7643d1bb7ec9891155ddb1401e9f8ef11e41eff2ea80a7477a1e4a2`  
		Last Modified: Tue, 04 Jul 2023 15:02:00 GMT  
		Size: 3.8 MB (3802027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c278f102957a8f2e4cef72c46fb72240db242ec7800b4e9f3660cdd59adb5d`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b369fa41d7f7a70ee18742f04da6ab36f01e9331cd686a3fc0d10f2a61df1ee`  
		Last Modified: Tue, 04 Jul 2023 15:01:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934fe752a2ee51b5ee65e779e62c11b4d010de2627c22aad530bf339442254a3`  
		Last Modified: Tue, 04 Jul 2023 15:06:40 GMT  
		Size: 121.6 MB (121646630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b74a8b78fc888acf5353ade379044a3c4401d9cfa1a8a627099e7abc5aeb5`  
		Last Modified: Tue, 04 Jul 2023 15:06:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
