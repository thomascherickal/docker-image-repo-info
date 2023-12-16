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
$ docker pull ros@sha256:90a2bba0c4008b24af489c729dc115eb0f094a4a7f97cf333aa68f9b8271b35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:00df27c44f83df6b27929e288381a300fccebadb55f02b6eddd8d47a1f39cd6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263474247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb855e9e7de7153ab4103e4bd4a1f3de2e51d5245af438addfe31f2e58eb8b20`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV ROS_DISTRO=humble
# Sat, 16 Dec 2023 09:48:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:48:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:48:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:48:22 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:49:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:49:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:49:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0ada8eb3ba4a4057bc136cc32ea1f9a40e1c3ce15dc63ba7b8c1d87f3a449`  
		Last Modified: Sat, 16 Dec 2023 10:07:50 GMT  
		Size: 106.4 MB (106425342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc4959e4ffab0d786c8a79e468f578e3810ba04c29171142974dc6eeaf47bce`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbfa1641c52f0f728bba612f70365bfbe31e5e1e70f74a3da7ed281ac21b5dd`  
		Last Modified: Sat, 16 Dec 2023 10:08:11 GMT  
		Size: 98.1 MB (98136973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a0420a620c13d502d8b84dac17c204f62403a8079773f8ed7eafa235d2a58`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 323.4 KB (323394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bceebb0a375312bdfb2177224bd933aa418b30299fe0ba54523d7228ffd7b8`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1fcfdc609174103028d12137fcacc10be9728649bf6d915ecd99eeb7bf259c`  
		Last Modified: Sat, 16 Dec 2023 10:08:02 GMT  
		Size: 23.1 MB (23095030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:de1983ea5424eb4eb7903d98ecc37421c1571bfb301c31c7e5c32b84ef27cbce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.2 MB (260185844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57235b0c751cf3b9aba7268ea8957084cea7be37731ba2d42f95d36272d91a94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:26:36 GMT
ENV ROS_DISTRO=humble
# Sat, 09 Dec 2023 03:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:28:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:28:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:28:47 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:29:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:29:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:30:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b431d8ff0eb473b1137123064337f774d9aae332a19ccf882a8780ff625d3e1`  
		Last Modified: Sat, 09 Dec 2023 04:08:02 GMT  
		Size: 108.2 MB (108238005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d360bc38d9b031e1ad1d941031d69c999289a3900d4a42aa89f530e507a28`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afbb351522278b6221470c49633619563770f9ac32723b7426ef621b144d170`  
		Last Modified: Sat, 09 Dec 2023 04:08:21 GMT  
		Size: 95.7 MB (95685333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3277393afa9d7a18aa86507b31b2e73fe3851938b051fb7514560bf46a9474f`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 323.3 KB (323260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904013a6a366b4cb788296626c5b768722fddfd246dcee0499304c21be8746df`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181892b7b86035dde3759f459ed3d391c902e80c66a201aac137444e68354cb9`  
		Last Modified: Sat, 09 Dec 2023 04:08:14 GMT  
		Size: 22.5 MB (22518192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:0bca12a965cdb20a8f04cf9d32d1d4ca904ea4047b28ae9fe0d2b5093a137b83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:d83f6a1bfc4ddc4e7e767ea5d3bc426c8fd520d4f13d8913cda03980dc8c0c8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **953.7 MB (953708433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0911782e12dd334370f1c03cb88cbbf4fb22e07c0f3e1e65e4fd3dfd49537a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV ROS_DISTRO=humble
# Sat, 16 Dec 2023 09:48:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:48:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:48:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:48:22 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:49:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:49:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:49:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:57:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0ada8eb3ba4a4057bc136cc32ea1f9a40e1c3ce15dc63ba7b8c1d87f3a449`  
		Last Modified: Sat, 16 Dec 2023 10:07:50 GMT  
		Size: 106.4 MB (106425342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc4959e4ffab0d786c8a79e468f578e3810ba04c29171142974dc6eeaf47bce`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbfa1641c52f0f728bba612f70365bfbe31e5e1e70f74a3da7ed281ac21b5dd`  
		Last Modified: Sat, 16 Dec 2023 10:08:11 GMT  
		Size: 98.1 MB (98136973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a0420a620c13d502d8b84dac17c204f62403a8079773f8ed7eafa235d2a58`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 323.4 KB (323394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bceebb0a375312bdfb2177224bd933aa418b30299fe0ba54523d7228ffd7b8`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1fcfdc609174103028d12137fcacc10be9728649bf6d915ecd99eeb7bf259c`  
		Last Modified: Sat, 16 Dec 2023 10:08:02 GMT  
		Size: 23.1 MB (23095030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41442fbad611a9661e94fcd8b2476246700199dd7da44557d911e0c4e4d90b3`  
		Last Modified: Sat, 16 Dec 2023 10:09:50 GMT  
		Size: 690.2 MB (690234186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a3990d3f430df5c1718043c1eefaaaaca47ab8bbd4fb52b9d34d69a53d8e33ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **918.3 MB (918290480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fea49a3b4fdff979b0d928cf3d32e614dd14e4538c19f4f7722658671a2ecb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:26:36 GMT
ENV ROS_DISTRO=humble
# Sat, 09 Dec 2023 03:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:28:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:28:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:28:47 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:29:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:29:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:30:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:41:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b431d8ff0eb473b1137123064337f774d9aae332a19ccf882a8780ff625d3e1`  
		Last Modified: Sat, 09 Dec 2023 04:08:02 GMT  
		Size: 108.2 MB (108238005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d360bc38d9b031e1ad1d941031d69c999289a3900d4a42aa89f530e507a28`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afbb351522278b6221470c49633619563770f9ac32723b7426ef621b144d170`  
		Last Modified: Sat, 09 Dec 2023 04:08:21 GMT  
		Size: 95.7 MB (95685333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3277393afa9d7a18aa86507b31b2e73fe3851938b051fb7514560bf46a9474f`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 323.3 KB (323260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904013a6a366b4cb788296626c5b768722fddfd246dcee0499304c21be8746df`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181892b7b86035dde3759f459ed3d391c902e80c66a201aac137444e68354cb9`  
		Last Modified: Sat, 09 Dec 2023 04:08:14 GMT  
		Size: 22.5 MB (22518192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0940f5e9b67d91c10113b7284a5b17b1ead4ae0b9a0413ee409f79a87310e8db`  
		Last Modified: Sat, 09 Dec 2023 04:10:00 GMT  
		Size: 658.1 MB (658104636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:0bca12a965cdb20a8f04cf9d32d1d4ca904ea4047b28ae9fe0d2b5093a137b83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:d83f6a1bfc4ddc4e7e767ea5d3bc426c8fd520d4f13d8913cda03980dc8c0c8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **953.7 MB (953708433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0911782e12dd334370f1c03cb88cbbf4fb22e07c0f3e1e65e4fd3dfd49537a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV ROS_DISTRO=humble
# Sat, 16 Dec 2023 09:48:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:48:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:48:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:48:22 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:49:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:49:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:49:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:57:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0ada8eb3ba4a4057bc136cc32ea1f9a40e1c3ce15dc63ba7b8c1d87f3a449`  
		Last Modified: Sat, 16 Dec 2023 10:07:50 GMT  
		Size: 106.4 MB (106425342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc4959e4ffab0d786c8a79e468f578e3810ba04c29171142974dc6eeaf47bce`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbfa1641c52f0f728bba612f70365bfbe31e5e1e70f74a3da7ed281ac21b5dd`  
		Last Modified: Sat, 16 Dec 2023 10:08:11 GMT  
		Size: 98.1 MB (98136973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a0420a620c13d502d8b84dac17c204f62403a8079773f8ed7eafa235d2a58`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 323.4 KB (323394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bceebb0a375312bdfb2177224bd933aa418b30299fe0ba54523d7228ffd7b8`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1fcfdc609174103028d12137fcacc10be9728649bf6d915ecd99eeb7bf259c`  
		Last Modified: Sat, 16 Dec 2023 10:08:02 GMT  
		Size: 23.1 MB (23095030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41442fbad611a9661e94fcd8b2476246700199dd7da44557d911e0c4e4d90b3`  
		Last Modified: Sat, 16 Dec 2023 10:09:50 GMT  
		Size: 690.2 MB (690234186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a3990d3f430df5c1718043c1eefaaaaca47ab8bbd4fb52b9d34d69a53d8e33ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **918.3 MB (918290480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fea49a3b4fdff979b0d928cf3d32e614dd14e4538c19f4f7722658671a2ecb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:26:36 GMT
ENV ROS_DISTRO=humble
# Sat, 09 Dec 2023 03:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:28:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:28:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:28:47 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:29:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:29:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:30:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:41:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b431d8ff0eb473b1137123064337f774d9aae332a19ccf882a8780ff625d3e1`  
		Last Modified: Sat, 09 Dec 2023 04:08:02 GMT  
		Size: 108.2 MB (108238005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d360bc38d9b031e1ad1d941031d69c999289a3900d4a42aa89f530e507a28`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afbb351522278b6221470c49633619563770f9ac32723b7426ef621b144d170`  
		Last Modified: Sat, 09 Dec 2023 04:08:21 GMT  
		Size: 95.7 MB (95685333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3277393afa9d7a18aa86507b31b2e73fe3851938b051fb7514560bf46a9474f`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 323.3 KB (323260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904013a6a366b4cb788296626c5b768722fddfd246dcee0499304c21be8746df`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181892b7b86035dde3759f459ed3d391c902e80c66a201aac137444e68354cb9`  
		Last Modified: Sat, 09 Dec 2023 04:08:14 GMT  
		Size: 22.5 MB (22518192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0940f5e9b67d91c10113b7284a5b17b1ead4ae0b9a0413ee409f79a87310e8db`  
		Last Modified: Sat, 09 Dec 2023 04:10:00 GMT  
		Size: 658.1 MB (658104636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:90a2bba0c4008b24af489c729dc115eb0f094a4a7f97cf333aa68f9b8271b35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:00df27c44f83df6b27929e288381a300fccebadb55f02b6eddd8d47a1f39cd6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263474247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb855e9e7de7153ab4103e4bd4a1f3de2e51d5245af438addfe31f2e58eb8b20`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV ROS_DISTRO=humble
# Sat, 16 Dec 2023 09:48:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:48:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:48:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:48:22 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:49:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:49:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:49:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0ada8eb3ba4a4057bc136cc32ea1f9a40e1c3ce15dc63ba7b8c1d87f3a449`  
		Last Modified: Sat, 16 Dec 2023 10:07:50 GMT  
		Size: 106.4 MB (106425342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc4959e4ffab0d786c8a79e468f578e3810ba04c29171142974dc6eeaf47bce`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbfa1641c52f0f728bba612f70365bfbe31e5e1e70f74a3da7ed281ac21b5dd`  
		Last Modified: Sat, 16 Dec 2023 10:08:11 GMT  
		Size: 98.1 MB (98136973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a0420a620c13d502d8b84dac17c204f62403a8079773f8ed7eafa235d2a58`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 323.4 KB (323394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bceebb0a375312bdfb2177224bd933aa418b30299fe0ba54523d7228ffd7b8`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1fcfdc609174103028d12137fcacc10be9728649bf6d915ecd99eeb7bf259c`  
		Last Modified: Sat, 16 Dec 2023 10:08:02 GMT  
		Size: 23.1 MB (23095030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:de1983ea5424eb4eb7903d98ecc37421c1571bfb301c31c7e5c32b84ef27cbce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.2 MB (260185844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57235b0c751cf3b9aba7268ea8957084cea7be37731ba2d42f95d36272d91a94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:26:36 GMT
ENV ROS_DISTRO=humble
# Sat, 09 Dec 2023 03:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:28:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:28:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:28:47 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:29:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:29:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:30:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b431d8ff0eb473b1137123064337f774d9aae332a19ccf882a8780ff625d3e1`  
		Last Modified: Sat, 09 Dec 2023 04:08:02 GMT  
		Size: 108.2 MB (108238005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d360bc38d9b031e1ad1d941031d69c999289a3900d4a42aa89f530e507a28`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afbb351522278b6221470c49633619563770f9ac32723b7426ef621b144d170`  
		Last Modified: Sat, 09 Dec 2023 04:08:21 GMT  
		Size: 95.7 MB (95685333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3277393afa9d7a18aa86507b31b2e73fe3851938b051fb7514560bf46a9474f`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 323.3 KB (323260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904013a6a366b4cb788296626c5b768722fddfd246dcee0499304c21be8746df`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181892b7b86035dde3759f459ed3d391c902e80c66a201aac137444e68354cb9`  
		Last Modified: Sat, 09 Dec 2023 04:08:14 GMT  
		Size: 22.5 MB (22518192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:90a2bba0c4008b24af489c729dc115eb0f094a4a7f97cf333aa68f9b8271b35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:00df27c44f83df6b27929e288381a300fccebadb55f02b6eddd8d47a1f39cd6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263474247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb855e9e7de7153ab4103e4bd4a1f3de2e51d5245af438addfe31f2e58eb8b20`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV ROS_DISTRO=humble
# Sat, 16 Dec 2023 09:48:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:48:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:48:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:48:22 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:49:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:49:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:49:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0ada8eb3ba4a4057bc136cc32ea1f9a40e1c3ce15dc63ba7b8c1d87f3a449`  
		Last Modified: Sat, 16 Dec 2023 10:07:50 GMT  
		Size: 106.4 MB (106425342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc4959e4ffab0d786c8a79e468f578e3810ba04c29171142974dc6eeaf47bce`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbfa1641c52f0f728bba612f70365bfbe31e5e1e70f74a3da7ed281ac21b5dd`  
		Last Modified: Sat, 16 Dec 2023 10:08:11 GMT  
		Size: 98.1 MB (98136973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a0420a620c13d502d8b84dac17c204f62403a8079773f8ed7eafa235d2a58`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 323.4 KB (323394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bceebb0a375312bdfb2177224bd933aa418b30299fe0ba54523d7228ffd7b8`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1fcfdc609174103028d12137fcacc10be9728649bf6d915ecd99eeb7bf259c`  
		Last Modified: Sat, 16 Dec 2023 10:08:02 GMT  
		Size: 23.1 MB (23095030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:de1983ea5424eb4eb7903d98ecc37421c1571bfb301c31c7e5c32b84ef27cbce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.2 MB (260185844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57235b0c751cf3b9aba7268ea8957084cea7be37731ba2d42f95d36272d91a94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:26:36 GMT
ENV ROS_DISTRO=humble
# Sat, 09 Dec 2023 03:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:28:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:28:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:28:47 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:29:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:29:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:30:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b431d8ff0eb473b1137123064337f774d9aae332a19ccf882a8780ff625d3e1`  
		Last Modified: Sat, 09 Dec 2023 04:08:02 GMT  
		Size: 108.2 MB (108238005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d360bc38d9b031e1ad1d941031d69c999289a3900d4a42aa89f530e507a28`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afbb351522278b6221470c49633619563770f9ac32723b7426ef621b144d170`  
		Last Modified: Sat, 09 Dec 2023 04:08:21 GMT  
		Size: 95.7 MB (95685333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3277393afa9d7a18aa86507b31b2e73fe3851938b051fb7514560bf46a9474f`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 323.3 KB (323260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904013a6a366b4cb788296626c5b768722fddfd246dcee0499304c21be8746df`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181892b7b86035dde3759f459ed3d391c902e80c66a201aac137444e68354cb9`  
		Last Modified: Sat, 09 Dec 2023 04:08:14 GMT  
		Size: 22.5 MB (22518192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:85acc9b2d264e57148dfa9612203d23ee02c1a7104c89edd112a935103d9eddf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:4b0bf2aae792e10ab700885269336aedbf893369865c40bb9f5b5c29b1b8b6fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141916393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dca6335b9188d38011cfaafc4ef5cbf0c7d48fd87cfb99446fa736cfe78fd991`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV ROS_DISTRO=humble
# Sat, 16 Dec 2023 09:48:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:48:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:48:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:48:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0ada8eb3ba4a4057bc136cc32ea1f9a40e1c3ce15dc63ba7b8c1d87f3a449`  
		Last Modified: Sat, 16 Dec 2023 10:07:50 GMT  
		Size: 106.4 MB (106425342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc4959e4ffab0d786c8a79e468f578e3810ba04c29171142974dc6eeaf47bce`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f62233550c2e06ab04666b1dfd7db6938eb5d67a836e3099afa1d94b12bdc150
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141656615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:747ebf74e4133b747aa436247a07440c6b7cca911584c4a01838727b652bd5ff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:26:36 GMT
ENV ROS_DISTRO=humble
# Sat, 09 Dec 2023 03:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:28:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:28:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:28:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b431d8ff0eb473b1137123064337f774d9aae332a19ccf882a8780ff625d3e1`  
		Last Modified: Sat, 09 Dec 2023 04:08:02 GMT  
		Size: 108.2 MB (108238005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d360bc38d9b031e1ad1d941031d69c999289a3900d4a42aa89f530e507a28`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:85acc9b2d264e57148dfa9612203d23ee02c1a7104c89edd112a935103d9eddf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:4b0bf2aae792e10ab700885269336aedbf893369865c40bb9f5b5c29b1b8b6fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141916393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dca6335b9188d38011cfaafc4ef5cbf0c7d48fd87cfb99446fa736cfe78fd991`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV ROS_DISTRO=humble
# Sat, 16 Dec 2023 09:48:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:48:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:48:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:48:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0ada8eb3ba4a4057bc136cc32ea1f9a40e1c3ce15dc63ba7b8c1d87f3a449`  
		Last Modified: Sat, 16 Dec 2023 10:07:50 GMT  
		Size: 106.4 MB (106425342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc4959e4ffab0d786c8a79e468f578e3810ba04c29171142974dc6eeaf47bce`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f62233550c2e06ab04666b1dfd7db6938eb5d67a836e3099afa1d94b12bdc150
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141656615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:747ebf74e4133b747aa436247a07440c6b7cca911584c4a01838727b652bd5ff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:26:36 GMT
ENV ROS_DISTRO=humble
# Sat, 09 Dec 2023 03:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:28:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:28:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:28:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b431d8ff0eb473b1137123064337f774d9aae332a19ccf882a8780ff625d3e1`  
		Last Modified: Sat, 09 Dec 2023 04:08:02 GMT  
		Size: 108.2 MB (108238005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d360bc38d9b031e1ad1d941031d69c999289a3900d4a42aa89f530e507a28`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron`

```console
$ docker pull ros@sha256:b0f2c04604fc90041b366d63d61c9266965cfd8c2ffbcadade785fc5f5a766a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron` - linux; amd64

```console
$ docker pull ros@sha256:7aba4e8557bece1bd7aaa8198b696c3a8881d7c467558d52c2e55294b650920c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.9 MB (268913981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb0f08b7399eee8dd8099a22355a12503df5805e530ba2d3e1aa358e354d798d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:57:38 GMT
ENV ROS_DISTRO=iron
# Sat, 16 Dec 2023 09:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:58:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:58:24 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:58:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:59:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06099ce56fcd99234533185f080ddf22e93ad779de2bf9f7beb9279f25ba7b1c`  
		Last Modified: Sat, 16 Dec 2023 10:10:18 GMT  
		Size: 124.2 MB (124210600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155efc7cb124d559757658cd6d76b6182a3db6d72e54c71976acaa758b6a7585`  
		Last Modified: Sat, 16 Dec 2023 10:09:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4a40dddb0bee6467345aa781b5fb8366bbfbdf8894179f22d2679c94c45c6a`  
		Last Modified: Sat, 16 Dec 2023 10:10:37 GMT  
		Size: 85.2 MB (85168507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b047eea6c49b7300964d5e5711df092f29f4f6ef54c9e4335ca993e47bae7875`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 308.8 KB (308838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b1f6bd3d7020613a1a62f7efe6a2010043b1600b6a5d741c6a5b83bc74b81a`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6eb861d9d15bcceecc4139716116c4ee9613074610f98a0ca183f6742e78ab5`  
		Last Modified: Sat, 16 Dec 2023 10:10:30 GMT  
		Size: 23.7 MB (23732538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f41991f67c6a3760c47857cdf7e628645ac7c9088ce0d1817f9a178fb9e8f6b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.5 MB (265470838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7b06231fb1bc6cc4cce828feb4661ccb0c0d337ae9723c4348009a1b66c320`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:41:12 GMT
ENV ROS_DISTRO=iron
# Sat, 09 Dec 2023 03:41:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:41:59 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:41:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:41:59 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:42:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:42:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:42:30 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222d7b3d268ded32b4ad650aed79d9be00a2b0e19c7e5496ef45d7e09430adf9`  
		Last Modified: Sat, 09 Dec 2023 04:10:34 GMT  
		Size: 125.8 MB (125775913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff428714d458caf501343d9a10a1540511c77e1808e726cb2b39cf5b725871a`  
		Last Modified: Sat, 09 Dec 2023 04:10:09 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12195a3969755cede1841333ad86c88205d160a792081abbe6eb597be1513882`  
		Last Modified: Sat, 09 Dec 2023 04:10:51 GMT  
		Size: 82.8 MB (82845353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd78deb6203197c2d6b1b64486c1f43e4082daea5b1dddb08d735e9b118d401`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 308.7 KB (308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fd95dc58fecd704a011c00b89936ba693fa704fcae6c6d66ccd85d0fe88931`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198c81f08313430c71a7721ea05a6ecb30d03552e69d14c08e92d7903cf86e8`  
		Last Modified: Sat, 09 Dec 2023 04:10:46 GMT  
		Size: 23.1 MB (23119813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-perception`

```console
$ docker pull ros@sha256:bcd36bae7318f3436acb69eac6a8743115921a7f462d3b4ac898a5e08d88d1e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-perception` - linux; amd64

```console
$ docker pull ros@sha256:e926a73e3f0405ff83c056b15e47288986bc8b1d0e6ab66d0ed8a015bdf7c52b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.9 MB (959858189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:721af958086dac84e13f416af1405bb2d2c12371212513c33e113c714d749d94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:57:38 GMT
ENV ROS_DISTRO=iron
# Sat, 16 Dec 2023 09:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:58:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:58:24 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:58:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:59:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:00:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06099ce56fcd99234533185f080ddf22e93ad779de2bf9f7beb9279f25ba7b1c`  
		Last Modified: Sat, 16 Dec 2023 10:10:18 GMT  
		Size: 124.2 MB (124210600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155efc7cb124d559757658cd6d76b6182a3db6d72e54c71976acaa758b6a7585`  
		Last Modified: Sat, 16 Dec 2023 10:09:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4a40dddb0bee6467345aa781b5fb8366bbfbdf8894179f22d2679c94c45c6a`  
		Last Modified: Sat, 16 Dec 2023 10:10:37 GMT  
		Size: 85.2 MB (85168507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b047eea6c49b7300964d5e5711df092f29f4f6ef54c9e4335ca993e47bae7875`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 308.8 KB (308838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b1f6bd3d7020613a1a62f7efe6a2010043b1600b6a5d741c6a5b83bc74b81a`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6eb861d9d15bcceecc4139716116c4ee9613074610f98a0ca183f6742e78ab5`  
		Last Modified: Sat, 16 Dec 2023 10:10:30 GMT  
		Size: 23.7 MB (23732538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec15ff624c6c9d63e9cc9d0e4c73890c1222f51715f61c93fdc99ea23781359f`  
		Last Modified: Sat, 16 Dec 2023 10:12:14 GMT  
		Size: 690.9 MB (690944208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ece6680e424bb2f3c17e92b7edb69414132e89970e13bd9bba3468bab29d2744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **924.2 MB (924202619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2449f31b251d4a948ed05d90617ed5f465198917f9da8309a31ed9c165bbff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:41:12 GMT
ENV ROS_DISTRO=iron
# Sat, 09 Dec 2023 03:41:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:41:59 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:41:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:41:59 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:42:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:42:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:42:30 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:44:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222d7b3d268ded32b4ad650aed79d9be00a2b0e19c7e5496ef45d7e09430adf9`  
		Last Modified: Sat, 09 Dec 2023 04:10:34 GMT  
		Size: 125.8 MB (125775913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff428714d458caf501343d9a10a1540511c77e1808e726cb2b39cf5b725871a`  
		Last Modified: Sat, 09 Dec 2023 04:10:09 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12195a3969755cede1841333ad86c88205d160a792081abbe6eb597be1513882`  
		Last Modified: Sat, 09 Dec 2023 04:10:51 GMT  
		Size: 82.8 MB (82845353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd78deb6203197c2d6b1b64486c1f43e4082daea5b1dddb08d735e9b118d401`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 308.7 KB (308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fd95dc58fecd704a011c00b89936ba693fa704fcae6c6d66ccd85d0fe88931`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198c81f08313430c71a7721ea05a6ecb30d03552e69d14c08e92d7903cf86e8`  
		Last Modified: Sat, 09 Dec 2023 04:10:46 GMT  
		Size: 23.1 MB (23119813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43178b7bb093094c03a37ce41185b297031fdac6e082a8b2f3dfa1ee3ba911b1`  
		Last Modified: Sat, 09 Dec 2023 04:12:25 GMT  
		Size: 658.7 MB (658731781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-perception-jammy`

```console
$ docker pull ros@sha256:bcd36bae7318f3436acb69eac6a8743115921a7f462d3b4ac898a5e08d88d1e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:e926a73e3f0405ff83c056b15e47288986bc8b1d0e6ab66d0ed8a015bdf7c52b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.9 MB (959858189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:721af958086dac84e13f416af1405bb2d2c12371212513c33e113c714d749d94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:57:38 GMT
ENV ROS_DISTRO=iron
# Sat, 16 Dec 2023 09:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:58:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:58:24 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:58:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:59:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:00:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06099ce56fcd99234533185f080ddf22e93ad779de2bf9f7beb9279f25ba7b1c`  
		Last Modified: Sat, 16 Dec 2023 10:10:18 GMT  
		Size: 124.2 MB (124210600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155efc7cb124d559757658cd6d76b6182a3db6d72e54c71976acaa758b6a7585`  
		Last Modified: Sat, 16 Dec 2023 10:09:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4a40dddb0bee6467345aa781b5fb8366bbfbdf8894179f22d2679c94c45c6a`  
		Last Modified: Sat, 16 Dec 2023 10:10:37 GMT  
		Size: 85.2 MB (85168507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b047eea6c49b7300964d5e5711df092f29f4f6ef54c9e4335ca993e47bae7875`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 308.8 KB (308838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b1f6bd3d7020613a1a62f7efe6a2010043b1600b6a5d741c6a5b83bc74b81a`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6eb861d9d15bcceecc4139716116c4ee9613074610f98a0ca183f6742e78ab5`  
		Last Modified: Sat, 16 Dec 2023 10:10:30 GMT  
		Size: 23.7 MB (23732538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec15ff624c6c9d63e9cc9d0e4c73890c1222f51715f61c93fdc99ea23781359f`  
		Last Modified: Sat, 16 Dec 2023 10:12:14 GMT  
		Size: 690.9 MB (690944208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ece6680e424bb2f3c17e92b7edb69414132e89970e13bd9bba3468bab29d2744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **924.2 MB (924202619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2449f31b251d4a948ed05d90617ed5f465198917f9da8309a31ed9c165bbff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:41:12 GMT
ENV ROS_DISTRO=iron
# Sat, 09 Dec 2023 03:41:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:41:59 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:41:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:41:59 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:42:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:42:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:42:30 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:44:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222d7b3d268ded32b4ad650aed79d9be00a2b0e19c7e5496ef45d7e09430adf9`  
		Last Modified: Sat, 09 Dec 2023 04:10:34 GMT  
		Size: 125.8 MB (125775913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff428714d458caf501343d9a10a1540511c77e1808e726cb2b39cf5b725871a`  
		Last Modified: Sat, 09 Dec 2023 04:10:09 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12195a3969755cede1841333ad86c88205d160a792081abbe6eb597be1513882`  
		Last Modified: Sat, 09 Dec 2023 04:10:51 GMT  
		Size: 82.8 MB (82845353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd78deb6203197c2d6b1b64486c1f43e4082daea5b1dddb08d735e9b118d401`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 308.7 KB (308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fd95dc58fecd704a011c00b89936ba693fa704fcae6c6d66ccd85d0fe88931`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198c81f08313430c71a7721ea05a6ecb30d03552e69d14c08e92d7903cf86e8`  
		Last Modified: Sat, 09 Dec 2023 04:10:46 GMT  
		Size: 23.1 MB (23119813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43178b7bb093094c03a37ce41185b297031fdac6e082a8b2f3dfa1ee3ba911b1`  
		Last Modified: Sat, 09 Dec 2023 04:12:25 GMT  
		Size: 658.7 MB (658731781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-base`

```console
$ docker pull ros@sha256:b0f2c04604fc90041b366d63d61c9266965cfd8c2ffbcadade785fc5f5a766a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:7aba4e8557bece1bd7aaa8198b696c3a8881d7c467558d52c2e55294b650920c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.9 MB (268913981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb0f08b7399eee8dd8099a22355a12503df5805e530ba2d3e1aa358e354d798d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:57:38 GMT
ENV ROS_DISTRO=iron
# Sat, 16 Dec 2023 09:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:58:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:58:24 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:58:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:59:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06099ce56fcd99234533185f080ddf22e93ad779de2bf9f7beb9279f25ba7b1c`  
		Last Modified: Sat, 16 Dec 2023 10:10:18 GMT  
		Size: 124.2 MB (124210600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155efc7cb124d559757658cd6d76b6182a3db6d72e54c71976acaa758b6a7585`  
		Last Modified: Sat, 16 Dec 2023 10:09:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4a40dddb0bee6467345aa781b5fb8366bbfbdf8894179f22d2679c94c45c6a`  
		Last Modified: Sat, 16 Dec 2023 10:10:37 GMT  
		Size: 85.2 MB (85168507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b047eea6c49b7300964d5e5711df092f29f4f6ef54c9e4335ca993e47bae7875`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 308.8 KB (308838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b1f6bd3d7020613a1a62f7efe6a2010043b1600b6a5d741c6a5b83bc74b81a`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6eb861d9d15bcceecc4139716116c4ee9613074610f98a0ca183f6742e78ab5`  
		Last Modified: Sat, 16 Dec 2023 10:10:30 GMT  
		Size: 23.7 MB (23732538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f41991f67c6a3760c47857cdf7e628645ac7c9088ce0d1817f9a178fb9e8f6b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.5 MB (265470838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7b06231fb1bc6cc4cce828feb4661ccb0c0d337ae9723c4348009a1b66c320`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:41:12 GMT
ENV ROS_DISTRO=iron
# Sat, 09 Dec 2023 03:41:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:41:59 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:41:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:41:59 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:42:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:42:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:42:30 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222d7b3d268ded32b4ad650aed79d9be00a2b0e19c7e5496ef45d7e09430adf9`  
		Last Modified: Sat, 09 Dec 2023 04:10:34 GMT  
		Size: 125.8 MB (125775913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff428714d458caf501343d9a10a1540511c77e1808e726cb2b39cf5b725871a`  
		Last Modified: Sat, 09 Dec 2023 04:10:09 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12195a3969755cede1841333ad86c88205d160a792081abbe6eb597be1513882`  
		Last Modified: Sat, 09 Dec 2023 04:10:51 GMT  
		Size: 82.8 MB (82845353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd78deb6203197c2d6b1b64486c1f43e4082daea5b1dddb08d735e9b118d401`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 308.7 KB (308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fd95dc58fecd704a011c00b89936ba693fa704fcae6c6d66ccd85d0fe88931`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198c81f08313430c71a7721ea05a6ecb30d03552e69d14c08e92d7903cf86e8`  
		Last Modified: Sat, 09 Dec 2023 04:10:46 GMT  
		Size: 23.1 MB (23119813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-base-jammy`

```console
$ docker pull ros@sha256:b0f2c04604fc90041b366d63d61c9266965cfd8c2ffbcadade785fc5f5a766a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:7aba4e8557bece1bd7aaa8198b696c3a8881d7c467558d52c2e55294b650920c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.9 MB (268913981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb0f08b7399eee8dd8099a22355a12503df5805e530ba2d3e1aa358e354d798d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:57:38 GMT
ENV ROS_DISTRO=iron
# Sat, 16 Dec 2023 09:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:58:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:58:24 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:58:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:59:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06099ce56fcd99234533185f080ddf22e93ad779de2bf9f7beb9279f25ba7b1c`  
		Last Modified: Sat, 16 Dec 2023 10:10:18 GMT  
		Size: 124.2 MB (124210600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155efc7cb124d559757658cd6d76b6182a3db6d72e54c71976acaa758b6a7585`  
		Last Modified: Sat, 16 Dec 2023 10:09:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4a40dddb0bee6467345aa781b5fb8366bbfbdf8894179f22d2679c94c45c6a`  
		Last Modified: Sat, 16 Dec 2023 10:10:37 GMT  
		Size: 85.2 MB (85168507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b047eea6c49b7300964d5e5711df092f29f4f6ef54c9e4335ca993e47bae7875`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 308.8 KB (308838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b1f6bd3d7020613a1a62f7efe6a2010043b1600b6a5d741c6a5b83bc74b81a`  
		Last Modified: Sat, 16 Dec 2023 10:10:26 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6eb861d9d15bcceecc4139716116c4ee9613074610f98a0ca183f6742e78ab5`  
		Last Modified: Sat, 16 Dec 2023 10:10:30 GMT  
		Size: 23.7 MB (23732538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f41991f67c6a3760c47857cdf7e628645ac7c9088ce0d1817f9a178fb9e8f6b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.5 MB (265470838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7b06231fb1bc6cc4cce828feb4661ccb0c0d337ae9723c4348009a1b66c320`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:41:12 GMT
ENV ROS_DISTRO=iron
# Sat, 09 Dec 2023 03:41:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:41:59 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:41:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:41:59 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:42:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:42:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:42:30 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:42:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222d7b3d268ded32b4ad650aed79d9be00a2b0e19c7e5496ef45d7e09430adf9`  
		Last Modified: Sat, 09 Dec 2023 04:10:34 GMT  
		Size: 125.8 MB (125775913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff428714d458caf501343d9a10a1540511c77e1808e726cb2b39cf5b725871a`  
		Last Modified: Sat, 09 Dec 2023 04:10:09 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12195a3969755cede1841333ad86c88205d160a792081abbe6eb597be1513882`  
		Last Modified: Sat, 09 Dec 2023 04:10:51 GMT  
		Size: 82.8 MB (82845353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd78deb6203197c2d6b1b64486c1f43e4082daea5b1dddb08d735e9b118d401`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 308.7 KB (308706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fd95dc58fecd704a011c00b89936ba693fa704fcae6c6d66ccd85d0fe88931`  
		Last Modified: Sat, 09 Dec 2023 04:10:42 GMT  
		Size: 2.4 KB (2442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198c81f08313430c71a7721ea05a6ecb30d03552e69d14c08e92d7903cf86e8`  
		Last Modified: Sat, 09 Dec 2023 04:10:46 GMT  
		Size: 23.1 MB (23119813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-core`

```console
$ docker pull ros@sha256:c5cce7ef12e45c20c4c2169958ecec5b5a641a1ee6d3250c3c8123f58a1283ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:2ce385edde40d9eabb8bfc6cd6ef43ef571ab544436efb80de667b5566c25fe7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.7 MB (159701651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8978306e2023f7e9d29582f066b293820590a67ff16aa429f9ac19d44902c75`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:57:38 GMT
ENV ROS_DISTRO=iron
# Sat, 16 Dec 2023 09:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:58:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:58:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06099ce56fcd99234533185f080ddf22e93ad779de2bf9f7beb9279f25ba7b1c`  
		Last Modified: Sat, 16 Dec 2023 10:10:18 GMT  
		Size: 124.2 MB (124210600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155efc7cb124d559757658cd6d76b6182a3db6d72e54c71976acaa758b6a7585`  
		Last Modified: Sat, 16 Dec 2023 10:09:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e6d5ef02575c92051c76329a99ee4201db4f2600c9f62d466aa4bb189544e07f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.2 MB (159194524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81629202ca594d1384cefff5fb5b23dd9ec54b4da1e052462b56ba27832c6d10`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:41:12 GMT
ENV ROS_DISTRO=iron
# Sat, 09 Dec 2023 03:41:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:41:59 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:41:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:41:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222d7b3d268ded32b4ad650aed79d9be00a2b0e19c7e5496ef45d7e09430adf9`  
		Last Modified: Sat, 09 Dec 2023 04:10:34 GMT  
		Size: 125.8 MB (125775913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff428714d458caf501343d9a10a1540511c77e1808e726cb2b39cf5b725871a`  
		Last Modified: Sat, 09 Dec 2023 04:10:09 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-core-jammy`

```console
$ docker pull ros@sha256:c5cce7ef12e45c20c4c2169958ecec5b5a641a1ee6d3250c3c8123f58a1283ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:2ce385edde40d9eabb8bfc6cd6ef43ef571ab544436efb80de667b5566c25fe7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.7 MB (159701651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8978306e2023f7e9d29582f066b293820590a67ff16aa429f9ac19d44902c75`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:57:38 GMT
ENV ROS_DISTRO=iron
# Sat, 16 Dec 2023 09:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:58:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:58:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:58:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06099ce56fcd99234533185f080ddf22e93ad779de2bf9f7beb9279f25ba7b1c`  
		Last Modified: Sat, 16 Dec 2023 10:10:18 GMT  
		Size: 124.2 MB (124210600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155efc7cb124d559757658cd6d76b6182a3db6d72e54c71976acaa758b6a7585`  
		Last Modified: Sat, 16 Dec 2023 10:09:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e6d5ef02575c92051c76329a99ee4201db4f2600c9f62d466aa4bb189544e07f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.2 MB (159194524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81629202ca594d1384cefff5fb5b23dd9ec54b4da1e052462b56ba27832c6d10`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:41:12 GMT
ENV ROS_DISTRO=iron
# Sat, 09 Dec 2023 03:41:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:41:59 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:41:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:41:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222d7b3d268ded32b4ad650aed79d9be00a2b0e19c7e5496ef45d7e09430adf9`  
		Last Modified: Sat, 09 Dec 2023 04:10:34 GMT  
		Size: 125.8 MB (125775913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff428714d458caf501343d9a10a1540511c77e1808e726cb2b39cf5b725871a`  
		Last Modified: Sat, 09 Dec 2023 04:10:09 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:90a2bba0c4008b24af489c729dc115eb0f094a4a7f97cf333aa68f9b8271b35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:00df27c44f83df6b27929e288381a300fccebadb55f02b6eddd8d47a1f39cd6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263474247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb855e9e7de7153ab4103e4bd4a1f3de2e51d5245af438addfe31f2e58eb8b20`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV ROS_DISTRO=humble
# Sat, 16 Dec 2023 09:48:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:48:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 09:48:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:48:22 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:49:23 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:49:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 09:49:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0ada8eb3ba4a4057bc136cc32ea1f9a40e1c3ce15dc63ba7b8c1d87f3a449`  
		Last Modified: Sat, 16 Dec 2023 10:07:50 GMT  
		Size: 106.4 MB (106425342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc4959e4ffab0d786c8a79e468f578e3810ba04c29171142974dc6eeaf47bce`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbfa1641c52f0f728bba612f70365bfbe31e5e1e70f74a3da7ed281ac21b5dd`  
		Last Modified: Sat, 16 Dec 2023 10:08:11 GMT  
		Size: 98.1 MB (98136973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a0420a620c13d502d8b84dac17c204f62403a8079773f8ed7eafa235d2a58`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 323.4 KB (323394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bceebb0a375312bdfb2177224bd933aa418b30299fe0ba54523d7228ffd7b8`  
		Last Modified: Sat, 16 Dec 2023 10:07:58 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1fcfdc609174103028d12137fcacc10be9728649bf6d915ecd99eeb7bf259c`  
		Last Modified: Sat, 16 Dec 2023 10:08:02 GMT  
		Size: 23.1 MB (23095030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:de1983ea5424eb4eb7903d98ecc37421c1571bfb301c31c7e5c32b84ef27cbce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.2 MB (260185844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57235b0c751cf3b9aba7268ea8957084cea7be37731ba2d42f95d36272d91a94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:26:36 GMT
ENV ROS_DISTRO=humble
# Sat, 09 Dec 2023 03:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:28:47 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:28:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:28:47 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:29:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:29:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:30:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b431d8ff0eb473b1137123064337f774d9aae332a19ccf882a8780ff625d3e1`  
		Last Modified: Sat, 09 Dec 2023 04:08:02 GMT  
		Size: 108.2 MB (108238005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93d360bc38d9b031e1ad1d941031d69c999289a3900d4a42aa89f530e507a28`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afbb351522278b6221470c49633619563770f9ac32723b7426ef621b144d170`  
		Last Modified: Sat, 09 Dec 2023 04:08:21 GMT  
		Size: 95.7 MB (95685333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3277393afa9d7a18aa86507b31b2e73fe3851938b051fb7514560bf46a9474f`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 323.3 KB (323260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904013a6a366b4cb788296626c5b768722fddfd246dcee0499304c21be8746df`  
		Last Modified: Sat, 09 Dec 2023 04:08:10 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181892b7b86035dde3759f459ed3d391c902e80c66a201aac137444e68354cb9`  
		Last Modified: Sat, 09 Dec 2023 04:08:14 GMT  
		Size: 22.5 MB (22518192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:1daa1992f1d29ff18cbe6979d8d1ab6bf6668920d2323c66f516310a91c8152c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:b18ca33cdeee0817fd39b018ddfbd8cc0cb693fbe89211dd3b77b19e7f386adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343170984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a26fadd8116de9bd16b53dffe5995a44be3e31ef87872347bbe08230e877b05c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:35:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:35:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:38:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:38:09 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:38:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:40:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425e951c42dd00ccb058ef6938f79b69db58bf09271ae9462bd5852cfd1353c`  
		Last Modified: Sat, 16 Dec 2023 10:05:10 GMT  
		Size: 1.2 MB (1198846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aba2266c05b2025e53b1daad133978c157924dd56b92b27baac4c2b131ac49`  
		Last Modified: Sat, 16 Dec 2023 10:05:08 GMT  
		Size: 5.6 MB (5553944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da082b0fcdb0e926380c93badeb52429200982b64c2886589a087e11ada6826`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bc03d4300aebd1e01a1bbb2281172eee19cd2e9729ff0035fb2504dc536e32`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307477be25c4a96d631a6b63babb9347b6135862ce19b60048cbff55c280d179`  
		Last Modified: Sat, 16 Dec 2023 10:05:35 GMT  
		Size: 177.0 MB (176962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db26ad757af2ab1db77cea22c3559b1a93d8efa9890510f708a7fe05c28f5fe2`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b296290a0b7485d1f8672c8bd730f9a988374c02b9aa1b44d426683e13463e`  
		Last Modified: Sat, 16 Dec 2023 10:05:52 GMT  
		Size: 50.9 MB (50941170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c97955e78d4b5d35849ebaa6e03664552e66de89a179f90cb181e5682e4cdfa`  
		Last Modified: Sat, 16 Dec 2023 10:05:44 GMT  
		Size: 311.3 KB (311298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8991dddd9b2f661c7710e6ccb2cf128eb8c80547efb3b8a1a3d9252155c0ea81`  
		Last Modified: Sat, 16 Dec 2023 10:05:55 GMT  
		Size: 79.6 MB (79616327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:a6a7e4a94a9f86c92df92c18301a2d2905e8615d7385271787b42edaa4fb84c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289255286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c779c68ac98eec285da4a980fbd6de29582b95d14857068629917b02aebf17b4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:37:05 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:37:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:37:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:37:14 GMT
ADD file:195375389d64193c828c6d3f379c7e35ea85256eb1c51d2bfeab73432ea46064 in / 
# Wed, 13 Dec 2023 10:37:15 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:37:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:37:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:38:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:40:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:40:14 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:40:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba68304511cfd178c72d64196a05b1343fbdbed6093d7b4db0c0d223510c40ab`  
		Last Modified: Sat, 16 Dec 2023 09:27:50 GMT  
		Size: 24.6 MB (24600972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5373ad55d8e8c0ab26bca9b592d8809358e69e59cff53121bcdd908a9f9639c`  
		Last Modified: Sat, 16 Dec 2023 09:50:09 GMT  
		Size: 1.2 MB (1199062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc25b246e660d5421dff1c723cfa2d5dfaa9c2ccfe1976b8fce4d4d1fedc8f5`  
		Last Modified: Sat, 16 Dec 2023 09:50:07 GMT  
		Size: 4.7 MB (4679510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4107a21097c89ac49236bbde53efe45ed4c81f1e01e65c2f0358d02b73486`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70488c95ce2761e3460cec20b973e12284798d5b20d16b9009f4352584dafdc6`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecfe88b9d5bac2517d37b869da63ba8b7baa4f12ca28f6d66809dd278d3b48b`  
		Last Modified: Sat, 16 Dec 2023 09:50:35 GMT  
		Size: 157.5 MB (157458423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b4028622de95be917a19e8013de1c97bde72b70b7382298556d8cf850713e`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2341748b0485b9245a864429765e19ae950f9c356eb506df8d842670477ff2`  
		Last Modified: Sat, 16 Dec 2023 09:50:48 GMT  
		Size: 40.5 MB (40504005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660415962c143fc9e45d4e1c2054c79634e094b208c845bbd583cc003fa989b0`  
		Last Modified: Sat, 16 Dec 2023 09:50:43 GMT  
		Size: 311.3 KB (311302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fd3825c19baab04ff606134bca9de817bb604a6b321072dc1193209a7d4a3`  
		Last Modified: Sat, 16 Dec 2023 09:50:52 GMT  
		Size: 60.5 MB (60499602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b6ba98c10af60c68d092a70a824dd3cc8b25ff52cccf8856918e03c3b471cc5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.0 MB (327042016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fec3efa1ad8e98f48e1c8d6237ae0f7d52ee6da5055a3e76a6fb45ca51abbdbc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:21:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:21:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:37:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 02:37:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV ROS_DISTRO=noetic
# Sat, 09 Dec 2023 02:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:40:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 09 Dec 2023 02:40:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 02:40:42 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 02:41:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:41:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 02:42:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2aa78ed8ad18394d7ae521e83b2810fec9fbb7d95aa074d794bb43e6e2bbfb`  
		Last Modified: Sat, 02 Dec 2023 06:56:12 GMT  
		Size: 1.2 MB (1198781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f106a95fef578814e019c4ac69f1cf32b15d5f85da2729a7ab2487c5d3505d`  
		Last Modified: Sat, 02 Dec 2023 06:56:11 GMT  
		Size: 5.5 MB (5532202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde5587588684db83e0c22fb5d4979df124ea1cb18322ace2e4c3ea5c96b6367`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c5b1b69c1b0400c6d51e9b08a29868443a22bc46ce96467a1b6fd75f9aa2c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c0f3f95aca8df1ff165733b239844d0700cbd97842b1699375b9137cd0075e`  
		Last Modified: Sat, 09 Dec 2023 03:56:30 GMT  
		Size: 175.6 MB (175614595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648bea585de95bdc098b0f496d2c461fc072dda803fe1be92b970893fd65443c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f261b12e1911ed6acc0c610902189f69372d1dbce997eb8ff1ede6dbf9e5ae21`  
		Last Modified: Sat, 09 Dec 2023 03:56:45 GMT  
		Size: 45.2 MB (45206492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92f89f65bd6464334de4ab44489a72c7bb00a4e5286a829f25300f62f3b1f25`  
		Last Modified: Sat, 09 Dec 2023 03:56:39 GMT  
		Size: 311.1 KB (311125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814329a852addc5f898a88b8ca07e7f891f15ddafaa210e9558da08b2bdc5e91`  
		Last Modified: Sat, 09 Dec 2023 03:56:48 GMT  
		Size: 72.0 MB (71972547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:7a2ceeae03b18d4431826e991e50f4679342923721ceee22f9b73c24d1944b6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:fa708c31c015be5e78e4a9bda39a726156b361020acf035d80c06076bbfab9b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835231372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73475f3f165b59772361e2ba0e88a3d134affb9861987f02e34850b7a7e8cda1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:35:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:35:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:38:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:38:09 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:38:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:40:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425e951c42dd00ccb058ef6938f79b69db58bf09271ae9462bd5852cfd1353c`  
		Last Modified: Sat, 16 Dec 2023 10:05:10 GMT  
		Size: 1.2 MB (1198846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aba2266c05b2025e53b1daad133978c157924dd56b92b27baac4c2b131ac49`  
		Last Modified: Sat, 16 Dec 2023 10:05:08 GMT  
		Size: 5.6 MB (5553944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da082b0fcdb0e926380c93badeb52429200982b64c2886589a087e11ada6826`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bc03d4300aebd1e01a1bbb2281172eee19cd2e9729ff0035fb2504dc536e32`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307477be25c4a96d631a6b63babb9347b6135862ce19b60048cbff55c280d179`  
		Last Modified: Sat, 16 Dec 2023 10:05:35 GMT  
		Size: 177.0 MB (176962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db26ad757af2ab1db77cea22c3559b1a93d8efa9890510f708a7fe05c28f5fe2`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b296290a0b7485d1f8672c8bd730f9a988374c02b9aa1b44d426683e13463e`  
		Last Modified: Sat, 16 Dec 2023 10:05:52 GMT  
		Size: 50.9 MB (50941170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c97955e78d4b5d35849ebaa6e03664552e66de89a179f90cb181e5682e4cdfa`  
		Last Modified: Sat, 16 Dec 2023 10:05:44 GMT  
		Size: 311.3 KB (311298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8991dddd9b2f661c7710e6ccb2cf128eb8c80547efb3b8a1a3d9252155c0ea81`  
		Last Modified: Sat, 16 Dec 2023 10:05:55 GMT  
		Size: 79.6 MB (79616327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccf1510df268376694568f812f9f639b378476209ab0731483dab043b2500fc`  
		Last Modified: Sat, 16 Dec 2023 10:07:26 GMT  
		Size: 492.1 MB (492060388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:0e23576a6710c1d26a02e2b4393d24e92cedb7b6ba7f35882b840897ccad15df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.3 MB (726265125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:351c4ffb7f029799e927a50613997af5468eb27ce8afd706c940e49b5290ab61`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:37:05 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:37:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:37:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:37:14 GMT
ADD file:195375389d64193c828c6d3f379c7e35ea85256eb1c51d2bfeab73432ea46064 in / 
# Wed, 13 Dec 2023 10:37:15 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:37:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:37:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:38:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:40:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:40:14 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:40:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:49:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba68304511cfd178c72d64196a05b1343fbdbed6093d7b4db0c0d223510c40ab`  
		Last Modified: Sat, 16 Dec 2023 09:27:50 GMT  
		Size: 24.6 MB (24600972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5373ad55d8e8c0ab26bca9b592d8809358e69e59cff53121bcdd908a9f9639c`  
		Last Modified: Sat, 16 Dec 2023 09:50:09 GMT  
		Size: 1.2 MB (1199062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc25b246e660d5421dff1c723cfa2d5dfaa9c2ccfe1976b8fce4d4d1fedc8f5`  
		Last Modified: Sat, 16 Dec 2023 09:50:07 GMT  
		Size: 4.7 MB (4679510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4107a21097c89ac49236bbde53efe45ed4c81f1e01e65c2f0358d02b73486`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70488c95ce2761e3460cec20b973e12284798d5b20d16b9009f4352584dafdc6`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecfe88b9d5bac2517d37b869da63ba8b7baa4f12ca28f6d66809dd278d3b48b`  
		Last Modified: Sat, 16 Dec 2023 09:50:35 GMT  
		Size: 157.5 MB (157458423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b4028622de95be917a19e8013de1c97bde72b70b7382298556d8cf850713e`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2341748b0485b9245a864429765e19ae950f9c356eb506df8d842670477ff2`  
		Last Modified: Sat, 16 Dec 2023 09:50:48 GMT  
		Size: 40.5 MB (40504005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660415962c143fc9e45d4e1c2054c79634e094b208c845bbd583cc003fa989b0`  
		Last Modified: Sat, 16 Dec 2023 09:50:43 GMT  
		Size: 311.3 KB (311302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fd3825c19baab04ff606134bca9de817bb604a6b321072dc1193209a7d4a3`  
		Last Modified: Sat, 16 Dec 2023 09:50:52 GMT  
		Size: 60.5 MB (60499602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95d8a7cb341a7266eed7a5be48d80d9a87edab798791d784447db400dda8e0d`  
		Last Modified: Sat, 16 Dec 2023 09:52:15 GMT  
		Size: 437.0 MB (437009839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:060d4ab2aee82f8df5712f3f8a44a0867b2e1626dd1b0c2b598f18eda060ce66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **789.7 MB (789725461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f7d9458507fe087e6e6a46b3e5fa4a3785b3288d18c0bceba93a48e2ab6250f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:21:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:21:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:37:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 02:37:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV ROS_DISTRO=noetic
# Sat, 09 Dec 2023 02:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:40:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 09 Dec 2023 02:40:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 02:40:42 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 02:41:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:41:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 02:42:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:51:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2aa78ed8ad18394d7ae521e83b2810fec9fbb7d95aa074d794bb43e6e2bbfb`  
		Last Modified: Sat, 02 Dec 2023 06:56:12 GMT  
		Size: 1.2 MB (1198781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f106a95fef578814e019c4ac69f1cf32b15d5f85da2729a7ab2487c5d3505d`  
		Last Modified: Sat, 02 Dec 2023 06:56:11 GMT  
		Size: 5.5 MB (5532202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde5587588684db83e0c22fb5d4979df124ea1cb18322ace2e4c3ea5c96b6367`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c5b1b69c1b0400c6d51e9b08a29868443a22bc46ce96467a1b6fd75f9aa2c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c0f3f95aca8df1ff165733b239844d0700cbd97842b1699375b9137cd0075e`  
		Last Modified: Sat, 09 Dec 2023 03:56:30 GMT  
		Size: 175.6 MB (175614595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648bea585de95bdc098b0f496d2c461fc072dda803fe1be92b970893fd65443c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f261b12e1911ed6acc0c610902189f69372d1dbce997eb8ff1ede6dbf9e5ae21`  
		Last Modified: Sat, 09 Dec 2023 03:56:45 GMT  
		Size: 45.2 MB (45206492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92f89f65bd6464334de4ab44489a72c7bb00a4e5286a829f25300f62f3b1f25`  
		Last Modified: Sat, 09 Dec 2023 03:56:39 GMT  
		Size: 311.1 KB (311125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814329a852addc5f898a88b8ca07e7f891f15ddafaa210e9558da08b2bdc5e91`  
		Last Modified: Sat, 09 Dec 2023 03:56:48 GMT  
		Size: 72.0 MB (71972547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b451059359bf1ff30b83aab3d4235ca6bd1b90a82ea53503e434ae19ac6f37`  
		Last Modified: Sat, 09 Dec 2023 03:58:12 GMT  
		Size: 462.7 MB (462683445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:7a2ceeae03b18d4431826e991e50f4679342923721ceee22f9b73c24d1944b6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:fa708c31c015be5e78e4a9bda39a726156b361020acf035d80c06076bbfab9b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835231372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73475f3f165b59772361e2ba0e88a3d134affb9861987f02e34850b7a7e8cda1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:35:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:35:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:38:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:38:09 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:38:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:40:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425e951c42dd00ccb058ef6938f79b69db58bf09271ae9462bd5852cfd1353c`  
		Last Modified: Sat, 16 Dec 2023 10:05:10 GMT  
		Size: 1.2 MB (1198846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aba2266c05b2025e53b1daad133978c157924dd56b92b27baac4c2b131ac49`  
		Last Modified: Sat, 16 Dec 2023 10:05:08 GMT  
		Size: 5.6 MB (5553944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da082b0fcdb0e926380c93badeb52429200982b64c2886589a087e11ada6826`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bc03d4300aebd1e01a1bbb2281172eee19cd2e9729ff0035fb2504dc536e32`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307477be25c4a96d631a6b63babb9347b6135862ce19b60048cbff55c280d179`  
		Last Modified: Sat, 16 Dec 2023 10:05:35 GMT  
		Size: 177.0 MB (176962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db26ad757af2ab1db77cea22c3559b1a93d8efa9890510f708a7fe05c28f5fe2`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b296290a0b7485d1f8672c8bd730f9a988374c02b9aa1b44d426683e13463e`  
		Last Modified: Sat, 16 Dec 2023 10:05:52 GMT  
		Size: 50.9 MB (50941170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c97955e78d4b5d35849ebaa6e03664552e66de89a179f90cb181e5682e4cdfa`  
		Last Modified: Sat, 16 Dec 2023 10:05:44 GMT  
		Size: 311.3 KB (311298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8991dddd9b2f661c7710e6ccb2cf128eb8c80547efb3b8a1a3d9252155c0ea81`  
		Last Modified: Sat, 16 Dec 2023 10:05:55 GMT  
		Size: 79.6 MB (79616327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccf1510df268376694568f812f9f639b378476209ab0731483dab043b2500fc`  
		Last Modified: Sat, 16 Dec 2023 10:07:26 GMT  
		Size: 492.1 MB (492060388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:0e23576a6710c1d26a02e2b4393d24e92cedb7b6ba7f35882b840897ccad15df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.3 MB (726265125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:351c4ffb7f029799e927a50613997af5468eb27ce8afd706c940e49b5290ab61`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:37:05 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:37:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:37:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:37:14 GMT
ADD file:195375389d64193c828c6d3f379c7e35ea85256eb1c51d2bfeab73432ea46064 in / 
# Wed, 13 Dec 2023 10:37:15 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:37:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:37:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:38:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:40:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:40:14 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:40:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:49:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba68304511cfd178c72d64196a05b1343fbdbed6093d7b4db0c0d223510c40ab`  
		Last Modified: Sat, 16 Dec 2023 09:27:50 GMT  
		Size: 24.6 MB (24600972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5373ad55d8e8c0ab26bca9b592d8809358e69e59cff53121bcdd908a9f9639c`  
		Last Modified: Sat, 16 Dec 2023 09:50:09 GMT  
		Size: 1.2 MB (1199062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc25b246e660d5421dff1c723cfa2d5dfaa9c2ccfe1976b8fce4d4d1fedc8f5`  
		Last Modified: Sat, 16 Dec 2023 09:50:07 GMT  
		Size: 4.7 MB (4679510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4107a21097c89ac49236bbde53efe45ed4c81f1e01e65c2f0358d02b73486`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70488c95ce2761e3460cec20b973e12284798d5b20d16b9009f4352584dafdc6`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecfe88b9d5bac2517d37b869da63ba8b7baa4f12ca28f6d66809dd278d3b48b`  
		Last Modified: Sat, 16 Dec 2023 09:50:35 GMT  
		Size: 157.5 MB (157458423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b4028622de95be917a19e8013de1c97bde72b70b7382298556d8cf850713e`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2341748b0485b9245a864429765e19ae950f9c356eb506df8d842670477ff2`  
		Last Modified: Sat, 16 Dec 2023 09:50:48 GMT  
		Size: 40.5 MB (40504005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660415962c143fc9e45d4e1c2054c79634e094b208c845bbd583cc003fa989b0`  
		Last Modified: Sat, 16 Dec 2023 09:50:43 GMT  
		Size: 311.3 KB (311302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fd3825c19baab04ff606134bca9de817bb604a6b321072dc1193209a7d4a3`  
		Last Modified: Sat, 16 Dec 2023 09:50:52 GMT  
		Size: 60.5 MB (60499602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95d8a7cb341a7266eed7a5be48d80d9a87edab798791d784447db400dda8e0d`  
		Last Modified: Sat, 16 Dec 2023 09:52:15 GMT  
		Size: 437.0 MB (437009839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:060d4ab2aee82f8df5712f3f8a44a0867b2e1626dd1b0c2b598f18eda060ce66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **789.7 MB (789725461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f7d9458507fe087e6e6a46b3e5fa4a3785b3288d18c0bceba93a48e2ab6250f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:21:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:21:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:37:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 02:37:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV ROS_DISTRO=noetic
# Sat, 09 Dec 2023 02:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:40:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 09 Dec 2023 02:40:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 02:40:42 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 02:41:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:41:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 02:42:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:51:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2aa78ed8ad18394d7ae521e83b2810fec9fbb7d95aa074d794bb43e6e2bbfb`  
		Last Modified: Sat, 02 Dec 2023 06:56:12 GMT  
		Size: 1.2 MB (1198781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f106a95fef578814e019c4ac69f1cf32b15d5f85da2729a7ab2487c5d3505d`  
		Last Modified: Sat, 02 Dec 2023 06:56:11 GMT  
		Size: 5.5 MB (5532202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde5587588684db83e0c22fb5d4979df124ea1cb18322ace2e4c3ea5c96b6367`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c5b1b69c1b0400c6d51e9b08a29868443a22bc46ce96467a1b6fd75f9aa2c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c0f3f95aca8df1ff165733b239844d0700cbd97842b1699375b9137cd0075e`  
		Last Modified: Sat, 09 Dec 2023 03:56:30 GMT  
		Size: 175.6 MB (175614595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648bea585de95bdc098b0f496d2c461fc072dda803fe1be92b970893fd65443c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f261b12e1911ed6acc0c610902189f69372d1dbce997eb8ff1ede6dbf9e5ae21`  
		Last Modified: Sat, 09 Dec 2023 03:56:45 GMT  
		Size: 45.2 MB (45206492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92f89f65bd6464334de4ab44489a72c7bb00a4e5286a829f25300f62f3b1f25`  
		Last Modified: Sat, 09 Dec 2023 03:56:39 GMT  
		Size: 311.1 KB (311125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814329a852addc5f898a88b8ca07e7f891f15ddafaa210e9558da08b2bdc5e91`  
		Last Modified: Sat, 09 Dec 2023 03:56:48 GMT  
		Size: 72.0 MB (71972547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b451059359bf1ff30b83aab3d4235ca6bd1b90a82ea53503e434ae19ac6f37`  
		Last Modified: Sat, 09 Dec 2023 03:58:12 GMT  
		Size: 462.7 MB (462683445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:5817e54de8cf13d1ed207a40feb1cbe73bb1ab2b9536d7bf5fa52a0c58083d96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:02af0855315492649518532844615e4e9a52f376507a99e62cbc95f6d2955148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359036286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2e0ef7eb7bc61c979bdcd559d8b847bb3f611d14b4c65a38997f4a83dafe21`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:35:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:35:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:38:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:38:09 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:38:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:40:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425e951c42dd00ccb058ef6938f79b69db58bf09271ae9462bd5852cfd1353c`  
		Last Modified: Sat, 16 Dec 2023 10:05:10 GMT  
		Size: 1.2 MB (1198846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aba2266c05b2025e53b1daad133978c157924dd56b92b27baac4c2b131ac49`  
		Last Modified: Sat, 16 Dec 2023 10:05:08 GMT  
		Size: 5.6 MB (5553944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da082b0fcdb0e926380c93badeb52429200982b64c2886589a087e11ada6826`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bc03d4300aebd1e01a1bbb2281172eee19cd2e9729ff0035fb2504dc536e32`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307477be25c4a96d631a6b63babb9347b6135862ce19b60048cbff55c280d179`  
		Last Modified: Sat, 16 Dec 2023 10:05:35 GMT  
		Size: 177.0 MB (176962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db26ad757af2ab1db77cea22c3559b1a93d8efa9890510f708a7fe05c28f5fe2`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b296290a0b7485d1f8672c8bd730f9a988374c02b9aa1b44d426683e13463e`  
		Last Modified: Sat, 16 Dec 2023 10:05:52 GMT  
		Size: 50.9 MB (50941170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c97955e78d4b5d35849ebaa6e03664552e66de89a179f90cb181e5682e4cdfa`  
		Last Modified: Sat, 16 Dec 2023 10:05:44 GMT  
		Size: 311.3 KB (311298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8991dddd9b2f661c7710e6ccb2cf128eb8c80547efb3b8a1a3d9252155c0ea81`  
		Last Modified: Sat, 16 Dec 2023 10:05:55 GMT  
		Size: 79.6 MB (79616327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fc26c0942e6ea571edbaa2b6dc7ca635460243636f430c0548ac8941b2eac8`  
		Last Modified: Sat, 16 Dec 2023 10:06:10 GMT  
		Size: 15.9 MB (15865302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:6b36005461cc659673ed1692889f039d16f52c2abd8ec3039e0501b08bf108f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303324544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cfb5f820bb7aba5ea28aade0eb2360f82e7de54e803d144424ba97b15dd335e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:37:05 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:37:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:37:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:37:14 GMT
ADD file:195375389d64193c828c6d3f379c7e35ea85256eb1c51d2bfeab73432ea46064 in / 
# Wed, 13 Dec 2023 10:37:15 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:37:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:37:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:38:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:40:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:40:14 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:40:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:42:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba68304511cfd178c72d64196a05b1343fbdbed6093d7b4db0c0d223510c40ab`  
		Last Modified: Sat, 16 Dec 2023 09:27:50 GMT  
		Size: 24.6 MB (24600972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5373ad55d8e8c0ab26bca9b592d8809358e69e59cff53121bcdd908a9f9639c`  
		Last Modified: Sat, 16 Dec 2023 09:50:09 GMT  
		Size: 1.2 MB (1199062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc25b246e660d5421dff1c723cfa2d5dfaa9c2ccfe1976b8fce4d4d1fedc8f5`  
		Last Modified: Sat, 16 Dec 2023 09:50:07 GMT  
		Size: 4.7 MB (4679510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4107a21097c89ac49236bbde53efe45ed4c81f1e01e65c2f0358d02b73486`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70488c95ce2761e3460cec20b973e12284798d5b20d16b9009f4352584dafdc6`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecfe88b9d5bac2517d37b869da63ba8b7baa4f12ca28f6d66809dd278d3b48b`  
		Last Modified: Sat, 16 Dec 2023 09:50:35 GMT  
		Size: 157.5 MB (157458423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b4028622de95be917a19e8013de1c97bde72b70b7382298556d8cf850713e`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2341748b0485b9245a864429765e19ae950f9c356eb506df8d842670477ff2`  
		Last Modified: Sat, 16 Dec 2023 09:50:48 GMT  
		Size: 40.5 MB (40504005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660415962c143fc9e45d4e1c2054c79634e094b208c845bbd583cc003fa989b0`  
		Last Modified: Sat, 16 Dec 2023 09:50:43 GMT  
		Size: 311.3 KB (311302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fd3825c19baab04ff606134bca9de817bb604a6b321072dc1193209a7d4a3`  
		Last Modified: Sat, 16 Dec 2023 09:50:52 GMT  
		Size: 60.5 MB (60499602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf539cad1625afd5268e42be8ea819a4579655da66af147aaa75ef57d51e3d44`  
		Last Modified: Sat, 16 Dec 2023 09:51:06 GMT  
		Size: 14.1 MB (14069258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:617726e642c65e21d7852caf72535906bfe8ac7d39176f532ba3826221fdaca9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.5 MB (342501946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00424f470173cb1cf2bac8f9c174ceac17664ad23cc2f78baea04a017580ba11`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:21:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:21:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:37:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 02:37:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV ROS_DISTRO=noetic
# Sat, 09 Dec 2023 02:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:40:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 09 Dec 2023 02:40:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 02:40:42 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 02:41:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:41:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 02:42:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:43:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2aa78ed8ad18394d7ae521e83b2810fec9fbb7d95aa074d794bb43e6e2bbfb`  
		Last Modified: Sat, 02 Dec 2023 06:56:12 GMT  
		Size: 1.2 MB (1198781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f106a95fef578814e019c4ac69f1cf32b15d5f85da2729a7ab2487c5d3505d`  
		Last Modified: Sat, 02 Dec 2023 06:56:11 GMT  
		Size: 5.5 MB (5532202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde5587588684db83e0c22fb5d4979df124ea1cb18322ace2e4c3ea5c96b6367`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c5b1b69c1b0400c6d51e9b08a29868443a22bc46ce96467a1b6fd75f9aa2c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c0f3f95aca8df1ff165733b239844d0700cbd97842b1699375b9137cd0075e`  
		Last Modified: Sat, 09 Dec 2023 03:56:30 GMT  
		Size: 175.6 MB (175614595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648bea585de95bdc098b0f496d2c461fc072dda803fe1be92b970893fd65443c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f261b12e1911ed6acc0c610902189f69372d1dbce997eb8ff1ede6dbf9e5ae21`  
		Last Modified: Sat, 09 Dec 2023 03:56:45 GMT  
		Size: 45.2 MB (45206492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92f89f65bd6464334de4ab44489a72c7bb00a4e5286a829f25300f62f3b1f25`  
		Last Modified: Sat, 09 Dec 2023 03:56:39 GMT  
		Size: 311.1 KB (311125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814329a852addc5f898a88b8ca07e7f891f15ddafaa210e9558da08b2bdc5e91`  
		Last Modified: Sat, 09 Dec 2023 03:56:48 GMT  
		Size: 72.0 MB (71972547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c70f89caeb2c4f123a07320b1bb566909a4cadd6213d4f641eb655b5f3e3f2f`  
		Last Modified: Sat, 09 Dec 2023 03:57:02 GMT  
		Size: 15.5 MB (15459930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:5817e54de8cf13d1ed207a40feb1cbe73bb1ab2b9536d7bf5fa52a0c58083d96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:02af0855315492649518532844615e4e9a52f376507a99e62cbc95f6d2955148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359036286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2e0ef7eb7bc61c979bdcd559d8b847bb3f611d14b4c65a38997f4a83dafe21`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:35:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:35:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:38:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:38:09 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:38:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:40:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425e951c42dd00ccb058ef6938f79b69db58bf09271ae9462bd5852cfd1353c`  
		Last Modified: Sat, 16 Dec 2023 10:05:10 GMT  
		Size: 1.2 MB (1198846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aba2266c05b2025e53b1daad133978c157924dd56b92b27baac4c2b131ac49`  
		Last Modified: Sat, 16 Dec 2023 10:05:08 GMT  
		Size: 5.6 MB (5553944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da082b0fcdb0e926380c93badeb52429200982b64c2886589a087e11ada6826`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bc03d4300aebd1e01a1bbb2281172eee19cd2e9729ff0035fb2504dc536e32`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307477be25c4a96d631a6b63babb9347b6135862ce19b60048cbff55c280d179`  
		Last Modified: Sat, 16 Dec 2023 10:05:35 GMT  
		Size: 177.0 MB (176962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db26ad757af2ab1db77cea22c3559b1a93d8efa9890510f708a7fe05c28f5fe2`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b296290a0b7485d1f8672c8bd730f9a988374c02b9aa1b44d426683e13463e`  
		Last Modified: Sat, 16 Dec 2023 10:05:52 GMT  
		Size: 50.9 MB (50941170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c97955e78d4b5d35849ebaa6e03664552e66de89a179f90cb181e5682e4cdfa`  
		Last Modified: Sat, 16 Dec 2023 10:05:44 GMT  
		Size: 311.3 KB (311298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8991dddd9b2f661c7710e6ccb2cf128eb8c80547efb3b8a1a3d9252155c0ea81`  
		Last Modified: Sat, 16 Dec 2023 10:05:55 GMT  
		Size: 79.6 MB (79616327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fc26c0942e6ea571edbaa2b6dc7ca635460243636f430c0548ac8941b2eac8`  
		Last Modified: Sat, 16 Dec 2023 10:06:10 GMT  
		Size: 15.9 MB (15865302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:6b36005461cc659673ed1692889f039d16f52c2abd8ec3039e0501b08bf108f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303324544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cfb5f820bb7aba5ea28aade0eb2360f82e7de54e803d144424ba97b15dd335e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:37:05 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:37:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:37:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:37:14 GMT
ADD file:195375389d64193c828c6d3f379c7e35ea85256eb1c51d2bfeab73432ea46064 in / 
# Wed, 13 Dec 2023 10:37:15 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:37:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:37:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:38:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:40:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:40:14 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:40:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:42:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba68304511cfd178c72d64196a05b1343fbdbed6093d7b4db0c0d223510c40ab`  
		Last Modified: Sat, 16 Dec 2023 09:27:50 GMT  
		Size: 24.6 MB (24600972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5373ad55d8e8c0ab26bca9b592d8809358e69e59cff53121bcdd908a9f9639c`  
		Last Modified: Sat, 16 Dec 2023 09:50:09 GMT  
		Size: 1.2 MB (1199062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc25b246e660d5421dff1c723cfa2d5dfaa9c2ccfe1976b8fce4d4d1fedc8f5`  
		Last Modified: Sat, 16 Dec 2023 09:50:07 GMT  
		Size: 4.7 MB (4679510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4107a21097c89ac49236bbde53efe45ed4c81f1e01e65c2f0358d02b73486`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70488c95ce2761e3460cec20b973e12284798d5b20d16b9009f4352584dafdc6`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecfe88b9d5bac2517d37b869da63ba8b7baa4f12ca28f6d66809dd278d3b48b`  
		Last Modified: Sat, 16 Dec 2023 09:50:35 GMT  
		Size: 157.5 MB (157458423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b4028622de95be917a19e8013de1c97bde72b70b7382298556d8cf850713e`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2341748b0485b9245a864429765e19ae950f9c356eb506df8d842670477ff2`  
		Last Modified: Sat, 16 Dec 2023 09:50:48 GMT  
		Size: 40.5 MB (40504005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660415962c143fc9e45d4e1c2054c79634e094b208c845bbd583cc003fa989b0`  
		Last Modified: Sat, 16 Dec 2023 09:50:43 GMT  
		Size: 311.3 KB (311302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fd3825c19baab04ff606134bca9de817bb604a6b321072dc1193209a7d4a3`  
		Last Modified: Sat, 16 Dec 2023 09:50:52 GMT  
		Size: 60.5 MB (60499602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf539cad1625afd5268e42be8ea819a4579655da66af147aaa75ef57d51e3d44`  
		Last Modified: Sat, 16 Dec 2023 09:51:06 GMT  
		Size: 14.1 MB (14069258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:617726e642c65e21d7852caf72535906bfe8ac7d39176f532ba3826221fdaca9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.5 MB (342501946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00424f470173cb1cf2bac8f9c174ceac17664ad23cc2f78baea04a017580ba11`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:21:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:21:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:37:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 02:37:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV ROS_DISTRO=noetic
# Sat, 09 Dec 2023 02:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:40:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 09 Dec 2023 02:40:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 02:40:42 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 02:41:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:41:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 02:42:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:43:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2aa78ed8ad18394d7ae521e83b2810fec9fbb7d95aa074d794bb43e6e2bbfb`  
		Last Modified: Sat, 02 Dec 2023 06:56:12 GMT  
		Size: 1.2 MB (1198781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f106a95fef578814e019c4ac69f1cf32b15d5f85da2729a7ab2487c5d3505d`  
		Last Modified: Sat, 02 Dec 2023 06:56:11 GMT  
		Size: 5.5 MB (5532202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde5587588684db83e0c22fb5d4979df124ea1cb18322ace2e4c3ea5c96b6367`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c5b1b69c1b0400c6d51e9b08a29868443a22bc46ce96467a1b6fd75f9aa2c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c0f3f95aca8df1ff165733b239844d0700cbd97842b1699375b9137cd0075e`  
		Last Modified: Sat, 09 Dec 2023 03:56:30 GMT  
		Size: 175.6 MB (175614595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648bea585de95bdc098b0f496d2c461fc072dda803fe1be92b970893fd65443c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f261b12e1911ed6acc0c610902189f69372d1dbce997eb8ff1ede6dbf9e5ae21`  
		Last Modified: Sat, 09 Dec 2023 03:56:45 GMT  
		Size: 45.2 MB (45206492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92f89f65bd6464334de4ab44489a72c7bb00a4e5286a829f25300f62f3b1f25`  
		Last Modified: Sat, 09 Dec 2023 03:56:39 GMT  
		Size: 311.1 KB (311125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814329a852addc5f898a88b8ca07e7f891f15ddafaa210e9558da08b2bdc5e91`  
		Last Modified: Sat, 09 Dec 2023 03:56:48 GMT  
		Size: 72.0 MB (71972547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c70f89caeb2c4f123a07320b1bb566909a4cadd6213d4f641eb655b5f3e3f2f`  
		Last Modified: Sat, 09 Dec 2023 03:57:02 GMT  
		Size: 15.5 MB (15459930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:1daa1992f1d29ff18cbe6979d8d1ab6bf6668920d2323c66f516310a91c8152c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:b18ca33cdeee0817fd39b018ddfbd8cc0cb693fbe89211dd3b77b19e7f386adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343170984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a26fadd8116de9bd16b53dffe5995a44be3e31ef87872347bbe08230e877b05c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:35:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:35:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:38:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:38:09 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:38:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:40:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425e951c42dd00ccb058ef6938f79b69db58bf09271ae9462bd5852cfd1353c`  
		Last Modified: Sat, 16 Dec 2023 10:05:10 GMT  
		Size: 1.2 MB (1198846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aba2266c05b2025e53b1daad133978c157924dd56b92b27baac4c2b131ac49`  
		Last Modified: Sat, 16 Dec 2023 10:05:08 GMT  
		Size: 5.6 MB (5553944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da082b0fcdb0e926380c93badeb52429200982b64c2886589a087e11ada6826`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bc03d4300aebd1e01a1bbb2281172eee19cd2e9729ff0035fb2504dc536e32`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307477be25c4a96d631a6b63babb9347b6135862ce19b60048cbff55c280d179`  
		Last Modified: Sat, 16 Dec 2023 10:05:35 GMT  
		Size: 177.0 MB (176962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db26ad757af2ab1db77cea22c3559b1a93d8efa9890510f708a7fe05c28f5fe2`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b296290a0b7485d1f8672c8bd730f9a988374c02b9aa1b44d426683e13463e`  
		Last Modified: Sat, 16 Dec 2023 10:05:52 GMT  
		Size: 50.9 MB (50941170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c97955e78d4b5d35849ebaa6e03664552e66de89a179f90cb181e5682e4cdfa`  
		Last Modified: Sat, 16 Dec 2023 10:05:44 GMT  
		Size: 311.3 KB (311298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8991dddd9b2f661c7710e6ccb2cf128eb8c80547efb3b8a1a3d9252155c0ea81`  
		Last Modified: Sat, 16 Dec 2023 10:05:55 GMT  
		Size: 79.6 MB (79616327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:a6a7e4a94a9f86c92df92c18301a2d2905e8615d7385271787b42edaa4fb84c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289255286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c779c68ac98eec285da4a980fbd6de29582b95d14857068629917b02aebf17b4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:37:05 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:37:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:37:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:37:14 GMT
ADD file:195375389d64193c828c6d3f379c7e35ea85256eb1c51d2bfeab73432ea46064 in / 
# Wed, 13 Dec 2023 10:37:15 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:37:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:37:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:38:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:40:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:40:14 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:40:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba68304511cfd178c72d64196a05b1343fbdbed6093d7b4db0c0d223510c40ab`  
		Last Modified: Sat, 16 Dec 2023 09:27:50 GMT  
		Size: 24.6 MB (24600972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5373ad55d8e8c0ab26bca9b592d8809358e69e59cff53121bcdd908a9f9639c`  
		Last Modified: Sat, 16 Dec 2023 09:50:09 GMT  
		Size: 1.2 MB (1199062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc25b246e660d5421dff1c723cfa2d5dfaa9c2ccfe1976b8fce4d4d1fedc8f5`  
		Last Modified: Sat, 16 Dec 2023 09:50:07 GMT  
		Size: 4.7 MB (4679510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4107a21097c89ac49236bbde53efe45ed4c81f1e01e65c2f0358d02b73486`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70488c95ce2761e3460cec20b973e12284798d5b20d16b9009f4352584dafdc6`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecfe88b9d5bac2517d37b869da63ba8b7baa4f12ca28f6d66809dd278d3b48b`  
		Last Modified: Sat, 16 Dec 2023 09:50:35 GMT  
		Size: 157.5 MB (157458423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b4028622de95be917a19e8013de1c97bde72b70b7382298556d8cf850713e`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2341748b0485b9245a864429765e19ae950f9c356eb506df8d842670477ff2`  
		Last Modified: Sat, 16 Dec 2023 09:50:48 GMT  
		Size: 40.5 MB (40504005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660415962c143fc9e45d4e1c2054c79634e094b208c845bbd583cc003fa989b0`  
		Last Modified: Sat, 16 Dec 2023 09:50:43 GMT  
		Size: 311.3 KB (311302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fd3825c19baab04ff606134bca9de817bb604a6b321072dc1193209a7d4a3`  
		Last Modified: Sat, 16 Dec 2023 09:50:52 GMT  
		Size: 60.5 MB (60499602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b6ba98c10af60c68d092a70a824dd3cc8b25ff52cccf8856918e03c3b471cc5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.0 MB (327042016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fec3efa1ad8e98f48e1c8d6237ae0f7d52ee6da5055a3e76a6fb45ca51abbdbc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:21:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:21:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:37:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 02:37:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV ROS_DISTRO=noetic
# Sat, 09 Dec 2023 02:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:40:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 09 Dec 2023 02:40:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 02:40:42 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 02:41:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:41:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 02:42:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2aa78ed8ad18394d7ae521e83b2810fec9fbb7d95aa074d794bb43e6e2bbfb`  
		Last Modified: Sat, 02 Dec 2023 06:56:12 GMT  
		Size: 1.2 MB (1198781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f106a95fef578814e019c4ac69f1cf32b15d5f85da2729a7ab2487c5d3505d`  
		Last Modified: Sat, 02 Dec 2023 06:56:11 GMT  
		Size: 5.5 MB (5532202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde5587588684db83e0c22fb5d4979df124ea1cb18322ace2e4c3ea5c96b6367`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c5b1b69c1b0400c6d51e9b08a29868443a22bc46ce96467a1b6fd75f9aa2c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c0f3f95aca8df1ff165733b239844d0700cbd97842b1699375b9137cd0075e`  
		Last Modified: Sat, 09 Dec 2023 03:56:30 GMT  
		Size: 175.6 MB (175614595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648bea585de95bdc098b0f496d2c461fc072dda803fe1be92b970893fd65443c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f261b12e1911ed6acc0c610902189f69372d1dbce997eb8ff1ede6dbf9e5ae21`  
		Last Modified: Sat, 09 Dec 2023 03:56:45 GMT  
		Size: 45.2 MB (45206492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92f89f65bd6464334de4ab44489a72c7bb00a4e5286a829f25300f62f3b1f25`  
		Last Modified: Sat, 09 Dec 2023 03:56:39 GMT  
		Size: 311.1 KB (311125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814329a852addc5f898a88b8ca07e7f891f15ddafaa210e9558da08b2bdc5e91`  
		Last Modified: Sat, 09 Dec 2023 03:56:48 GMT  
		Size: 72.0 MB (71972547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:1daa1992f1d29ff18cbe6979d8d1ab6bf6668920d2323c66f516310a91c8152c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:b18ca33cdeee0817fd39b018ddfbd8cc0cb693fbe89211dd3b77b19e7f386adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343170984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a26fadd8116de9bd16b53dffe5995a44be3e31ef87872347bbe08230e877b05c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:35:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:35:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:38:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:38:09 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:38:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:40:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425e951c42dd00ccb058ef6938f79b69db58bf09271ae9462bd5852cfd1353c`  
		Last Modified: Sat, 16 Dec 2023 10:05:10 GMT  
		Size: 1.2 MB (1198846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aba2266c05b2025e53b1daad133978c157924dd56b92b27baac4c2b131ac49`  
		Last Modified: Sat, 16 Dec 2023 10:05:08 GMT  
		Size: 5.6 MB (5553944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da082b0fcdb0e926380c93badeb52429200982b64c2886589a087e11ada6826`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bc03d4300aebd1e01a1bbb2281172eee19cd2e9729ff0035fb2504dc536e32`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307477be25c4a96d631a6b63babb9347b6135862ce19b60048cbff55c280d179`  
		Last Modified: Sat, 16 Dec 2023 10:05:35 GMT  
		Size: 177.0 MB (176962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db26ad757af2ab1db77cea22c3559b1a93d8efa9890510f708a7fe05c28f5fe2`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b296290a0b7485d1f8672c8bd730f9a988374c02b9aa1b44d426683e13463e`  
		Last Modified: Sat, 16 Dec 2023 10:05:52 GMT  
		Size: 50.9 MB (50941170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c97955e78d4b5d35849ebaa6e03664552e66de89a179f90cb181e5682e4cdfa`  
		Last Modified: Sat, 16 Dec 2023 10:05:44 GMT  
		Size: 311.3 KB (311298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8991dddd9b2f661c7710e6ccb2cf128eb8c80547efb3b8a1a3d9252155c0ea81`  
		Last Modified: Sat, 16 Dec 2023 10:05:55 GMT  
		Size: 79.6 MB (79616327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:a6a7e4a94a9f86c92df92c18301a2d2905e8615d7385271787b42edaa4fb84c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289255286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c779c68ac98eec285da4a980fbd6de29582b95d14857068629917b02aebf17b4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:37:05 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:37:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:37:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:37:14 GMT
ADD file:195375389d64193c828c6d3f379c7e35ea85256eb1c51d2bfeab73432ea46064 in / 
# Wed, 13 Dec 2023 10:37:15 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:37:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:37:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:38:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:40:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:40:14 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:40:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba68304511cfd178c72d64196a05b1343fbdbed6093d7b4db0c0d223510c40ab`  
		Last Modified: Sat, 16 Dec 2023 09:27:50 GMT  
		Size: 24.6 MB (24600972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5373ad55d8e8c0ab26bca9b592d8809358e69e59cff53121bcdd908a9f9639c`  
		Last Modified: Sat, 16 Dec 2023 09:50:09 GMT  
		Size: 1.2 MB (1199062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc25b246e660d5421dff1c723cfa2d5dfaa9c2ccfe1976b8fce4d4d1fedc8f5`  
		Last Modified: Sat, 16 Dec 2023 09:50:07 GMT  
		Size: 4.7 MB (4679510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4107a21097c89ac49236bbde53efe45ed4c81f1e01e65c2f0358d02b73486`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70488c95ce2761e3460cec20b973e12284798d5b20d16b9009f4352584dafdc6`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecfe88b9d5bac2517d37b869da63ba8b7baa4f12ca28f6d66809dd278d3b48b`  
		Last Modified: Sat, 16 Dec 2023 09:50:35 GMT  
		Size: 157.5 MB (157458423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b4028622de95be917a19e8013de1c97bde72b70b7382298556d8cf850713e`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2341748b0485b9245a864429765e19ae950f9c356eb506df8d842670477ff2`  
		Last Modified: Sat, 16 Dec 2023 09:50:48 GMT  
		Size: 40.5 MB (40504005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660415962c143fc9e45d4e1c2054c79634e094b208c845bbd583cc003fa989b0`  
		Last Modified: Sat, 16 Dec 2023 09:50:43 GMT  
		Size: 311.3 KB (311302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fd3825c19baab04ff606134bca9de817bb604a6b321072dc1193209a7d4a3`  
		Last Modified: Sat, 16 Dec 2023 09:50:52 GMT  
		Size: 60.5 MB (60499602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b6ba98c10af60c68d092a70a824dd3cc8b25ff52cccf8856918e03c3b471cc5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.0 MB (327042016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fec3efa1ad8e98f48e1c8d6237ae0f7d52ee6da5055a3e76a6fb45ca51abbdbc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:21:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:21:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:37:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 02:37:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV ROS_DISTRO=noetic
# Sat, 09 Dec 2023 02:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:40:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 09 Dec 2023 02:40:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 02:40:42 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 02:41:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:41:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 02:42:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2aa78ed8ad18394d7ae521e83b2810fec9fbb7d95aa074d794bb43e6e2bbfb`  
		Last Modified: Sat, 02 Dec 2023 06:56:12 GMT  
		Size: 1.2 MB (1198781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f106a95fef578814e019c4ac69f1cf32b15d5f85da2729a7ab2487c5d3505d`  
		Last Modified: Sat, 02 Dec 2023 06:56:11 GMT  
		Size: 5.5 MB (5532202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde5587588684db83e0c22fb5d4979df124ea1cb18322ace2e4c3ea5c96b6367`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c5b1b69c1b0400c6d51e9b08a29868443a22bc46ce96467a1b6fd75f9aa2c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c0f3f95aca8df1ff165733b239844d0700cbd97842b1699375b9137cd0075e`  
		Last Modified: Sat, 09 Dec 2023 03:56:30 GMT  
		Size: 175.6 MB (175614595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648bea585de95bdc098b0f496d2c461fc072dda803fe1be92b970893fd65443c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f261b12e1911ed6acc0c610902189f69372d1dbce997eb8ff1ede6dbf9e5ae21`  
		Last Modified: Sat, 09 Dec 2023 03:56:45 GMT  
		Size: 45.2 MB (45206492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92f89f65bd6464334de4ab44489a72c7bb00a4e5286a829f25300f62f3b1f25`  
		Last Modified: Sat, 09 Dec 2023 03:56:39 GMT  
		Size: 311.1 KB (311125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814329a852addc5f898a88b8ca07e7f891f15ddafaa210e9558da08b2bdc5e91`  
		Last Modified: Sat, 09 Dec 2023 03:56:48 GMT  
		Size: 72.0 MB (71972547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:bb6f19ef59ff33c37a77d53128567048c6026526e2cde9a7d03998324a429e9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:6c3d1c582c2b6d28c0873ef8830fa7009d7c133deff33110e608b8a3d4fc1d3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212302189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e86a2e87f5ee62ba3387862b4bf453b2c08bf22ea33af6e127be70e416ba88`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:35:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:35:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:38:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:38:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425e951c42dd00ccb058ef6938f79b69db58bf09271ae9462bd5852cfd1353c`  
		Last Modified: Sat, 16 Dec 2023 10:05:10 GMT  
		Size: 1.2 MB (1198846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aba2266c05b2025e53b1daad133978c157924dd56b92b27baac4c2b131ac49`  
		Last Modified: Sat, 16 Dec 2023 10:05:08 GMT  
		Size: 5.6 MB (5553944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da082b0fcdb0e926380c93badeb52429200982b64c2886589a087e11ada6826`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bc03d4300aebd1e01a1bbb2281172eee19cd2e9729ff0035fb2504dc536e32`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307477be25c4a96d631a6b63babb9347b6135862ce19b60048cbff55c280d179`  
		Last Modified: Sat, 16 Dec 2023 10:05:35 GMT  
		Size: 177.0 MB (176962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db26ad757af2ab1db77cea22c3559b1a93d8efa9890510f708a7fe05c28f5fe2`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:28bb604051b10c25f4a37d070854a85a6cc436b0d7dde3a10fc46ae64bec79c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187940377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9daae24dfaedd2dfe709a4a184f6a9f6fad1d16fb324ede62db313c1a5c03c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:37:05 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:37:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:37:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:37:14 GMT
ADD file:195375389d64193c828c6d3f379c7e35ea85256eb1c51d2bfeab73432ea46064 in / 
# Wed, 13 Dec 2023 10:37:15 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:37:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:37:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:38:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:40:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:40:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ba68304511cfd178c72d64196a05b1343fbdbed6093d7b4db0c0d223510c40ab`  
		Last Modified: Sat, 16 Dec 2023 09:27:50 GMT  
		Size: 24.6 MB (24600972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5373ad55d8e8c0ab26bca9b592d8809358e69e59cff53121bcdd908a9f9639c`  
		Last Modified: Sat, 16 Dec 2023 09:50:09 GMT  
		Size: 1.2 MB (1199062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc25b246e660d5421dff1c723cfa2d5dfaa9c2ccfe1976b8fce4d4d1fedc8f5`  
		Last Modified: Sat, 16 Dec 2023 09:50:07 GMT  
		Size: 4.7 MB (4679510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4107a21097c89ac49236bbde53efe45ed4c81f1e01e65c2f0358d02b73486`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70488c95ce2761e3460cec20b973e12284798d5b20d16b9009f4352584dafdc6`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecfe88b9d5bac2517d37b869da63ba8b7baa4f12ca28f6d66809dd278d3b48b`  
		Last Modified: Sat, 16 Dec 2023 09:50:35 GMT  
		Size: 157.5 MB (157458423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b4028622de95be917a19e8013de1c97bde72b70b7382298556d8cf850713e`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b1d00726fd3fa46d77524a8053bd609365b5abae3a17a67f3683bf297ee8bd0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.6 MB (209551852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ef109a0615f2e6a12306ea2f79634e967bff0243f3dedb39dd1725cacedabe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:21:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:21:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:37:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 02:37:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV ROS_DISTRO=noetic
# Sat, 09 Dec 2023 02:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:40:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 09 Dec 2023 02:40:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 02:40:42 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2aa78ed8ad18394d7ae521e83b2810fec9fbb7d95aa074d794bb43e6e2bbfb`  
		Last Modified: Sat, 02 Dec 2023 06:56:12 GMT  
		Size: 1.2 MB (1198781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f106a95fef578814e019c4ac69f1cf32b15d5f85da2729a7ab2487c5d3505d`  
		Last Modified: Sat, 02 Dec 2023 06:56:11 GMT  
		Size: 5.5 MB (5532202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde5587588684db83e0c22fb5d4979df124ea1cb18322ace2e4c3ea5c96b6367`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c5b1b69c1b0400c6d51e9b08a29868443a22bc46ce96467a1b6fd75f9aa2c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c0f3f95aca8df1ff165733b239844d0700cbd97842b1699375b9137cd0075e`  
		Last Modified: Sat, 09 Dec 2023 03:56:30 GMT  
		Size: 175.6 MB (175614595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648bea585de95bdc098b0f496d2c461fc072dda803fe1be92b970893fd65443c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:bb6f19ef59ff33c37a77d53128567048c6026526e2cde9a7d03998324a429e9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:6c3d1c582c2b6d28c0873ef8830fa7009d7c133deff33110e608b8a3d4fc1d3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212302189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e86a2e87f5ee62ba3387862b4bf453b2c08bf22ea33af6e127be70e416ba88`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:35:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:35:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:38:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:38:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425e951c42dd00ccb058ef6938f79b69db58bf09271ae9462bd5852cfd1353c`  
		Last Modified: Sat, 16 Dec 2023 10:05:10 GMT  
		Size: 1.2 MB (1198846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aba2266c05b2025e53b1daad133978c157924dd56b92b27baac4c2b131ac49`  
		Last Modified: Sat, 16 Dec 2023 10:05:08 GMT  
		Size: 5.6 MB (5553944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da082b0fcdb0e926380c93badeb52429200982b64c2886589a087e11ada6826`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bc03d4300aebd1e01a1bbb2281172eee19cd2e9729ff0035fb2504dc536e32`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307477be25c4a96d631a6b63babb9347b6135862ce19b60048cbff55c280d179`  
		Last Modified: Sat, 16 Dec 2023 10:05:35 GMT  
		Size: 177.0 MB (176962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db26ad757af2ab1db77cea22c3559b1a93d8efa9890510f708a7fe05c28f5fe2`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:28bb604051b10c25f4a37d070854a85a6cc436b0d7dde3a10fc46ae64bec79c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187940377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9daae24dfaedd2dfe709a4a184f6a9f6fad1d16fb324ede62db313c1a5c03c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:37:05 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:37:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:37:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:37:14 GMT
ADD file:195375389d64193c828c6d3f379c7e35ea85256eb1c51d2bfeab73432ea46064 in / 
# Wed, 13 Dec 2023 10:37:15 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:37:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:37:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:38:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:40:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:40:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ba68304511cfd178c72d64196a05b1343fbdbed6093d7b4db0c0d223510c40ab`  
		Last Modified: Sat, 16 Dec 2023 09:27:50 GMT  
		Size: 24.6 MB (24600972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5373ad55d8e8c0ab26bca9b592d8809358e69e59cff53121bcdd908a9f9639c`  
		Last Modified: Sat, 16 Dec 2023 09:50:09 GMT  
		Size: 1.2 MB (1199062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc25b246e660d5421dff1c723cfa2d5dfaa9c2ccfe1976b8fce4d4d1fedc8f5`  
		Last Modified: Sat, 16 Dec 2023 09:50:07 GMT  
		Size: 4.7 MB (4679510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4107a21097c89ac49236bbde53efe45ed4c81f1e01e65c2f0358d02b73486`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70488c95ce2761e3460cec20b973e12284798d5b20d16b9009f4352584dafdc6`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecfe88b9d5bac2517d37b869da63ba8b7baa4f12ca28f6d66809dd278d3b48b`  
		Last Modified: Sat, 16 Dec 2023 09:50:35 GMT  
		Size: 157.5 MB (157458423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b4028622de95be917a19e8013de1c97bde72b70b7382298556d8cf850713e`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b1d00726fd3fa46d77524a8053bd609365b5abae3a17a67f3683bf297ee8bd0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.6 MB (209551852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ef109a0615f2e6a12306ea2f79634e967bff0243f3dedb39dd1725cacedabe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:21:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:21:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:37:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 02:37:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV ROS_DISTRO=noetic
# Sat, 09 Dec 2023 02:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:40:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 09 Dec 2023 02:40:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 02:40:42 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2aa78ed8ad18394d7ae521e83b2810fec9fbb7d95aa074d794bb43e6e2bbfb`  
		Last Modified: Sat, 02 Dec 2023 06:56:12 GMT  
		Size: 1.2 MB (1198781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f106a95fef578814e019c4ac69f1cf32b15d5f85da2729a7ab2487c5d3505d`  
		Last Modified: Sat, 02 Dec 2023 06:56:11 GMT  
		Size: 5.5 MB (5532202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde5587588684db83e0c22fb5d4979df124ea1cb18322ace2e4c3ea5c96b6367`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c5b1b69c1b0400c6d51e9b08a29868443a22bc46ce96467a1b6fd75f9aa2c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c0f3f95aca8df1ff165733b239844d0700cbd97842b1699375b9137cd0075e`  
		Last Modified: Sat, 09 Dec 2023 03:56:30 GMT  
		Size: 175.6 MB (175614595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648bea585de95bdc098b0f496d2c461fc072dda803fe1be92b970893fd65443c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:973b57ee8b574e73dff0d325300087699c709aea0f1caea297073b03b651a2e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:a622251c8ca9faf0934a334226bd9e6a834e703cc692256e7598075afa3ad865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (269010853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9b7ad76d81130b0f13180698f8f21bd195bab51ce87e5996cb2e8b034f805e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 10:01:19 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Dec 2023 10:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 10:02:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 10:02:03 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 10:02:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 10:02:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 10:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98275009df19cd63037e51d5e5e08d572f414a5f83f29855904a397ebd75d2c9`  
		Last Modified: Sat, 16 Dec 2023 10:12:42 GMT  
		Size: 124.3 MB (124265338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8219eca9dd8e6069ed8f853817c0daed8f36c590be4dd038f29a08ebf2e867a7`  
		Last Modified: Sat, 16 Dec 2023 10:12:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27dc4d0e1602dc1a995fb217537671c6672edcaefd875900cd6b95529e18b50`  
		Last Modified: Sat, 16 Dec 2023 10:13:01 GMT  
		Size: 85.2 MB (85171231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2021430433a34f30f7577dc457480693a19277a672e32f30e122942183191eeb`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 302.4 KB (302360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192c516049c2ce35141ccefea9e40cf1312dbcf5328bd09c11706615aef6a66`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 2.5 KB (2476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1682439cc7c141ccfb75c63904f7b22f1930482b24f40000a074c36065060`  
		Last Modified: Sat, 16 Dec 2023 10:12:54 GMT  
		Size: 23.8 MB (23778395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cbd910dca67ae3ebfc6682b4ef7b1579b9d262ac26f859fe4baf7263e879050a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.6 MB (265571658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3280ac2e20a52720758d75352e44338afbcb8d05530ac0f9fd5b1373221ae1c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:44:43 GMT
ENV ROS_DISTRO=rolling
# Sat, 09 Dec 2023 03:45:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:45:25 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:45:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:45:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:46:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd15dfc8b58da909440d32361b5569fe381f290286d4437944659ab1f111dc7`  
		Last Modified: Sat, 09 Dec 2023 04:12:59 GMT  
		Size: 125.8 MB (125834956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10a1080ae60125887c9831085264830a2f4ab287db2dd7686f5a7e755df7c13`  
		Last Modified: Sat, 09 Dec 2023 04:12:34 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572c203fb61638e5b00d3de9e3bac0f4b598f4fde21a6f77f5771cca8a857d6`  
		Last Modified: Sat, 09 Dec 2023 04:13:18 GMT  
		Size: 82.8 MB (82848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766998918be38f758abf9473673311fbd57620dfcc63ff003401bf793f9d04ef`  
		Last Modified: Sat, 09 Dec 2023 04:13:09 GMT  
		Size: 302.2 KB (302206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c6ef4858e91a47e949495aaa6c7f8513680c0713bc96e7782e28528d59238e`  
		Last Modified: Sat, 09 Dec 2023 04:13:08 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09a62cc9bcd00dda0816010e2e73b5442c2f81f59fed40a75fd6e18d3cc9539`  
		Last Modified: Sat, 09 Dec 2023 04:13:13 GMT  
		Size: 23.2 MB (23165376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:f34b007ab7c0cb04e1ce0cff50a2f1415409be2c6bf435e3022e866bb51af303
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:6151ad7951a8781a34c97c005ce05f403078c7dcca16d706d9eef1093f61f1a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.9 MB (959929356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0718394ecbcd8ce13296e31b6308cf467656cdd700dee924fec354b7d5f5f5cc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 10:01:19 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Dec 2023 10:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 10:02:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 10:02:03 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 10:02:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 10:02:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 10:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:04:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98275009df19cd63037e51d5e5e08d572f414a5f83f29855904a397ebd75d2c9`  
		Last Modified: Sat, 16 Dec 2023 10:12:42 GMT  
		Size: 124.3 MB (124265338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8219eca9dd8e6069ed8f853817c0daed8f36c590be4dd038f29a08ebf2e867a7`  
		Last Modified: Sat, 16 Dec 2023 10:12:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27dc4d0e1602dc1a995fb217537671c6672edcaefd875900cd6b95529e18b50`  
		Last Modified: Sat, 16 Dec 2023 10:13:01 GMT  
		Size: 85.2 MB (85171231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2021430433a34f30f7577dc457480693a19277a672e32f30e122942183191eeb`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 302.4 KB (302360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192c516049c2ce35141ccefea9e40cf1312dbcf5328bd09c11706615aef6a66`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 2.5 KB (2476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1682439cc7c141ccfb75c63904f7b22f1930482b24f40000a074c36065060`  
		Last Modified: Sat, 16 Dec 2023 10:12:54 GMT  
		Size: 23.8 MB (23778395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57a4afd56de5507b6b4e4f069caaa8f53b58bae8cedfda1bb72aec1ebbc3043`  
		Last Modified: Sat, 16 Dec 2023 10:14:38 GMT  
		Size: 690.9 MB (690918503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4848289bf828700f36ca27dd9ee027cb7a924cc2b7eafcb911f806a36d28a247
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **924.3 MB (924328458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ace7eaf9ea07c3d1c369a8905bebb825bde9bdc5ea181558c8d3e34a801d5033`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:44:43 GMT
ENV ROS_DISTRO=rolling
# Sat, 09 Dec 2023 03:45:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:45:25 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:45:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:45:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:46:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:47:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd15dfc8b58da909440d32361b5569fe381f290286d4437944659ab1f111dc7`  
		Last Modified: Sat, 09 Dec 2023 04:12:59 GMT  
		Size: 125.8 MB (125834956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10a1080ae60125887c9831085264830a2f4ab287db2dd7686f5a7e755df7c13`  
		Last Modified: Sat, 09 Dec 2023 04:12:34 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572c203fb61638e5b00d3de9e3bac0f4b598f4fde21a6f77f5771cca8a857d6`  
		Last Modified: Sat, 09 Dec 2023 04:13:18 GMT  
		Size: 82.8 MB (82848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766998918be38f758abf9473673311fbd57620dfcc63ff003401bf793f9d04ef`  
		Last Modified: Sat, 09 Dec 2023 04:13:09 GMT  
		Size: 302.2 KB (302206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c6ef4858e91a47e949495aaa6c7f8513680c0713bc96e7782e28528d59238e`  
		Last Modified: Sat, 09 Dec 2023 04:13:08 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09a62cc9bcd00dda0816010e2e73b5442c2f81f59fed40a75fd6e18d3cc9539`  
		Last Modified: Sat, 09 Dec 2023 04:13:13 GMT  
		Size: 23.2 MB (23165376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab690d250573851195fd7fc3985e017fb5f1ae136e8ca590d98606b894d55795`  
		Last Modified: Sat, 09 Dec 2023 04:14:51 GMT  
		Size: 658.8 MB (658756800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:f34b007ab7c0cb04e1ce0cff50a2f1415409be2c6bf435e3022e866bb51af303
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:6151ad7951a8781a34c97c005ce05f403078c7dcca16d706d9eef1093f61f1a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.9 MB (959929356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0718394ecbcd8ce13296e31b6308cf467656cdd700dee924fec354b7d5f5f5cc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 10:01:19 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Dec 2023 10:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 10:02:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 10:02:03 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 10:02:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 10:02:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 10:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:04:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98275009df19cd63037e51d5e5e08d572f414a5f83f29855904a397ebd75d2c9`  
		Last Modified: Sat, 16 Dec 2023 10:12:42 GMT  
		Size: 124.3 MB (124265338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8219eca9dd8e6069ed8f853817c0daed8f36c590be4dd038f29a08ebf2e867a7`  
		Last Modified: Sat, 16 Dec 2023 10:12:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27dc4d0e1602dc1a995fb217537671c6672edcaefd875900cd6b95529e18b50`  
		Last Modified: Sat, 16 Dec 2023 10:13:01 GMT  
		Size: 85.2 MB (85171231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2021430433a34f30f7577dc457480693a19277a672e32f30e122942183191eeb`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 302.4 KB (302360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192c516049c2ce35141ccefea9e40cf1312dbcf5328bd09c11706615aef6a66`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 2.5 KB (2476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1682439cc7c141ccfb75c63904f7b22f1930482b24f40000a074c36065060`  
		Last Modified: Sat, 16 Dec 2023 10:12:54 GMT  
		Size: 23.8 MB (23778395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57a4afd56de5507b6b4e4f069caaa8f53b58bae8cedfda1bb72aec1ebbc3043`  
		Last Modified: Sat, 16 Dec 2023 10:14:38 GMT  
		Size: 690.9 MB (690918503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4848289bf828700f36ca27dd9ee027cb7a924cc2b7eafcb911f806a36d28a247
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **924.3 MB (924328458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ace7eaf9ea07c3d1c369a8905bebb825bde9bdc5ea181558c8d3e34a801d5033`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:44:43 GMT
ENV ROS_DISTRO=rolling
# Sat, 09 Dec 2023 03:45:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:45:25 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:45:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:45:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:46:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:47:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd15dfc8b58da909440d32361b5569fe381f290286d4437944659ab1f111dc7`  
		Last Modified: Sat, 09 Dec 2023 04:12:59 GMT  
		Size: 125.8 MB (125834956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10a1080ae60125887c9831085264830a2f4ab287db2dd7686f5a7e755df7c13`  
		Last Modified: Sat, 09 Dec 2023 04:12:34 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572c203fb61638e5b00d3de9e3bac0f4b598f4fde21a6f77f5771cca8a857d6`  
		Last Modified: Sat, 09 Dec 2023 04:13:18 GMT  
		Size: 82.8 MB (82848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766998918be38f758abf9473673311fbd57620dfcc63ff003401bf793f9d04ef`  
		Last Modified: Sat, 09 Dec 2023 04:13:09 GMT  
		Size: 302.2 KB (302206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c6ef4858e91a47e949495aaa6c7f8513680c0713bc96e7782e28528d59238e`  
		Last Modified: Sat, 09 Dec 2023 04:13:08 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09a62cc9bcd00dda0816010e2e73b5442c2f81f59fed40a75fd6e18d3cc9539`  
		Last Modified: Sat, 09 Dec 2023 04:13:13 GMT  
		Size: 23.2 MB (23165376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab690d250573851195fd7fc3985e017fb5f1ae136e8ca590d98606b894d55795`  
		Last Modified: Sat, 09 Dec 2023 04:14:51 GMT  
		Size: 658.8 MB (658756800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:973b57ee8b574e73dff0d325300087699c709aea0f1caea297073b03b651a2e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:a622251c8ca9faf0934a334226bd9e6a834e703cc692256e7598075afa3ad865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (269010853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9b7ad76d81130b0f13180698f8f21bd195bab51ce87e5996cb2e8b034f805e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 10:01:19 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Dec 2023 10:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 10:02:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 10:02:03 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 10:02:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 10:02:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 10:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98275009df19cd63037e51d5e5e08d572f414a5f83f29855904a397ebd75d2c9`  
		Last Modified: Sat, 16 Dec 2023 10:12:42 GMT  
		Size: 124.3 MB (124265338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8219eca9dd8e6069ed8f853817c0daed8f36c590be4dd038f29a08ebf2e867a7`  
		Last Modified: Sat, 16 Dec 2023 10:12:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27dc4d0e1602dc1a995fb217537671c6672edcaefd875900cd6b95529e18b50`  
		Last Modified: Sat, 16 Dec 2023 10:13:01 GMT  
		Size: 85.2 MB (85171231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2021430433a34f30f7577dc457480693a19277a672e32f30e122942183191eeb`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 302.4 KB (302360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192c516049c2ce35141ccefea9e40cf1312dbcf5328bd09c11706615aef6a66`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 2.5 KB (2476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1682439cc7c141ccfb75c63904f7b22f1930482b24f40000a074c36065060`  
		Last Modified: Sat, 16 Dec 2023 10:12:54 GMT  
		Size: 23.8 MB (23778395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cbd910dca67ae3ebfc6682b4ef7b1579b9d262ac26f859fe4baf7263e879050a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.6 MB (265571658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3280ac2e20a52720758d75352e44338afbcb8d05530ac0f9fd5b1373221ae1c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:44:43 GMT
ENV ROS_DISTRO=rolling
# Sat, 09 Dec 2023 03:45:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:45:25 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:45:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:45:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:46:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd15dfc8b58da909440d32361b5569fe381f290286d4437944659ab1f111dc7`  
		Last Modified: Sat, 09 Dec 2023 04:12:59 GMT  
		Size: 125.8 MB (125834956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10a1080ae60125887c9831085264830a2f4ab287db2dd7686f5a7e755df7c13`  
		Last Modified: Sat, 09 Dec 2023 04:12:34 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572c203fb61638e5b00d3de9e3bac0f4b598f4fde21a6f77f5771cca8a857d6`  
		Last Modified: Sat, 09 Dec 2023 04:13:18 GMT  
		Size: 82.8 MB (82848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766998918be38f758abf9473673311fbd57620dfcc63ff003401bf793f9d04ef`  
		Last Modified: Sat, 09 Dec 2023 04:13:09 GMT  
		Size: 302.2 KB (302206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c6ef4858e91a47e949495aaa6c7f8513680c0713bc96e7782e28528d59238e`  
		Last Modified: Sat, 09 Dec 2023 04:13:08 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09a62cc9bcd00dda0816010e2e73b5442c2f81f59fed40a75fd6e18d3cc9539`  
		Last Modified: Sat, 09 Dec 2023 04:13:13 GMT  
		Size: 23.2 MB (23165376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:973b57ee8b574e73dff0d325300087699c709aea0f1caea297073b03b651a2e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:a622251c8ca9faf0934a334226bd9e6a834e703cc692256e7598075afa3ad865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (269010853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9b7ad76d81130b0f13180698f8f21bd195bab51ce87e5996cb2e8b034f805e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 10:01:19 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Dec 2023 10:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 10:02:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 10:02:03 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 10:02:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 10:02:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Dec 2023 10:02:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98275009df19cd63037e51d5e5e08d572f414a5f83f29855904a397ebd75d2c9`  
		Last Modified: Sat, 16 Dec 2023 10:12:42 GMT  
		Size: 124.3 MB (124265338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8219eca9dd8e6069ed8f853817c0daed8f36c590be4dd038f29a08ebf2e867a7`  
		Last Modified: Sat, 16 Dec 2023 10:12:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27dc4d0e1602dc1a995fb217537671c6672edcaefd875900cd6b95529e18b50`  
		Last Modified: Sat, 16 Dec 2023 10:13:01 GMT  
		Size: 85.2 MB (85171231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2021430433a34f30f7577dc457480693a19277a672e32f30e122942183191eeb`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 302.4 KB (302360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192c516049c2ce35141ccefea9e40cf1312dbcf5328bd09c11706615aef6a66`  
		Last Modified: Sat, 16 Dec 2023 10:12:50 GMT  
		Size: 2.5 KB (2476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1682439cc7c141ccfb75c63904f7b22f1930482b24f40000a074c36065060`  
		Last Modified: Sat, 16 Dec 2023 10:12:54 GMT  
		Size: 23.8 MB (23778395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cbd910dca67ae3ebfc6682b4ef7b1579b9d262ac26f859fe4baf7263e879050a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.6 MB (265571658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3280ac2e20a52720758d75352e44338afbcb8d05530ac0f9fd5b1373221ae1c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:44:43 GMT
ENV ROS_DISTRO=rolling
# Sat, 09 Dec 2023 03:45:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:45:25 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 03:45:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 09 Dec 2023 03:45:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 09 Dec 2023 03:46:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd15dfc8b58da909440d32361b5569fe381f290286d4437944659ab1f111dc7`  
		Last Modified: Sat, 09 Dec 2023 04:12:59 GMT  
		Size: 125.8 MB (125834956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10a1080ae60125887c9831085264830a2f4ab287db2dd7686f5a7e755df7c13`  
		Last Modified: Sat, 09 Dec 2023 04:12:34 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572c203fb61638e5b00d3de9e3bac0f4b598f4fde21a6f77f5771cca8a857d6`  
		Last Modified: Sat, 09 Dec 2023 04:13:18 GMT  
		Size: 82.8 MB (82848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766998918be38f758abf9473673311fbd57620dfcc63ff003401bf793f9d04ef`  
		Last Modified: Sat, 09 Dec 2023 04:13:09 GMT  
		Size: 302.2 KB (302206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c6ef4858e91a47e949495aaa6c7f8513680c0713bc96e7782e28528d59238e`  
		Last Modified: Sat, 09 Dec 2023 04:13:08 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09a62cc9bcd00dda0816010e2e73b5442c2f81f59fed40a75fd6e18d3cc9539`  
		Last Modified: Sat, 09 Dec 2023 04:13:13 GMT  
		Size: 23.2 MB (23165376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:36d1aca2cf670f4e9b16c2021a1340cd0c7e902e8b6830c8319414367d7023ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:20fd0776c5588c51efb53ffd1037b107a8601fcad9a41dbc8abcaf2a602f3c64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.8 MB (159756391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8e995011741325e0828dacff2e6e021e61aff79c9ee1d4e66164428987d2a2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 10:01:19 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Dec 2023 10:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 10:02:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 10:02:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98275009df19cd63037e51d5e5e08d572f414a5f83f29855904a397ebd75d2c9`  
		Last Modified: Sat, 16 Dec 2023 10:12:42 GMT  
		Size: 124.3 MB (124265338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8219eca9dd8e6069ed8f853817c0daed8f36c590be4dd038f29a08ebf2e867a7`  
		Last Modified: Sat, 16 Dec 2023 10:12:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1b2f3360f79f3023923bc3b16c31f75dbe31e86333cbabdd974ab025a0e0b767
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.3 MB (159253568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3bc41593c96be1bcc32822e3921c9b89b75d48db992ff1503d7206edea4abc9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:44:43 GMT
ENV ROS_DISTRO=rolling
# Sat, 09 Dec 2023 03:45:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:45:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd15dfc8b58da909440d32361b5569fe381f290286d4437944659ab1f111dc7`  
		Last Modified: Sat, 09 Dec 2023 04:12:59 GMT  
		Size: 125.8 MB (125834956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10a1080ae60125887c9831085264830a2f4ab287db2dd7686f5a7e755df7c13`  
		Last Modified: Sat, 09 Dec 2023 04:12:34 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:36d1aca2cf670f4e9b16c2021a1340cd0c7e902e8b6830c8319414367d7023ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:20fd0776c5588c51efb53ffd1037b107a8601fcad9a41dbc8abcaf2a602f3c64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.8 MB (159756391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8e995011741325e0828dacff2e6e021e61aff79c9ee1d4e66164428987d2a2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:47:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:47:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:47:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:47:09 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 10:01:19 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Dec 2023 10:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:02:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 16 Dec 2023 10:02:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 10:02:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e86ad086b67313d4c63edb54bf2739950b802e91ebad161233ae79cff83b4`  
		Last Modified: Sat, 16 Dec 2023 10:07:37 GMT  
		Size: 1.2 MB (1213112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f66abb2468094dfcd781577a433d6fc74be14642bfe0f0b63ac67cce0679d29`  
		Last Modified: Sat, 16 Dec 2023 10:07:35 GMT  
		Size: 3.8 MB (3828953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4d4129a1bd712f495f49388f1c237a1e5ff7500d95497da5c895c1a99d1bf`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faca2ff023aa84f963f8ab3b5d4201af5875210a7faf28361f4a988b79f42eb`  
		Last Modified: Sat, 16 Dec 2023 10:07:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98275009df19cd63037e51d5e5e08d572f414a5f83f29855904a397ebd75d2c9`  
		Last Modified: Sat, 16 Dec 2023 10:12:42 GMT  
		Size: 124.3 MB (124265338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8219eca9dd8e6069ed8f853817c0daed8f36c590be4dd038f29a08ebf2e867a7`  
		Last Modified: Sat, 16 Dec 2023 10:12:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1b2f3360f79f3023923bc3b16c31f75dbe31e86333cbabdd974ab025a0e0b767
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.3 MB (159253568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3bc41593c96be1bcc32822e3921c9b89b75d48db992ff1503d7206edea4abc9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:36:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:36:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:26:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 03:26:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 03:26:35 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 03:44:43 GMT
ENV ROS_DISTRO=rolling
# Sat, 09 Dec 2023 03:45:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 03:45:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 09 Dec 2023 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 03:45:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ce86a03a18f78cf25cdf581531142e7367f0fe08a1fdd01402d6c7f4ce8d2b`  
		Last Modified: Sat, 02 Dec 2023 06:58:34 GMT  
		Size: 1.2 MB (1214421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8480855a5f2a943f3f15f49e414e94fa9a8a0ad577b7c9d09b27005d302b32b`  
		Last Modified: Sat, 02 Dec 2023 06:58:32 GMT  
		Size: 3.8 MB (3801844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247041a3c82a275fcd35663dc8f27e9bc46099c0eca866f2a2e681bab1a7a51e`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2995a5554b05abb8e45be71dc37311fbd85ba0defe04664d65193e81ed735c`  
		Last Modified: Sat, 09 Dec 2023 04:07:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd15dfc8b58da909440d32361b5569fe381f290286d4437944659ab1f111dc7`  
		Last Modified: Sat, 09 Dec 2023 04:12:59 GMT  
		Size: 125.8 MB (125834956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10a1080ae60125887c9831085264830a2f4ab287db2dd7686f5a7e755df7c13`  
		Last Modified: Sat, 09 Dec 2023 04:12:34 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
