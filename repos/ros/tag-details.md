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
$ docker pull ros@sha256:4654de0b83601ee9ba956b2f577bc565fcfd835ca24517e2a951829fa240240e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:3386540ad674d7bfb39325a2149be58b014e815eeff7a66cccbc780396ae3127
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263161054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c5b16395dfe505769d26b47f928ae646c2131a887ebffa63e5b7a65cd71d51`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 03:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:43:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:43:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:43:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:44:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:44:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:44:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:44:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbaaf0d07ce9923344bb5649335dc9cb1d9d75b9072a4184813e3b6e96cb98c`  
		Last Modified: Fri, 16 Jun 2023 04:03:50 GMT  
		Size: 106.3 MB (106346667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40d88d0af61448739222d5fd5bd85608277cce56a574273ff20a89fafee8515`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06384a5e54f3042dafc74cc55288bce3a86696a3c17cf79b130581cdd63910b`  
		Last Modified: Fri, 16 Jun 2023 04:04:12 GMT  
		Size: 97.9 MB (97949822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e750d54d785aa1696c573420a62fbb7249cde12d2084a2fab4201df081b90eb7`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 304.7 KB (304732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d351a048bcc5f2d84a3e60e35390a6f29c2da9dd56e1d7478de0b6015895c42`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d66d96470f76515998af23908ea849dca005a88cdf897bde234aa1a43bdd548`  
		Last Modified: Fri, 16 Jun 2023 04:04:03 GMT  
		Size: 23.1 MB (23082395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b4ae4682141d9624af5809f23a0a29d1d3a7dc5b4b7def019fed5b698e1b68d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255900791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2042c6cf46a0742277ab1a4b86e3785f5a7201c35a1960c7c56de6f566b24eb1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 01:24:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:24:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:24:14 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:25:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:25:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:25:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:26:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd26ad58cb49fafe39c24b3bac2e32d04bfee88571404562a416d9a0b6e0e78`  
		Last Modified: Fri, 16 Jun 2023 01:47:20 GMT  
		Size: 104.1 MB (104105616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd9359913df651c74c9e52f793ef0787865e50d9d61a4515ec8ef65c3d8ae3`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4d0b2bfe8969ffafd9009e3ee13526ff43c422fd23b56b102cfe070bfbeb1d`  
		Last Modified: Fri, 16 Jun 2023 01:47:40 GMT  
		Size: 95.6 MB (95581977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6528dc26f11a52b5d26d871d234047f129fdfd2736560765c9b8918ab231f9ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:29 GMT  
		Size: 304.7 KB (304728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f858a72b36e06d019e79b66337b74798e8b8128d7e7011e4651167c411dd94`  
		Last Modified: Fri, 16 Jun 2023 01:47:28 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a104ce69ef6960d329543d66bbb31b14c8efcbd03ca03fb5685f111378d86ac`  
		Last Modified: Fri, 16 Jun 2023 01:47:32 GMT  
		Size: 22.5 MB (22499835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:af99f3d4a5e38bd2e7faa015bb7bf8fbdc5c9fa06666c7d46634aab0d27673e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:ec8953a89ab8dfe1738c60f681534607bdcc857bf31b4ea08287f0591c2c037e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **952.3 MB (952254277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f1eea91da5ca26679b3aca584a5c533050fd4bfba081b9fd25a24246217f1c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 03:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:43:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:43:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:43:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:44:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:44:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:44:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:44:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:52:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbaaf0d07ce9923344bb5649335dc9cb1d9d75b9072a4184813e3b6e96cb98c`  
		Last Modified: Fri, 16 Jun 2023 04:03:50 GMT  
		Size: 106.3 MB (106346667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40d88d0af61448739222d5fd5bd85608277cce56a574273ff20a89fafee8515`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06384a5e54f3042dafc74cc55288bce3a86696a3c17cf79b130581cdd63910b`  
		Last Modified: Fri, 16 Jun 2023 04:04:12 GMT  
		Size: 97.9 MB (97949822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e750d54d785aa1696c573420a62fbb7249cde12d2084a2fab4201df081b90eb7`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 304.7 KB (304732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d351a048bcc5f2d84a3e60e35390a6f29c2da9dd56e1d7478de0b6015895c42`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d66d96470f76515998af23908ea849dca005a88cdf897bde234aa1a43bdd548`  
		Last Modified: Fri, 16 Jun 2023 04:04:03 GMT  
		Size: 23.1 MB (23082395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ee2fdbc06c020771b437e47cef5bc8e78aa40bd8ff770ee5c16e8dec7929b6`  
		Last Modified: Fri, 16 Jun 2023 04:05:52 GMT  
		Size: 689.1 MB (689093223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d61b92432b6a90161c3d9c3a28b65566ffe68ca5ce5b428e70f6106ac472a082
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **913.7 MB (913737173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ba2bd65a665f8203e1563ae808861cd7fc69e386ea751667e890a279a27a3a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 01:24:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:24:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:24:14 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:25:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:25:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:25:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:26:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:35:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd26ad58cb49fafe39c24b3bac2e32d04bfee88571404562a416d9a0b6e0e78`  
		Last Modified: Fri, 16 Jun 2023 01:47:20 GMT  
		Size: 104.1 MB (104105616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd9359913df651c74c9e52f793ef0787865e50d9d61a4515ec8ef65c3d8ae3`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4d0b2bfe8969ffafd9009e3ee13526ff43c422fd23b56b102cfe070bfbeb1d`  
		Last Modified: Fri, 16 Jun 2023 01:47:40 GMT  
		Size: 95.6 MB (95581977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6528dc26f11a52b5d26d871d234047f129fdfd2736560765c9b8918ab231f9ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:29 GMT  
		Size: 304.7 KB (304728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f858a72b36e06d019e79b66337b74798e8b8128d7e7011e4651167c411dd94`  
		Last Modified: Fri, 16 Jun 2023 01:47:28 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a104ce69ef6960d329543d66bbb31b14c8efcbd03ca03fb5685f111378d86ac`  
		Last Modified: Fri, 16 Jun 2023 01:47:32 GMT  
		Size: 22.5 MB (22499835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a3a320c361d7ba357e063be93adb6916fbffd603207bcd22bdd214870f1be1`  
		Last Modified: Fri, 16 Jun 2023 01:49:15 GMT  
		Size: 657.8 MB (657836382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:af99f3d4a5e38bd2e7faa015bb7bf8fbdc5c9fa06666c7d46634aab0d27673e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:ec8953a89ab8dfe1738c60f681534607bdcc857bf31b4ea08287f0591c2c037e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **952.3 MB (952254277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f1eea91da5ca26679b3aca584a5c533050fd4bfba081b9fd25a24246217f1c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 03:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:43:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:43:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:43:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:44:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:44:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:44:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:44:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:52:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbaaf0d07ce9923344bb5649335dc9cb1d9d75b9072a4184813e3b6e96cb98c`  
		Last Modified: Fri, 16 Jun 2023 04:03:50 GMT  
		Size: 106.3 MB (106346667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40d88d0af61448739222d5fd5bd85608277cce56a574273ff20a89fafee8515`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06384a5e54f3042dafc74cc55288bce3a86696a3c17cf79b130581cdd63910b`  
		Last Modified: Fri, 16 Jun 2023 04:04:12 GMT  
		Size: 97.9 MB (97949822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e750d54d785aa1696c573420a62fbb7249cde12d2084a2fab4201df081b90eb7`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 304.7 KB (304732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d351a048bcc5f2d84a3e60e35390a6f29c2da9dd56e1d7478de0b6015895c42`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d66d96470f76515998af23908ea849dca005a88cdf897bde234aa1a43bdd548`  
		Last Modified: Fri, 16 Jun 2023 04:04:03 GMT  
		Size: 23.1 MB (23082395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ee2fdbc06c020771b437e47cef5bc8e78aa40bd8ff770ee5c16e8dec7929b6`  
		Last Modified: Fri, 16 Jun 2023 04:05:52 GMT  
		Size: 689.1 MB (689093223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d61b92432b6a90161c3d9c3a28b65566ffe68ca5ce5b428e70f6106ac472a082
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **913.7 MB (913737173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ba2bd65a665f8203e1563ae808861cd7fc69e386ea751667e890a279a27a3a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 01:24:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:24:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:24:14 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:25:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:25:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:25:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:26:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:35:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd26ad58cb49fafe39c24b3bac2e32d04bfee88571404562a416d9a0b6e0e78`  
		Last Modified: Fri, 16 Jun 2023 01:47:20 GMT  
		Size: 104.1 MB (104105616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd9359913df651c74c9e52f793ef0787865e50d9d61a4515ec8ef65c3d8ae3`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4d0b2bfe8969ffafd9009e3ee13526ff43c422fd23b56b102cfe070bfbeb1d`  
		Last Modified: Fri, 16 Jun 2023 01:47:40 GMT  
		Size: 95.6 MB (95581977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6528dc26f11a52b5d26d871d234047f129fdfd2736560765c9b8918ab231f9ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:29 GMT  
		Size: 304.7 KB (304728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f858a72b36e06d019e79b66337b74798e8b8128d7e7011e4651167c411dd94`  
		Last Modified: Fri, 16 Jun 2023 01:47:28 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a104ce69ef6960d329543d66bbb31b14c8efcbd03ca03fb5685f111378d86ac`  
		Last Modified: Fri, 16 Jun 2023 01:47:32 GMT  
		Size: 22.5 MB (22499835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a3a320c361d7ba357e063be93adb6916fbffd603207bcd22bdd214870f1be1`  
		Last Modified: Fri, 16 Jun 2023 01:49:15 GMT  
		Size: 657.8 MB (657836382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:4654de0b83601ee9ba956b2f577bc565fcfd835ca24517e2a951829fa240240e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:3386540ad674d7bfb39325a2149be58b014e815eeff7a66cccbc780396ae3127
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263161054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c5b16395dfe505769d26b47f928ae646c2131a887ebffa63e5b7a65cd71d51`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 03:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:43:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:43:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:43:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:44:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:44:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:44:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:44:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbaaf0d07ce9923344bb5649335dc9cb1d9d75b9072a4184813e3b6e96cb98c`  
		Last Modified: Fri, 16 Jun 2023 04:03:50 GMT  
		Size: 106.3 MB (106346667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40d88d0af61448739222d5fd5bd85608277cce56a574273ff20a89fafee8515`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06384a5e54f3042dafc74cc55288bce3a86696a3c17cf79b130581cdd63910b`  
		Last Modified: Fri, 16 Jun 2023 04:04:12 GMT  
		Size: 97.9 MB (97949822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e750d54d785aa1696c573420a62fbb7249cde12d2084a2fab4201df081b90eb7`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 304.7 KB (304732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d351a048bcc5f2d84a3e60e35390a6f29c2da9dd56e1d7478de0b6015895c42`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d66d96470f76515998af23908ea849dca005a88cdf897bde234aa1a43bdd548`  
		Last Modified: Fri, 16 Jun 2023 04:04:03 GMT  
		Size: 23.1 MB (23082395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b4ae4682141d9624af5809f23a0a29d1d3a7dc5b4b7def019fed5b698e1b68d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255900791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2042c6cf46a0742277ab1a4b86e3785f5a7201c35a1960c7c56de6f566b24eb1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 01:24:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:24:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:24:14 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:25:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:25:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:25:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:26:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd26ad58cb49fafe39c24b3bac2e32d04bfee88571404562a416d9a0b6e0e78`  
		Last Modified: Fri, 16 Jun 2023 01:47:20 GMT  
		Size: 104.1 MB (104105616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd9359913df651c74c9e52f793ef0787865e50d9d61a4515ec8ef65c3d8ae3`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4d0b2bfe8969ffafd9009e3ee13526ff43c422fd23b56b102cfe070bfbeb1d`  
		Last Modified: Fri, 16 Jun 2023 01:47:40 GMT  
		Size: 95.6 MB (95581977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6528dc26f11a52b5d26d871d234047f129fdfd2736560765c9b8918ab231f9ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:29 GMT  
		Size: 304.7 KB (304728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f858a72b36e06d019e79b66337b74798e8b8128d7e7011e4651167c411dd94`  
		Last Modified: Fri, 16 Jun 2023 01:47:28 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a104ce69ef6960d329543d66bbb31b14c8efcbd03ca03fb5685f111378d86ac`  
		Last Modified: Fri, 16 Jun 2023 01:47:32 GMT  
		Size: 22.5 MB (22499835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:4654de0b83601ee9ba956b2f577bc565fcfd835ca24517e2a951829fa240240e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:3386540ad674d7bfb39325a2149be58b014e815eeff7a66cccbc780396ae3127
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263161054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c5b16395dfe505769d26b47f928ae646c2131a887ebffa63e5b7a65cd71d51`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 03:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:43:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:43:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:43:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:44:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:44:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:44:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:44:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbaaf0d07ce9923344bb5649335dc9cb1d9d75b9072a4184813e3b6e96cb98c`  
		Last Modified: Fri, 16 Jun 2023 04:03:50 GMT  
		Size: 106.3 MB (106346667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40d88d0af61448739222d5fd5bd85608277cce56a574273ff20a89fafee8515`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06384a5e54f3042dafc74cc55288bce3a86696a3c17cf79b130581cdd63910b`  
		Last Modified: Fri, 16 Jun 2023 04:04:12 GMT  
		Size: 97.9 MB (97949822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e750d54d785aa1696c573420a62fbb7249cde12d2084a2fab4201df081b90eb7`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 304.7 KB (304732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d351a048bcc5f2d84a3e60e35390a6f29c2da9dd56e1d7478de0b6015895c42`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d66d96470f76515998af23908ea849dca005a88cdf897bde234aa1a43bdd548`  
		Last Modified: Fri, 16 Jun 2023 04:04:03 GMT  
		Size: 23.1 MB (23082395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b4ae4682141d9624af5809f23a0a29d1d3a7dc5b4b7def019fed5b698e1b68d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255900791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2042c6cf46a0742277ab1a4b86e3785f5a7201c35a1960c7c56de6f566b24eb1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 01:24:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:24:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:24:14 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:25:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:25:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:25:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:26:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd26ad58cb49fafe39c24b3bac2e32d04bfee88571404562a416d9a0b6e0e78`  
		Last Modified: Fri, 16 Jun 2023 01:47:20 GMT  
		Size: 104.1 MB (104105616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd9359913df651c74c9e52f793ef0787865e50d9d61a4515ec8ef65c3d8ae3`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4d0b2bfe8969ffafd9009e3ee13526ff43c422fd23b56b102cfe070bfbeb1d`  
		Last Modified: Fri, 16 Jun 2023 01:47:40 GMT  
		Size: 95.6 MB (95581977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6528dc26f11a52b5d26d871d234047f129fdfd2736560765c9b8918ab231f9ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:29 GMT  
		Size: 304.7 KB (304728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f858a72b36e06d019e79b66337b74798e8b8128d7e7011e4651167c411dd94`  
		Last Modified: Fri, 16 Jun 2023 01:47:28 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a104ce69ef6960d329543d66bbb31b14c8efcbd03ca03fb5685f111378d86ac`  
		Last Modified: Fri, 16 Jun 2023 01:47:32 GMT  
		Size: 22.5 MB (22499835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:c8df40b8e9f13776b2235a0d1e693d545e668378ad727863bf4d28ccf65a0bf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:f7ef48f81f85002b43232085036aec373a85ad61598dd54377b6da36001225f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141821695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9711169d734ddeb793a10d6a574a3684c654ac287e0326028f8ab175ff018fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 03:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:43:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:43:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:43:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbaaf0d07ce9923344bb5649335dc9cb1d9d75b9072a4184813e3b6e96cb98c`  
		Last Modified: Fri, 16 Jun 2023 04:03:50 GMT  
		Size: 106.3 MB (106346667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40d88d0af61448739222d5fd5bd85608277cce56a574273ff20a89fafee8515`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b31f2fae8410afe0c74ab102763105e2ec5da8e27d979a8db9e7024041696706
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137511828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aa16bdb00e99e3333019911ea2398f2589753729bf9a4438a2d6d709edb44a5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 01:24:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:24:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:24:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd26ad58cb49fafe39c24b3bac2e32d04bfee88571404562a416d9a0b6e0e78`  
		Last Modified: Fri, 16 Jun 2023 01:47:20 GMT  
		Size: 104.1 MB (104105616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd9359913df651c74c9e52f793ef0787865e50d9d61a4515ec8ef65c3d8ae3`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:c8df40b8e9f13776b2235a0d1e693d545e668378ad727863bf4d28ccf65a0bf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:f7ef48f81f85002b43232085036aec373a85ad61598dd54377b6da36001225f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141821695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9711169d734ddeb793a10d6a574a3684c654ac287e0326028f8ab175ff018fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 03:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:43:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:43:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:43:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbaaf0d07ce9923344bb5649335dc9cb1d9d75b9072a4184813e3b6e96cb98c`  
		Last Modified: Fri, 16 Jun 2023 04:03:50 GMT  
		Size: 106.3 MB (106346667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40d88d0af61448739222d5fd5bd85608277cce56a574273ff20a89fafee8515`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b31f2fae8410afe0c74ab102763105e2ec5da8e27d979a8db9e7024041696706
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137511828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aa16bdb00e99e3333019911ea2398f2589753729bf9a4438a2d6d709edb44a5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 01:24:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:24:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:24:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd26ad58cb49fafe39c24b3bac2e32d04bfee88571404562a416d9a0b6e0e78`  
		Last Modified: Fri, 16 Jun 2023 01:47:20 GMT  
		Size: 104.1 MB (104105616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd9359913df651c74c9e52f793ef0787865e50d9d61a4515ec8ef65c3d8ae3`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron`

```console
$ docker pull ros@sha256:4bc6a75bdfc1787088a373b07f851fe41e57198dfa8f48f2febae2e4e233a65c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron` - linux; amd64

```console
$ docker pull ros@sha256:69399d4a82e41cf4c2fcd751886c1ccc472ac27c115b0d3ec62678d46dd6ee90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268561480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8223749b08214cbaf072ef59fa30f69d3662e7152a145f23e1e49634b5178ad3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:52:41 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 03:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:53:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:53:26 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:53:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:53:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9a4b6088658276f8fd1f323dccdcbb861073b76cd6349072032f5fdaa2308b`  
		Last Modified: Fri, 16 Jun 2023 04:06:19 GMT  
		Size: 124.1 MB (124124424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e6f6e49e9b268b418486630a7ba4b97c13b80a80f9264b2a655e0f0a395d7`  
		Last Modified: Fri, 16 Jun 2023 04:06:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439087c92f7f6e12a142bd39dc7cb8a1ca5d69f39bb6fd3ca975acb89c9d6ac`  
		Last Modified: Fri, 16 Jun 2023 04:06:39 GMT  
		Size: 85.0 MB (84994710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34237af467a507ca4d19e10a051e77c334109ef97c28f8df3d0138188d5facf0`  
		Last Modified: Fri, 16 Jun 2023 04:06:28 GMT  
		Size: 291.6 KB (291640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8439ca8819e994b1e7dcd6debd7f51f0c0ca681463f29e88c0d676fba1637630`  
		Last Modified: Fri, 16 Jun 2023 04:06:28 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc933ad7e1ecb3369fd1ba6557a11d42c83c4fb1e3dedafecc4dd69606c3b4b0`  
		Last Modified: Fri, 16 Jun 2023 04:06:32 GMT  
		Size: 23.7 MB (23673251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0662819c52a556bc9eab61c8938cffaa034a0a52f5c4eb35e411ceb1010fa7d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261115629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b057980795b54497e34d2dc0a3f187b5e9dc87acd145f870ea1130bde0ee15a2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:36:04 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 01:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:36:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:36:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:36:51 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:37:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:37:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:37:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:37:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e41c2e8b43236d79b82b2ce24c1f568a4a3ea25c30dfdc4895cce00480072`  
		Last Modified: Fri, 16 Jun 2023 01:49:43 GMT  
		Size: 121.6 MB (121612466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14e36042bc13bfe0d1c0fb91a96ad3ed768c36fbac710c2082179a1022f1da`  
		Last Modified: Fri, 16 Jun 2023 01:49:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dd2b650fb1c286b3dff3669c7aae3e05912b51d94d17eb5a407cd00018441f`  
		Last Modified: Fri, 16 Jun 2023 01:50:00 GMT  
		Size: 82.7 MB (82735938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e705dd681bbe2976d37a56a63de3fca5f64f664bf74df5f44d55cf7594f220`  
		Last Modified: Fri, 16 Jun 2023 01:49:52 GMT  
		Size: 291.6 KB (291642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55bffa5d4241cc12158e182f1f2911c4259e7fe2223cb64d6de2ebdd44fdc9f`  
		Last Modified: Fri, 16 Jun 2023 01:49:52 GMT  
		Size: 2.4 KB (2425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad30b122e91303d3344340a62434a315fded6e665b21c6e58c5c0d3e37eafe`  
		Last Modified: Fri, 16 Jun 2023 01:49:56 GMT  
		Size: 23.1 MB (23066945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-perception`

```console
$ docker pull ros@sha256:260a2a092220cf47c697c857fe236880800095cfad491f01ed39b7ae1dc97eb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-perception` - linux; amd64

```console
$ docker pull ros@sha256:3fde4d5abb69e4d10106af4a7334fc4a412b49fd2874c7ec8e37a0640d04bb04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **958.3 MB (958317463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f910b2235d88f9a769d3409daf7d779650461dc4c65d6dc690c5fcfc64d456`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:52:41 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 03:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:53:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:53:26 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:53:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:53:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:55:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9a4b6088658276f8fd1f323dccdcbb861073b76cd6349072032f5fdaa2308b`  
		Last Modified: Fri, 16 Jun 2023 04:06:19 GMT  
		Size: 124.1 MB (124124424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e6f6e49e9b268b418486630a7ba4b97c13b80a80f9264b2a655e0f0a395d7`  
		Last Modified: Fri, 16 Jun 2023 04:06:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439087c92f7f6e12a142bd39dc7cb8a1ca5d69f39bb6fd3ca975acb89c9d6ac`  
		Last Modified: Fri, 16 Jun 2023 04:06:39 GMT  
		Size: 85.0 MB (84994710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34237af467a507ca4d19e10a051e77c334109ef97c28f8df3d0138188d5facf0`  
		Last Modified: Fri, 16 Jun 2023 04:06:28 GMT  
		Size: 291.6 KB (291640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8439ca8819e994b1e7dcd6debd7f51f0c0ca681463f29e88c0d676fba1637630`  
		Last Modified: Fri, 16 Jun 2023 04:06:28 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc933ad7e1ecb3369fd1ba6557a11d42c83c4fb1e3dedafecc4dd69606c3b4b0`  
		Last Modified: Fri, 16 Jun 2023 04:06:32 GMT  
		Size: 23.7 MB (23673251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea445e950d5ff71f0dca0f2722e50be59d87f2c3309d0e5b1293381c7cce2451`  
		Last Modified: Fri, 16 Jun 2023 04:08:17 GMT  
		Size: 689.8 MB (689755983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a1000b5ce8f9065076303a1bf27a4a1f5cdd78b88dca83a3803ae55a3753a4bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **919.6 MB (919579173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f163a9bf133a35e8875b769adaae4a497ce581544ecce46376555301d5b60c7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:36:04 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 01:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:36:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:36:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:36:51 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:37:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:37:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:37:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:37:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:39:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e41c2e8b43236d79b82b2ce24c1f568a4a3ea25c30dfdc4895cce00480072`  
		Last Modified: Fri, 16 Jun 2023 01:49:43 GMT  
		Size: 121.6 MB (121612466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14e36042bc13bfe0d1c0fb91a96ad3ed768c36fbac710c2082179a1022f1da`  
		Last Modified: Fri, 16 Jun 2023 01:49:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dd2b650fb1c286b3dff3669c7aae3e05912b51d94d17eb5a407cd00018441f`  
		Last Modified: Fri, 16 Jun 2023 01:50:00 GMT  
		Size: 82.7 MB (82735938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e705dd681bbe2976d37a56a63de3fca5f64f664bf74df5f44d55cf7594f220`  
		Last Modified: Fri, 16 Jun 2023 01:49:52 GMT  
		Size: 291.6 KB (291642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55bffa5d4241cc12158e182f1f2911c4259e7fe2223cb64d6de2ebdd44fdc9f`  
		Last Modified: Fri, 16 Jun 2023 01:49:52 GMT  
		Size: 2.4 KB (2425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad30b122e91303d3344340a62434a315fded6e665b21c6e58c5c0d3e37eafe`  
		Last Modified: Fri, 16 Jun 2023 01:49:56 GMT  
		Size: 23.1 MB (23066945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de9f4e16e2bf2315ed74154cad4b2811feb72a14d500ce2ce263fdc05282000`  
		Last Modified: Fri, 16 Jun 2023 01:51:33 GMT  
		Size: 658.5 MB (658463544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-perception-jammy`

```console
$ docker pull ros@sha256:260a2a092220cf47c697c857fe236880800095cfad491f01ed39b7ae1dc97eb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:3fde4d5abb69e4d10106af4a7334fc4a412b49fd2874c7ec8e37a0640d04bb04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **958.3 MB (958317463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f910b2235d88f9a769d3409daf7d779650461dc4c65d6dc690c5fcfc64d456`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:52:41 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 03:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:53:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:53:26 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:53:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:53:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:55:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9a4b6088658276f8fd1f323dccdcbb861073b76cd6349072032f5fdaa2308b`  
		Last Modified: Fri, 16 Jun 2023 04:06:19 GMT  
		Size: 124.1 MB (124124424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e6f6e49e9b268b418486630a7ba4b97c13b80a80f9264b2a655e0f0a395d7`  
		Last Modified: Fri, 16 Jun 2023 04:06:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439087c92f7f6e12a142bd39dc7cb8a1ca5d69f39bb6fd3ca975acb89c9d6ac`  
		Last Modified: Fri, 16 Jun 2023 04:06:39 GMT  
		Size: 85.0 MB (84994710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34237af467a507ca4d19e10a051e77c334109ef97c28f8df3d0138188d5facf0`  
		Last Modified: Fri, 16 Jun 2023 04:06:28 GMT  
		Size: 291.6 KB (291640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8439ca8819e994b1e7dcd6debd7f51f0c0ca681463f29e88c0d676fba1637630`  
		Last Modified: Fri, 16 Jun 2023 04:06:28 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc933ad7e1ecb3369fd1ba6557a11d42c83c4fb1e3dedafecc4dd69606c3b4b0`  
		Last Modified: Fri, 16 Jun 2023 04:06:32 GMT  
		Size: 23.7 MB (23673251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea445e950d5ff71f0dca0f2722e50be59d87f2c3309d0e5b1293381c7cce2451`  
		Last Modified: Fri, 16 Jun 2023 04:08:17 GMT  
		Size: 689.8 MB (689755983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a1000b5ce8f9065076303a1bf27a4a1f5cdd78b88dca83a3803ae55a3753a4bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **919.6 MB (919579173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f163a9bf133a35e8875b769adaae4a497ce581544ecce46376555301d5b60c7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:36:04 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 01:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:36:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:36:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:36:51 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:37:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:37:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:37:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:37:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:39:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e41c2e8b43236d79b82b2ce24c1f568a4a3ea25c30dfdc4895cce00480072`  
		Last Modified: Fri, 16 Jun 2023 01:49:43 GMT  
		Size: 121.6 MB (121612466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14e36042bc13bfe0d1c0fb91a96ad3ed768c36fbac710c2082179a1022f1da`  
		Last Modified: Fri, 16 Jun 2023 01:49:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dd2b650fb1c286b3dff3669c7aae3e05912b51d94d17eb5a407cd00018441f`  
		Last Modified: Fri, 16 Jun 2023 01:50:00 GMT  
		Size: 82.7 MB (82735938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e705dd681bbe2976d37a56a63de3fca5f64f664bf74df5f44d55cf7594f220`  
		Last Modified: Fri, 16 Jun 2023 01:49:52 GMT  
		Size: 291.6 KB (291642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55bffa5d4241cc12158e182f1f2911c4259e7fe2223cb64d6de2ebdd44fdc9f`  
		Last Modified: Fri, 16 Jun 2023 01:49:52 GMT  
		Size: 2.4 KB (2425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad30b122e91303d3344340a62434a315fded6e665b21c6e58c5c0d3e37eafe`  
		Last Modified: Fri, 16 Jun 2023 01:49:56 GMT  
		Size: 23.1 MB (23066945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de9f4e16e2bf2315ed74154cad4b2811feb72a14d500ce2ce263fdc05282000`  
		Last Modified: Fri, 16 Jun 2023 01:51:33 GMT  
		Size: 658.5 MB (658463544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-base`

```console
$ docker pull ros@sha256:4bc6a75bdfc1787088a373b07f851fe41e57198dfa8f48f2febae2e4e233a65c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:69399d4a82e41cf4c2fcd751886c1ccc472ac27c115b0d3ec62678d46dd6ee90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268561480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8223749b08214cbaf072ef59fa30f69d3662e7152a145f23e1e49634b5178ad3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:52:41 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 03:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:53:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:53:26 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:53:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:53:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9a4b6088658276f8fd1f323dccdcbb861073b76cd6349072032f5fdaa2308b`  
		Last Modified: Fri, 16 Jun 2023 04:06:19 GMT  
		Size: 124.1 MB (124124424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e6f6e49e9b268b418486630a7ba4b97c13b80a80f9264b2a655e0f0a395d7`  
		Last Modified: Fri, 16 Jun 2023 04:06:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439087c92f7f6e12a142bd39dc7cb8a1ca5d69f39bb6fd3ca975acb89c9d6ac`  
		Last Modified: Fri, 16 Jun 2023 04:06:39 GMT  
		Size: 85.0 MB (84994710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34237af467a507ca4d19e10a051e77c334109ef97c28f8df3d0138188d5facf0`  
		Last Modified: Fri, 16 Jun 2023 04:06:28 GMT  
		Size: 291.6 KB (291640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8439ca8819e994b1e7dcd6debd7f51f0c0ca681463f29e88c0d676fba1637630`  
		Last Modified: Fri, 16 Jun 2023 04:06:28 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc933ad7e1ecb3369fd1ba6557a11d42c83c4fb1e3dedafecc4dd69606c3b4b0`  
		Last Modified: Fri, 16 Jun 2023 04:06:32 GMT  
		Size: 23.7 MB (23673251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0662819c52a556bc9eab61c8938cffaa034a0a52f5c4eb35e411ceb1010fa7d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261115629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b057980795b54497e34d2dc0a3f187b5e9dc87acd145f870ea1130bde0ee15a2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:36:04 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 01:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:36:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:36:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:36:51 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:37:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:37:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:37:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:37:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e41c2e8b43236d79b82b2ce24c1f568a4a3ea25c30dfdc4895cce00480072`  
		Last Modified: Fri, 16 Jun 2023 01:49:43 GMT  
		Size: 121.6 MB (121612466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14e36042bc13bfe0d1c0fb91a96ad3ed768c36fbac710c2082179a1022f1da`  
		Last Modified: Fri, 16 Jun 2023 01:49:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dd2b650fb1c286b3dff3669c7aae3e05912b51d94d17eb5a407cd00018441f`  
		Last Modified: Fri, 16 Jun 2023 01:50:00 GMT  
		Size: 82.7 MB (82735938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e705dd681bbe2976d37a56a63de3fca5f64f664bf74df5f44d55cf7594f220`  
		Last Modified: Fri, 16 Jun 2023 01:49:52 GMT  
		Size: 291.6 KB (291642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55bffa5d4241cc12158e182f1f2911c4259e7fe2223cb64d6de2ebdd44fdc9f`  
		Last Modified: Fri, 16 Jun 2023 01:49:52 GMT  
		Size: 2.4 KB (2425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad30b122e91303d3344340a62434a315fded6e665b21c6e58c5c0d3e37eafe`  
		Last Modified: Fri, 16 Jun 2023 01:49:56 GMT  
		Size: 23.1 MB (23066945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-base-jammy`

```console
$ docker pull ros@sha256:4bc6a75bdfc1787088a373b07f851fe41e57198dfa8f48f2febae2e4e233a65c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:69399d4a82e41cf4c2fcd751886c1ccc472ac27c115b0d3ec62678d46dd6ee90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268561480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8223749b08214cbaf072ef59fa30f69d3662e7152a145f23e1e49634b5178ad3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:52:41 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 03:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:53:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:53:26 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:53:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:53:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9a4b6088658276f8fd1f323dccdcbb861073b76cd6349072032f5fdaa2308b`  
		Last Modified: Fri, 16 Jun 2023 04:06:19 GMT  
		Size: 124.1 MB (124124424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e6f6e49e9b268b418486630a7ba4b97c13b80a80f9264b2a655e0f0a395d7`  
		Last Modified: Fri, 16 Jun 2023 04:06:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439087c92f7f6e12a142bd39dc7cb8a1ca5d69f39bb6fd3ca975acb89c9d6ac`  
		Last Modified: Fri, 16 Jun 2023 04:06:39 GMT  
		Size: 85.0 MB (84994710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34237af467a507ca4d19e10a051e77c334109ef97c28f8df3d0138188d5facf0`  
		Last Modified: Fri, 16 Jun 2023 04:06:28 GMT  
		Size: 291.6 KB (291640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8439ca8819e994b1e7dcd6debd7f51f0c0ca681463f29e88c0d676fba1637630`  
		Last Modified: Fri, 16 Jun 2023 04:06:28 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc933ad7e1ecb3369fd1ba6557a11d42c83c4fb1e3dedafecc4dd69606c3b4b0`  
		Last Modified: Fri, 16 Jun 2023 04:06:32 GMT  
		Size: 23.7 MB (23673251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0662819c52a556bc9eab61c8938cffaa034a0a52f5c4eb35e411ceb1010fa7d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261115629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b057980795b54497e34d2dc0a3f187b5e9dc87acd145f870ea1130bde0ee15a2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:36:04 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 01:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:36:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:36:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:36:51 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:37:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:37:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:37:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:37:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e41c2e8b43236d79b82b2ce24c1f568a4a3ea25c30dfdc4895cce00480072`  
		Last Modified: Fri, 16 Jun 2023 01:49:43 GMT  
		Size: 121.6 MB (121612466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14e36042bc13bfe0d1c0fb91a96ad3ed768c36fbac710c2082179a1022f1da`  
		Last Modified: Fri, 16 Jun 2023 01:49:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dd2b650fb1c286b3dff3669c7aae3e05912b51d94d17eb5a407cd00018441f`  
		Last Modified: Fri, 16 Jun 2023 01:50:00 GMT  
		Size: 82.7 MB (82735938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e705dd681bbe2976d37a56a63de3fca5f64f664bf74df5f44d55cf7594f220`  
		Last Modified: Fri, 16 Jun 2023 01:49:52 GMT  
		Size: 291.6 KB (291642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55bffa5d4241cc12158e182f1f2911c4259e7fe2223cb64d6de2ebdd44fdc9f`  
		Last Modified: Fri, 16 Jun 2023 01:49:52 GMT  
		Size: 2.4 KB (2425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad30b122e91303d3344340a62434a315fded6e665b21c6e58c5c0d3e37eafe`  
		Last Modified: Fri, 16 Jun 2023 01:49:56 GMT  
		Size: 23.1 MB (23066945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-core`

```console
$ docker pull ros@sha256:4bf38277efb1e3a2ad743b3250336294dff020d62e7e5311ac99b668f14d9e2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:b285e5d789c6f340bdbbcd74e5cd22b9dbbf624d55ace5ee7610e462f00d172d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159599452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e138ae3a4edb9bd2de1e8bf6da6c383a9b488eca036c847741035aec0f0659`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:52:41 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 03:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:53:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:53:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9a4b6088658276f8fd1f323dccdcbb861073b76cd6349072032f5fdaa2308b`  
		Last Modified: Fri, 16 Jun 2023 04:06:19 GMT  
		Size: 124.1 MB (124124424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e6f6e49e9b268b418486630a7ba4b97c13b80a80f9264b2a655e0f0a395d7`  
		Last Modified: Fri, 16 Jun 2023 04:06:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ec16631ea5fd743af62667e8849d73f8cbc81f0ee4beaec85c1e8a019798317c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155018679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fe6f1c8df8149aaa3bc208f0042e2cbd748743843abddf667803840535fa8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:36:04 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 01:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:36:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:36:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:36:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e41c2e8b43236d79b82b2ce24c1f568a4a3ea25c30dfdc4895cce00480072`  
		Last Modified: Fri, 16 Jun 2023 01:49:43 GMT  
		Size: 121.6 MB (121612466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14e36042bc13bfe0d1c0fb91a96ad3ed768c36fbac710c2082179a1022f1da`  
		Last Modified: Fri, 16 Jun 2023 01:49:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:iron-ros-core-jammy`

```console
$ docker pull ros@sha256:4bf38277efb1e3a2ad743b3250336294dff020d62e7e5311ac99b668f14d9e2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:b285e5d789c6f340bdbbcd74e5cd22b9dbbf624d55ace5ee7610e462f00d172d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159599452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e138ae3a4edb9bd2de1e8bf6da6c383a9b488eca036c847741035aec0f0659`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:52:41 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 03:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:53:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:53:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:53:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9a4b6088658276f8fd1f323dccdcbb861073b76cd6349072032f5fdaa2308b`  
		Last Modified: Fri, 16 Jun 2023 04:06:19 GMT  
		Size: 124.1 MB (124124424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e6f6e49e9b268b418486630a7ba4b97c13b80a80f9264b2a655e0f0a395d7`  
		Last Modified: Fri, 16 Jun 2023 04:06:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ec16631ea5fd743af62667e8849d73f8cbc81f0ee4beaec85c1e8a019798317c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155018679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fe6f1c8df8149aaa3bc208f0042e2cbd748743843abddf667803840535fa8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:36:04 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 01:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:36:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:36:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:36:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e41c2e8b43236d79b82b2ce24c1f568a4a3ea25c30dfdc4895cce00480072`  
		Last Modified: Fri, 16 Jun 2023 01:49:43 GMT  
		Size: 121.6 MB (121612466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14e36042bc13bfe0d1c0fb91a96ad3ed768c36fbac710c2082179a1022f1da`  
		Last Modified: Fri, 16 Jun 2023 01:49:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:4654de0b83601ee9ba956b2f577bc565fcfd835ca24517e2a951829fa240240e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:3386540ad674d7bfb39325a2149be58b014e815eeff7a66cccbc780396ae3127
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263161054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c5b16395dfe505769d26b47f928ae646c2131a887ebffa63e5b7a65cd71d51`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 03:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:43:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:43:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:43:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:44:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:44:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:44:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:44:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbaaf0d07ce9923344bb5649335dc9cb1d9d75b9072a4184813e3b6e96cb98c`  
		Last Modified: Fri, 16 Jun 2023 04:03:50 GMT  
		Size: 106.3 MB (106346667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40d88d0af61448739222d5fd5bd85608277cce56a574273ff20a89fafee8515`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06384a5e54f3042dafc74cc55288bce3a86696a3c17cf79b130581cdd63910b`  
		Last Modified: Fri, 16 Jun 2023 04:04:12 GMT  
		Size: 97.9 MB (97949822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e750d54d785aa1696c573420a62fbb7249cde12d2084a2fab4201df081b90eb7`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 304.7 KB (304732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d351a048bcc5f2d84a3e60e35390a6f29c2da9dd56e1d7478de0b6015895c42`  
		Last Modified: Fri, 16 Jun 2023 04:03:59 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d66d96470f76515998af23908ea849dca005a88cdf897bde234aa1a43bdd548`  
		Last Modified: Fri, 16 Jun 2023 04:04:03 GMT  
		Size: 23.1 MB (23082395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b4ae4682141d9624af5809f23a0a29d1d3a7dc5b4b7def019fed5b698e1b68d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255900791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2042c6cf46a0742277ab1a4b86e3785f5a7201c35a1960c7c56de6f566b24eb1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV ROS_DISTRO=humble
# Fri, 16 Jun 2023 01:24:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:24:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:24:14 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:25:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:25:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:25:26 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:26:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd26ad58cb49fafe39c24b3bac2e32d04bfee88571404562a416d9a0b6e0e78`  
		Last Modified: Fri, 16 Jun 2023 01:47:20 GMT  
		Size: 104.1 MB (104105616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd9359913df651c74c9e52f793ef0787865e50d9d61a4515ec8ef65c3d8ae3`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4d0b2bfe8969ffafd9009e3ee13526ff43c422fd23b56b102cfe070bfbeb1d`  
		Last Modified: Fri, 16 Jun 2023 01:47:40 GMT  
		Size: 95.6 MB (95581977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6528dc26f11a52b5d26d871d234047f129fdfd2736560765c9b8918ab231f9ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:29 GMT  
		Size: 304.7 KB (304728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f858a72b36e06d019e79b66337b74798e8b8128d7e7011e4651167c411dd94`  
		Last Modified: Fri, 16 Jun 2023 01:47:28 GMT  
		Size: 2.4 KB (2423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a104ce69ef6960d329543d66bbb31b14c8efcbd03ca03fb5685f111378d86ac`  
		Last Modified: Fri, 16 Jun 2023 01:47:32 GMT  
		Size: 22.5 MB (22499835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:4ddbf9fe490a2629368f8098ee74c8909f012ac8517c43054f3c1c05f1a3b153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:cf0560a7a15a302cd5dda5fb04cf923b5b924b6dba1d735b4378690122bfacd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.8 MB (437784429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d4283db9f4ca525b8449e73d343c187e3e857c536e45f8aa25fd5c68366abe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:55:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 01:51:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 01:53:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 01:53:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 01:53:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 01:53:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 01:54:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc27456075680427d55e79ddce0ccec278d1f81ab5181d13386de5ac3f085b90`  
		Last Modified: Fri, 02 Jun 2023 01:02:13 GMT  
		Size: 818.9 KB (818915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c91ad7650f55a57d952458067fa5d43fc42f60aa1300eac0321468efd7f1d`  
		Last Modified: Fri, 02 Jun 2023 02:17:44 GMT  
		Size: 4.9 MB (4878354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56880df8951662a18430445a0e7468b38fa19051e1a794dc42acd993c654fd7b`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c446f0efbdf1c500e962b4679d40098c4c78b579337a83db9751a38b81af7977`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca30d8fccfd9d0b20ea4671a7149e2fdeafd9ee437142de1c9258ee630cc8a8e`  
		Last Modified: Fri, 02 Jun 2023 02:18:15 GMT  
		Size: 259.6 MB (259624496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ae89dc938d7ae36da910586975ad26b87e5df2518d41458f036579d59e3bcc`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b828d11571bf9a2dc34d01f3e018cfbed980a688e0eb6fd7bdf4d501881a0ca`  
		Last Modified: Fri, 02 Jun 2023 02:18:33 GMT  
		Size: 70.5 MB (70459587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7216ece951b98edd7bcceb7db17617751c38d6588b4d2d74d8a7eb422c043f9`  
		Last Modified: Fri, 02 Jun 2023 02:18:23 GMT  
		Size: 283.5 KB (283472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c51a5623d92bc9baa994ddf65fae7b7f119507f0ff98b7153b8366b19881542`  
		Last Modified: Fri, 02 Jun 2023 02:18:34 GMT  
		Size: 75.0 MB (75000399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:a6462ac509b46124de518bbd7e6a3996ec45f1b4e54e873f139a984befc49b71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.4 MB (386377333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5700c425b40584d653d47042b986cb3483c51410da1df4617d41bbf1531f43e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:52:11 GMT
ARG RELEASE
# Tue, 30 May 2023 09:52:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:52:20 GMT
ADD file:d570ab6bd7d664cc6547b6ae228cf825333d9d841969911c7d62afe3ed440803 in / 
# Tue, 30 May 2023 09:52:21 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:03:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 00:03:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 00:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 00:07:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 00:07:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 00:07:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 00:08:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76bc0c6b06fc92c1f911be6147b55b6430301b80e4062178329c4fa8a0f79f51`  
		Last Modified: Thu, 01 Jun 2023 23:54:31 GMT  
		Size: 22.3 MB (22312178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f87f37d6a7831a2d27cf9ba67dbb404857632b477ce335ecbe521cd84db2d`  
		Last Modified: Fri, 02 Jun 2023 00:15:23 GMT  
		Size: 820.3 KB (820335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a424966fc7947ef55ca4db8ed69abeb762dbe613d82cb7b6c248b55d4a76fe8d`  
		Last Modified: Fri, 02 Jun 2023 00:15:22 GMT  
		Size: 4.1 MB (4090754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f2b5759d6a592db8d9e7c54cea41255e28a308bb00dd901b0b89e127833484`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fe4f77d9ba9445f2717bc343def12bf6a5abffaaea9978f6a7cd08e9dfdd96`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed06e4959894fd0c27932146a90ade048f580b919f2003dc021fe1a3b771c7`  
		Last Modified: Fri, 02 Jun 2023 00:15:54 GMT  
		Size: 239.1 MB (239083601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028706c953b925fc2ae8b0353286f1e65b796003820978cacf6b3fafd5b523d3`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6586e09f1cb6a3e98681e7381415216b056728fc1638e63d0dfb7185bd95e`  
		Last Modified: Fri, 02 Jun 2023 00:16:10 GMT  
		Size: 55.0 MB (55033923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d0b06f450c92b4d108057aa9ea1678dd83381dde934812520c7557e827262f`  
		Last Modified: Fri, 02 Jun 2023 00:16:03 GMT  
		Size: 283.5 KB (283459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e9ec93d69d137562906fd1dfdef9c60300d24a8dc97255f8d2d9621b30a922`  
		Last Modified: Fri, 02 Jun 2023 00:16:13 GMT  
		Size: 64.8 MB (64751236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:016c8d65cd94acf72f71f1cccb07f5ccc7b37cd06a15e4ae8797ca9049393ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.3 MB (412347515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78be2a7f6c6d7ca30d92068bbcae735ea8a2e62719c7a58882a5bc433307434a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:07:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:54:30 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Mon, 03 Jul 2023 18:54:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LC_ALL=C.UTF-8
# Mon, 03 Jul 2023 18:54:32 GMT
ENV ROS_DISTRO=melodic
# Mon, 03 Jul 2023 18:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:00 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 03 Jul 2023 18:59:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Jul 2023 18:59:00 GMT
CMD ["bash"]
# Mon, 03 Jul 2023 18:59:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Jul 2023 19:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f5d58f6c858f92b45f1d3e366bcabef3c6821ccaa9ee17c59beb643029cb4d`  
		Last Modified: Fri, 02 Jun 2023 00:41:19 GMT  
		Size: 819.0 KB (818994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e738cf9edf30ed3cf9686d84733d2d3d3ee28a85c58ada09fabd9660ed336`  
		Last Modified: Fri, 02 Jun 2023 00:41:18 GMT  
		Size: 4.5 MB (4461671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb15c91065685951357c563d50225475bf62ccf00e185b08b5d5aa0d828f9e9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddaf40387f745b8b6c023a4647f5ce4a9f784107d4ba1d4356d41f6ccd21a5d9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d28df4590da4d1b3e217e5b8b28fed95ce13c54228ee8335465c1b72839ef3c`  
		Last Modified: Mon, 03 Jul 2023 19:09:17 GMT  
		Size: 252.5 MB (252524042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffda3f020806b222794eaaa7b5f1cf412f7ebf13aad2e650fd36980f6649787`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce65a51b0331e8a1ff1c5bd34f6cf61bb21789c246ed43c0465eecddf10e14`  
		Last Modified: Mon, 03 Jul 2023 19:09:32 GMT  
		Size: 63.3 MB (63279594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5c3f121b18d97b4bd63e2476c9c60549acd8148c5c11fd04bd08f5c70d877`  
		Last Modified: Mon, 03 Jul 2023 19:09:26 GMT  
		Size: 284.8 KB (284817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a658836e677ca17fd290d1d7bb810935536e4e53a459435294c426cad64b3`  
		Last Modified: Mon, 03 Jul 2023 19:09:34 GMT  
		Size: 67.2 MB (67234662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:6ff5bbef95a9f44589ed642a7b01ad5621dcea3da50569cbf931c10f626516d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:f20110db44563528486b919197d2ace26dbb768374d193cf37f62b417437b42b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **743.5 MB (743487700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea660cee3be0fea18dba191d8d826d30534b4d63c276b3c3234bacd84cc8738`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:55:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 01:51:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 01:53:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 01:53:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 01:53:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 01:53:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 01:54:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:58:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc27456075680427d55e79ddce0ccec278d1f81ab5181d13386de5ac3f085b90`  
		Last Modified: Fri, 02 Jun 2023 01:02:13 GMT  
		Size: 818.9 KB (818915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c91ad7650f55a57d952458067fa5d43fc42f60aa1300eac0321468efd7f1d`  
		Last Modified: Fri, 02 Jun 2023 02:17:44 GMT  
		Size: 4.9 MB (4878354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56880df8951662a18430445a0e7468b38fa19051e1a794dc42acd993c654fd7b`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c446f0efbdf1c500e962b4679d40098c4c78b579337a83db9751a38b81af7977`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca30d8fccfd9d0b20ea4671a7149e2fdeafd9ee437142de1c9258ee630cc8a8e`  
		Last Modified: Fri, 02 Jun 2023 02:18:15 GMT  
		Size: 259.6 MB (259624496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ae89dc938d7ae36da910586975ad26b87e5df2518d41458f036579d59e3bcc`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b828d11571bf9a2dc34d01f3e018cfbed980a688e0eb6fd7bdf4d501881a0ca`  
		Last Modified: Fri, 02 Jun 2023 02:18:33 GMT  
		Size: 70.5 MB (70459587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7216ece951b98edd7bcceb7db17617751c38d6588b4d2d74d8a7eb422c043f9`  
		Last Modified: Fri, 02 Jun 2023 02:18:23 GMT  
		Size: 283.5 KB (283472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c51a5623d92bc9baa994ddf65fae7b7f119507f0ff98b7153b8366b19881542`  
		Last Modified: Fri, 02 Jun 2023 02:18:34 GMT  
		Size: 75.0 MB (75000399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e397b7c71c1be86e2bf8ae268cce09ff4347e4d71c72e1711c7aa099ca1d1510`  
		Last Modified: Fri, 02 Jun 2023 02:19:38 GMT  
		Size: 305.7 MB (305703271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:06e5ec5b16d971455af1a0510658fdec5b94c3a1eb948d1fbcd2b26c7ee1ef23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.7 MB (646699906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c5a16eb2ff6b4abe2b15548e8e5347eadcd4641965013edf87bc88886e80bd5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:52:11 GMT
ARG RELEASE
# Tue, 30 May 2023 09:52:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:52:20 GMT
ADD file:d570ab6bd7d664cc6547b6ae228cf825333d9d841969911c7d62afe3ed440803 in / 
# Tue, 30 May 2023 09:52:21 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:03:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 00:03:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 00:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 00:07:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 00:07:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 00:07:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 00:08:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:14:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76bc0c6b06fc92c1f911be6147b55b6430301b80e4062178329c4fa8a0f79f51`  
		Last Modified: Thu, 01 Jun 2023 23:54:31 GMT  
		Size: 22.3 MB (22312178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f87f37d6a7831a2d27cf9ba67dbb404857632b477ce335ecbe521cd84db2d`  
		Last Modified: Fri, 02 Jun 2023 00:15:23 GMT  
		Size: 820.3 KB (820335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a424966fc7947ef55ca4db8ed69abeb762dbe613d82cb7b6c248b55d4a76fe8d`  
		Last Modified: Fri, 02 Jun 2023 00:15:22 GMT  
		Size: 4.1 MB (4090754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f2b5759d6a592db8d9e7c54cea41255e28a308bb00dd901b0b89e127833484`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fe4f77d9ba9445f2717bc343def12bf6a5abffaaea9978f6a7cd08e9dfdd96`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed06e4959894fd0c27932146a90ade048f580b919f2003dc021fe1a3b771c7`  
		Last Modified: Fri, 02 Jun 2023 00:15:54 GMT  
		Size: 239.1 MB (239083601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028706c953b925fc2ae8b0353286f1e65b796003820978cacf6b3fafd5b523d3`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6586e09f1cb6a3e98681e7381415216b056728fc1638e63d0dfb7185bd95e`  
		Last Modified: Fri, 02 Jun 2023 00:16:10 GMT  
		Size: 55.0 MB (55033923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d0b06f450c92b4d108057aa9ea1678dd83381dde934812520c7557e827262f`  
		Last Modified: Fri, 02 Jun 2023 00:16:03 GMT  
		Size: 283.5 KB (283459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e9ec93d69d137562906fd1dfdef9c60300d24a8dc97255f8d2d9621b30a922`  
		Last Modified: Fri, 02 Jun 2023 00:16:13 GMT  
		Size: 64.8 MB (64751236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594b3855b25b075922bf634e58c144589bc3d8b64d02fa234977253e79ce764e`  
		Last Modified: Fri, 02 Jun 2023 00:17:10 GMT  
		Size: 260.3 MB (260322573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:449681c53ff4136c59d6a975ac4478e4a736aa89f0d0c676eb688afda5ccf294
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.4 MB (704353620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0564d239811a89435a03b6cfe936fc147f9e68c53be7fb058950ec8a851fd07a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:07:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:54:30 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Mon, 03 Jul 2023 18:54:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LC_ALL=C.UTF-8
# Mon, 03 Jul 2023 18:54:32 GMT
ENV ROS_DISTRO=melodic
# Mon, 03 Jul 2023 18:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:00 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 03 Jul 2023 18:59:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Jul 2023 18:59:00 GMT
CMD ["bash"]
# Mon, 03 Jul 2023 18:59:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Jul 2023 19:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 19:07:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f5d58f6c858f92b45f1d3e366bcabef3c6821ccaa9ee17c59beb643029cb4d`  
		Last Modified: Fri, 02 Jun 2023 00:41:19 GMT  
		Size: 819.0 KB (818994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e738cf9edf30ed3cf9686d84733d2d3d3ee28a85c58ada09fabd9660ed336`  
		Last Modified: Fri, 02 Jun 2023 00:41:18 GMT  
		Size: 4.5 MB (4461671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb15c91065685951357c563d50225475bf62ccf00e185b08b5d5aa0d828f9e9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddaf40387f745b8b6c023a4647f5ce4a9f784107d4ba1d4356d41f6ccd21a5d9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d28df4590da4d1b3e217e5b8b28fed95ce13c54228ee8335465c1b72839ef3c`  
		Last Modified: Mon, 03 Jul 2023 19:09:17 GMT  
		Size: 252.5 MB (252524042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffda3f020806b222794eaaa7b5f1cf412f7ebf13aad2e650fd36980f6649787`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce65a51b0331e8a1ff1c5bd34f6cf61bb21789c246ed43c0465eecddf10e14`  
		Last Modified: Mon, 03 Jul 2023 19:09:32 GMT  
		Size: 63.3 MB (63279594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5c3f121b18d97b4bd63e2476c9c60549acd8148c5c11fd04bd08f5c70d877`  
		Last Modified: Mon, 03 Jul 2023 19:09:26 GMT  
		Size: 284.8 KB (284817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a658836e677ca17fd290d1d7bb810935536e4e53a459435294c426cad64b3`  
		Last Modified: Mon, 03 Jul 2023 19:09:34 GMT  
		Size: 67.2 MB (67234662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598fa718252c092ab10ae79ff168cc8abd04d179e020bdaeb6c1dbca1aae9de0`  
		Last Modified: Mon, 03 Jul 2023 19:10:26 GMT  
		Size: 292.0 MB (292006105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:6ff5bbef95a9f44589ed642a7b01ad5621dcea3da50569cbf931c10f626516d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:f20110db44563528486b919197d2ace26dbb768374d193cf37f62b417437b42b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **743.5 MB (743487700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea660cee3be0fea18dba191d8d826d30534b4d63c276b3c3234bacd84cc8738`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:55:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 01:51:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 01:53:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 01:53:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 01:53:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 01:53:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 01:54:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:58:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc27456075680427d55e79ddce0ccec278d1f81ab5181d13386de5ac3f085b90`  
		Last Modified: Fri, 02 Jun 2023 01:02:13 GMT  
		Size: 818.9 KB (818915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c91ad7650f55a57d952458067fa5d43fc42f60aa1300eac0321468efd7f1d`  
		Last Modified: Fri, 02 Jun 2023 02:17:44 GMT  
		Size: 4.9 MB (4878354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56880df8951662a18430445a0e7468b38fa19051e1a794dc42acd993c654fd7b`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c446f0efbdf1c500e962b4679d40098c4c78b579337a83db9751a38b81af7977`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca30d8fccfd9d0b20ea4671a7149e2fdeafd9ee437142de1c9258ee630cc8a8e`  
		Last Modified: Fri, 02 Jun 2023 02:18:15 GMT  
		Size: 259.6 MB (259624496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ae89dc938d7ae36da910586975ad26b87e5df2518d41458f036579d59e3bcc`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b828d11571bf9a2dc34d01f3e018cfbed980a688e0eb6fd7bdf4d501881a0ca`  
		Last Modified: Fri, 02 Jun 2023 02:18:33 GMT  
		Size: 70.5 MB (70459587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7216ece951b98edd7bcceb7db17617751c38d6588b4d2d74d8a7eb422c043f9`  
		Last Modified: Fri, 02 Jun 2023 02:18:23 GMT  
		Size: 283.5 KB (283472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c51a5623d92bc9baa994ddf65fae7b7f119507f0ff98b7153b8366b19881542`  
		Last Modified: Fri, 02 Jun 2023 02:18:34 GMT  
		Size: 75.0 MB (75000399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e397b7c71c1be86e2bf8ae268cce09ff4347e4d71c72e1711c7aa099ca1d1510`  
		Last Modified: Fri, 02 Jun 2023 02:19:38 GMT  
		Size: 305.7 MB (305703271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:06e5ec5b16d971455af1a0510658fdec5b94c3a1eb948d1fbcd2b26c7ee1ef23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.7 MB (646699906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c5a16eb2ff6b4abe2b15548e8e5347eadcd4641965013edf87bc88886e80bd5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:52:11 GMT
ARG RELEASE
# Tue, 30 May 2023 09:52:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:52:20 GMT
ADD file:d570ab6bd7d664cc6547b6ae228cf825333d9d841969911c7d62afe3ed440803 in / 
# Tue, 30 May 2023 09:52:21 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:03:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 00:03:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 00:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 00:07:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 00:07:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 00:07:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 00:08:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:14:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76bc0c6b06fc92c1f911be6147b55b6430301b80e4062178329c4fa8a0f79f51`  
		Last Modified: Thu, 01 Jun 2023 23:54:31 GMT  
		Size: 22.3 MB (22312178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f87f37d6a7831a2d27cf9ba67dbb404857632b477ce335ecbe521cd84db2d`  
		Last Modified: Fri, 02 Jun 2023 00:15:23 GMT  
		Size: 820.3 KB (820335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a424966fc7947ef55ca4db8ed69abeb762dbe613d82cb7b6c248b55d4a76fe8d`  
		Last Modified: Fri, 02 Jun 2023 00:15:22 GMT  
		Size: 4.1 MB (4090754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f2b5759d6a592db8d9e7c54cea41255e28a308bb00dd901b0b89e127833484`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fe4f77d9ba9445f2717bc343def12bf6a5abffaaea9978f6a7cd08e9dfdd96`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed06e4959894fd0c27932146a90ade048f580b919f2003dc021fe1a3b771c7`  
		Last Modified: Fri, 02 Jun 2023 00:15:54 GMT  
		Size: 239.1 MB (239083601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028706c953b925fc2ae8b0353286f1e65b796003820978cacf6b3fafd5b523d3`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6586e09f1cb6a3e98681e7381415216b056728fc1638e63d0dfb7185bd95e`  
		Last Modified: Fri, 02 Jun 2023 00:16:10 GMT  
		Size: 55.0 MB (55033923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d0b06f450c92b4d108057aa9ea1678dd83381dde934812520c7557e827262f`  
		Last Modified: Fri, 02 Jun 2023 00:16:03 GMT  
		Size: 283.5 KB (283459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e9ec93d69d137562906fd1dfdef9c60300d24a8dc97255f8d2d9621b30a922`  
		Last Modified: Fri, 02 Jun 2023 00:16:13 GMT  
		Size: 64.8 MB (64751236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594b3855b25b075922bf634e58c144589bc3d8b64d02fa234977253e79ce764e`  
		Last Modified: Fri, 02 Jun 2023 00:17:10 GMT  
		Size: 260.3 MB (260322573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:449681c53ff4136c59d6a975ac4478e4a736aa89f0d0c676eb688afda5ccf294
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.4 MB (704353620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0564d239811a89435a03b6cfe936fc147f9e68c53be7fb058950ec8a851fd07a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:07:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:54:30 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Mon, 03 Jul 2023 18:54:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LC_ALL=C.UTF-8
# Mon, 03 Jul 2023 18:54:32 GMT
ENV ROS_DISTRO=melodic
# Mon, 03 Jul 2023 18:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:00 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 03 Jul 2023 18:59:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Jul 2023 18:59:00 GMT
CMD ["bash"]
# Mon, 03 Jul 2023 18:59:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Jul 2023 19:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 19:07:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f5d58f6c858f92b45f1d3e366bcabef3c6821ccaa9ee17c59beb643029cb4d`  
		Last Modified: Fri, 02 Jun 2023 00:41:19 GMT  
		Size: 819.0 KB (818994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e738cf9edf30ed3cf9686d84733d2d3d3ee28a85c58ada09fabd9660ed336`  
		Last Modified: Fri, 02 Jun 2023 00:41:18 GMT  
		Size: 4.5 MB (4461671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb15c91065685951357c563d50225475bf62ccf00e185b08b5d5aa0d828f9e9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddaf40387f745b8b6c023a4647f5ce4a9f784107d4ba1d4356d41f6ccd21a5d9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d28df4590da4d1b3e217e5b8b28fed95ce13c54228ee8335465c1b72839ef3c`  
		Last Modified: Mon, 03 Jul 2023 19:09:17 GMT  
		Size: 252.5 MB (252524042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffda3f020806b222794eaaa7b5f1cf412f7ebf13aad2e650fd36980f6649787`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce65a51b0331e8a1ff1c5bd34f6cf61bb21789c246ed43c0465eecddf10e14`  
		Last Modified: Mon, 03 Jul 2023 19:09:32 GMT  
		Size: 63.3 MB (63279594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5c3f121b18d97b4bd63e2476c9c60549acd8148c5c11fd04bd08f5c70d877`  
		Last Modified: Mon, 03 Jul 2023 19:09:26 GMT  
		Size: 284.8 KB (284817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a658836e677ca17fd290d1d7bb810935536e4e53a459435294c426cad64b3`  
		Last Modified: Mon, 03 Jul 2023 19:09:34 GMT  
		Size: 67.2 MB (67234662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598fa718252c092ab10ae79ff168cc8abd04d179e020bdaeb6c1dbca1aae9de0`  
		Last Modified: Mon, 03 Jul 2023 19:10:26 GMT  
		Size: 292.0 MB (292006105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:15d713ea6fe5716022bb724d02945ed91dbd3377e270adb902775590832af265
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:4df4ce3983c5549904e8c82101a1c8a20b11988eaf3159329fefadefdffdd10d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.9 MB (448871124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c721fd7bee450eff4590e74a9775c3cb9004ccf81c657122992bc2199e47768e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:55:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 01:51:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 01:53:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 01:53:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 01:53:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 01:53:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 01:54:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc27456075680427d55e79ddce0ccec278d1f81ab5181d13386de5ac3f085b90`  
		Last Modified: Fri, 02 Jun 2023 01:02:13 GMT  
		Size: 818.9 KB (818915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c91ad7650f55a57d952458067fa5d43fc42f60aa1300eac0321468efd7f1d`  
		Last Modified: Fri, 02 Jun 2023 02:17:44 GMT  
		Size: 4.9 MB (4878354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56880df8951662a18430445a0e7468b38fa19051e1a794dc42acd993c654fd7b`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c446f0efbdf1c500e962b4679d40098c4c78b579337a83db9751a38b81af7977`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca30d8fccfd9d0b20ea4671a7149e2fdeafd9ee437142de1c9258ee630cc8a8e`  
		Last Modified: Fri, 02 Jun 2023 02:18:15 GMT  
		Size: 259.6 MB (259624496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ae89dc938d7ae36da910586975ad26b87e5df2518d41458f036579d59e3bcc`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b828d11571bf9a2dc34d01f3e018cfbed980a688e0eb6fd7bdf4d501881a0ca`  
		Last Modified: Fri, 02 Jun 2023 02:18:33 GMT  
		Size: 70.5 MB (70459587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7216ece951b98edd7bcceb7db17617751c38d6588b4d2d74d8a7eb422c043f9`  
		Last Modified: Fri, 02 Jun 2023 02:18:23 GMT  
		Size: 283.5 KB (283472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c51a5623d92bc9baa994ddf65fae7b7f119507f0ff98b7153b8366b19881542`  
		Last Modified: Fri, 02 Jun 2023 02:18:34 GMT  
		Size: 75.0 MB (75000399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0f42811905b2540524a0cc3439632e8069cb1823b24ac5ba5f86ebc31e4e42`  
		Last Modified: Fri, 02 Jun 2023 02:18:46 GMT  
		Size: 11.1 MB (11086695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:924aac9793d2bd2e6c4155606aa3abec0612fbf4d0048b7f18a33f4206eeb59a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.5 MB (396501012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dba414ade9b7721a44ab4ba78577adaaddac9ed3a7f1ce78c19eedd75d70afff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:52:11 GMT
ARG RELEASE
# Tue, 30 May 2023 09:52:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:52:20 GMT
ADD file:d570ab6bd7d664cc6547b6ae228cf825333d9d841969911c7d62afe3ed440803 in / 
# Tue, 30 May 2023 09:52:21 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:03:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 00:03:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 00:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 00:07:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 00:07:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 00:07:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 00:08:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:09:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76bc0c6b06fc92c1f911be6147b55b6430301b80e4062178329c4fa8a0f79f51`  
		Last Modified: Thu, 01 Jun 2023 23:54:31 GMT  
		Size: 22.3 MB (22312178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f87f37d6a7831a2d27cf9ba67dbb404857632b477ce335ecbe521cd84db2d`  
		Last Modified: Fri, 02 Jun 2023 00:15:23 GMT  
		Size: 820.3 KB (820335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a424966fc7947ef55ca4db8ed69abeb762dbe613d82cb7b6c248b55d4a76fe8d`  
		Last Modified: Fri, 02 Jun 2023 00:15:22 GMT  
		Size: 4.1 MB (4090754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f2b5759d6a592db8d9e7c54cea41255e28a308bb00dd901b0b89e127833484`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fe4f77d9ba9445f2717bc343def12bf6a5abffaaea9978f6a7cd08e9dfdd96`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed06e4959894fd0c27932146a90ade048f580b919f2003dc021fe1a3b771c7`  
		Last Modified: Fri, 02 Jun 2023 00:15:54 GMT  
		Size: 239.1 MB (239083601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028706c953b925fc2ae8b0353286f1e65b796003820978cacf6b3fafd5b523d3`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6586e09f1cb6a3e98681e7381415216b056728fc1638e63d0dfb7185bd95e`  
		Last Modified: Fri, 02 Jun 2023 00:16:10 GMT  
		Size: 55.0 MB (55033923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d0b06f450c92b4d108057aa9ea1678dd83381dde934812520c7557e827262f`  
		Last Modified: Fri, 02 Jun 2023 00:16:03 GMT  
		Size: 283.5 KB (283459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e9ec93d69d137562906fd1dfdef9c60300d24a8dc97255f8d2d9621b30a922`  
		Last Modified: Fri, 02 Jun 2023 00:16:13 GMT  
		Size: 64.8 MB (64751236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42626b24ca50691c98bff90cb9ea40c7f1c277b27d97bfc02f87438d4f077fc3`  
		Last Modified: Fri, 02 Jun 2023 00:16:26 GMT  
		Size: 10.1 MB (10123679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2fe63bac2154e2abfb6d097f65a355cad26cf94e45f5efc9b748814a93cd22bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.1 MB (423088490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b4dc839116cf28cde32859381873255851381bf0c32edc2d8e2c5e369ae160`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:07:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:54:30 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Mon, 03 Jul 2023 18:54:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LC_ALL=C.UTF-8
# Mon, 03 Jul 2023 18:54:32 GMT
ENV ROS_DISTRO=melodic
# Mon, 03 Jul 2023 18:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:00 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 03 Jul 2023 18:59:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Jul 2023 18:59:00 GMT
CMD ["bash"]
# Mon, 03 Jul 2023 18:59:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Jul 2023 19:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 19:01:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f5d58f6c858f92b45f1d3e366bcabef3c6821ccaa9ee17c59beb643029cb4d`  
		Last Modified: Fri, 02 Jun 2023 00:41:19 GMT  
		Size: 819.0 KB (818994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e738cf9edf30ed3cf9686d84733d2d3d3ee28a85c58ada09fabd9660ed336`  
		Last Modified: Fri, 02 Jun 2023 00:41:18 GMT  
		Size: 4.5 MB (4461671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb15c91065685951357c563d50225475bf62ccf00e185b08b5d5aa0d828f9e9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddaf40387f745b8b6c023a4647f5ce4a9f784107d4ba1d4356d41f6ccd21a5d9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d28df4590da4d1b3e217e5b8b28fed95ce13c54228ee8335465c1b72839ef3c`  
		Last Modified: Mon, 03 Jul 2023 19:09:17 GMT  
		Size: 252.5 MB (252524042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffda3f020806b222794eaaa7b5f1cf412f7ebf13aad2e650fd36980f6649787`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce65a51b0331e8a1ff1c5bd34f6cf61bb21789c246ed43c0465eecddf10e14`  
		Last Modified: Mon, 03 Jul 2023 19:09:32 GMT  
		Size: 63.3 MB (63279594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5c3f121b18d97b4bd63e2476c9c60549acd8148c5c11fd04bd08f5c70d877`  
		Last Modified: Mon, 03 Jul 2023 19:09:26 GMT  
		Size: 284.8 KB (284817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a658836e677ca17fd290d1d7bb810935536e4e53a459435294c426cad64b3`  
		Last Modified: Mon, 03 Jul 2023 19:09:34 GMT  
		Size: 67.2 MB (67234662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db13672ba81dc9baa7763bdf694a4b962ddcf0ed01dd1823883bb41d3f09e29`  
		Last Modified: Mon, 03 Jul 2023 19:09:47 GMT  
		Size: 10.7 MB (10740975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:15d713ea6fe5716022bb724d02945ed91dbd3377e270adb902775590832af265
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:4df4ce3983c5549904e8c82101a1c8a20b11988eaf3159329fefadefdffdd10d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.9 MB (448871124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c721fd7bee450eff4590e74a9775c3cb9004ccf81c657122992bc2199e47768e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:55:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 01:51:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 01:53:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 01:53:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 01:53:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 01:53:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 01:54:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc27456075680427d55e79ddce0ccec278d1f81ab5181d13386de5ac3f085b90`  
		Last Modified: Fri, 02 Jun 2023 01:02:13 GMT  
		Size: 818.9 KB (818915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c91ad7650f55a57d952458067fa5d43fc42f60aa1300eac0321468efd7f1d`  
		Last Modified: Fri, 02 Jun 2023 02:17:44 GMT  
		Size: 4.9 MB (4878354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56880df8951662a18430445a0e7468b38fa19051e1a794dc42acd993c654fd7b`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c446f0efbdf1c500e962b4679d40098c4c78b579337a83db9751a38b81af7977`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca30d8fccfd9d0b20ea4671a7149e2fdeafd9ee437142de1c9258ee630cc8a8e`  
		Last Modified: Fri, 02 Jun 2023 02:18:15 GMT  
		Size: 259.6 MB (259624496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ae89dc938d7ae36da910586975ad26b87e5df2518d41458f036579d59e3bcc`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b828d11571bf9a2dc34d01f3e018cfbed980a688e0eb6fd7bdf4d501881a0ca`  
		Last Modified: Fri, 02 Jun 2023 02:18:33 GMT  
		Size: 70.5 MB (70459587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7216ece951b98edd7bcceb7db17617751c38d6588b4d2d74d8a7eb422c043f9`  
		Last Modified: Fri, 02 Jun 2023 02:18:23 GMT  
		Size: 283.5 KB (283472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c51a5623d92bc9baa994ddf65fae7b7f119507f0ff98b7153b8366b19881542`  
		Last Modified: Fri, 02 Jun 2023 02:18:34 GMT  
		Size: 75.0 MB (75000399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0f42811905b2540524a0cc3439632e8069cb1823b24ac5ba5f86ebc31e4e42`  
		Last Modified: Fri, 02 Jun 2023 02:18:46 GMT  
		Size: 11.1 MB (11086695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:924aac9793d2bd2e6c4155606aa3abec0612fbf4d0048b7f18a33f4206eeb59a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.5 MB (396501012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dba414ade9b7721a44ab4ba78577adaaddac9ed3a7f1ce78c19eedd75d70afff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:52:11 GMT
ARG RELEASE
# Tue, 30 May 2023 09:52:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:52:20 GMT
ADD file:d570ab6bd7d664cc6547b6ae228cf825333d9d841969911c7d62afe3ed440803 in / 
# Tue, 30 May 2023 09:52:21 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:03:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 00:03:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 00:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 00:07:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 00:07:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 00:07:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 00:08:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:09:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76bc0c6b06fc92c1f911be6147b55b6430301b80e4062178329c4fa8a0f79f51`  
		Last Modified: Thu, 01 Jun 2023 23:54:31 GMT  
		Size: 22.3 MB (22312178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f87f37d6a7831a2d27cf9ba67dbb404857632b477ce335ecbe521cd84db2d`  
		Last Modified: Fri, 02 Jun 2023 00:15:23 GMT  
		Size: 820.3 KB (820335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a424966fc7947ef55ca4db8ed69abeb762dbe613d82cb7b6c248b55d4a76fe8d`  
		Last Modified: Fri, 02 Jun 2023 00:15:22 GMT  
		Size: 4.1 MB (4090754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f2b5759d6a592db8d9e7c54cea41255e28a308bb00dd901b0b89e127833484`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fe4f77d9ba9445f2717bc343def12bf6a5abffaaea9978f6a7cd08e9dfdd96`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed06e4959894fd0c27932146a90ade048f580b919f2003dc021fe1a3b771c7`  
		Last Modified: Fri, 02 Jun 2023 00:15:54 GMT  
		Size: 239.1 MB (239083601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028706c953b925fc2ae8b0353286f1e65b796003820978cacf6b3fafd5b523d3`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6586e09f1cb6a3e98681e7381415216b056728fc1638e63d0dfb7185bd95e`  
		Last Modified: Fri, 02 Jun 2023 00:16:10 GMT  
		Size: 55.0 MB (55033923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d0b06f450c92b4d108057aa9ea1678dd83381dde934812520c7557e827262f`  
		Last Modified: Fri, 02 Jun 2023 00:16:03 GMT  
		Size: 283.5 KB (283459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e9ec93d69d137562906fd1dfdef9c60300d24a8dc97255f8d2d9621b30a922`  
		Last Modified: Fri, 02 Jun 2023 00:16:13 GMT  
		Size: 64.8 MB (64751236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42626b24ca50691c98bff90cb9ea40c7f1c277b27d97bfc02f87438d4f077fc3`  
		Last Modified: Fri, 02 Jun 2023 00:16:26 GMT  
		Size: 10.1 MB (10123679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2fe63bac2154e2abfb6d097f65a355cad26cf94e45f5efc9b748814a93cd22bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.1 MB (423088490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b4dc839116cf28cde32859381873255851381bf0c32edc2d8e2c5e369ae160`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:07:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:54:30 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Mon, 03 Jul 2023 18:54:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LC_ALL=C.UTF-8
# Mon, 03 Jul 2023 18:54:32 GMT
ENV ROS_DISTRO=melodic
# Mon, 03 Jul 2023 18:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:00 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 03 Jul 2023 18:59:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Jul 2023 18:59:00 GMT
CMD ["bash"]
# Mon, 03 Jul 2023 18:59:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Jul 2023 19:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 19:01:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f5d58f6c858f92b45f1d3e366bcabef3c6821ccaa9ee17c59beb643029cb4d`  
		Last Modified: Fri, 02 Jun 2023 00:41:19 GMT  
		Size: 819.0 KB (818994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e738cf9edf30ed3cf9686d84733d2d3d3ee28a85c58ada09fabd9660ed336`  
		Last Modified: Fri, 02 Jun 2023 00:41:18 GMT  
		Size: 4.5 MB (4461671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb15c91065685951357c563d50225475bf62ccf00e185b08b5d5aa0d828f9e9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddaf40387f745b8b6c023a4647f5ce4a9f784107d4ba1d4356d41f6ccd21a5d9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d28df4590da4d1b3e217e5b8b28fed95ce13c54228ee8335465c1b72839ef3c`  
		Last Modified: Mon, 03 Jul 2023 19:09:17 GMT  
		Size: 252.5 MB (252524042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffda3f020806b222794eaaa7b5f1cf412f7ebf13aad2e650fd36980f6649787`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce65a51b0331e8a1ff1c5bd34f6cf61bb21789c246ed43c0465eecddf10e14`  
		Last Modified: Mon, 03 Jul 2023 19:09:32 GMT  
		Size: 63.3 MB (63279594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5c3f121b18d97b4bd63e2476c9c60549acd8148c5c11fd04bd08f5c70d877`  
		Last Modified: Mon, 03 Jul 2023 19:09:26 GMT  
		Size: 284.8 KB (284817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a658836e677ca17fd290d1d7bb810935536e4e53a459435294c426cad64b3`  
		Last Modified: Mon, 03 Jul 2023 19:09:34 GMT  
		Size: 67.2 MB (67234662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db13672ba81dc9baa7763bdf694a4b962ddcf0ed01dd1823883bb41d3f09e29`  
		Last Modified: Mon, 03 Jul 2023 19:09:47 GMT  
		Size: 10.7 MB (10740975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:4ddbf9fe490a2629368f8098ee74c8909f012ac8517c43054f3c1c05f1a3b153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:cf0560a7a15a302cd5dda5fb04cf923b5b924b6dba1d735b4378690122bfacd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.8 MB (437784429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d4283db9f4ca525b8449e73d343c187e3e857c536e45f8aa25fd5c68366abe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:55:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 01:51:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 01:53:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 01:53:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 01:53:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 01:53:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 01:54:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc27456075680427d55e79ddce0ccec278d1f81ab5181d13386de5ac3f085b90`  
		Last Modified: Fri, 02 Jun 2023 01:02:13 GMT  
		Size: 818.9 KB (818915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c91ad7650f55a57d952458067fa5d43fc42f60aa1300eac0321468efd7f1d`  
		Last Modified: Fri, 02 Jun 2023 02:17:44 GMT  
		Size: 4.9 MB (4878354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56880df8951662a18430445a0e7468b38fa19051e1a794dc42acd993c654fd7b`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c446f0efbdf1c500e962b4679d40098c4c78b579337a83db9751a38b81af7977`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca30d8fccfd9d0b20ea4671a7149e2fdeafd9ee437142de1c9258ee630cc8a8e`  
		Last Modified: Fri, 02 Jun 2023 02:18:15 GMT  
		Size: 259.6 MB (259624496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ae89dc938d7ae36da910586975ad26b87e5df2518d41458f036579d59e3bcc`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b828d11571bf9a2dc34d01f3e018cfbed980a688e0eb6fd7bdf4d501881a0ca`  
		Last Modified: Fri, 02 Jun 2023 02:18:33 GMT  
		Size: 70.5 MB (70459587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7216ece951b98edd7bcceb7db17617751c38d6588b4d2d74d8a7eb422c043f9`  
		Last Modified: Fri, 02 Jun 2023 02:18:23 GMT  
		Size: 283.5 KB (283472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c51a5623d92bc9baa994ddf65fae7b7f119507f0ff98b7153b8366b19881542`  
		Last Modified: Fri, 02 Jun 2023 02:18:34 GMT  
		Size: 75.0 MB (75000399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:a6462ac509b46124de518bbd7e6a3996ec45f1b4e54e873f139a984befc49b71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.4 MB (386377333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5700c425b40584d653d47042b986cb3483c51410da1df4617d41bbf1531f43e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:52:11 GMT
ARG RELEASE
# Tue, 30 May 2023 09:52:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:52:20 GMT
ADD file:d570ab6bd7d664cc6547b6ae228cf825333d9d841969911c7d62afe3ed440803 in / 
# Tue, 30 May 2023 09:52:21 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:03:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 00:03:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 00:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 00:07:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 00:07:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 00:07:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 00:08:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76bc0c6b06fc92c1f911be6147b55b6430301b80e4062178329c4fa8a0f79f51`  
		Last Modified: Thu, 01 Jun 2023 23:54:31 GMT  
		Size: 22.3 MB (22312178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f87f37d6a7831a2d27cf9ba67dbb404857632b477ce335ecbe521cd84db2d`  
		Last Modified: Fri, 02 Jun 2023 00:15:23 GMT  
		Size: 820.3 KB (820335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a424966fc7947ef55ca4db8ed69abeb762dbe613d82cb7b6c248b55d4a76fe8d`  
		Last Modified: Fri, 02 Jun 2023 00:15:22 GMT  
		Size: 4.1 MB (4090754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f2b5759d6a592db8d9e7c54cea41255e28a308bb00dd901b0b89e127833484`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fe4f77d9ba9445f2717bc343def12bf6a5abffaaea9978f6a7cd08e9dfdd96`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed06e4959894fd0c27932146a90ade048f580b919f2003dc021fe1a3b771c7`  
		Last Modified: Fri, 02 Jun 2023 00:15:54 GMT  
		Size: 239.1 MB (239083601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028706c953b925fc2ae8b0353286f1e65b796003820978cacf6b3fafd5b523d3`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6586e09f1cb6a3e98681e7381415216b056728fc1638e63d0dfb7185bd95e`  
		Last Modified: Fri, 02 Jun 2023 00:16:10 GMT  
		Size: 55.0 MB (55033923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d0b06f450c92b4d108057aa9ea1678dd83381dde934812520c7557e827262f`  
		Last Modified: Fri, 02 Jun 2023 00:16:03 GMT  
		Size: 283.5 KB (283459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e9ec93d69d137562906fd1dfdef9c60300d24a8dc97255f8d2d9621b30a922`  
		Last Modified: Fri, 02 Jun 2023 00:16:13 GMT  
		Size: 64.8 MB (64751236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:016c8d65cd94acf72f71f1cccb07f5ccc7b37cd06a15e4ae8797ca9049393ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.3 MB (412347515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78be2a7f6c6d7ca30d92068bbcae735ea8a2e62719c7a58882a5bc433307434a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:07:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:54:30 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Mon, 03 Jul 2023 18:54:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LC_ALL=C.UTF-8
# Mon, 03 Jul 2023 18:54:32 GMT
ENV ROS_DISTRO=melodic
# Mon, 03 Jul 2023 18:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:00 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 03 Jul 2023 18:59:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Jul 2023 18:59:00 GMT
CMD ["bash"]
# Mon, 03 Jul 2023 18:59:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Jul 2023 19:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f5d58f6c858f92b45f1d3e366bcabef3c6821ccaa9ee17c59beb643029cb4d`  
		Last Modified: Fri, 02 Jun 2023 00:41:19 GMT  
		Size: 819.0 KB (818994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e738cf9edf30ed3cf9686d84733d2d3d3ee28a85c58ada09fabd9660ed336`  
		Last Modified: Fri, 02 Jun 2023 00:41:18 GMT  
		Size: 4.5 MB (4461671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb15c91065685951357c563d50225475bf62ccf00e185b08b5d5aa0d828f9e9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddaf40387f745b8b6c023a4647f5ce4a9f784107d4ba1d4356d41f6ccd21a5d9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d28df4590da4d1b3e217e5b8b28fed95ce13c54228ee8335465c1b72839ef3c`  
		Last Modified: Mon, 03 Jul 2023 19:09:17 GMT  
		Size: 252.5 MB (252524042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffda3f020806b222794eaaa7b5f1cf412f7ebf13aad2e650fd36980f6649787`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce65a51b0331e8a1ff1c5bd34f6cf61bb21789c246ed43c0465eecddf10e14`  
		Last Modified: Mon, 03 Jul 2023 19:09:32 GMT  
		Size: 63.3 MB (63279594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5c3f121b18d97b4bd63e2476c9c60549acd8148c5c11fd04bd08f5c70d877`  
		Last Modified: Mon, 03 Jul 2023 19:09:26 GMT  
		Size: 284.8 KB (284817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a658836e677ca17fd290d1d7bb810935536e4e53a459435294c426cad64b3`  
		Last Modified: Mon, 03 Jul 2023 19:09:34 GMT  
		Size: 67.2 MB (67234662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:4ddbf9fe490a2629368f8098ee74c8909f012ac8517c43054f3c1c05f1a3b153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:cf0560a7a15a302cd5dda5fb04cf923b5b924b6dba1d735b4378690122bfacd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.8 MB (437784429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d4283db9f4ca525b8449e73d343c187e3e857c536e45f8aa25fd5c68366abe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:55:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 01:51:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 01:53:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 01:53:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 01:53:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 01:53:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 01:54:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc27456075680427d55e79ddce0ccec278d1f81ab5181d13386de5ac3f085b90`  
		Last Modified: Fri, 02 Jun 2023 01:02:13 GMT  
		Size: 818.9 KB (818915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c91ad7650f55a57d952458067fa5d43fc42f60aa1300eac0321468efd7f1d`  
		Last Modified: Fri, 02 Jun 2023 02:17:44 GMT  
		Size: 4.9 MB (4878354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56880df8951662a18430445a0e7468b38fa19051e1a794dc42acd993c654fd7b`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c446f0efbdf1c500e962b4679d40098c4c78b579337a83db9751a38b81af7977`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca30d8fccfd9d0b20ea4671a7149e2fdeafd9ee437142de1c9258ee630cc8a8e`  
		Last Modified: Fri, 02 Jun 2023 02:18:15 GMT  
		Size: 259.6 MB (259624496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ae89dc938d7ae36da910586975ad26b87e5df2518d41458f036579d59e3bcc`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b828d11571bf9a2dc34d01f3e018cfbed980a688e0eb6fd7bdf4d501881a0ca`  
		Last Modified: Fri, 02 Jun 2023 02:18:33 GMT  
		Size: 70.5 MB (70459587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7216ece951b98edd7bcceb7db17617751c38d6588b4d2d74d8a7eb422c043f9`  
		Last Modified: Fri, 02 Jun 2023 02:18:23 GMT  
		Size: 283.5 KB (283472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c51a5623d92bc9baa994ddf65fae7b7f119507f0ff98b7153b8366b19881542`  
		Last Modified: Fri, 02 Jun 2023 02:18:34 GMT  
		Size: 75.0 MB (75000399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:a6462ac509b46124de518bbd7e6a3996ec45f1b4e54e873f139a984befc49b71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.4 MB (386377333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5700c425b40584d653d47042b986cb3483c51410da1df4617d41bbf1531f43e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:52:11 GMT
ARG RELEASE
# Tue, 30 May 2023 09:52:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:52:20 GMT
ADD file:d570ab6bd7d664cc6547b6ae228cf825333d9d841969911c7d62afe3ed440803 in / 
# Tue, 30 May 2023 09:52:21 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:03:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 00:03:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 00:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 00:07:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 00:07:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 00:07:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 00:08:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76bc0c6b06fc92c1f911be6147b55b6430301b80e4062178329c4fa8a0f79f51`  
		Last Modified: Thu, 01 Jun 2023 23:54:31 GMT  
		Size: 22.3 MB (22312178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f87f37d6a7831a2d27cf9ba67dbb404857632b477ce335ecbe521cd84db2d`  
		Last Modified: Fri, 02 Jun 2023 00:15:23 GMT  
		Size: 820.3 KB (820335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a424966fc7947ef55ca4db8ed69abeb762dbe613d82cb7b6c248b55d4a76fe8d`  
		Last Modified: Fri, 02 Jun 2023 00:15:22 GMT  
		Size: 4.1 MB (4090754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f2b5759d6a592db8d9e7c54cea41255e28a308bb00dd901b0b89e127833484`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fe4f77d9ba9445f2717bc343def12bf6a5abffaaea9978f6a7cd08e9dfdd96`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed06e4959894fd0c27932146a90ade048f580b919f2003dc021fe1a3b771c7`  
		Last Modified: Fri, 02 Jun 2023 00:15:54 GMT  
		Size: 239.1 MB (239083601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028706c953b925fc2ae8b0353286f1e65b796003820978cacf6b3fafd5b523d3`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6586e09f1cb6a3e98681e7381415216b056728fc1638e63d0dfb7185bd95e`  
		Last Modified: Fri, 02 Jun 2023 00:16:10 GMT  
		Size: 55.0 MB (55033923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d0b06f450c92b4d108057aa9ea1678dd83381dde934812520c7557e827262f`  
		Last Modified: Fri, 02 Jun 2023 00:16:03 GMT  
		Size: 283.5 KB (283459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e9ec93d69d137562906fd1dfdef9c60300d24a8dc97255f8d2d9621b30a922`  
		Last Modified: Fri, 02 Jun 2023 00:16:13 GMT  
		Size: 64.8 MB (64751236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:016c8d65cd94acf72f71f1cccb07f5ccc7b37cd06a15e4ae8797ca9049393ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.3 MB (412347515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78be2a7f6c6d7ca30d92068bbcae735ea8a2e62719c7a58882a5bc433307434a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:07:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:54:30 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Mon, 03 Jul 2023 18:54:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LC_ALL=C.UTF-8
# Mon, 03 Jul 2023 18:54:32 GMT
ENV ROS_DISTRO=melodic
# Mon, 03 Jul 2023 18:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:00 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 03 Jul 2023 18:59:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Jul 2023 18:59:00 GMT
CMD ["bash"]
# Mon, 03 Jul 2023 18:59:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Jul 2023 19:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f5d58f6c858f92b45f1d3e366bcabef3c6821ccaa9ee17c59beb643029cb4d`  
		Last Modified: Fri, 02 Jun 2023 00:41:19 GMT  
		Size: 819.0 KB (818994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e738cf9edf30ed3cf9686d84733d2d3d3ee28a85c58ada09fabd9660ed336`  
		Last Modified: Fri, 02 Jun 2023 00:41:18 GMT  
		Size: 4.5 MB (4461671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb15c91065685951357c563d50225475bf62ccf00e185b08b5d5aa0d828f9e9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddaf40387f745b8b6c023a4647f5ce4a9f784107d4ba1d4356d41f6ccd21a5d9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d28df4590da4d1b3e217e5b8b28fed95ce13c54228ee8335465c1b72839ef3c`  
		Last Modified: Mon, 03 Jul 2023 19:09:17 GMT  
		Size: 252.5 MB (252524042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffda3f020806b222794eaaa7b5f1cf412f7ebf13aad2e650fd36980f6649787`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce65a51b0331e8a1ff1c5bd34f6cf61bb21789c246ed43c0465eecddf10e14`  
		Last Modified: Mon, 03 Jul 2023 19:09:32 GMT  
		Size: 63.3 MB (63279594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5c3f121b18d97b4bd63e2476c9c60549acd8148c5c11fd04bd08f5c70d877`  
		Last Modified: Mon, 03 Jul 2023 19:09:26 GMT  
		Size: 284.8 KB (284817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a658836e677ca17fd290d1d7bb810935536e4e53a459435294c426cad64b3`  
		Last Modified: Mon, 03 Jul 2023 19:09:34 GMT  
		Size: 67.2 MB (67234662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:81cbc7f7e5eb14c5a959f5911994601686f074bb3cc80a885c004f195145cda6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:48e8d1a31ad24e96ad0782975f5c100db5699c35027989c0007d51ba3c716222
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (292040971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15029dc3a16127803aed2c78de541ccc1a2112400e2e07e0f744bc8d050cb32e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:55:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 01:51:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 01:53:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 01:53:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 01:53:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc27456075680427d55e79ddce0ccec278d1f81ab5181d13386de5ac3f085b90`  
		Last Modified: Fri, 02 Jun 2023 01:02:13 GMT  
		Size: 818.9 KB (818915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c91ad7650f55a57d952458067fa5d43fc42f60aa1300eac0321468efd7f1d`  
		Last Modified: Fri, 02 Jun 2023 02:17:44 GMT  
		Size: 4.9 MB (4878354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56880df8951662a18430445a0e7468b38fa19051e1a794dc42acd993c654fd7b`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c446f0efbdf1c500e962b4679d40098c4c78b579337a83db9751a38b81af7977`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca30d8fccfd9d0b20ea4671a7149e2fdeafd9ee437142de1c9258ee630cc8a8e`  
		Last Modified: Fri, 02 Jun 2023 02:18:15 GMT  
		Size: 259.6 MB (259624496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ae89dc938d7ae36da910586975ad26b87e5df2518d41458f036579d59e3bcc`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:5743c99153d4cc4d5b8697491aac8b91a429fb1d8e16b26a02cd6ba02bf256cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266308715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c125f894b1cf0db2acd3c4015e19c4e94cb190fa56c2ba2725989124c137716`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:52:11 GMT
ARG RELEASE
# Tue, 30 May 2023 09:52:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:52:20 GMT
ADD file:d570ab6bd7d664cc6547b6ae228cf825333d9d841969911c7d62afe3ed440803 in / 
# Tue, 30 May 2023 09:52:21 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:03:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 00:03:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 00:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 00:07:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 00:07:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:76bc0c6b06fc92c1f911be6147b55b6430301b80e4062178329c4fa8a0f79f51`  
		Last Modified: Thu, 01 Jun 2023 23:54:31 GMT  
		Size: 22.3 MB (22312178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f87f37d6a7831a2d27cf9ba67dbb404857632b477ce335ecbe521cd84db2d`  
		Last Modified: Fri, 02 Jun 2023 00:15:23 GMT  
		Size: 820.3 KB (820335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a424966fc7947ef55ca4db8ed69abeb762dbe613d82cb7b6c248b55d4a76fe8d`  
		Last Modified: Fri, 02 Jun 2023 00:15:22 GMT  
		Size: 4.1 MB (4090754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f2b5759d6a592db8d9e7c54cea41255e28a308bb00dd901b0b89e127833484`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fe4f77d9ba9445f2717bc343def12bf6a5abffaaea9978f6a7cd08e9dfdd96`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed06e4959894fd0c27932146a90ade048f580b919f2003dc021fe1a3b771c7`  
		Last Modified: Fri, 02 Jun 2023 00:15:54 GMT  
		Size: 239.1 MB (239083601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028706c953b925fc2ae8b0353286f1e65b796003820978cacf6b3fafd5b523d3`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:341577c558cc811914067f5d0b854c89fe1fdc8f96907671f0e275f7ec9ee129
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.5 MB (281548442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be19dee15a45e0dd38b7693830b6100dfa265640333034efbd53df11195376ff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:07:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:54:30 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Mon, 03 Jul 2023 18:54:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LC_ALL=C.UTF-8
# Mon, 03 Jul 2023 18:54:32 GMT
ENV ROS_DISTRO=melodic
# Mon, 03 Jul 2023 18:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:00 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 03 Jul 2023 18:59:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Jul 2023 18:59:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f5d58f6c858f92b45f1d3e366bcabef3c6821ccaa9ee17c59beb643029cb4d`  
		Last Modified: Fri, 02 Jun 2023 00:41:19 GMT  
		Size: 819.0 KB (818994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e738cf9edf30ed3cf9686d84733d2d3d3ee28a85c58ada09fabd9660ed336`  
		Last Modified: Fri, 02 Jun 2023 00:41:18 GMT  
		Size: 4.5 MB (4461671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb15c91065685951357c563d50225475bf62ccf00e185b08b5d5aa0d828f9e9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddaf40387f745b8b6c023a4647f5ce4a9f784107d4ba1d4356d41f6ccd21a5d9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d28df4590da4d1b3e217e5b8b28fed95ce13c54228ee8335465c1b72839ef3c`  
		Last Modified: Mon, 03 Jul 2023 19:09:17 GMT  
		Size: 252.5 MB (252524042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffda3f020806b222794eaaa7b5f1cf412f7ebf13aad2e650fd36980f6649787`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:81cbc7f7e5eb14c5a959f5911994601686f074bb3cc80a885c004f195145cda6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:48e8d1a31ad24e96ad0782975f5c100db5699c35027989c0007d51ba3c716222
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (292040971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15029dc3a16127803aed2c78de541ccc1a2112400e2e07e0f744bc8d050cb32e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:55:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 01:51:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 01:53:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 01:53:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 01:53:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc27456075680427d55e79ddce0ccec278d1f81ab5181d13386de5ac3f085b90`  
		Last Modified: Fri, 02 Jun 2023 01:02:13 GMT  
		Size: 818.9 KB (818915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c91ad7650f55a57d952458067fa5d43fc42f60aa1300eac0321468efd7f1d`  
		Last Modified: Fri, 02 Jun 2023 02:17:44 GMT  
		Size: 4.9 MB (4878354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56880df8951662a18430445a0e7468b38fa19051e1a794dc42acd993c654fd7b`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c446f0efbdf1c500e962b4679d40098c4c78b579337a83db9751a38b81af7977`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca30d8fccfd9d0b20ea4671a7149e2fdeafd9ee437142de1c9258ee630cc8a8e`  
		Last Modified: Fri, 02 Jun 2023 02:18:15 GMT  
		Size: 259.6 MB (259624496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ae89dc938d7ae36da910586975ad26b87e5df2518d41458f036579d59e3bcc`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:5743c99153d4cc4d5b8697491aac8b91a429fb1d8e16b26a02cd6ba02bf256cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266308715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c125f894b1cf0db2acd3c4015e19c4e94cb190fa56c2ba2725989124c137716`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:52:11 GMT
ARG RELEASE
# Tue, 30 May 2023 09:52:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:52:20 GMT
ADD file:d570ab6bd7d664cc6547b6ae228cf825333d9d841969911c7d62afe3ed440803 in / 
# Tue, 30 May 2023 09:52:21 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:03:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 00:03:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 00:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 00:07:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 00:07:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:76bc0c6b06fc92c1f911be6147b55b6430301b80e4062178329c4fa8a0f79f51`  
		Last Modified: Thu, 01 Jun 2023 23:54:31 GMT  
		Size: 22.3 MB (22312178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f87f37d6a7831a2d27cf9ba67dbb404857632b477ce335ecbe521cd84db2d`  
		Last Modified: Fri, 02 Jun 2023 00:15:23 GMT  
		Size: 820.3 KB (820335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a424966fc7947ef55ca4db8ed69abeb762dbe613d82cb7b6c248b55d4a76fe8d`  
		Last Modified: Fri, 02 Jun 2023 00:15:22 GMT  
		Size: 4.1 MB (4090754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f2b5759d6a592db8d9e7c54cea41255e28a308bb00dd901b0b89e127833484`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fe4f77d9ba9445f2717bc343def12bf6a5abffaaea9978f6a7cd08e9dfdd96`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed06e4959894fd0c27932146a90ade048f580b919f2003dc021fe1a3b771c7`  
		Last Modified: Fri, 02 Jun 2023 00:15:54 GMT  
		Size: 239.1 MB (239083601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028706c953b925fc2ae8b0353286f1e65b796003820978cacf6b3fafd5b523d3`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:341577c558cc811914067f5d0b854c89fe1fdc8f96907671f0e275f7ec9ee129
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.5 MB (281548442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be19dee15a45e0dd38b7693830b6100dfa265640333034efbd53df11195376ff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:07:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:54:30 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Mon, 03 Jul 2023 18:54:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LC_ALL=C.UTF-8
# Mon, 03 Jul 2023 18:54:32 GMT
ENV ROS_DISTRO=melodic
# Mon, 03 Jul 2023 18:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:00 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 03 Jul 2023 18:59:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Jul 2023 18:59:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f5d58f6c858f92b45f1d3e366bcabef3c6821ccaa9ee17c59beb643029cb4d`  
		Last Modified: Fri, 02 Jun 2023 00:41:19 GMT  
		Size: 819.0 KB (818994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e738cf9edf30ed3cf9686d84733d2d3d3ee28a85c58ada09fabd9660ed336`  
		Last Modified: Fri, 02 Jun 2023 00:41:18 GMT  
		Size: 4.5 MB (4461671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb15c91065685951357c563d50225475bf62ccf00e185b08b5d5aa0d828f9e9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddaf40387f745b8b6c023a4647f5ce4a9f784107d4ba1d4356d41f6ccd21a5d9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d28df4590da4d1b3e217e5b8b28fed95ce13c54228ee8335465c1b72839ef3c`  
		Last Modified: Mon, 03 Jul 2023 19:09:17 GMT  
		Size: 252.5 MB (252524042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffda3f020806b222794eaaa7b5f1cf412f7ebf13aad2e650fd36980f6649787`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:85d6814a41fb2b53ee1a72f6a9bbd6db5349e3f53144d7a3977678d9226d6c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:e494f7045c604c02e24951e5fadac6970192d9750e74fed4dce6a84553a1bbe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343227046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176ab51cd7218002277e110aa91f9a6ba9e07ea86a8b687079ecd5407dbe1ee4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:26:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 03:30:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 03:31:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:31:29 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:31:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:32:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac94a680e3659eb88af9a60aa46eabe11de358d05cb19cf9d535083358650`  
		Last Modified: Fri, 16 Jun 2023 02:35:08 GMT  
		Size: 1.2 MB (1198722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c1fc3d4979a8cbea7949ab14296db71b51de166f987d5b8427b73ada3f02c0`  
		Last Modified: Fri, 16 Jun 2023 03:59:52 GMT  
		Size: 5.6 MB (5553799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c84d683cefaf172b68dda67c6436651b8b1563cbf6581f6d107056879bd8dd`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7b26995f6b2a9cf9efe6abea26c654753ad281e510d846acd0a50df8ecc32`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f480dd10200e3a3923db8466a2f0ace22c6a438b1fcce66e58aff7277e61ab`  
		Last Modified: Fri, 16 Jun 2023 04:00:18 GMT  
		Size: 177.0 MB (177045651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245827a1732fa0f267df2f15bcade007d9f966ca6b66aff8674eb1f2c65ff8d`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b92cb1be2be4c3303b48ae3153b399a674ba5205267a8f230094b09f4ead9`  
		Last Modified: Fri, 16 Jun 2023 04:00:35 GMT  
		Size: 50.9 MB (50939959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85074d427c0ad42d999081cdae5264fcbc3612d8f6f050416f85fe68af3ff5aa`  
		Last Modified: Fri, 16 Jun 2023 04:00:28 GMT  
		Size: 300.9 KB (300905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55740d8cb9ba6388e9f43d993eb6efead35161d874bfdc0fab522b741534dc`  
		Last Modified: Fri, 16 Jun 2023 04:00:39 GMT  
		Size: 79.6 MB (79605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:00362f93138beaccc2f24ca7603855ad9e5c4c1d0fb3276731ec5cd2c9e1a194
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289312397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb397f715f738fabd09fe73d93f3af1988aebe53ecd1c2e419665dd65abef97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:09:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:09:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:11:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:11:22 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:11:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:13:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067db60a914b1db17390d08b8bd7e865dee500a51f35b6cc416f2f439f353955`  
		Last Modified: Fri, 16 Jun 2023 01:22:14 GMT  
		Size: 1.2 MB (1198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0881c824748bc118255bd7e676957b191f4d1fc5d9312139c1c52620c3cd2e`  
		Last Modified: Fri, 16 Jun 2023 01:22:12 GMT  
		Size: 4.7 MB (4679255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d12de37bd26c3e5b7c318c866dbb1b2da51ef7fcaf919748173b86af8be76`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60445b0a24d3a271c0344aada562719e7fb4093cd08e1c827d0f3cbe06c14a`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd28f326a43c2f4336c4d7942bad0b2e7c7c66948c45b89e2c444d11da9334`  
		Last Modified: Fri, 16 Jun 2023 01:22:40 GMT  
		Size: 157.5 MB (157544285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ab69607baa56a10b8698b59afe82be893274534a3bfca0e72b462dc40e149`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c737eaceaa561ec3829766a4f983d37b1a8025bb5a684dbc6943a7bbb893cf92`  
		Last Modified: Fri, 16 Jun 2023 01:22:55 GMT  
		Size: 40.5 MB (40503879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81c90a8a3c1dd33072bbaaad0ec5513a44ec458e3c6cdeb7f56a9db0d526ad`  
		Last Modified: Fri, 16 Jun 2023 01:22:50 GMT  
		Size: 300.9 KB (300910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634e8abbac2de0a96b0e64208fce0b241335c3727fae9cd287fd4703feee414a`  
		Last Modified: Fri, 16 Jun 2023 01:22:59 GMT  
		Size: 60.5 MB (60493810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b3439a82a31dd441d66f51a748e0e809e6c78e908aba0aa15301036e23e8b42d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.0 MB (322952047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a18787368117d0921c898948b5cb1fa8f7142c1c97d3fcc1821c758f2c593289`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:05:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:08:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:08:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:08:23 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ce101c5379362c5d849146976146cdb15940589c3378f71530e726706b160`  
		Last Modified: Fri, 16 Jun 2023 01:43:18 GMT  
		Size: 1.2 MB (1199977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7326ceba9de7061d919892605fd699e778fbaf87d16a5e3c3506e23a475fa`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 5.5 MB (5533346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8660fa6a9889b47b0cdedcd38551c4c097b74330bc7a35fd279ee17d32d7d67e`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097712cf91a87b7360886785f2a964a56ce10c8e4f3a77000f83523967fa20a`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff70657adfd24e02a562b4b09fdd26c26299a6001899ed61f0a8d56fb4e6f7`  
		Last Modified: Fri, 16 Jun 2023 01:43:49 GMT  
		Size: 171.5 MB (171538574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a43a9a62bd1e51770b576e70e4a54589303e48ac0c92cd9b8e010d58561397`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b2416bfb26d974c3da81f7eee6b7acfdb4eccae5aa2c72651e419946abed85`  
		Last Modified: Fri, 16 Jun 2023 01:44:03 GMT  
		Size: 45.2 MB (45205161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1bfa67a8583b7c003a10dc5da1e0a39d70b559bb0ef4854efb785d8a227d1e`  
		Last Modified: Fri, 16 Jun 2023 01:43:58 GMT  
		Size: 300.9 KB (300915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4152459f508eaf13deb06ac7708780ad620739b8cd3b7719a65bc728be19dd88`  
		Last Modified: Fri, 16 Jun 2023 01:44:06 GMT  
		Size: 72.0 MB (71971225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:f26739ec9d163557c72e3561d5f7b21c6baa36650e29a0e630fc54c552029285
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:6fe3eeb0a6c79f2c9fed542d0949d758f5023d19f2b21e4cbf19429045e0bb70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.5 MB (835546300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a04683087cbd99125d821c04802461d90d0820274819cb79387718ae4969be`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:26:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 03:30:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 03:31:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:31:29 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:31:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:32:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:38:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac94a680e3659eb88af9a60aa46eabe11de358d05cb19cf9d535083358650`  
		Last Modified: Fri, 16 Jun 2023 02:35:08 GMT  
		Size: 1.2 MB (1198722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c1fc3d4979a8cbea7949ab14296db71b51de166f987d5b8427b73ada3f02c0`  
		Last Modified: Fri, 16 Jun 2023 03:59:52 GMT  
		Size: 5.6 MB (5553799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c84d683cefaf172b68dda67c6436651b8b1563cbf6581f6d107056879bd8dd`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7b26995f6b2a9cf9efe6abea26c654753ad281e510d846acd0a50df8ecc32`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f480dd10200e3a3923db8466a2f0ace22c6a438b1fcce66e58aff7277e61ab`  
		Last Modified: Fri, 16 Jun 2023 04:00:18 GMT  
		Size: 177.0 MB (177045651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245827a1732fa0f267df2f15bcade007d9f966ca6b66aff8674eb1f2c65ff8d`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b92cb1be2be4c3303b48ae3153b399a674ba5205267a8f230094b09f4ead9`  
		Last Modified: Fri, 16 Jun 2023 04:00:35 GMT  
		Size: 50.9 MB (50939959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85074d427c0ad42d999081cdae5264fcbc3612d8f6f050416f85fe68af3ff5aa`  
		Last Modified: Fri, 16 Jun 2023 04:00:28 GMT  
		Size: 300.9 KB (300905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55740d8cb9ba6388e9f43d993eb6efead35161d874bfdc0fab522b741534dc`  
		Last Modified: Fri, 16 Jun 2023 04:00:39 GMT  
		Size: 79.6 MB (79605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acc02334f74bcb721a785ee4b4876c2179768930144af5368ca9ae294e1ae6b`  
		Last Modified: Fri, 16 Jun 2023 04:02:09 GMT  
		Size: 492.3 MB (492319254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:550b08de7d4654499a028a0c76e0f617b0924843176f9bd78deb83f943efdb19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.5 MB (726511769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a21ccaa1a6f6253d41e5a3a1d3cda0c100fd9c1aa95187718b464b7c78664716`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:09:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:09:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:11:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:11:22 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:11:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:13:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:21:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067db60a914b1db17390d08b8bd7e865dee500a51f35b6cc416f2f439f353955`  
		Last Modified: Fri, 16 Jun 2023 01:22:14 GMT  
		Size: 1.2 MB (1198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0881c824748bc118255bd7e676957b191f4d1fc5d9312139c1c52620c3cd2e`  
		Last Modified: Fri, 16 Jun 2023 01:22:12 GMT  
		Size: 4.7 MB (4679255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d12de37bd26c3e5b7c318c866dbb1b2da51ef7fcaf919748173b86af8be76`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60445b0a24d3a271c0344aada562719e7fb4093cd08e1c827d0f3cbe06c14a`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd28f326a43c2f4336c4d7942bad0b2e7c7c66948c45b89e2c444d11da9334`  
		Last Modified: Fri, 16 Jun 2023 01:22:40 GMT  
		Size: 157.5 MB (157544285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ab69607baa56a10b8698b59afe82be893274534a3bfca0e72b462dc40e149`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c737eaceaa561ec3829766a4f983d37b1a8025bb5a684dbc6943a7bbb893cf92`  
		Last Modified: Fri, 16 Jun 2023 01:22:55 GMT  
		Size: 40.5 MB (40503879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81c90a8a3c1dd33072bbaaad0ec5513a44ec458e3c6cdeb7f56a9db0d526ad`  
		Last Modified: Fri, 16 Jun 2023 01:22:50 GMT  
		Size: 300.9 KB (300910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634e8abbac2de0a96b0e64208fce0b241335c3727fae9cd287fd4703feee414a`  
		Last Modified: Fri, 16 Jun 2023 01:22:59 GMT  
		Size: 60.5 MB (60493810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf34daf709d5030ce3ecce404fb19c763e8035e85a55252f3d1899e0da1718c5`  
		Last Modified: Fri, 16 Jun 2023 01:24:21 GMT  
		Size: 437.2 MB (437199372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1d0487cdc96ec575cc7508097c8d8e1b0b0fc14d70e3478e43d04d0c4ef88130
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.8 MB (785846180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff2ba19a83eca63cca34a699af128f82405633e67c43dfc99c5ed633ecc329f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:05:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:08:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:08:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:08:23 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:19:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ce101c5379362c5d849146976146cdb15940589c3378f71530e726706b160`  
		Last Modified: Fri, 16 Jun 2023 01:43:18 GMT  
		Size: 1.2 MB (1199977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7326ceba9de7061d919892605fd699e778fbaf87d16a5e3c3506e23a475fa`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 5.5 MB (5533346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8660fa6a9889b47b0cdedcd38551c4c097b74330bc7a35fd279ee17d32d7d67e`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097712cf91a87b7360886785f2a964a56ce10c8e4f3a77000f83523967fa20a`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff70657adfd24e02a562b4b09fdd26c26299a6001899ed61f0a8d56fb4e6f7`  
		Last Modified: Fri, 16 Jun 2023 01:43:49 GMT  
		Size: 171.5 MB (171538574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a43a9a62bd1e51770b576e70e4a54589303e48ac0c92cd9b8e010d58561397`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b2416bfb26d974c3da81f7eee6b7acfdb4eccae5aa2c72651e419946abed85`  
		Last Modified: Fri, 16 Jun 2023 01:44:03 GMT  
		Size: 45.2 MB (45205161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1bfa67a8583b7c003a10dc5da1e0a39d70b559bb0ef4854efb785d8a227d1e`  
		Last Modified: Fri, 16 Jun 2023 01:43:58 GMT  
		Size: 300.9 KB (300915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4152459f508eaf13deb06ac7708780ad620739b8cd3b7719a65bc728be19dd88`  
		Last Modified: Fri, 16 Jun 2023 01:44:06 GMT  
		Size: 72.0 MB (71971225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e30f904686801514f906f4b10630900fa5c7551ceb8e71256813143c09bdc64`  
		Last Modified: Fri, 16 Jun 2023 01:45:29 GMT  
		Size: 462.9 MB (462894133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:f26739ec9d163557c72e3561d5f7b21c6baa36650e29a0e630fc54c552029285
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:6fe3eeb0a6c79f2c9fed542d0949d758f5023d19f2b21e4cbf19429045e0bb70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.5 MB (835546300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a04683087cbd99125d821c04802461d90d0820274819cb79387718ae4969be`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:26:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 03:30:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 03:31:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:31:29 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:31:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:32:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:38:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac94a680e3659eb88af9a60aa46eabe11de358d05cb19cf9d535083358650`  
		Last Modified: Fri, 16 Jun 2023 02:35:08 GMT  
		Size: 1.2 MB (1198722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c1fc3d4979a8cbea7949ab14296db71b51de166f987d5b8427b73ada3f02c0`  
		Last Modified: Fri, 16 Jun 2023 03:59:52 GMT  
		Size: 5.6 MB (5553799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c84d683cefaf172b68dda67c6436651b8b1563cbf6581f6d107056879bd8dd`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7b26995f6b2a9cf9efe6abea26c654753ad281e510d846acd0a50df8ecc32`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f480dd10200e3a3923db8466a2f0ace22c6a438b1fcce66e58aff7277e61ab`  
		Last Modified: Fri, 16 Jun 2023 04:00:18 GMT  
		Size: 177.0 MB (177045651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245827a1732fa0f267df2f15bcade007d9f966ca6b66aff8674eb1f2c65ff8d`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b92cb1be2be4c3303b48ae3153b399a674ba5205267a8f230094b09f4ead9`  
		Last Modified: Fri, 16 Jun 2023 04:00:35 GMT  
		Size: 50.9 MB (50939959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85074d427c0ad42d999081cdae5264fcbc3612d8f6f050416f85fe68af3ff5aa`  
		Last Modified: Fri, 16 Jun 2023 04:00:28 GMT  
		Size: 300.9 KB (300905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55740d8cb9ba6388e9f43d993eb6efead35161d874bfdc0fab522b741534dc`  
		Last Modified: Fri, 16 Jun 2023 04:00:39 GMT  
		Size: 79.6 MB (79605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acc02334f74bcb721a785ee4b4876c2179768930144af5368ca9ae294e1ae6b`  
		Last Modified: Fri, 16 Jun 2023 04:02:09 GMT  
		Size: 492.3 MB (492319254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:550b08de7d4654499a028a0c76e0f617b0924843176f9bd78deb83f943efdb19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.5 MB (726511769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a21ccaa1a6f6253d41e5a3a1d3cda0c100fd9c1aa95187718b464b7c78664716`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:09:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:09:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:11:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:11:22 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:11:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:13:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:21:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067db60a914b1db17390d08b8bd7e865dee500a51f35b6cc416f2f439f353955`  
		Last Modified: Fri, 16 Jun 2023 01:22:14 GMT  
		Size: 1.2 MB (1198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0881c824748bc118255bd7e676957b191f4d1fc5d9312139c1c52620c3cd2e`  
		Last Modified: Fri, 16 Jun 2023 01:22:12 GMT  
		Size: 4.7 MB (4679255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d12de37bd26c3e5b7c318c866dbb1b2da51ef7fcaf919748173b86af8be76`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60445b0a24d3a271c0344aada562719e7fb4093cd08e1c827d0f3cbe06c14a`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd28f326a43c2f4336c4d7942bad0b2e7c7c66948c45b89e2c444d11da9334`  
		Last Modified: Fri, 16 Jun 2023 01:22:40 GMT  
		Size: 157.5 MB (157544285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ab69607baa56a10b8698b59afe82be893274534a3bfca0e72b462dc40e149`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c737eaceaa561ec3829766a4f983d37b1a8025bb5a684dbc6943a7bbb893cf92`  
		Last Modified: Fri, 16 Jun 2023 01:22:55 GMT  
		Size: 40.5 MB (40503879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81c90a8a3c1dd33072bbaaad0ec5513a44ec458e3c6cdeb7f56a9db0d526ad`  
		Last Modified: Fri, 16 Jun 2023 01:22:50 GMT  
		Size: 300.9 KB (300910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634e8abbac2de0a96b0e64208fce0b241335c3727fae9cd287fd4703feee414a`  
		Last Modified: Fri, 16 Jun 2023 01:22:59 GMT  
		Size: 60.5 MB (60493810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf34daf709d5030ce3ecce404fb19c763e8035e85a55252f3d1899e0da1718c5`  
		Last Modified: Fri, 16 Jun 2023 01:24:21 GMT  
		Size: 437.2 MB (437199372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1d0487cdc96ec575cc7508097c8d8e1b0b0fc14d70e3478e43d04d0c4ef88130
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.8 MB (785846180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff2ba19a83eca63cca34a699af128f82405633e67c43dfc99c5ed633ecc329f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:05:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:08:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:08:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:08:23 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:19:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ce101c5379362c5d849146976146cdb15940589c3378f71530e726706b160`  
		Last Modified: Fri, 16 Jun 2023 01:43:18 GMT  
		Size: 1.2 MB (1199977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7326ceba9de7061d919892605fd699e778fbaf87d16a5e3c3506e23a475fa`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 5.5 MB (5533346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8660fa6a9889b47b0cdedcd38551c4c097b74330bc7a35fd279ee17d32d7d67e`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097712cf91a87b7360886785f2a964a56ce10c8e4f3a77000f83523967fa20a`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff70657adfd24e02a562b4b09fdd26c26299a6001899ed61f0a8d56fb4e6f7`  
		Last Modified: Fri, 16 Jun 2023 01:43:49 GMT  
		Size: 171.5 MB (171538574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a43a9a62bd1e51770b576e70e4a54589303e48ac0c92cd9b8e010d58561397`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b2416bfb26d974c3da81f7eee6b7acfdb4eccae5aa2c72651e419946abed85`  
		Last Modified: Fri, 16 Jun 2023 01:44:03 GMT  
		Size: 45.2 MB (45205161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1bfa67a8583b7c003a10dc5da1e0a39d70b559bb0ef4854efb785d8a227d1e`  
		Last Modified: Fri, 16 Jun 2023 01:43:58 GMT  
		Size: 300.9 KB (300915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4152459f508eaf13deb06ac7708780ad620739b8cd3b7719a65bc728be19dd88`  
		Last Modified: Fri, 16 Jun 2023 01:44:06 GMT  
		Size: 72.0 MB (71971225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e30f904686801514f906f4b10630900fa5c7551ceb8e71256813143c09bdc64`  
		Last Modified: Fri, 16 Jun 2023 01:45:29 GMT  
		Size: 462.9 MB (462894133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:5187097b91f9867166db8f194b79252e56e40a0511c962cf1219dac1dad353fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:7596ae45e6213d6d22b2e70c609d63c1e68710f8fd1d659b9068b7ef2e114784
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359089529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96011a938d22d860cf0a4045881fa476fc88372a3239443154f1e9c3c15bdf3b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:26:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 03:30:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 03:31:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:31:29 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:31:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:32:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:33:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac94a680e3659eb88af9a60aa46eabe11de358d05cb19cf9d535083358650`  
		Last Modified: Fri, 16 Jun 2023 02:35:08 GMT  
		Size: 1.2 MB (1198722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c1fc3d4979a8cbea7949ab14296db71b51de166f987d5b8427b73ada3f02c0`  
		Last Modified: Fri, 16 Jun 2023 03:59:52 GMT  
		Size: 5.6 MB (5553799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c84d683cefaf172b68dda67c6436651b8b1563cbf6581f6d107056879bd8dd`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7b26995f6b2a9cf9efe6abea26c654753ad281e510d846acd0a50df8ecc32`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f480dd10200e3a3923db8466a2f0ace22c6a438b1fcce66e58aff7277e61ab`  
		Last Modified: Fri, 16 Jun 2023 04:00:18 GMT  
		Size: 177.0 MB (177045651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245827a1732fa0f267df2f15bcade007d9f966ca6b66aff8674eb1f2c65ff8d`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b92cb1be2be4c3303b48ae3153b399a674ba5205267a8f230094b09f4ead9`  
		Last Modified: Fri, 16 Jun 2023 04:00:35 GMT  
		Size: 50.9 MB (50939959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85074d427c0ad42d999081cdae5264fcbc3612d8f6f050416f85fe68af3ff5aa`  
		Last Modified: Fri, 16 Jun 2023 04:00:28 GMT  
		Size: 300.9 KB (300905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55740d8cb9ba6388e9f43d993eb6efead35161d874bfdc0fab522b741534dc`  
		Last Modified: Fri, 16 Jun 2023 04:00:39 GMT  
		Size: 79.6 MB (79605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0f46f7d05999238bd6bdacade5341b7aad7647305b8a480ce11228cd64a100`  
		Last Modified: Fri, 16 Jun 2023 04:00:53 GMT  
		Size: 15.9 MB (15862483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:96f0cd7c36703298b6d10cea53ed186745d1875bbd705af26b48292f4a03cbcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303380002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2c9ebb6e567b285a1a35bd8427241336bc911dbc24f6b4bf16ed25e546a9b08`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:09:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:09:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:11:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:11:22 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:11:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:13:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:14:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067db60a914b1db17390d08b8bd7e865dee500a51f35b6cc416f2f439f353955`  
		Last Modified: Fri, 16 Jun 2023 01:22:14 GMT  
		Size: 1.2 MB (1198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0881c824748bc118255bd7e676957b191f4d1fc5d9312139c1c52620c3cd2e`  
		Last Modified: Fri, 16 Jun 2023 01:22:12 GMT  
		Size: 4.7 MB (4679255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d12de37bd26c3e5b7c318c866dbb1b2da51ef7fcaf919748173b86af8be76`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60445b0a24d3a271c0344aada562719e7fb4093cd08e1c827d0f3cbe06c14a`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd28f326a43c2f4336c4d7942bad0b2e7c7c66948c45b89e2c444d11da9334`  
		Last Modified: Fri, 16 Jun 2023 01:22:40 GMT  
		Size: 157.5 MB (157544285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ab69607baa56a10b8698b59afe82be893274534a3bfca0e72b462dc40e149`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c737eaceaa561ec3829766a4f983d37b1a8025bb5a684dbc6943a7bbb893cf92`  
		Last Modified: Fri, 16 Jun 2023 01:22:55 GMT  
		Size: 40.5 MB (40503879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81c90a8a3c1dd33072bbaaad0ec5513a44ec458e3c6cdeb7f56a9db0d526ad`  
		Last Modified: Fri, 16 Jun 2023 01:22:50 GMT  
		Size: 300.9 KB (300910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634e8abbac2de0a96b0e64208fce0b241335c3727fae9cd287fd4703feee414a`  
		Last Modified: Fri, 16 Jun 2023 01:22:59 GMT  
		Size: 60.5 MB (60493810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38270c2d2b62df0c0984bde9e3ba14458e7f2af31ba66b11cdf9b3e693f01ad`  
		Last Modified: Fri, 16 Jun 2023 01:23:13 GMT  
		Size: 14.1 MB (14067605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:aaa16ee2386152940990c1eea8db66d40fbb79187f45cda6055360abf39d0029
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.4 MB (338411235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37de2da2b87b1a4c91b41c110c0665bd787fb4b6b035cf24e10b346628d6a2fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:05:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:08:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:08:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:08:23 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ce101c5379362c5d849146976146cdb15940589c3378f71530e726706b160`  
		Last Modified: Fri, 16 Jun 2023 01:43:18 GMT  
		Size: 1.2 MB (1199977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7326ceba9de7061d919892605fd699e778fbaf87d16a5e3c3506e23a475fa`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 5.5 MB (5533346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8660fa6a9889b47b0cdedcd38551c4c097b74330bc7a35fd279ee17d32d7d67e`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097712cf91a87b7360886785f2a964a56ce10c8e4f3a77000f83523967fa20a`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff70657adfd24e02a562b4b09fdd26c26299a6001899ed61f0a8d56fb4e6f7`  
		Last Modified: Fri, 16 Jun 2023 01:43:49 GMT  
		Size: 171.5 MB (171538574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a43a9a62bd1e51770b576e70e4a54589303e48ac0c92cd9b8e010d58561397`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b2416bfb26d974c3da81f7eee6b7acfdb4eccae5aa2c72651e419946abed85`  
		Last Modified: Fri, 16 Jun 2023 01:44:03 GMT  
		Size: 45.2 MB (45205161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1bfa67a8583b7c003a10dc5da1e0a39d70b559bb0ef4854efb785d8a227d1e`  
		Last Modified: Fri, 16 Jun 2023 01:43:58 GMT  
		Size: 300.9 KB (300915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4152459f508eaf13deb06ac7708780ad620739b8cd3b7719a65bc728be19dd88`  
		Last Modified: Fri, 16 Jun 2023 01:44:06 GMT  
		Size: 72.0 MB (71971225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7bdc321a49b00d166ccf367c13b2b415ca1c5ddcbc9c4f3547e683beea5c2c`  
		Last Modified: Fri, 16 Jun 2023 01:44:20 GMT  
		Size: 15.5 MB (15459188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:5187097b91f9867166db8f194b79252e56e40a0511c962cf1219dac1dad353fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:7596ae45e6213d6d22b2e70c609d63c1e68710f8fd1d659b9068b7ef2e114784
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359089529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96011a938d22d860cf0a4045881fa476fc88372a3239443154f1e9c3c15bdf3b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:26:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 03:30:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 03:31:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:31:29 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:31:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:32:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:33:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac94a680e3659eb88af9a60aa46eabe11de358d05cb19cf9d535083358650`  
		Last Modified: Fri, 16 Jun 2023 02:35:08 GMT  
		Size: 1.2 MB (1198722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c1fc3d4979a8cbea7949ab14296db71b51de166f987d5b8427b73ada3f02c0`  
		Last Modified: Fri, 16 Jun 2023 03:59:52 GMT  
		Size: 5.6 MB (5553799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c84d683cefaf172b68dda67c6436651b8b1563cbf6581f6d107056879bd8dd`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7b26995f6b2a9cf9efe6abea26c654753ad281e510d846acd0a50df8ecc32`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f480dd10200e3a3923db8466a2f0ace22c6a438b1fcce66e58aff7277e61ab`  
		Last Modified: Fri, 16 Jun 2023 04:00:18 GMT  
		Size: 177.0 MB (177045651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245827a1732fa0f267df2f15bcade007d9f966ca6b66aff8674eb1f2c65ff8d`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b92cb1be2be4c3303b48ae3153b399a674ba5205267a8f230094b09f4ead9`  
		Last Modified: Fri, 16 Jun 2023 04:00:35 GMT  
		Size: 50.9 MB (50939959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85074d427c0ad42d999081cdae5264fcbc3612d8f6f050416f85fe68af3ff5aa`  
		Last Modified: Fri, 16 Jun 2023 04:00:28 GMT  
		Size: 300.9 KB (300905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55740d8cb9ba6388e9f43d993eb6efead35161d874bfdc0fab522b741534dc`  
		Last Modified: Fri, 16 Jun 2023 04:00:39 GMT  
		Size: 79.6 MB (79605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0f46f7d05999238bd6bdacade5341b7aad7647305b8a480ce11228cd64a100`  
		Last Modified: Fri, 16 Jun 2023 04:00:53 GMT  
		Size: 15.9 MB (15862483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:96f0cd7c36703298b6d10cea53ed186745d1875bbd705af26b48292f4a03cbcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303380002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2c9ebb6e567b285a1a35bd8427241336bc911dbc24f6b4bf16ed25e546a9b08`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:09:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:09:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:11:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:11:22 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:11:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:13:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:14:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067db60a914b1db17390d08b8bd7e865dee500a51f35b6cc416f2f439f353955`  
		Last Modified: Fri, 16 Jun 2023 01:22:14 GMT  
		Size: 1.2 MB (1198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0881c824748bc118255bd7e676957b191f4d1fc5d9312139c1c52620c3cd2e`  
		Last Modified: Fri, 16 Jun 2023 01:22:12 GMT  
		Size: 4.7 MB (4679255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d12de37bd26c3e5b7c318c866dbb1b2da51ef7fcaf919748173b86af8be76`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60445b0a24d3a271c0344aada562719e7fb4093cd08e1c827d0f3cbe06c14a`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd28f326a43c2f4336c4d7942bad0b2e7c7c66948c45b89e2c444d11da9334`  
		Last Modified: Fri, 16 Jun 2023 01:22:40 GMT  
		Size: 157.5 MB (157544285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ab69607baa56a10b8698b59afe82be893274534a3bfca0e72b462dc40e149`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c737eaceaa561ec3829766a4f983d37b1a8025bb5a684dbc6943a7bbb893cf92`  
		Last Modified: Fri, 16 Jun 2023 01:22:55 GMT  
		Size: 40.5 MB (40503879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81c90a8a3c1dd33072bbaaad0ec5513a44ec458e3c6cdeb7f56a9db0d526ad`  
		Last Modified: Fri, 16 Jun 2023 01:22:50 GMT  
		Size: 300.9 KB (300910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634e8abbac2de0a96b0e64208fce0b241335c3727fae9cd287fd4703feee414a`  
		Last Modified: Fri, 16 Jun 2023 01:22:59 GMT  
		Size: 60.5 MB (60493810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38270c2d2b62df0c0984bde9e3ba14458e7f2af31ba66b11cdf9b3e693f01ad`  
		Last Modified: Fri, 16 Jun 2023 01:23:13 GMT  
		Size: 14.1 MB (14067605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:aaa16ee2386152940990c1eea8db66d40fbb79187f45cda6055360abf39d0029
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.4 MB (338411235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37de2da2b87b1a4c91b41c110c0665bd787fb4b6b035cf24e10b346628d6a2fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:05:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:08:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:08:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:08:23 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ce101c5379362c5d849146976146cdb15940589c3378f71530e726706b160`  
		Last Modified: Fri, 16 Jun 2023 01:43:18 GMT  
		Size: 1.2 MB (1199977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7326ceba9de7061d919892605fd699e778fbaf87d16a5e3c3506e23a475fa`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 5.5 MB (5533346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8660fa6a9889b47b0cdedcd38551c4c097b74330bc7a35fd279ee17d32d7d67e`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097712cf91a87b7360886785f2a964a56ce10c8e4f3a77000f83523967fa20a`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff70657adfd24e02a562b4b09fdd26c26299a6001899ed61f0a8d56fb4e6f7`  
		Last Modified: Fri, 16 Jun 2023 01:43:49 GMT  
		Size: 171.5 MB (171538574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a43a9a62bd1e51770b576e70e4a54589303e48ac0c92cd9b8e010d58561397`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b2416bfb26d974c3da81f7eee6b7acfdb4eccae5aa2c72651e419946abed85`  
		Last Modified: Fri, 16 Jun 2023 01:44:03 GMT  
		Size: 45.2 MB (45205161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1bfa67a8583b7c003a10dc5da1e0a39d70b559bb0ef4854efb785d8a227d1e`  
		Last Modified: Fri, 16 Jun 2023 01:43:58 GMT  
		Size: 300.9 KB (300915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4152459f508eaf13deb06ac7708780ad620739b8cd3b7719a65bc728be19dd88`  
		Last Modified: Fri, 16 Jun 2023 01:44:06 GMT  
		Size: 72.0 MB (71971225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7bdc321a49b00d166ccf367c13b2b415ca1c5ddcbc9c4f3547e683beea5c2c`  
		Last Modified: Fri, 16 Jun 2023 01:44:20 GMT  
		Size: 15.5 MB (15459188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:85d6814a41fb2b53ee1a72f6a9bbd6db5349e3f53144d7a3977678d9226d6c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:e494f7045c604c02e24951e5fadac6970192d9750e74fed4dce6a84553a1bbe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343227046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176ab51cd7218002277e110aa91f9a6ba9e07ea86a8b687079ecd5407dbe1ee4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:26:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 03:30:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 03:31:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:31:29 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:31:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:32:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac94a680e3659eb88af9a60aa46eabe11de358d05cb19cf9d535083358650`  
		Last Modified: Fri, 16 Jun 2023 02:35:08 GMT  
		Size: 1.2 MB (1198722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c1fc3d4979a8cbea7949ab14296db71b51de166f987d5b8427b73ada3f02c0`  
		Last Modified: Fri, 16 Jun 2023 03:59:52 GMT  
		Size: 5.6 MB (5553799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c84d683cefaf172b68dda67c6436651b8b1563cbf6581f6d107056879bd8dd`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7b26995f6b2a9cf9efe6abea26c654753ad281e510d846acd0a50df8ecc32`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f480dd10200e3a3923db8466a2f0ace22c6a438b1fcce66e58aff7277e61ab`  
		Last Modified: Fri, 16 Jun 2023 04:00:18 GMT  
		Size: 177.0 MB (177045651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245827a1732fa0f267df2f15bcade007d9f966ca6b66aff8674eb1f2c65ff8d`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b92cb1be2be4c3303b48ae3153b399a674ba5205267a8f230094b09f4ead9`  
		Last Modified: Fri, 16 Jun 2023 04:00:35 GMT  
		Size: 50.9 MB (50939959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85074d427c0ad42d999081cdae5264fcbc3612d8f6f050416f85fe68af3ff5aa`  
		Last Modified: Fri, 16 Jun 2023 04:00:28 GMT  
		Size: 300.9 KB (300905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55740d8cb9ba6388e9f43d993eb6efead35161d874bfdc0fab522b741534dc`  
		Last Modified: Fri, 16 Jun 2023 04:00:39 GMT  
		Size: 79.6 MB (79605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:00362f93138beaccc2f24ca7603855ad9e5c4c1d0fb3276731ec5cd2c9e1a194
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289312397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb397f715f738fabd09fe73d93f3af1988aebe53ecd1c2e419665dd65abef97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:09:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:09:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:11:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:11:22 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:11:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:13:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067db60a914b1db17390d08b8bd7e865dee500a51f35b6cc416f2f439f353955`  
		Last Modified: Fri, 16 Jun 2023 01:22:14 GMT  
		Size: 1.2 MB (1198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0881c824748bc118255bd7e676957b191f4d1fc5d9312139c1c52620c3cd2e`  
		Last Modified: Fri, 16 Jun 2023 01:22:12 GMT  
		Size: 4.7 MB (4679255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d12de37bd26c3e5b7c318c866dbb1b2da51ef7fcaf919748173b86af8be76`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60445b0a24d3a271c0344aada562719e7fb4093cd08e1c827d0f3cbe06c14a`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd28f326a43c2f4336c4d7942bad0b2e7c7c66948c45b89e2c444d11da9334`  
		Last Modified: Fri, 16 Jun 2023 01:22:40 GMT  
		Size: 157.5 MB (157544285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ab69607baa56a10b8698b59afe82be893274534a3bfca0e72b462dc40e149`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c737eaceaa561ec3829766a4f983d37b1a8025bb5a684dbc6943a7bbb893cf92`  
		Last Modified: Fri, 16 Jun 2023 01:22:55 GMT  
		Size: 40.5 MB (40503879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81c90a8a3c1dd33072bbaaad0ec5513a44ec458e3c6cdeb7f56a9db0d526ad`  
		Last Modified: Fri, 16 Jun 2023 01:22:50 GMT  
		Size: 300.9 KB (300910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634e8abbac2de0a96b0e64208fce0b241335c3727fae9cd287fd4703feee414a`  
		Last Modified: Fri, 16 Jun 2023 01:22:59 GMT  
		Size: 60.5 MB (60493810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b3439a82a31dd441d66f51a748e0e809e6c78e908aba0aa15301036e23e8b42d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.0 MB (322952047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a18787368117d0921c898948b5cb1fa8f7142c1c97d3fcc1821c758f2c593289`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:05:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:08:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:08:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:08:23 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ce101c5379362c5d849146976146cdb15940589c3378f71530e726706b160`  
		Last Modified: Fri, 16 Jun 2023 01:43:18 GMT  
		Size: 1.2 MB (1199977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7326ceba9de7061d919892605fd699e778fbaf87d16a5e3c3506e23a475fa`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 5.5 MB (5533346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8660fa6a9889b47b0cdedcd38551c4c097b74330bc7a35fd279ee17d32d7d67e`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097712cf91a87b7360886785f2a964a56ce10c8e4f3a77000f83523967fa20a`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff70657adfd24e02a562b4b09fdd26c26299a6001899ed61f0a8d56fb4e6f7`  
		Last Modified: Fri, 16 Jun 2023 01:43:49 GMT  
		Size: 171.5 MB (171538574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a43a9a62bd1e51770b576e70e4a54589303e48ac0c92cd9b8e010d58561397`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b2416bfb26d974c3da81f7eee6b7acfdb4eccae5aa2c72651e419946abed85`  
		Last Modified: Fri, 16 Jun 2023 01:44:03 GMT  
		Size: 45.2 MB (45205161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1bfa67a8583b7c003a10dc5da1e0a39d70b559bb0ef4854efb785d8a227d1e`  
		Last Modified: Fri, 16 Jun 2023 01:43:58 GMT  
		Size: 300.9 KB (300915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4152459f508eaf13deb06ac7708780ad620739b8cd3b7719a65bc728be19dd88`  
		Last Modified: Fri, 16 Jun 2023 01:44:06 GMT  
		Size: 72.0 MB (71971225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:85d6814a41fb2b53ee1a72f6a9bbd6db5349e3f53144d7a3977678d9226d6c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:e494f7045c604c02e24951e5fadac6970192d9750e74fed4dce6a84553a1bbe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343227046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176ab51cd7218002277e110aa91f9a6ba9e07ea86a8b687079ecd5407dbe1ee4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:26:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 03:30:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 03:31:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:31:29 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:31:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:32:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac94a680e3659eb88af9a60aa46eabe11de358d05cb19cf9d535083358650`  
		Last Modified: Fri, 16 Jun 2023 02:35:08 GMT  
		Size: 1.2 MB (1198722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c1fc3d4979a8cbea7949ab14296db71b51de166f987d5b8427b73ada3f02c0`  
		Last Modified: Fri, 16 Jun 2023 03:59:52 GMT  
		Size: 5.6 MB (5553799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c84d683cefaf172b68dda67c6436651b8b1563cbf6581f6d107056879bd8dd`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7b26995f6b2a9cf9efe6abea26c654753ad281e510d846acd0a50df8ecc32`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f480dd10200e3a3923db8466a2f0ace22c6a438b1fcce66e58aff7277e61ab`  
		Last Modified: Fri, 16 Jun 2023 04:00:18 GMT  
		Size: 177.0 MB (177045651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245827a1732fa0f267df2f15bcade007d9f966ca6b66aff8674eb1f2c65ff8d`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b92cb1be2be4c3303b48ae3153b399a674ba5205267a8f230094b09f4ead9`  
		Last Modified: Fri, 16 Jun 2023 04:00:35 GMT  
		Size: 50.9 MB (50939959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85074d427c0ad42d999081cdae5264fcbc3612d8f6f050416f85fe68af3ff5aa`  
		Last Modified: Fri, 16 Jun 2023 04:00:28 GMT  
		Size: 300.9 KB (300905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55740d8cb9ba6388e9f43d993eb6efead35161d874bfdc0fab522b741534dc`  
		Last Modified: Fri, 16 Jun 2023 04:00:39 GMT  
		Size: 79.6 MB (79605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:00362f93138beaccc2f24ca7603855ad9e5c4c1d0fb3276731ec5cd2c9e1a194
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289312397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb397f715f738fabd09fe73d93f3af1988aebe53ecd1c2e419665dd65abef97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:09:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:09:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:11:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:11:22 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:11:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:13:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067db60a914b1db17390d08b8bd7e865dee500a51f35b6cc416f2f439f353955`  
		Last Modified: Fri, 16 Jun 2023 01:22:14 GMT  
		Size: 1.2 MB (1198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0881c824748bc118255bd7e676957b191f4d1fc5d9312139c1c52620c3cd2e`  
		Last Modified: Fri, 16 Jun 2023 01:22:12 GMT  
		Size: 4.7 MB (4679255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d12de37bd26c3e5b7c318c866dbb1b2da51ef7fcaf919748173b86af8be76`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60445b0a24d3a271c0344aada562719e7fb4093cd08e1c827d0f3cbe06c14a`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd28f326a43c2f4336c4d7942bad0b2e7c7c66948c45b89e2c444d11da9334`  
		Last Modified: Fri, 16 Jun 2023 01:22:40 GMT  
		Size: 157.5 MB (157544285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ab69607baa56a10b8698b59afe82be893274534a3bfca0e72b462dc40e149`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c737eaceaa561ec3829766a4f983d37b1a8025bb5a684dbc6943a7bbb893cf92`  
		Last Modified: Fri, 16 Jun 2023 01:22:55 GMT  
		Size: 40.5 MB (40503879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca81c90a8a3c1dd33072bbaaad0ec5513a44ec458e3c6cdeb7f56a9db0d526ad`  
		Last Modified: Fri, 16 Jun 2023 01:22:50 GMT  
		Size: 300.9 KB (300910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634e8abbac2de0a96b0e64208fce0b241335c3727fae9cd287fd4703feee414a`  
		Last Modified: Fri, 16 Jun 2023 01:22:59 GMT  
		Size: 60.5 MB (60493810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b3439a82a31dd441d66f51a748e0e809e6c78e908aba0aa15301036e23e8b42d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.0 MB (322952047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a18787368117d0921c898948b5cb1fa8f7142c1c97d3fcc1821c758f2c593289`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:05:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:08:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:08:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:08:23 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ce101c5379362c5d849146976146cdb15940589c3378f71530e726706b160`  
		Last Modified: Fri, 16 Jun 2023 01:43:18 GMT  
		Size: 1.2 MB (1199977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7326ceba9de7061d919892605fd699e778fbaf87d16a5e3c3506e23a475fa`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 5.5 MB (5533346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8660fa6a9889b47b0cdedcd38551c4c097b74330bc7a35fd279ee17d32d7d67e`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097712cf91a87b7360886785f2a964a56ce10c8e4f3a77000f83523967fa20a`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff70657adfd24e02a562b4b09fdd26c26299a6001899ed61f0a8d56fb4e6f7`  
		Last Modified: Fri, 16 Jun 2023 01:43:49 GMT  
		Size: 171.5 MB (171538574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a43a9a62bd1e51770b576e70e4a54589303e48ac0c92cd9b8e010d58561397`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b2416bfb26d974c3da81f7eee6b7acfdb4eccae5aa2c72651e419946abed85`  
		Last Modified: Fri, 16 Jun 2023 01:44:03 GMT  
		Size: 45.2 MB (45205161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1bfa67a8583b7c003a10dc5da1e0a39d70b559bb0ef4854efb785d8a227d1e`  
		Last Modified: Fri, 16 Jun 2023 01:43:58 GMT  
		Size: 300.9 KB (300915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4152459f508eaf13deb06ac7708780ad620739b8cd3b7719a65bc728be19dd88`  
		Last Modified: Fri, 16 Jun 2023 01:44:06 GMT  
		Size: 72.0 MB (71971225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:e1889fa73a738575e5f19cc1ec1becc1b18c6cf63aeef91fbc56fc356c77fdbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:37084b9972c0fd2ef118eec80c749551cfad67ca88c8de4a900e5bdf749b5f68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212381108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06cdf08f23aa4d698b7d5377017f796cdcb9c701b8e7e5e8d3a6953bb4924b09`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:26:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 03:30:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 03:31:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:31:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac94a680e3659eb88af9a60aa46eabe11de358d05cb19cf9d535083358650`  
		Last Modified: Fri, 16 Jun 2023 02:35:08 GMT  
		Size: 1.2 MB (1198722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c1fc3d4979a8cbea7949ab14296db71b51de166f987d5b8427b73ada3f02c0`  
		Last Modified: Fri, 16 Jun 2023 03:59:52 GMT  
		Size: 5.6 MB (5553799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c84d683cefaf172b68dda67c6436651b8b1563cbf6581f6d107056879bd8dd`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7b26995f6b2a9cf9efe6abea26c654753ad281e510d846acd0a50df8ecc32`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f480dd10200e3a3923db8466a2f0ace22c6a438b1fcce66e58aff7277e61ab`  
		Last Modified: Fri, 16 Jun 2023 04:00:18 GMT  
		Size: 177.0 MB (177045651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245827a1732fa0f267df2f15bcade007d9f966ca6b66aff8674eb1f2c65ff8d`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:fedd732d5c2543cd83cca86cdc9c4d5c5ed67e3b35a5e30feb6ee17f52acd53c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (188013798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19ebdc1715edcc59196c6c3efbaf12c01535fffb2e80808368c76f8898cea37`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:09:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:09:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:11:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:11:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067db60a914b1db17390d08b8bd7e865dee500a51f35b6cc416f2f439f353955`  
		Last Modified: Fri, 16 Jun 2023 01:22:14 GMT  
		Size: 1.2 MB (1198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0881c824748bc118255bd7e676957b191f4d1fc5d9312139c1c52620c3cd2e`  
		Last Modified: Fri, 16 Jun 2023 01:22:12 GMT  
		Size: 4.7 MB (4679255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d12de37bd26c3e5b7c318c866dbb1b2da51ef7fcaf919748173b86af8be76`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60445b0a24d3a271c0344aada562719e7fb4093cd08e1c827d0f3cbe06c14a`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd28f326a43c2f4336c4d7942bad0b2e7c7c66948c45b89e2c444d11da9334`  
		Last Modified: Fri, 16 Jun 2023 01:22:40 GMT  
		Size: 157.5 MB (157544285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ab69607baa56a10b8698b59afe82be893274534a3bfca0e72b462dc40e149`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8bae94704e0339230b871f71d667a499e958bb10a52745b3ad287893b5a8ad56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.5 MB (205474746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36edb17b6ade6bf4a129685f1623dc52ce6d75b0e48f77b2fd834ba8639950b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:05:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:08:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:08:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:08:23 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ce101c5379362c5d849146976146cdb15940589c3378f71530e726706b160`  
		Last Modified: Fri, 16 Jun 2023 01:43:18 GMT  
		Size: 1.2 MB (1199977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7326ceba9de7061d919892605fd699e778fbaf87d16a5e3c3506e23a475fa`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 5.5 MB (5533346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8660fa6a9889b47b0cdedcd38551c4c097b74330bc7a35fd279ee17d32d7d67e`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097712cf91a87b7360886785f2a964a56ce10c8e4f3a77000f83523967fa20a`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff70657adfd24e02a562b4b09fdd26c26299a6001899ed61f0a8d56fb4e6f7`  
		Last Modified: Fri, 16 Jun 2023 01:43:49 GMT  
		Size: 171.5 MB (171538574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a43a9a62bd1e51770b576e70e4a54589303e48ac0c92cd9b8e010d58561397`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:e1889fa73a738575e5f19cc1ec1becc1b18c6cf63aeef91fbc56fc356c77fdbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:37084b9972c0fd2ef118eec80c749551cfad67ca88c8de4a900e5bdf749b5f68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212381108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06cdf08f23aa4d698b7d5377017f796cdcb9c701b8e7e5e8d3a6953bb4924b09`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:26:02 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:30:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 03:30:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:30:05 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 03:31:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:31:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 03:31:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:31:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ac94a680e3659eb88af9a60aa46eabe11de358d05cb19cf9d535083358650`  
		Last Modified: Fri, 16 Jun 2023 02:35:08 GMT  
		Size: 1.2 MB (1198722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c1fc3d4979a8cbea7949ab14296db71b51de166f987d5b8427b73ada3f02c0`  
		Last Modified: Fri, 16 Jun 2023 03:59:52 GMT  
		Size: 5.6 MB (5553799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c84d683cefaf172b68dda67c6436651b8b1563cbf6581f6d107056879bd8dd`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7b26995f6b2a9cf9efe6abea26c654753ad281e510d846acd0a50df8ecc32`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f480dd10200e3a3923db8466a2f0ace22c6a438b1fcce66e58aff7277e61ab`  
		Last Modified: Fri, 16 Jun 2023 04:00:18 GMT  
		Size: 177.0 MB (177045651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245827a1732fa0f267df2f15bcade007d9f966ca6b66aff8674eb1f2c65ff8d`  
		Last Modified: Fri, 16 Jun 2023 03:59:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:fedd732d5c2543cd83cca86cdc9c4d5c5ed67e3b35a5e30feb6ee17f52acd53c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.0 MB (188013798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19ebdc1715edcc59196c6c3efbaf12c01535fffb2e80808368c76f8898cea37`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:09:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:09:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:09:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:09:08 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:11:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:11:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:11:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067db60a914b1db17390d08b8bd7e865dee500a51f35b6cc416f2f439f353955`  
		Last Modified: Fri, 16 Jun 2023 01:22:14 GMT  
		Size: 1.2 MB (1198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0881c824748bc118255bd7e676957b191f4d1fc5d9312139c1c52620c3cd2e`  
		Last Modified: Fri, 16 Jun 2023 01:22:12 GMT  
		Size: 4.7 MB (4679255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d12de37bd26c3e5b7c318c866dbb1b2da51ef7fcaf919748173b86af8be76`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60445b0a24d3a271c0344aada562719e7fb4093cd08e1c827d0f3cbe06c14a`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd28f326a43c2f4336c4d7942bad0b2e7c7c66948c45b89e2c444d11da9334`  
		Last Modified: Fri, 16 Jun 2023 01:22:40 GMT  
		Size: 157.5 MB (157544285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ab69607baa56a10b8698b59afe82be893274534a3bfca0e72b462dc40e149`  
		Last Modified: Fri, 16 Jun 2023 01:22:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8bae94704e0339230b871f71d667a499e958bb10a52745b3ad287893b5a8ad56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.5 MB (205474746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36edb17b6ade6bf4a129685f1623dc52ce6d75b0e48f77b2fd834ba8639950b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 16 Jun 2023 01:05:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:05:25 GMT
ENV ROS_DISTRO=noetic
# Fri, 16 Jun 2023 01:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:08:23 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 16 Jun 2023 01:08:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:08:23 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ce101c5379362c5d849146976146cdb15940589c3378f71530e726706b160`  
		Last Modified: Fri, 16 Jun 2023 01:43:18 GMT  
		Size: 1.2 MB (1199977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7326ceba9de7061d919892605fd699e778fbaf87d16a5e3c3506e23a475fa`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 5.5 MB (5533346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8660fa6a9889b47b0cdedcd38551c4c097b74330bc7a35fd279ee17d32d7d67e`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097712cf91a87b7360886785f2a964a56ce10c8e4f3a77000f83523967fa20a`  
		Last Modified: Fri, 16 Jun 2023 01:43:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff70657adfd24e02a562b4b09fdd26c26299a6001899ed61f0a8d56fb4e6f7`  
		Last Modified: Fri, 16 Jun 2023 01:43:49 GMT  
		Size: 171.5 MB (171538574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a43a9a62bd1e51770b576e70e4a54589303e48ac0c92cd9b8e010d58561397`  
		Last Modified: Fri, 16 Jun 2023 01:43:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:8d1542a5b120a611e721c321ba054d3c6053f56b5bd0704d647b3a9e91bccb0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:8497de34b4fe4b0df00111367044c08064e38fb418b1a33df6dd2bfdbdde7dc4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268602115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ad0b914c35f8238a129916ac0034e4c3d1fbb552bb4d81abec3e7d61848578`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:56:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 03:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:56:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:56:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:56:45 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:57:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:57:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:57:15 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:57:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633a85d8b769a40385318439a6f0f1cad7c66a4116b0059a2c48c5c4342830bf`  
		Last Modified: Fri, 16 Jun 2023 04:08:46 GMT  
		Size: 124.1 MB (124135661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca2b18dfa14242c98eb39564e643e0d31b3be2d041ad51b216e2ca5ffe9fd95`  
		Last Modified: Fri, 16 Jun 2023 04:08:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171da17a95f927ae2c266d0d3de58b3fe4341927154d17e35721facfe3eac4f4`  
		Last Modified: Fri, 16 Jun 2023 04:09:06 GMT  
		Size: 85.0 MB (84994585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3468ea45a1acf261f7788a676e5842a16525bcd22e5c962fcda17578cea607d5`  
		Last Modified: Fri, 16 Jun 2023 04:08:55 GMT  
		Size: 288.4 KB (288357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a388e36085189206d87204728e5488d1842c2bb7aa1a1f220ee7918585cd7354`  
		Last Modified: Fri, 16 Jun 2023 04:08:55 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9083010f25afa882d316ac8c410ca3dc4b74217062605e9d8013032f4dad4d20`  
		Last Modified: Fri, 16 Jun 2023 04:08:59 GMT  
		Size: 23.7 MB (23706079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:00e264fc348260357cfa64dc9632a7798d457407b7260614f0b3c52a08e9c1e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261151859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aeeb1514fc5be644e97b6a96e425f0d87d44b0b90568313d892ef297a615a97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:39:25 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 01:40:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:40:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:40:08 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:40:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:40:32 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:40:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7681b598e87b602bd3949a3eee83c75b9389326287e67fb4ebddffee4803501b`  
		Last Modified: Fri, 16 Jun 2023 01:52:06 GMT  
		Size: 121.6 MB (121622225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263fa8c020c1c3a7ec3dbfe871c520c497b02eb4e41e9c902faca840f7463c4`  
		Last Modified: Fri, 16 Jun 2023 01:51:41 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079c2928d31a9d9aadbba7319d84caaec10ef28b5b361956af0f8b4442f1747`  
		Last Modified: Fri, 16 Jun 2023 01:52:23 GMT  
		Size: 82.7 MB (82736302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67183db26ea86b357090e2f539378fbadc07d4018e4664be54ff17a4e204f43`  
		Last Modified: Fri, 16 Jun 2023 01:52:14 GMT  
		Size: 288.4 KB (288368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42b58b1c944ab4dbdf7a9517731ae92f60c0b52ffc38ce2b84830cf3eb7c320`  
		Last Modified: Fri, 16 Jun 2023 01:52:14 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850a5dcaad9eadb53879cc755bfcb0822a3ee0ae43e624742da2c4d26af362b0`  
		Last Modified: Fri, 16 Jun 2023 01:52:18 GMT  
		Size: 23.1 MB (23096329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:89fe3730271a56b684065cb18307a1d43d8d37249225dfc4df37dc43596efbb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:404112afacd92f527f984c5eb67fa99545778bebc4493f90108b3ac68b728b6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **958.4 MB (958372278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b906d3d4a9070d782cb6d380f249baa14b49bc9c90b2f6a36168243630bd27`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:56:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 03:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:56:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:56:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:56:45 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:57:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:57:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:57:15 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:57:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633a85d8b769a40385318439a6f0f1cad7c66a4116b0059a2c48c5c4342830bf`  
		Last Modified: Fri, 16 Jun 2023 04:08:46 GMT  
		Size: 124.1 MB (124135661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca2b18dfa14242c98eb39564e643e0d31b3be2d041ad51b216e2ca5ffe9fd95`  
		Last Modified: Fri, 16 Jun 2023 04:08:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171da17a95f927ae2c266d0d3de58b3fe4341927154d17e35721facfe3eac4f4`  
		Last Modified: Fri, 16 Jun 2023 04:09:06 GMT  
		Size: 85.0 MB (84994585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3468ea45a1acf261f7788a676e5842a16525bcd22e5c962fcda17578cea607d5`  
		Last Modified: Fri, 16 Jun 2023 04:08:55 GMT  
		Size: 288.4 KB (288357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a388e36085189206d87204728e5488d1842c2bb7aa1a1f220ee7918585cd7354`  
		Last Modified: Fri, 16 Jun 2023 04:08:55 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9083010f25afa882d316ac8c410ca3dc4b74217062605e9d8013032f4dad4d20`  
		Last Modified: Fri, 16 Jun 2023 04:08:59 GMT  
		Size: 23.7 MB (23706079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b11258a0ffaa211656df523f4bfdcc63731fb659bc3f504287135be537ad0d`  
		Last Modified: Fri, 16 Jun 2023 04:10:44 GMT  
		Size: 689.8 MB (689770163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:21f61e7c7791edddb2349ca5155187919a5732f7027d369f26887b6e6e11667b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **919.6 MB (919615081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a3604a059bf89b93332fd8869af4feba6203a290b8c6d340d41d2ef8f43101a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:39:25 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 01:40:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:40:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:40:08 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:40:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:40:32 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:40:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:42:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7681b598e87b602bd3949a3eee83c75b9389326287e67fb4ebddffee4803501b`  
		Last Modified: Fri, 16 Jun 2023 01:52:06 GMT  
		Size: 121.6 MB (121622225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263fa8c020c1c3a7ec3dbfe871c520c497b02eb4e41e9c902faca840f7463c4`  
		Last Modified: Fri, 16 Jun 2023 01:51:41 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079c2928d31a9d9aadbba7319d84caaec10ef28b5b361956af0f8b4442f1747`  
		Last Modified: Fri, 16 Jun 2023 01:52:23 GMT  
		Size: 82.7 MB (82736302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67183db26ea86b357090e2f539378fbadc07d4018e4664be54ff17a4e204f43`  
		Last Modified: Fri, 16 Jun 2023 01:52:14 GMT  
		Size: 288.4 KB (288368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42b58b1c944ab4dbdf7a9517731ae92f60c0b52ffc38ce2b84830cf3eb7c320`  
		Last Modified: Fri, 16 Jun 2023 01:52:14 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850a5dcaad9eadb53879cc755bfcb0822a3ee0ae43e624742da2c4d26af362b0`  
		Last Modified: Fri, 16 Jun 2023 01:52:18 GMT  
		Size: 23.1 MB (23096329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b961f8f30d2ba754db8817a228ab0b459093408fc2bb2d090f57c90ea9a464fe`  
		Last Modified: Fri, 16 Jun 2023 01:53:55 GMT  
		Size: 658.5 MB (658463222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:89fe3730271a56b684065cb18307a1d43d8d37249225dfc4df37dc43596efbb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:404112afacd92f527f984c5eb67fa99545778bebc4493f90108b3ac68b728b6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **958.4 MB (958372278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b906d3d4a9070d782cb6d380f249baa14b49bc9c90b2f6a36168243630bd27`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:56:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 03:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:56:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:56:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:56:45 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:57:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:57:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:57:15 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:57:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633a85d8b769a40385318439a6f0f1cad7c66a4116b0059a2c48c5c4342830bf`  
		Last Modified: Fri, 16 Jun 2023 04:08:46 GMT  
		Size: 124.1 MB (124135661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca2b18dfa14242c98eb39564e643e0d31b3be2d041ad51b216e2ca5ffe9fd95`  
		Last Modified: Fri, 16 Jun 2023 04:08:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171da17a95f927ae2c266d0d3de58b3fe4341927154d17e35721facfe3eac4f4`  
		Last Modified: Fri, 16 Jun 2023 04:09:06 GMT  
		Size: 85.0 MB (84994585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3468ea45a1acf261f7788a676e5842a16525bcd22e5c962fcda17578cea607d5`  
		Last Modified: Fri, 16 Jun 2023 04:08:55 GMT  
		Size: 288.4 KB (288357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a388e36085189206d87204728e5488d1842c2bb7aa1a1f220ee7918585cd7354`  
		Last Modified: Fri, 16 Jun 2023 04:08:55 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9083010f25afa882d316ac8c410ca3dc4b74217062605e9d8013032f4dad4d20`  
		Last Modified: Fri, 16 Jun 2023 04:08:59 GMT  
		Size: 23.7 MB (23706079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b11258a0ffaa211656df523f4bfdcc63731fb659bc3f504287135be537ad0d`  
		Last Modified: Fri, 16 Jun 2023 04:10:44 GMT  
		Size: 689.8 MB (689770163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:21f61e7c7791edddb2349ca5155187919a5732f7027d369f26887b6e6e11667b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **919.6 MB (919615081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a3604a059bf89b93332fd8869af4feba6203a290b8c6d340d41d2ef8f43101a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:39:25 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 01:40:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:40:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:40:08 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:40:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:40:32 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:40:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:42:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7681b598e87b602bd3949a3eee83c75b9389326287e67fb4ebddffee4803501b`  
		Last Modified: Fri, 16 Jun 2023 01:52:06 GMT  
		Size: 121.6 MB (121622225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263fa8c020c1c3a7ec3dbfe871c520c497b02eb4e41e9c902faca840f7463c4`  
		Last Modified: Fri, 16 Jun 2023 01:51:41 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079c2928d31a9d9aadbba7319d84caaec10ef28b5b361956af0f8b4442f1747`  
		Last Modified: Fri, 16 Jun 2023 01:52:23 GMT  
		Size: 82.7 MB (82736302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67183db26ea86b357090e2f539378fbadc07d4018e4664be54ff17a4e204f43`  
		Last Modified: Fri, 16 Jun 2023 01:52:14 GMT  
		Size: 288.4 KB (288368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42b58b1c944ab4dbdf7a9517731ae92f60c0b52ffc38ce2b84830cf3eb7c320`  
		Last Modified: Fri, 16 Jun 2023 01:52:14 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850a5dcaad9eadb53879cc755bfcb0822a3ee0ae43e624742da2c4d26af362b0`  
		Last Modified: Fri, 16 Jun 2023 01:52:18 GMT  
		Size: 23.1 MB (23096329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b961f8f30d2ba754db8817a228ab0b459093408fc2bb2d090f57c90ea9a464fe`  
		Last Modified: Fri, 16 Jun 2023 01:53:55 GMT  
		Size: 658.5 MB (658463222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:8d1542a5b120a611e721c321ba054d3c6053f56b5bd0704d647b3a9e91bccb0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:8497de34b4fe4b0df00111367044c08064e38fb418b1a33df6dd2bfdbdde7dc4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268602115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ad0b914c35f8238a129916ac0034e4c3d1fbb552bb4d81abec3e7d61848578`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:56:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 03:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:56:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:56:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:56:45 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:57:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:57:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:57:15 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:57:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633a85d8b769a40385318439a6f0f1cad7c66a4116b0059a2c48c5c4342830bf`  
		Last Modified: Fri, 16 Jun 2023 04:08:46 GMT  
		Size: 124.1 MB (124135661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca2b18dfa14242c98eb39564e643e0d31b3be2d041ad51b216e2ca5ffe9fd95`  
		Last Modified: Fri, 16 Jun 2023 04:08:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171da17a95f927ae2c266d0d3de58b3fe4341927154d17e35721facfe3eac4f4`  
		Last Modified: Fri, 16 Jun 2023 04:09:06 GMT  
		Size: 85.0 MB (84994585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3468ea45a1acf261f7788a676e5842a16525bcd22e5c962fcda17578cea607d5`  
		Last Modified: Fri, 16 Jun 2023 04:08:55 GMT  
		Size: 288.4 KB (288357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a388e36085189206d87204728e5488d1842c2bb7aa1a1f220ee7918585cd7354`  
		Last Modified: Fri, 16 Jun 2023 04:08:55 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9083010f25afa882d316ac8c410ca3dc4b74217062605e9d8013032f4dad4d20`  
		Last Modified: Fri, 16 Jun 2023 04:08:59 GMT  
		Size: 23.7 MB (23706079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:00e264fc348260357cfa64dc9632a7798d457407b7260614f0b3c52a08e9c1e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261151859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aeeb1514fc5be644e97b6a96e425f0d87d44b0b90568313d892ef297a615a97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:39:25 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 01:40:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:40:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:40:08 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:40:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:40:32 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:40:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7681b598e87b602bd3949a3eee83c75b9389326287e67fb4ebddffee4803501b`  
		Last Modified: Fri, 16 Jun 2023 01:52:06 GMT  
		Size: 121.6 MB (121622225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263fa8c020c1c3a7ec3dbfe871c520c497b02eb4e41e9c902faca840f7463c4`  
		Last Modified: Fri, 16 Jun 2023 01:51:41 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079c2928d31a9d9aadbba7319d84caaec10ef28b5b361956af0f8b4442f1747`  
		Last Modified: Fri, 16 Jun 2023 01:52:23 GMT  
		Size: 82.7 MB (82736302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67183db26ea86b357090e2f539378fbadc07d4018e4664be54ff17a4e204f43`  
		Last Modified: Fri, 16 Jun 2023 01:52:14 GMT  
		Size: 288.4 KB (288368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42b58b1c944ab4dbdf7a9517731ae92f60c0b52ffc38ce2b84830cf3eb7c320`  
		Last Modified: Fri, 16 Jun 2023 01:52:14 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850a5dcaad9eadb53879cc755bfcb0822a3ee0ae43e624742da2c4d26af362b0`  
		Last Modified: Fri, 16 Jun 2023 01:52:18 GMT  
		Size: 23.1 MB (23096329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:8d1542a5b120a611e721c321ba054d3c6053f56b5bd0704d647b3a9e91bccb0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:8497de34b4fe4b0df00111367044c08064e38fb418b1a33df6dd2bfdbdde7dc4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268602115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ad0b914c35f8238a129916ac0034e4c3d1fbb552bb4d81abec3e7d61848578`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:56:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 03:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:56:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:56:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:56:45 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 03:57:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:57:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 03:57:15 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 03:57:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633a85d8b769a40385318439a6f0f1cad7c66a4116b0059a2c48c5c4342830bf`  
		Last Modified: Fri, 16 Jun 2023 04:08:46 GMT  
		Size: 124.1 MB (124135661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca2b18dfa14242c98eb39564e643e0d31b3be2d041ad51b216e2ca5ffe9fd95`  
		Last Modified: Fri, 16 Jun 2023 04:08:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171da17a95f927ae2c266d0d3de58b3fe4341927154d17e35721facfe3eac4f4`  
		Last Modified: Fri, 16 Jun 2023 04:09:06 GMT  
		Size: 85.0 MB (84994585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3468ea45a1acf261f7788a676e5842a16525bcd22e5c962fcda17578cea607d5`  
		Last Modified: Fri, 16 Jun 2023 04:08:55 GMT  
		Size: 288.4 KB (288357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a388e36085189206d87204728e5488d1842c2bb7aa1a1f220ee7918585cd7354`  
		Last Modified: Fri, 16 Jun 2023 04:08:55 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9083010f25afa882d316ac8c410ca3dc4b74217062605e9d8013032f4dad4d20`  
		Last Modified: Fri, 16 Jun 2023 04:08:59 GMT  
		Size: 23.7 MB (23706079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:00e264fc348260357cfa64dc9632a7798d457407b7260614f0b3c52a08e9c1e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261151859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aeeb1514fc5be644e97b6a96e425f0d87d44b0b90568313d892ef297a615a97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:39:25 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 01:40:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:40:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:40:08 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 01:40:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 16 Jun 2023 01:40:32 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 16 Jun 2023 01:40:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7681b598e87b602bd3949a3eee83c75b9389326287e67fb4ebddffee4803501b`  
		Last Modified: Fri, 16 Jun 2023 01:52:06 GMT  
		Size: 121.6 MB (121622225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263fa8c020c1c3a7ec3dbfe871c520c497b02eb4e41e9c902faca840f7463c4`  
		Last Modified: Fri, 16 Jun 2023 01:51:41 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079c2928d31a9d9aadbba7319d84caaec10ef28b5b361956af0f8b4442f1747`  
		Last Modified: Fri, 16 Jun 2023 01:52:23 GMT  
		Size: 82.7 MB (82736302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67183db26ea86b357090e2f539378fbadc07d4018e4664be54ff17a4e204f43`  
		Last Modified: Fri, 16 Jun 2023 01:52:14 GMT  
		Size: 288.4 KB (288368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42b58b1c944ab4dbdf7a9517731ae92f60c0b52ffc38ce2b84830cf3eb7c320`  
		Last Modified: Fri, 16 Jun 2023 01:52:14 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850a5dcaad9eadb53879cc755bfcb0822a3ee0ae43e624742da2c4d26af362b0`  
		Last Modified: Fri, 16 Jun 2023 01:52:18 GMT  
		Size: 23.1 MB (23096329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:f9122d7d25389b2b923dcbdfc2e43cd562f3aff7fcbee022dafdfaec05ee9351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:9994ed2d554dbd38612aeb1fb123cc287d3dac987d9a11547b64801416e55be2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159610689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d69cbdcfef7db7c7a55cf088b40bc72c704ea9b8896f8126a6065a60d162df53`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:56:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 03:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:56:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:56:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:56:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633a85d8b769a40385318439a6f0f1cad7c66a4116b0059a2c48c5c4342830bf`  
		Last Modified: Fri, 16 Jun 2023 04:08:46 GMT  
		Size: 124.1 MB (124135661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca2b18dfa14242c98eb39564e643e0d31b3be2d041ad51b216e2ca5ffe9fd95`  
		Last Modified: Fri, 16 Jun 2023 04:08:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:97b9968865d1d85a4d9ed85d10fe31068e591bcc7e31ec322178b68346393337
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155028439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960ebba83544fe11d889235dcbdcfc80ae3ac8027467afff79efc65952ccc2bc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:39:25 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 01:40:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:40:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:40:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7681b598e87b602bd3949a3eee83c75b9389326287e67fb4ebddffee4803501b`  
		Last Modified: Fri, 16 Jun 2023 01:52:06 GMT  
		Size: 121.6 MB (121622225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263fa8c020c1c3a7ec3dbfe871c520c497b02eb4e41e9c902faca840f7463c4`  
		Last Modified: Fri, 16 Jun 2023 01:51:41 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:f9122d7d25389b2b923dcbdfc2e43cd562f3aff7fcbee022dafdfaec05ee9351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:9994ed2d554dbd38612aeb1fb123cc287d3dac987d9a11547b64801416e55be2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159610689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d69cbdcfef7db7c7a55cf088b40bc72c704ea9b8896f8126a6065a60d162df53`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:41:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:41:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 03:41:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 03:41:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 03:41:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 03:56:05 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 03:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 03:56:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 03:56:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 03:56:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b169f458fb68eaad31436347ddfc7e25dd97c37d8cb63f22e84e7f95d4fa19b`  
		Last Modified: Fri, 16 Jun 2023 04:03:37 GMT  
		Size: 1.2 MB (1212828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf80c9011de772b9b9ef6bbfe82a4f648cba6a09b044082641c5a232558d5a`  
		Last Modified: Fri, 16 Jun 2023 04:03:35 GMT  
		Size: 3.8 MB (3828743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa9834c66b60b85dc4ddfef495ea84f47531b25092c93ce7cea642ccf57ef2b`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d2a49f11b048e53a72852bd937876370b9ba2c2448fff57054b14f67466f0`  
		Last Modified: Fri, 16 Jun 2023 04:03:34 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633a85d8b769a40385318439a6f0f1cad7c66a4116b0059a2c48c5c4342830bf`  
		Last Modified: Fri, 16 Jun 2023 04:08:46 GMT  
		Size: 124.1 MB (124135661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca2b18dfa14242c98eb39564e643e0d31b3be2d041ad51b216e2ca5ffe9fd95`  
		Last Modified: Fri, 16 Jun 2023 04:08:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:97b9968865d1d85a4d9ed85d10fe31068e591bcc7e31ec322178b68346393337
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155028439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960ebba83544fe11d889235dcbdcfc80ae3ac8027467afff79efc65952ccc2bc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:39:25 GMT
ENV ROS_DISTRO=rolling
# Fri, 16 Jun 2023 01:40:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:40:08 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:40:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:40:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7681b598e87b602bd3949a3eee83c75b9389326287e67fb4ebddffee4803501b`  
		Last Modified: Fri, 16 Jun 2023 01:52:06 GMT  
		Size: 121.6 MB (121622225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263fa8c020c1c3a7ec3dbfe871c520c497b02eb4e41e9c902faca840f7463c4`  
		Last Modified: Fri, 16 Jun 2023 01:51:41 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
