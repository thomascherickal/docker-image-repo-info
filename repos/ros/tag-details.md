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
$ docker pull ros@sha256:6e776f1a869bccaee01cbd2397a6b9c74499f5ffca2e995b5ac6a1b894aefd56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:add9970136f8920882152f611577326f7e23b0ef9a7069b8152de089ee9ac730
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250620496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2208eebb028dc4838ab0afc9b35e3de393855272172cdf1748b12e3c6704fe16`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 04:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:43:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:43:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:43:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:44:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e812731a44ee6ed8eb6f479ee177db4e6f5dc9b8f586e3bec76b68bd87b057`  
		Last Modified: Fri, 02 Sep 2022 05:09:37 GMT  
		Size: 120.1 MB (120084257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ce07703bc6ca66551202ce709d2db142f2284d1758e1ae63b0089816db684`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1890f880d76adc2a15589d899c1971bfe3b8c53a24b095b14ff503208a19d2fc`  
		Last Modified: Fri, 02 Sep 2022 05:09:58 GMT  
		Size: 73.3 MB (73321532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1250a9090832c70a8cbb5b16a1c4fb04bd15cb731dc383b88e5e8920a07637`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 262.8 KB (262804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e10b955d6703772baf23131f34012e192b6651bae2f45d5ec1de94db2d65c9`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 2.4 KB (2425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7586ba8a53515e3a1b9937feaad2e7fede1adbc084ac2d100da1e4a7babb88cf`  
		Last Modified: Fri, 02 Sep 2022 05:09:51 GMT  
		Size: 21.7 MB (21663632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1d667d617e8cf2205c98aec3d4e9667a704e7e1270e6ccceacff672383ee73cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.0 MB (226030547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3f71e64f6f4bbd5dfdb2c020a056ff2446a5c0468227138239c599b8f10b13`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:09:25 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 06:10:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:10:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:10:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:10:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:11:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6669566fcc115df3d85e1176e7e645889db7959d6a954ba485ed11367dc9863a`  
		Last Modified: Fri, 02 Sep 2022 06:32:07 GMT  
		Size: 104.3 MB (104266721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d0c7829bec3aa8e600c8677d001a505e7a97ce46e7e8d34a667fa41b38b06a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5f8d617cb17da8504e284767c00fc2feed07e2f35c7a7b4313b804d53e56b8`  
		Last Modified: Fri, 02 Sep 2022 06:32:28 GMT  
		Size: 67.4 MB (67449113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6935c838d5eb4cd0b713a76063e82036a165b8bc62634dec158e4729749a38`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 262.7 KB (262739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707611d281f0c907bf51272891d4009de29c408cf77e296e33d8b7dc31983b3`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 2.4 KB (2378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a2c9bbb7d25390f08e6efb8200c4a037a6c8bd6980b91e33212c2d3378a6d`  
		Last Modified: Fri, 02 Sep 2022 06:32:21 GMT  
		Size: 20.4 MB (20366833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:6e776f1a869bccaee01cbd2397a6b9c74499f5ffca2e995b5ac6a1b894aefd56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:add9970136f8920882152f611577326f7e23b0ef9a7069b8152de089ee9ac730
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250620496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2208eebb028dc4838ab0afc9b35e3de393855272172cdf1748b12e3c6704fe16`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 04:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:43:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:43:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:43:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:44:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e812731a44ee6ed8eb6f479ee177db4e6f5dc9b8f586e3bec76b68bd87b057`  
		Last Modified: Fri, 02 Sep 2022 05:09:37 GMT  
		Size: 120.1 MB (120084257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ce07703bc6ca66551202ce709d2db142f2284d1758e1ae63b0089816db684`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1890f880d76adc2a15589d899c1971bfe3b8c53a24b095b14ff503208a19d2fc`  
		Last Modified: Fri, 02 Sep 2022 05:09:58 GMT  
		Size: 73.3 MB (73321532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1250a9090832c70a8cbb5b16a1c4fb04bd15cb731dc383b88e5e8920a07637`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 262.8 KB (262804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e10b955d6703772baf23131f34012e192b6651bae2f45d5ec1de94db2d65c9`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 2.4 KB (2425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7586ba8a53515e3a1b9937feaad2e7fede1adbc084ac2d100da1e4a7babb88cf`  
		Last Modified: Fri, 02 Sep 2022 05:09:51 GMT  
		Size: 21.7 MB (21663632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1d667d617e8cf2205c98aec3d4e9667a704e7e1270e6ccceacff672383ee73cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.0 MB (226030547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3f71e64f6f4bbd5dfdb2c020a056ff2446a5c0468227138239c599b8f10b13`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:09:25 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 06:10:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:10:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:10:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:10:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:11:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6669566fcc115df3d85e1176e7e645889db7959d6a954ba485ed11367dc9863a`  
		Last Modified: Fri, 02 Sep 2022 06:32:07 GMT  
		Size: 104.3 MB (104266721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d0c7829bec3aa8e600c8677d001a505e7a97ce46e7e8d34a667fa41b38b06a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5f8d617cb17da8504e284767c00fc2feed07e2f35c7a7b4313b804d53e56b8`  
		Last Modified: Fri, 02 Sep 2022 06:32:28 GMT  
		Size: 67.4 MB (67449113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6935c838d5eb4cd0b713a76063e82036a165b8bc62634dec158e4729749a38`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 262.7 KB (262739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707611d281f0c907bf51272891d4009de29c408cf77e296e33d8b7dc31983b3`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 2.4 KB (2378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a2c9bbb7d25390f08e6efb8200c4a037a6c8bd6980b91e33212c2d3378a6d`  
		Last Modified: Fri, 02 Sep 2022 06:32:21 GMT  
		Size: 20.4 MB (20366833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:6e776f1a869bccaee01cbd2397a6b9c74499f5ffca2e995b5ac6a1b894aefd56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:add9970136f8920882152f611577326f7e23b0ef9a7069b8152de089ee9ac730
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250620496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2208eebb028dc4838ab0afc9b35e3de393855272172cdf1748b12e3c6704fe16`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 04:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:43:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:43:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:43:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:44:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e812731a44ee6ed8eb6f479ee177db4e6f5dc9b8f586e3bec76b68bd87b057`  
		Last Modified: Fri, 02 Sep 2022 05:09:37 GMT  
		Size: 120.1 MB (120084257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ce07703bc6ca66551202ce709d2db142f2284d1758e1ae63b0089816db684`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1890f880d76adc2a15589d899c1971bfe3b8c53a24b095b14ff503208a19d2fc`  
		Last Modified: Fri, 02 Sep 2022 05:09:58 GMT  
		Size: 73.3 MB (73321532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1250a9090832c70a8cbb5b16a1c4fb04bd15cb731dc383b88e5e8920a07637`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 262.8 KB (262804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e10b955d6703772baf23131f34012e192b6651bae2f45d5ec1de94db2d65c9`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 2.4 KB (2425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7586ba8a53515e3a1b9937feaad2e7fede1adbc084ac2d100da1e4a7babb88cf`  
		Last Modified: Fri, 02 Sep 2022 05:09:51 GMT  
		Size: 21.7 MB (21663632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1d667d617e8cf2205c98aec3d4e9667a704e7e1270e6ccceacff672383ee73cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.0 MB (226030547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3f71e64f6f4bbd5dfdb2c020a056ff2446a5c0468227138239c599b8f10b13`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:09:25 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 06:10:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:10:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:10:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:10:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:11:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6669566fcc115df3d85e1176e7e645889db7959d6a954ba485ed11367dc9863a`  
		Last Modified: Fri, 02 Sep 2022 06:32:07 GMT  
		Size: 104.3 MB (104266721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d0c7829bec3aa8e600c8677d001a505e7a97ce46e7e8d34a667fa41b38b06a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5f8d617cb17da8504e284767c00fc2feed07e2f35c7a7b4313b804d53e56b8`  
		Last Modified: Fri, 02 Sep 2022 06:32:28 GMT  
		Size: 67.4 MB (67449113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6935c838d5eb4cd0b713a76063e82036a165b8bc62634dec158e4729749a38`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 262.7 KB (262739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707611d281f0c907bf51272891d4009de29c408cf77e296e33d8b7dc31983b3`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 2.4 KB (2378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a2c9bbb7d25390f08e6efb8200c4a037a6c8bd6980b91e33212c2d3378a6d`  
		Last Modified: Fri, 02 Sep 2022 06:32:21 GMT  
		Size: 20.4 MB (20366833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:e40175e9b9fa3dfcb3b23c44e66c441aed7e825d561b11fb3c55e256bbd77a79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:68cb31a4783276ba8e372670025bc0bff8ef25aa6d267fd3f42f951bbb884a2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155370103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:986192fb90672dc6f66fd52c763b34d9a48034d6ba196e6b7405d9b9d693558f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 04:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:43:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:43:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e812731a44ee6ed8eb6f479ee177db4e6f5dc9b8f586e3bec76b68bd87b057`  
		Last Modified: Fri, 02 Sep 2022 05:09:37 GMT  
		Size: 120.1 MB (120084257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ce07703bc6ca66551202ce709d2db142f2284d1758e1ae63b0089816db684`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7f9005dd7ebcdadf141323e4565fabc2cb83540712209e98ddb71eebefb729c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137949484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45ef402b59da714c63118e97bdf771216fbd936d7092d7468eefe82c5d598ba3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:09:25 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 06:10:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:10:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:10:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6669566fcc115df3d85e1176e7e645889db7959d6a954ba485ed11367dc9863a`  
		Last Modified: Fri, 02 Sep 2022 06:32:07 GMT  
		Size: 104.3 MB (104266721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d0c7829bec3aa8e600c8677d001a505e7a97ce46e7e8d34a667fa41b38b06a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:e40175e9b9fa3dfcb3b23c44e66c441aed7e825d561b11fb3c55e256bbd77a79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:68cb31a4783276ba8e372670025bc0bff8ef25aa6d267fd3f42f951bbb884a2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155370103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:986192fb90672dc6f66fd52c763b34d9a48034d6ba196e6b7405d9b9d693558f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 04:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:43:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:43:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e812731a44ee6ed8eb6f479ee177db4e6f5dc9b8f586e3bec76b68bd87b057`  
		Last Modified: Fri, 02 Sep 2022 05:09:37 GMT  
		Size: 120.1 MB (120084257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ce07703bc6ca66551202ce709d2db142f2284d1758e1ae63b0089816db684`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7f9005dd7ebcdadf141323e4565fabc2cb83540712209e98ddb71eebefb729c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137949484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45ef402b59da714c63118e97bdf771216fbd936d7092d7468eefe82c5d598ba3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:09:25 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 06:10:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:10:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:10:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6669566fcc115df3d85e1176e7e645889db7959d6a954ba485ed11367dc9863a`  
		Last Modified: Fri, 02 Sep 2022 06:32:07 GMT  
		Size: 104.3 MB (104266721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d0c7829bec3aa8e600c8677d001a505e7a97ce46e7e8d34a667fa41b38b06a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:b2604bfd133b7e3dc6b3dd10db191684904699c854f403e04b861d4285f2f6d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:3f78e8a90b6e387d4514aaae5162af4052a93d94d9c4239f3e53d3954232b05a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.6 MB (348586994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2511058a237dd47bcb3f87129403b6fda84704691af09610879963ae37bfb1de`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 04:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:43:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:43:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:43:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:44:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:44:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:44:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:44:17 GMT
ENV ROS1_DISTRO=noetic
# Fri, 02 Sep 2022 04:44:17 GMT
ENV ROS2_DISTRO=foxy
# Fri, 02 Sep 2022 04:44:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:44:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:44:53 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e812731a44ee6ed8eb6f479ee177db4e6f5dc9b8f586e3bec76b68bd87b057`  
		Last Modified: Fri, 02 Sep 2022 05:09:37 GMT  
		Size: 120.1 MB (120084257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ce07703bc6ca66551202ce709d2db142f2284d1758e1ae63b0089816db684`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1890f880d76adc2a15589d899c1971bfe3b8c53a24b095b14ff503208a19d2fc`  
		Last Modified: Fri, 02 Sep 2022 05:09:58 GMT  
		Size: 73.3 MB (73321532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1250a9090832c70a8cbb5b16a1c4fb04bd15cb731dc383b88e5e8920a07637`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 262.8 KB (262804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e10b955d6703772baf23131f34012e192b6651bae2f45d5ec1de94db2d65c9`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 2.4 KB (2425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7586ba8a53515e3a1b9937feaad2e7fede1adbc084ac2d100da1e4a7babb88cf`  
		Last Modified: Fri, 02 Sep 2022 05:09:51 GMT  
		Size: 21.7 MB (21663632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4edcbcf9416ff36cdf21ebba78c090a721c2336ca975593da6eb8673fc001580`  
		Last Modified: Fri, 02 Sep 2022 05:10:15 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99f71dd80fe6b49b3017302c5cccc836ffd1c6cc3eb356f93e988cc3f179b42`  
		Last Modified: Fri, 02 Sep 2022 05:10:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6134584ea0d3a53090e953339399b9b3c8e07b079e17de3d728a076949e813`  
		Last Modified: Fri, 02 Sep 2022 05:10:29 GMT  
		Size: 76.4 MB (76429691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a059b78d35d8a1d65a5ccf510075adf5ea99daa2406f4d49535cefc53a951c2f`  
		Last Modified: Fri, 02 Sep 2022 05:10:19 GMT  
		Size: 21.5 MB (21536176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8666bcd29d3c8ee38ee47d39511a6abd61f7528a39d1298f59510fa77ece2ec6`  
		Last Modified: Fri, 02 Sep 2022 05:10:15 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:93324f0bbf50d7c100828255acace9d27a2f96869f1a518f64b9979a1b3401d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.3 MB (316260468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28974b4228d1ba4a1d1b9c027a3034eae9f83a201f4bcce4594f696c5aed09b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:09:25 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 06:10:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:10:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:10:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:10:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:11:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:11:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:11:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:11:38 GMT
ENV ROS1_DISTRO=noetic
# Fri, 02 Sep 2022 06:11:39 GMT
ENV ROS2_DISTRO=foxy
# Fri, 02 Sep 2022 06:12:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:12:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:12:27 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6669566fcc115df3d85e1176e7e645889db7959d6a954ba485ed11367dc9863a`  
		Last Modified: Fri, 02 Sep 2022 06:32:07 GMT  
		Size: 104.3 MB (104266721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d0c7829bec3aa8e600c8677d001a505e7a97ce46e7e8d34a667fa41b38b06a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5f8d617cb17da8504e284767c00fc2feed07e2f35c7a7b4313b804d53e56b8`  
		Last Modified: Fri, 02 Sep 2022 06:32:28 GMT  
		Size: 67.4 MB (67449113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6935c838d5eb4cd0b713a76063e82036a165b8bc62634dec158e4729749a38`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 262.7 KB (262739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707611d281f0c907bf51272891d4009de29c408cf77e296e33d8b7dc31983b3`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 2.4 KB (2378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a2c9bbb7d25390f08e6efb8200c4a037a6c8bd6980b91e33212c2d3378a6d`  
		Last Modified: Fri, 02 Sep 2022 06:32:21 GMT  
		Size: 20.4 MB (20366833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af4cff9d793717a3b0b2b2160532e7259e9405b855066328b8b9598efd67ee1`  
		Last Modified: Fri, 02 Sep 2022 06:32:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504cdf7ed57b671e8d8daec007271bb91637e5b2096e97548c9477c5d6c136c`  
		Last Modified: Fri, 02 Sep 2022 06:32:57 GMT  
		Size: 76.3 MB (76272363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eb24295f6999a7615200529277faaa909fe8e54299869367a29d93d3dd292b`  
		Last Modified: Fri, 02 Sep 2022 06:32:45 GMT  
		Size: 14.0 MB (13957088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7845311198d12e618960114780dc461e807ac599281d889b1da242ecd02d0575`  
		Last Modified: Fri, 02 Sep 2022 06:32:42 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:b2604bfd133b7e3dc6b3dd10db191684904699c854f403e04b861d4285f2f6d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:3f78e8a90b6e387d4514aaae5162af4052a93d94d9c4239f3e53d3954232b05a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.6 MB (348586994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2511058a237dd47bcb3f87129403b6fda84704691af09610879963ae37bfb1de`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 04:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:43:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:43:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:43:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:44:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:44:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:44:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:44:17 GMT
ENV ROS1_DISTRO=noetic
# Fri, 02 Sep 2022 04:44:17 GMT
ENV ROS2_DISTRO=foxy
# Fri, 02 Sep 2022 04:44:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:44:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:44:53 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e812731a44ee6ed8eb6f479ee177db4e6f5dc9b8f586e3bec76b68bd87b057`  
		Last Modified: Fri, 02 Sep 2022 05:09:37 GMT  
		Size: 120.1 MB (120084257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ce07703bc6ca66551202ce709d2db142f2284d1758e1ae63b0089816db684`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1890f880d76adc2a15589d899c1971bfe3b8c53a24b095b14ff503208a19d2fc`  
		Last Modified: Fri, 02 Sep 2022 05:09:58 GMT  
		Size: 73.3 MB (73321532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1250a9090832c70a8cbb5b16a1c4fb04bd15cb731dc383b88e5e8920a07637`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 262.8 KB (262804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e10b955d6703772baf23131f34012e192b6651bae2f45d5ec1de94db2d65c9`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 2.4 KB (2425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7586ba8a53515e3a1b9937feaad2e7fede1adbc084ac2d100da1e4a7babb88cf`  
		Last Modified: Fri, 02 Sep 2022 05:09:51 GMT  
		Size: 21.7 MB (21663632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4edcbcf9416ff36cdf21ebba78c090a721c2336ca975593da6eb8673fc001580`  
		Last Modified: Fri, 02 Sep 2022 05:10:15 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99f71dd80fe6b49b3017302c5cccc836ffd1c6cc3eb356f93e988cc3f179b42`  
		Last Modified: Fri, 02 Sep 2022 05:10:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6134584ea0d3a53090e953339399b9b3c8e07b079e17de3d728a076949e813`  
		Last Modified: Fri, 02 Sep 2022 05:10:29 GMT  
		Size: 76.4 MB (76429691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a059b78d35d8a1d65a5ccf510075adf5ea99daa2406f4d49535cefc53a951c2f`  
		Last Modified: Fri, 02 Sep 2022 05:10:19 GMT  
		Size: 21.5 MB (21536176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8666bcd29d3c8ee38ee47d39511a6abd61f7528a39d1298f59510fa77ece2ec6`  
		Last Modified: Fri, 02 Sep 2022 05:10:15 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:93324f0bbf50d7c100828255acace9d27a2f96869f1a518f64b9979a1b3401d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.3 MB (316260468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28974b4228d1ba4a1d1b9c027a3034eae9f83a201f4bcce4594f696c5aed09b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:09:25 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 06:10:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:10:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:10:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:10:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:11:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:11:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:11:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:11:38 GMT
ENV ROS1_DISTRO=noetic
# Fri, 02 Sep 2022 06:11:39 GMT
ENV ROS2_DISTRO=foxy
# Fri, 02 Sep 2022 06:12:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:12:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:12:27 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6669566fcc115df3d85e1176e7e645889db7959d6a954ba485ed11367dc9863a`  
		Last Modified: Fri, 02 Sep 2022 06:32:07 GMT  
		Size: 104.3 MB (104266721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d0c7829bec3aa8e600c8677d001a505e7a97ce46e7e8d34a667fa41b38b06a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5f8d617cb17da8504e284767c00fc2feed07e2f35c7a7b4313b804d53e56b8`  
		Last Modified: Fri, 02 Sep 2022 06:32:28 GMT  
		Size: 67.4 MB (67449113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6935c838d5eb4cd0b713a76063e82036a165b8bc62634dec158e4729749a38`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 262.7 KB (262739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707611d281f0c907bf51272891d4009de29c408cf77e296e33d8b7dc31983b3`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 2.4 KB (2378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a2c9bbb7d25390f08e6efb8200c4a037a6c8bd6980b91e33212c2d3378a6d`  
		Last Modified: Fri, 02 Sep 2022 06:32:21 GMT  
		Size: 20.4 MB (20366833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af4cff9d793717a3b0b2b2160532e7259e9405b855066328b8b9598efd67ee1`  
		Last Modified: Fri, 02 Sep 2022 06:32:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504cdf7ed57b671e8d8daec007271bb91637e5b2096e97548c9477c5d6c136c`  
		Last Modified: Fri, 02 Sep 2022 06:32:57 GMT  
		Size: 76.3 MB (76272363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eb24295f6999a7615200529277faaa909fe8e54299869367a29d93d3dd292b`  
		Last Modified: Fri, 02 Sep 2022 06:32:45 GMT  
		Size: 14.0 MB (13957088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7845311198d12e618960114780dc461e807ac599281d889b1da242ecd02d0575`  
		Last Modified: Fri, 02 Sep 2022 06:32:42 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:80b410560d4c6217c5ad0e47135f58931589e010e445c0fbac7b91813153a068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:f672d5cb53360aa4035d84824f862a68a1345e40a5f81682914a6d5165402b30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234856213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c2bcc3f4298470b8a7514532c09dddef7e113b1f5007d4031d4fcc9069cd754`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:44:56 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 04:45:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:45:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:45:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:45:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:46:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:46:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:46:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:46:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4606a5228ccb52337657838c69716d528a1cd36a6adb320134ad9f72dac1b0`  
		Last Modified: Fri, 02 Sep 2022 05:10:57 GMT  
		Size: 103.9 MB (103882165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1077970b7ff447bda164171d709fbff427233431a1b4e67f2c042babb86581d`  
		Last Modified: Fri, 02 Sep 2022 05:10:40 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1623dc240f1486b24057900a44b1773cb529bb6eb79de2586e3d68e4612aca5d`  
		Last Modified: Fri, 02 Sep 2022 05:11:17 GMT  
		Size: 73.3 MB (73278501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c19349a79634056717413469829a12bf9869bc820130019d21c041134468f6a`  
		Last Modified: Fri, 02 Sep 2022 05:11:07 GMT  
		Size: 273.4 KB (273436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d38666d25b1c976245f649412489ae8d72bdaf049159320f9d06e29d9c12ab`  
		Last Modified: Fri, 02 Sep 2022 05:11:07 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5b062abae098c506dc5944c0c2dd15738658bdca2359cff971286f3a21ac3`  
		Last Modified: Fri, 02 Sep 2022 05:11:10 GMT  
		Size: 22.1 MB (22133844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a7f6bb5a877a5ba0f25f271f0079ae570c68ff7e9a44d02468c9666ce66bce1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.1 MB (223120494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eeb6d456ca2d70acf0155a743233e88ab8edb362c32681de00b3259d83398dc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:12:34 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 06:13:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:13:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:13:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:13:29 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:14:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8748d4d2e380f35f3f861300c963969ef7260eefceff507f1e50bd06ccef5d1b`  
		Last Modified: Fri, 02 Sep 2022 06:33:25 GMT  
		Size: 100.3 MB (100301804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363bb25086532984cf99e912aec1161a7245b35ec1b5fb036806f4dda79295d`  
		Last Modified: Fri, 02 Sep 2022 06:33:08 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12cf99d1383ed912dd7b18ef3a19fe93c9860a073e8a76527236b6b5894e88e`  
		Last Modified: Fri, 02 Sep 2022 06:33:46 GMT  
		Size: 67.4 MB (67403683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24ce2aa32cbce42f9f12184c4d915b4ac1e8e4b438de6156c4a10f7459ab6f8`  
		Last Modified: Fri, 02 Sep 2022 06:33:36 GMT  
		Size: 273.4 KB (273386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a772003c0836f539f5bf55a49c1fa9f11468cfbd78ba3f7a73a46e3d8e570a74`  
		Last Modified: Fri, 02 Sep 2022 06:33:36 GMT  
		Size: 2.4 KB (2357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f386332a78442333412b533715e9e70bd4a86218c8e1d521a624f8de5850dc65`  
		Last Modified: Fri, 02 Sep 2022 06:33:39 GMT  
		Size: 21.5 MB (21456501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:80b410560d4c6217c5ad0e47135f58931589e010e445c0fbac7b91813153a068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:f672d5cb53360aa4035d84824f862a68a1345e40a5f81682914a6d5165402b30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234856213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c2bcc3f4298470b8a7514532c09dddef7e113b1f5007d4031d4fcc9069cd754`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:44:56 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 04:45:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:45:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:45:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:45:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:46:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:46:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:46:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:46:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4606a5228ccb52337657838c69716d528a1cd36a6adb320134ad9f72dac1b0`  
		Last Modified: Fri, 02 Sep 2022 05:10:57 GMT  
		Size: 103.9 MB (103882165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1077970b7ff447bda164171d709fbff427233431a1b4e67f2c042babb86581d`  
		Last Modified: Fri, 02 Sep 2022 05:10:40 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1623dc240f1486b24057900a44b1773cb529bb6eb79de2586e3d68e4612aca5d`  
		Last Modified: Fri, 02 Sep 2022 05:11:17 GMT  
		Size: 73.3 MB (73278501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c19349a79634056717413469829a12bf9869bc820130019d21c041134468f6a`  
		Last Modified: Fri, 02 Sep 2022 05:11:07 GMT  
		Size: 273.4 KB (273436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d38666d25b1c976245f649412489ae8d72bdaf049159320f9d06e29d9c12ab`  
		Last Modified: Fri, 02 Sep 2022 05:11:07 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5b062abae098c506dc5944c0c2dd15738658bdca2359cff971286f3a21ac3`  
		Last Modified: Fri, 02 Sep 2022 05:11:10 GMT  
		Size: 22.1 MB (22133844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a7f6bb5a877a5ba0f25f271f0079ae570c68ff7e9a44d02468c9666ce66bce1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.1 MB (223120494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eeb6d456ca2d70acf0155a743233e88ab8edb362c32681de00b3259d83398dc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:12:34 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 06:13:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:13:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:13:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:13:29 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:14:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8748d4d2e380f35f3f861300c963969ef7260eefceff507f1e50bd06ccef5d1b`  
		Last Modified: Fri, 02 Sep 2022 06:33:25 GMT  
		Size: 100.3 MB (100301804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363bb25086532984cf99e912aec1161a7245b35ec1b5fb036806f4dda79295d`  
		Last Modified: Fri, 02 Sep 2022 06:33:08 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12cf99d1383ed912dd7b18ef3a19fe93c9860a073e8a76527236b6b5894e88e`  
		Last Modified: Fri, 02 Sep 2022 06:33:46 GMT  
		Size: 67.4 MB (67403683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24ce2aa32cbce42f9f12184c4d915b4ac1e8e4b438de6156c4a10f7459ab6f8`  
		Last Modified: Fri, 02 Sep 2022 06:33:36 GMT  
		Size: 273.4 KB (273386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a772003c0836f539f5bf55a49c1fa9f11468cfbd78ba3f7a73a46e3d8e570a74`  
		Last Modified: Fri, 02 Sep 2022 06:33:36 GMT  
		Size: 2.4 KB (2357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f386332a78442333412b533715e9e70bd4a86218c8e1d521a624f8de5850dc65`  
		Last Modified: Fri, 02 Sep 2022 06:33:39 GMT  
		Size: 21.5 MB (21456501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:80b410560d4c6217c5ad0e47135f58931589e010e445c0fbac7b91813153a068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:f672d5cb53360aa4035d84824f862a68a1345e40a5f81682914a6d5165402b30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234856213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c2bcc3f4298470b8a7514532c09dddef7e113b1f5007d4031d4fcc9069cd754`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:44:56 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 04:45:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:45:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:45:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:45:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:46:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:46:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:46:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:46:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4606a5228ccb52337657838c69716d528a1cd36a6adb320134ad9f72dac1b0`  
		Last Modified: Fri, 02 Sep 2022 05:10:57 GMT  
		Size: 103.9 MB (103882165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1077970b7ff447bda164171d709fbff427233431a1b4e67f2c042babb86581d`  
		Last Modified: Fri, 02 Sep 2022 05:10:40 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1623dc240f1486b24057900a44b1773cb529bb6eb79de2586e3d68e4612aca5d`  
		Last Modified: Fri, 02 Sep 2022 05:11:17 GMT  
		Size: 73.3 MB (73278501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c19349a79634056717413469829a12bf9869bc820130019d21c041134468f6a`  
		Last Modified: Fri, 02 Sep 2022 05:11:07 GMT  
		Size: 273.4 KB (273436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d38666d25b1c976245f649412489ae8d72bdaf049159320f9d06e29d9c12ab`  
		Last Modified: Fri, 02 Sep 2022 05:11:07 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5b062abae098c506dc5944c0c2dd15738658bdca2359cff971286f3a21ac3`  
		Last Modified: Fri, 02 Sep 2022 05:11:10 GMT  
		Size: 22.1 MB (22133844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a7f6bb5a877a5ba0f25f271f0079ae570c68ff7e9a44d02468c9666ce66bce1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.1 MB (223120494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eeb6d456ca2d70acf0155a743233e88ab8edb362c32681de00b3259d83398dc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:12:34 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 06:13:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:13:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:13:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:13:29 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:14:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8748d4d2e380f35f3f861300c963969ef7260eefceff507f1e50bd06ccef5d1b`  
		Last Modified: Fri, 02 Sep 2022 06:33:25 GMT  
		Size: 100.3 MB (100301804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363bb25086532984cf99e912aec1161a7245b35ec1b5fb036806f4dda79295d`  
		Last Modified: Fri, 02 Sep 2022 06:33:08 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12cf99d1383ed912dd7b18ef3a19fe93c9860a073e8a76527236b6b5894e88e`  
		Last Modified: Fri, 02 Sep 2022 06:33:46 GMT  
		Size: 67.4 MB (67403683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24ce2aa32cbce42f9f12184c4d915b4ac1e8e4b438de6156c4a10f7459ab6f8`  
		Last Modified: Fri, 02 Sep 2022 06:33:36 GMT  
		Size: 273.4 KB (273386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a772003c0836f539f5bf55a49c1fa9f11468cfbd78ba3f7a73a46e3d8e570a74`  
		Last Modified: Fri, 02 Sep 2022 06:33:36 GMT  
		Size: 2.4 KB (2357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f386332a78442333412b533715e9e70bd4a86218c8e1d521a624f8de5850dc65`  
		Last Modified: Fri, 02 Sep 2022 06:33:39 GMT  
		Size: 21.5 MB (21456501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:af75a6165fc1a7948e08a1311898961c09f1d7ff0d395ff034b6dce4051f0f88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:103d58131043fe218f9fb1aeb8c1110d81005458d71000f117bb7219f62fad6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.2 MB (139168012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91dbd16d87b5a79f30e898cd6e666e9491ca7ee7a46ac3a074a0f236c4b8c699`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:44:56 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 04:45:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:45:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:45:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:45:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4606a5228ccb52337657838c69716d528a1cd36a6adb320134ad9f72dac1b0`  
		Last Modified: Fri, 02 Sep 2022 05:10:57 GMT  
		Size: 103.9 MB (103882165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1077970b7ff447bda164171d709fbff427233431a1b4e67f2c042babb86581d`  
		Last Modified: Fri, 02 Sep 2022 05:10:40 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:838ab80e8d98df58a43974406f0f74ec79da08fcc53298b5dbd131bbf927e579
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (133984567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b6f2a9ce53de5cdc09b0af75f38391698c3568fb15f5fd9fcd27916a4684cd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:12:34 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 06:13:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:13:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:13:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:13:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8748d4d2e380f35f3f861300c963969ef7260eefceff507f1e50bd06ccef5d1b`  
		Last Modified: Fri, 02 Sep 2022 06:33:25 GMT  
		Size: 100.3 MB (100301804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363bb25086532984cf99e912aec1161a7245b35ec1b5fb036806f4dda79295d`  
		Last Modified: Fri, 02 Sep 2022 06:33:08 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:af75a6165fc1a7948e08a1311898961c09f1d7ff0d395ff034b6dce4051f0f88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:103d58131043fe218f9fb1aeb8c1110d81005458d71000f117bb7219f62fad6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.2 MB (139168012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91dbd16d87b5a79f30e898cd6e666e9491ca7ee7a46ac3a074a0f236c4b8c699`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:44:56 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 04:45:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:45:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:45:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:45:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4606a5228ccb52337657838c69716d528a1cd36a6adb320134ad9f72dac1b0`  
		Last Modified: Fri, 02 Sep 2022 05:10:57 GMT  
		Size: 103.9 MB (103882165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1077970b7ff447bda164171d709fbff427233431a1b4e67f2c042babb86581d`  
		Last Modified: Fri, 02 Sep 2022 05:10:40 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:838ab80e8d98df58a43974406f0f74ec79da08fcc53298b5dbd131bbf927e579
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (133984567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b6f2a9ce53de5cdc09b0af75f38391698c3568fb15f5fd9fcd27916a4684cd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:12:34 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 06:13:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:13:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:13:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:13:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8748d4d2e380f35f3f861300c963969ef7260eefceff507f1e50bd06ccef5d1b`  
		Last Modified: Fri, 02 Sep 2022 06:33:25 GMT  
		Size: 100.3 MB (100301804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363bb25086532984cf99e912aec1161a7245b35ec1b5fb036806f4dda79295d`  
		Last Modified: Fri, 02 Sep 2022 06:33:08 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:22ee99dc880227995936dbb6da9a14e848c742830f2bf85cb057ed464390d364
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:6f868677049d21360ab3c77c7117cf3432bb0a45d625645fbbd4bad00010ddd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.0 MB (330025494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a9b3283ccd5b50b76c43a25043d7b2fe3b0b97cad79b7e7a209c764f66f454`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:44:56 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 04:45:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:45:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:45:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:45:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:46:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:46:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:46:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:46:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:46:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:46:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:46:34 GMT
ENV ROS1_DISTRO=noetic
# Fri, 02 Sep 2022 04:46:35 GMT
ENV ROS2_DISTRO=galactic
# Fri, 02 Sep 2022 04:47:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:11 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4606a5228ccb52337657838c69716d528a1cd36a6adb320134ad9f72dac1b0`  
		Last Modified: Fri, 02 Sep 2022 05:10:57 GMT  
		Size: 103.9 MB (103882165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1077970b7ff447bda164171d709fbff427233431a1b4e67f2c042babb86581d`  
		Last Modified: Fri, 02 Sep 2022 05:10:40 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1623dc240f1486b24057900a44b1773cb529bb6eb79de2586e3d68e4612aca5d`  
		Last Modified: Fri, 02 Sep 2022 05:11:17 GMT  
		Size: 73.3 MB (73278501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c19349a79634056717413469829a12bf9869bc820130019d21c041134468f6a`  
		Last Modified: Fri, 02 Sep 2022 05:11:07 GMT  
		Size: 273.4 KB (273436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d38666d25b1c976245f649412489ae8d72bdaf049159320f9d06e29d9c12ab`  
		Last Modified: Fri, 02 Sep 2022 05:11:07 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5b062abae098c506dc5944c0c2dd15738658bdca2359cff971286f3a21ac3`  
		Last Modified: Fri, 02 Sep 2022 05:11:10 GMT  
		Size: 22.1 MB (22133844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7042ec89f6d891cd95e94cd61209c7e05dec6bd0e5b8cea8f7de6e185eb2ba`  
		Last Modified: Fri, 02 Sep 2022 05:11:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59e95c9ba69710b05bbe0a10f7f318f27145d50937efd6e935208ddd6c651e0`  
		Last Modified: Fri, 02 Sep 2022 05:11:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91760914880a09803690d5d594d1b8e2bbe9dccf90c45668e5ce3e5519fe434c`  
		Last Modified: Fri, 02 Sep 2022 05:11:44 GMT  
		Size: 78.7 MB (78704188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c0409b4aafa794ecb20b46c1cd8f1de9548ba0dbbceb823a6c697f943457ea`  
		Last Modified: Fri, 02 Sep 2022 05:11:33 GMT  
		Size: 16.5 MB (16464464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ef861301145847f95ebf92976fe0df9dd8b6488b5c0d2ecd116013da505730`  
		Last Modified: Fri, 02 Sep 2022 05:11:30 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b03b0585dae277c423431638c72c5a7ea90380933359105488449689f9b57462
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317333746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d611b627755504b47760f810f7b8b6759576f445cd4984bd1b67c8cd68f35d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:12:34 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 06:13:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:13:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:13:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:13:29 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:14:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:14:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:14:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:14:41 GMT
ENV ROS1_DISTRO=noetic
# Fri, 02 Sep 2022 06:14:42 GMT
ENV ROS2_DISTRO=galactic
# Fri, 02 Sep 2022 06:15:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:31 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8748d4d2e380f35f3f861300c963969ef7260eefceff507f1e50bd06ccef5d1b`  
		Last Modified: Fri, 02 Sep 2022 06:33:25 GMT  
		Size: 100.3 MB (100301804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363bb25086532984cf99e912aec1161a7245b35ec1b5fb036806f4dda79295d`  
		Last Modified: Fri, 02 Sep 2022 06:33:08 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12cf99d1383ed912dd7b18ef3a19fe93c9860a073e8a76527236b6b5894e88e`  
		Last Modified: Fri, 02 Sep 2022 06:33:46 GMT  
		Size: 67.4 MB (67403683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24ce2aa32cbce42f9f12184c4d915b4ac1e8e4b438de6156c4a10f7459ab6f8`  
		Last Modified: Fri, 02 Sep 2022 06:33:36 GMT  
		Size: 273.4 KB (273386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a772003c0836f539f5bf55a49c1fa9f11468cfbd78ba3f7a73a46e3d8e570a74`  
		Last Modified: Fri, 02 Sep 2022 06:33:36 GMT  
		Size: 2.4 KB (2357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f386332a78442333412b533715e9e70bd4a86218c8e1d521a624f8de5850dc65`  
		Last Modified: Fri, 02 Sep 2022 06:33:39 GMT  
		Size: 21.5 MB (21456501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35b4d97dd3d85e0d54e092c4c5c94b14e60ea7e0384b3371b0976aed94ffd99`  
		Last Modified: Fri, 02 Sep 2022 06:34:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f31c095457557e622e75253fcc2655666122138e7438b9b6fefd1a1ceb9df2`  
		Last Modified: Fri, 02 Sep 2022 06:34:15 GMT  
		Size: 78.5 MB (78450553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b619a2e8c20b525fc9ad7204ea04c498200493661903ee9ae8a582b328d2be`  
		Last Modified: Fri, 02 Sep 2022 06:34:04 GMT  
		Size: 15.8 MB (15762227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028e36679f7c95f83c78b2f893fdaa8d82374dee0789ce9a3ae1d4ade3572f5b`  
		Last Modified: Fri, 02 Sep 2022 06:34:01 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:22ee99dc880227995936dbb6da9a14e848c742830f2bf85cb057ed464390d364
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:6f868677049d21360ab3c77c7117cf3432bb0a45d625645fbbd4bad00010ddd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.0 MB (330025494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a9b3283ccd5b50b76c43a25043d7b2fe3b0b97cad79b7e7a209c764f66f454`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:44:56 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 04:45:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:45:40 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:45:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:45:40 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:46:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:46:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:46:09 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:46:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:46:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:46:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:46:34 GMT
ENV ROS1_DISTRO=noetic
# Fri, 02 Sep 2022 04:46:35 GMT
ENV ROS2_DISTRO=galactic
# Fri, 02 Sep 2022 04:47:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:11 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4606a5228ccb52337657838c69716d528a1cd36a6adb320134ad9f72dac1b0`  
		Last Modified: Fri, 02 Sep 2022 05:10:57 GMT  
		Size: 103.9 MB (103882165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1077970b7ff447bda164171d709fbff427233431a1b4e67f2c042babb86581d`  
		Last Modified: Fri, 02 Sep 2022 05:10:40 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1623dc240f1486b24057900a44b1773cb529bb6eb79de2586e3d68e4612aca5d`  
		Last Modified: Fri, 02 Sep 2022 05:11:17 GMT  
		Size: 73.3 MB (73278501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c19349a79634056717413469829a12bf9869bc820130019d21c041134468f6a`  
		Last Modified: Fri, 02 Sep 2022 05:11:07 GMT  
		Size: 273.4 KB (273436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d38666d25b1c976245f649412489ae8d72bdaf049159320f9d06e29d9c12ab`  
		Last Modified: Fri, 02 Sep 2022 05:11:07 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5b062abae098c506dc5944c0c2dd15738658bdca2359cff971286f3a21ac3`  
		Last Modified: Fri, 02 Sep 2022 05:11:10 GMT  
		Size: 22.1 MB (22133844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7042ec89f6d891cd95e94cd61209c7e05dec6bd0e5b8cea8f7de6e185eb2ba`  
		Last Modified: Fri, 02 Sep 2022 05:11:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59e95c9ba69710b05bbe0a10f7f318f27145d50937efd6e935208ddd6c651e0`  
		Last Modified: Fri, 02 Sep 2022 05:11:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91760914880a09803690d5d594d1b8e2bbe9dccf90c45668e5ce3e5519fe434c`  
		Last Modified: Fri, 02 Sep 2022 05:11:44 GMT  
		Size: 78.7 MB (78704188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c0409b4aafa794ecb20b46c1cd8f1de9548ba0dbbceb823a6c697f943457ea`  
		Last Modified: Fri, 02 Sep 2022 05:11:33 GMT  
		Size: 16.5 MB (16464464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ef861301145847f95ebf92976fe0df9dd8b6488b5c0d2ecd116013da505730`  
		Last Modified: Fri, 02 Sep 2022 05:11:30 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b03b0585dae277c423431638c72c5a7ea90380933359105488449689f9b57462
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317333746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d611b627755504b47760f810f7b8b6759576f445cd4984bd1b67c8cd68f35d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:12:34 GMT
ENV ROS_DISTRO=galactic
# Fri, 02 Sep 2022 06:13:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:13:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:13:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:13:29 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:14:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:14:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:14:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:14:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:14:41 GMT
ENV ROS1_DISTRO=noetic
# Fri, 02 Sep 2022 06:14:42 GMT
ENV ROS2_DISTRO=galactic
# Fri, 02 Sep 2022 06:15:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:31 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8748d4d2e380f35f3f861300c963969ef7260eefceff507f1e50bd06ccef5d1b`  
		Last Modified: Fri, 02 Sep 2022 06:33:25 GMT  
		Size: 100.3 MB (100301804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363bb25086532984cf99e912aec1161a7245b35ec1b5fb036806f4dda79295d`  
		Last Modified: Fri, 02 Sep 2022 06:33:08 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12cf99d1383ed912dd7b18ef3a19fe93c9860a073e8a76527236b6b5894e88e`  
		Last Modified: Fri, 02 Sep 2022 06:33:46 GMT  
		Size: 67.4 MB (67403683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24ce2aa32cbce42f9f12184c4d915b4ac1e8e4b438de6156c4a10f7459ab6f8`  
		Last Modified: Fri, 02 Sep 2022 06:33:36 GMT  
		Size: 273.4 KB (273386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a772003c0836f539f5bf55a49c1fa9f11468cfbd78ba3f7a73a46e3d8e570a74`  
		Last Modified: Fri, 02 Sep 2022 06:33:36 GMT  
		Size: 2.4 KB (2357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f386332a78442333412b533715e9e70bd4a86218c8e1d521a624f8de5850dc65`  
		Last Modified: Fri, 02 Sep 2022 06:33:39 GMT  
		Size: 21.5 MB (21456501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35b4d97dd3d85e0d54e092c4c5c94b14e60ea7e0384b3371b0976aed94ffd99`  
		Last Modified: Fri, 02 Sep 2022 06:34:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f31c095457557e622e75253fcc2655666122138e7438b9b6fefd1a1ceb9df2`  
		Last Modified: Fri, 02 Sep 2022 06:34:15 GMT  
		Size: 78.5 MB (78450553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b619a2e8c20b525fc9ad7204ea04c498200493661903ee9ae8a582b328d2be`  
		Last Modified: Fri, 02 Sep 2022 06:34:04 GMT  
		Size: 15.8 MB (15762227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028e36679f7c95f83c78b2f893fdaa8d82374dee0789ce9a3ae1d4ade3572f5b`  
		Last Modified: Fri, 02 Sep 2022 06:34:01 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble`

```console
$ docker pull ros@sha256:2957f3c0f64a2887b5f8e81d3aef38e99963dbe3a9b50e1ad1846fb422b45b8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:b5afc3c15a18c85bd4472228addb045cfa1be4955efd4f7d1f5bc2bd1ea938a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262767288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0afc637f4748749ba7294a29cff472a9aff855e9b3f1c1a4641daf1c47f61306`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 04:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:49:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:49:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:49:26 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:50:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:50:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:50:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:51:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f3dbe0ec1046bb9bdd0276165d66b03aafb64279b2077b7fbdac5b1047b98e`  
		Last Modified: Fri, 02 Sep 2022 05:12:12 GMT  
		Size: 106.2 MB (106189810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ef6ac4127ac4c6d2c35e9befe4af09debd87c5e55110651f46e88a35c631`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47e8a6f8a449077cfb0901a9b21c22e899338a0bc99ca9be0951bf6b3256c1a`  
		Last Modified: Fri, 02 Sep 2022 05:12:36 GMT  
		Size: 97.8 MB (97849527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40faf29acfa4fc6c1747729238c7b69b3c05983e5f81a16389a75b6b7fad4ed7`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 285.6 KB (285574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df57c7f1a275a97de9412ce0ca9182e86900074cda4ea3b82bb20d7a3c374a0c`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3101d89bfa03579ba584f494cd916ad9cd928e61dec78734db0bf203c0ae68`  
		Last Modified: Fri, 02 Sep 2022 05:12:26 GMT  
		Size: 23.0 MB (23007608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:41a4bf37d3bafe29278c7df4d27d9632379e135f6cdb0adaca4a9b27129e52ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (255011616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40cf39c2d4982fb75e99085a66a9adac5a4689114fa27e86bfa647dca3b08fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:16:00 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 06:16:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:16:49 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:16:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:16:51 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:17:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:17:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:17:39 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:17:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0976d669787f3fcd6abd2508a3d2424decead22cd66d405b4da7e9c988499a6a`  
		Last Modified: Fri, 02 Sep 2022 06:34:43 GMT  
		Size: 103.9 MB (103924320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf3fa151f78e7974d35e7b47f6903b56457dff01611cabf07d24d4ad288b33f`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04ff1eccf75d5a0a9ed12a8822d1ecf37c92116c7e660f92c8a125f4b5b869b`  
		Last Modified: Fri, 02 Sep 2022 06:35:07 GMT  
		Size: 95.2 MB (95214806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d93b09dedad3c115236fd0ec61587b6872929fddf38f3c50298742c5e54a9c`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 285.5 KB (285519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa0bcbf474ccec4a8b2b8e6782135e6a9ee15328201b05e761764988c680c41`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 2.4 KB (2363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862c83aa445983369fee4e683ab2e4f96cd4c4855ec8f187c71c40aa65661a74`  
		Last Modified: Fri, 02 Sep 2022 06:34:57 GMT  
		Size: 22.4 MB (22428152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:fc462abebf7623ae860ed76ce79cd0b4d87fc397256733bfe77e7eeb6beb4b61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:1f7150af030fb952e645d29f203b3fcded126ff0a6266e3d555bf84f40a99d0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1084481041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:339e4abc3190c0e39084941988ade2c960baa9c0960645bab9326c3b9c7a40f0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 04:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:49:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:49:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:49:26 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:50:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:50:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:50:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:51:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:59:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f3dbe0ec1046bb9bdd0276165d66b03aafb64279b2077b7fbdac5b1047b98e`  
		Last Modified: Fri, 02 Sep 2022 05:12:12 GMT  
		Size: 106.2 MB (106189810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ef6ac4127ac4c6d2c35e9befe4af09debd87c5e55110651f46e88a35c631`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47e8a6f8a449077cfb0901a9b21c22e899338a0bc99ca9be0951bf6b3256c1a`  
		Last Modified: Fri, 02 Sep 2022 05:12:36 GMT  
		Size: 97.8 MB (97849527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40faf29acfa4fc6c1747729238c7b69b3c05983e5f81a16389a75b6b7fad4ed7`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 285.6 KB (285574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df57c7f1a275a97de9412ce0ca9182e86900074cda4ea3b82bb20d7a3c374a0c`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3101d89bfa03579ba584f494cd916ad9cd928e61dec78734db0bf203c0ae68`  
		Last Modified: Fri, 02 Sep 2022 05:12:26 GMT  
		Size: 23.0 MB (23007608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b8f4b49d484fdb89a848443988e3313cabbc0d97d79fb1f0486bea4a9d3e0`  
		Last Modified: Fri, 02 Sep 2022 05:14:29 GMT  
		Size: 821.7 MB (821713753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3572e737aa2da23c08602b4ce98c5d720c7af10851d9bd0b39bf487b4089187c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1034489364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4d00c6b3d7b6a26c3255ca9d4338a58f29eeb94001c8fe46f5b099d60dbc99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:16:00 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 06:16:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:16:49 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:16:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:16:51 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:17:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:17:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:17:39 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:17:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:20:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0976d669787f3fcd6abd2508a3d2424decead22cd66d405b4da7e9c988499a6a`  
		Last Modified: Fri, 02 Sep 2022 06:34:43 GMT  
		Size: 103.9 MB (103924320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf3fa151f78e7974d35e7b47f6903b56457dff01611cabf07d24d4ad288b33f`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04ff1eccf75d5a0a9ed12a8822d1ecf37c92116c7e660f92c8a125f4b5b869b`  
		Last Modified: Fri, 02 Sep 2022 06:35:07 GMT  
		Size: 95.2 MB (95214806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d93b09dedad3c115236fd0ec61587b6872929fddf38f3c50298742c5e54a9c`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 285.5 KB (285519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa0bcbf474ccec4a8b2b8e6782135e6a9ee15328201b05e761764988c680c41`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 2.4 KB (2363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862c83aa445983369fee4e683ab2e4f96cd4c4855ec8f187c71c40aa65661a74`  
		Last Modified: Fri, 02 Sep 2022 06:34:57 GMT  
		Size: 22.4 MB (22428152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8f1eed52c64364a3769b39c14cac8996c20a510429ccf137f2f591ef7d1f9c`  
		Last Modified: Fri, 02 Sep 2022 06:36:59 GMT  
		Size: 779.5 MB (779477748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:fc462abebf7623ae860ed76ce79cd0b4d87fc397256733bfe77e7eeb6beb4b61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:1f7150af030fb952e645d29f203b3fcded126ff0a6266e3d555bf84f40a99d0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1084481041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:339e4abc3190c0e39084941988ade2c960baa9c0960645bab9326c3b9c7a40f0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 04:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:49:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:49:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:49:26 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:50:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:50:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:50:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:51:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:59:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f3dbe0ec1046bb9bdd0276165d66b03aafb64279b2077b7fbdac5b1047b98e`  
		Last Modified: Fri, 02 Sep 2022 05:12:12 GMT  
		Size: 106.2 MB (106189810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ef6ac4127ac4c6d2c35e9befe4af09debd87c5e55110651f46e88a35c631`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47e8a6f8a449077cfb0901a9b21c22e899338a0bc99ca9be0951bf6b3256c1a`  
		Last Modified: Fri, 02 Sep 2022 05:12:36 GMT  
		Size: 97.8 MB (97849527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40faf29acfa4fc6c1747729238c7b69b3c05983e5f81a16389a75b6b7fad4ed7`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 285.6 KB (285574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df57c7f1a275a97de9412ce0ca9182e86900074cda4ea3b82bb20d7a3c374a0c`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3101d89bfa03579ba584f494cd916ad9cd928e61dec78734db0bf203c0ae68`  
		Last Modified: Fri, 02 Sep 2022 05:12:26 GMT  
		Size: 23.0 MB (23007608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b8f4b49d484fdb89a848443988e3313cabbc0d97d79fb1f0486bea4a9d3e0`  
		Last Modified: Fri, 02 Sep 2022 05:14:29 GMT  
		Size: 821.7 MB (821713753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3572e737aa2da23c08602b4ce98c5d720c7af10851d9bd0b39bf487b4089187c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1034489364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4d00c6b3d7b6a26c3255ca9d4338a58f29eeb94001c8fe46f5b099d60dbc99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:16:00 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 06:16:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:16:49 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:16:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:16:51 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:17:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:17:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:17:39 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:17:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:20:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0976d669787f3fcd6abd2508a3d2424decead22cd66d405b4da7e9c988499a6a`  
		Last Modified: Fri, 02 Sep 2022 06:34:43 GMT  
		Size: 103.9 MB (103924320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf3fa151f78e7974d35e7b47f6903b56457dff01611cabf07d24d4ad288b33f`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04ff1eccf75d5a0a9ed12a8822d1ecf37c92116c7e660f92c8a125f4b5b869b`  
		Last Modified: Fri, 02 Sep 2022 06:35:07 GMT  
		Size: 95.2 MB (95214806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d93b09dedad3c115236fd0ec61587b6872929fddf38f3c50298742c5e54a9c`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 285.5 KB (285519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa0bcbf474ccec4a8b2b8e6782135e6a9ee15328201b05e761764988c680c41`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 2.4 KB (2363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862c83aa445983369fee4e683ab2e4f96cd4c4855ec8f187c71c40aa65661a74`  
		Last Modified: Fri, 02 Sep 2022 06:34:57 GMT  
		Size: 22.4 MB (22428152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8f1eed52c64364a3769b39c14cac8996c20a510429ccf137f2f591ef7d1f9c`  
		Last Modified: Fri, 02 Sep 2022 06:36:59 GMT  
		Size: 779.5 MB (779477748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:2957f3c0f64a2887b5f8e81d3aef38e99963dbe3a9b50e1ad1846fb422b45b8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:b5afc3c15a18c85bd4472228addb045cfa1be4955efd4f7d1f5bc2bd1ea938a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262767288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0afc637f4748749ba7294a29cff472a9aff855e9b3f1c1a4641daf1c47f61306`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 04:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:49:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:49:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:49:26 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:50:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:50:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:50:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:51:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f3dbe0ec1046bb9bdd0276165d66b03aafb64279b2077b7fbdac5b1047b98e`  
		Last Modified: Fri, 02 Sep 2022 05:12:12 GMT  
		Size: 106.2 MB (106189810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ef6ac4127ac4c6d2c35e9befe4af09debd87c5e55110651f46e88a35c631`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47e8a6f8a449077cfb0901a9b21c22e899338a0bc99ca9be0951bf6b3256c1a`  
		Last Modified: Fri, 02 Sep 2022 05:12:36 GMT  
		Size: 97.8 MB (97849527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40faf29acfa4fc6c1747729238c7b69b3c05983e5f81a16389a75b6b7fad4ed7`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 285.6 KB (285574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df57c7f1a275a97de9412ce0ca9182e86900074cda4ea3b82bb20d7a3c374a0c`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3101d89bfa03579ba584f494cd916ad9cd928e61dec78734db0bf203c0ae68`  
		Last Modified: Fri, 02 Sep 2022 05:12:26 GMT  
		Size: 23.0 MB (23007608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:41a4bf37d3bafe29278c7df4d27d9632379e135f6cdb0adaca4a9b27129e52ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (255011616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40cf39c2d4982fb75e99085a66a9adac5a4689114fa27e86bfa647dca3b08fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:16:00 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 06:16:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:16:49 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:16:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:16:51 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:17:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:17:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:17:39 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:17:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0976d669787f3fcd6abd2508a3d2424decead22cd66d405b4da7e9c988499a6a`  
		Last Modified: Fri, 02 Sep 2022 06:34:43 GMT  
		Size: 103.9 MB (103924320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf3fa151f78e7974d35e7b47f6903b56457dff01611cabf07d24d4ad288b33f`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04ff1eccf75d5a0a9ed12a8822d1ecf37c92116c7e660f92c8a125f4b5b869b`  
		Last Modified: Fri, 02 Sep 2022 06:35:07 GMT  
		Size: 95.2 MB (95214806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d93b09dedad3c115236fd0ec61587b6872929fddf38f3c50298742c5e54a9c`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 285.5 KB (285519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa0bcbf474ccec4a8b2b8e6782135e6a9ee15328201b05e761764988c680c41`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 2.4 KB (2363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862c83aa445983369fee4e683ab2e4f96cd4c4855ec8f187c71c40aa65661a74`  
		Last Modified: Fri, 02 Sep 2022 06:34:57 GMT  
		Size: 22.4 MB (22428152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:2957f3c0f64a2887b5f8e81d3aef38e99963dbe3a9b50e1ad1846fb422b45b8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:b5afc3c15a18c85bd4472228addb045cfa1be4955efd4f7d1f5bc2bd1ea938a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262767288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0afc637f4748749ba7294a29cff472a9aff855e9b3f1c1a4641daf1c47f61306`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 04:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:49:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:49:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:49:26 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:50:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:50:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:50:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:51:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f3dbe0ec1046bb9bdd0276165d66b03aafb64279b2077b7fbdac5b1047b98e`  
		Last Modified: Fri, 02 Sep 2022 05:12:12 GMT  
		Size: 106.2 MB (106189810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ef6ac4127ac4c6d2c35e9befe4af09debd87c5e55110651f46e88a35c631`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47e8a6f8a449077cfb0901a9b21c22e899338a0bc99ca9be0951bf6b3256c1a`  
		Last Modified: Fri, 02 Sep 2022 05:12:36 GMT  
		Size: 97.8 MB (97849527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40faf29acfa4fc6c1747729238c7b69b3c05983e5f81a16389a75b6b7fad4ed7`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 285.6 KB (285574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df57c7f1a275a97de9412ce0ca9182e86900074cda4ea3b82bb20d7a3c374a0c`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3101d89bfa03579ba584f494cd916ad9cd928e61dec78734db0bf203c0ae68`  
		Last Modified: Fri, 02 Sep 2022 05:12:26 GMT  
		Size: 23.0 MB (23007608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:41a4bf37d3bafe29278c7df4d27d9632379e135f6cdb0adaca4a9b27129e52ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (255011616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40cf39c2d4982fb75e99085a66a9adac5a4689114fa27e86bfa647dca3b08fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:16:00 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 06:16:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:16:49 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:16:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:16:51 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:17:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:17:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:17:39 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:17:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0976d669787f3fcd6abd2508a3d2424decead22cd66d405b4da7e9c988499a6a`  
		Last Modified: Fri, 02 Sep 2022 06:34:43 GMT  
		Size: 103.9 MB (103924320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf3fa151f78e7974d35e7b47f6903b56457dff01611cabf07d24d4ad288b33f`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04ff1eccf75d5a0a9ed12a8822d1ecf37c92116c7e660f92c8a125f4b5b869b`  
		Last Modified: Fri, 02 Sep 2022 06:35:07 GMT  
		Size: 95.2 MB (95214806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d93b09dedad3c115236fd0ec61587b6872929fddf38f3c50298742c5e54a9c`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 285.5 KB (285519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa0bcbf474ccec4a8b2b8e6782135e6a9ee15328201b05e761764988c680c41`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 2.4 KB (2363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862c83aa445983369fee4e683ab2e4f96cd4c4855ec8f187c71c40aa65661a74`  
		Last Modified: Fri, 02 Sep 2022 06:34:57 GMT  
		Size: 22.4 MB (22428152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:d43aaaae847685889a49a4d9c6b95bba609dafa1071e655f50e499f3bac29940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:9563bfd3172e8574e1715fcb30492c30b83fb2df3cf85d3ea29cc7057654b280
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141622125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ff91d7a0709c149df8e6061c129ad8b19cad65d1d90d21a7c4dd39918822a3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 04:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:49:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:49:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:49:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f3dbe0ec1046bb9bdd0276165d66b03aafb64279b2077b7fbdac5b1047b98e`  
		Last Modified: Fri, 02 Sep 2022 05:12:12 GMT  
		Size: 106.2 MB (106189810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ef6ac4127ac4c6d2c35e9befe4af09debd87c5e55110651f46e88a35c631`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ed4c506a70a1fc02f42a9a6bbceb12d7353f1ee5f1af0f84fcb5e438de32a1b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137080776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ffd6f978c34b81f405c704c5a77b8d042c18d88a04910e6d93f2e48a9da3277`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:16:00 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 06:16:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:16:49 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:16:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:16:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0976d669787f3fcd6abd2508a3d2424decead22cd66d405b4da7e9c988499a6a`  
		Last Modified: Fri, 02 Sep 2022 06:34:43 GMT  
		Size: 103.9 MB (103924320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf3fa151f78e7974d35e7b47f6903b56457dff01611cabf07d24d4ad288b33f`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:d43aaaae847685889a49a4d9c6b95bba609dafa1071e655f50e499f3bac29940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:9563bfd3172e8574e1715fcb30492c30b83fb2df3cf85d3ea29cc7057654b280
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141622125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ff91d7a0709c149df8e6061c129ad8b19cad65d1d90d21a7c4dd39918822a3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 04:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:49:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:49:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:49:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f3dbe0ec1046bb9bdd0276165d66b03aafb64279b2077b7fbdac5b1047b98e`  
		Last Modified: Fri, 02 Sep 2022 05:12:12 GMT  
		Size: 106.2 MB (106189810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ef6ac4127ac4c6d2c35e9befe4af09debd87c5e55110651f46e88a35c631`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ed4c506a70a1fc02f42a9a6bbceb12d7353f1ee5f1af0f84fcb5e438de32a1b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137080776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ffd6f978c34b81f405c704c5a77b8d042c18d88a04910e6d93f2e48a9da3277`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:16:00 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 06:16:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:16:49 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:16:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:16:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0976d669787f3fcd6abd2508a3d2424decead22cd66d405b4da7e9c988499a6a`  
		Last Modified: Fri, 02 Sep 2022 06:34:43 GMT  
		Size: 103.9 MB (103924320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf3fa151f78e7974d35e7b47f6903b56457dff01611cabf07d24d4ad288b33f`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:2957f3c0f64a2887b5f8e81d3aef38e99963dbe3a9b50e1ad1846fb422b45b8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:b5afc3c15a18c85bd4472228addb045cfa1be4955efd4f7d1f5bc2bd1ea938a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262767288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0afc637f4748749ba7294a29cff472a9aff855e9b3f1c1a4641daf1c47f61306`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 04:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:49:26 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:49:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:49:26 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:50:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:50:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:50:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:51:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f3dbe0ec1046bb9bdd0276165d66b03aafb64279b2077b7fbdac5b1047b98e`  
		Last Modified: Fri, 02 Sep 2022 05:12:12 GMT  
		Size: 106.2 MB (106189810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ef6ac4127ac4c6d2c35e9befe4af09debd87c5e55110651f46e88a35c631`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47e8a6f8a449077cfb0901a9b21c22e899338a0bc99ca9be0951bf6b3256c1a`  
		Last Modified: Fri, 02 Sep 2022 05:12:36 GMT  
		Size: 97.8 MB (97849527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40faf29acfa4fc6c1747729238c7b69b3c05983e5f81a16389a75b6b7fad4ed7`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 285.6 KB (285574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df57c7f1a275a97de9412ce0ca9182e86900074cda4ea3b82bb20d7a3c374a0c`  
		Last Modified: Fri, 02 Sep 2022 05:12:22 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3101d89bfa03579ba584f494cd916ad9cd928e61dec78734db0bf203c0ae68`  
		Last Modified: Fri, 02 Sep 2022 05:12:26 GMT  
		Size: 23.0 MB (23007608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:41a4bf37d3bafe29278c7df4d27d9632379e135f6cdb0adaca4a9b27129e52ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (255011616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40cf39c2d4982fb75e99085a66a9adac5a4689114fa27e86bfa647dca3b08fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:16:00 GMT
ENV ROS_DISTRO=humble
# Fri, 02 Sep 2022 06:16:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:16:49 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:16:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:16:51 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:17:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:17:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:17:39 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:17:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0976d669787f3fcd6abd2508a3d2424decead22cd66d405b4da7e9c988499a6a`  
		Last Modified: Fri, 02 Sep 2022 06:34:43 GMT  
		Size: 103.9 MB (103924320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf3fa151f78e7974d35e7b47f6903b56457dff01611cabf07d24d4ad288b33f`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04ff1eccf75d5a0a9ed12a8822d1ecf37c92116c7e660f92c8a125f4b5b869b`  
		Last Modified: Fri, 02 Sep 2022 06:35:07 GMT  
		Size: 95.2 MB (95214806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d93b09dedad3c115236fd0ec61587b6872929fddf38f3c50298742c5e54a9c`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 285.5 KB (285519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa0bcbf474ccec4a8b2b8e6782135e6a9ee15328201b05e761764988c680c41`  
		Last Modified: Fri, 02 Sep 2022 06:34:54 GMT  
		Size: 2.4 KB (2363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862c83aa445983369fee4e683ab2e4f96cd4c4855ec8f187c71c40aa65661a74`  
		Last Modified: Fri, 02 Sep 2022 06:34:57 GMT  
		Size: 22.4 MB (22428152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:599c778f902462e7b2da29cb5ce052fd683cc30b3e17868a8bd373a6145f2bea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:e894f44bf088cc62986b1aae33d8a8ec96810c746194983ce48d373f28c2eb60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437515827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e77b7e42944fc41a062c94ba1e54f9bc75737c6f1ee3293947939145ea10318`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:20:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 04:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:22:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:22:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:22:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:23:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:23:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc21f3c6df3e09da41edf5cd277be198a0b9ce9de84590bce7c7f8169fe8458`  
		Last Modified: Fri, 02 Sep 2022 05:04:14 GMT  
		Size: 4.9 MB (4873660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601897ffb3e3526f97b7f3ac57655aa3b636d8d501e997e89629b654dd7e8dc`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02d512a7003472763130f30478d4f0c5e440cc42c6e111764af77b527686d5`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a32123d45b8f75cdc98623e79fe3c15f9f2da76e2827622e844770c38afa4`  
		Last Modified: Fri, 02 Sep 2022 05:04:53 GMT  
		Size: 259.6 MB (259559627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abce6b68d4012a79d622c3088e409f52f46a4c2d57e7d45df885e9a566a052c`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0804aad7d24aedc9674dd262573672ffb24e77bd0b94b38774dd4c1344a65`  
		Last Modified: Fri, 02 Sep 2022 05:05:12 GMT  
		Size: 70.3 MB (70259712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4c705dfb136d0edfefa4b6ea486990b27430cb1acb7e7aa9c680225f5845c`  
		Last Modified: Fri, 02 Sep 2022 05:05:02 GMT  
		Size: 284.7 KB (284711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463d8179e60fd0676ccb9cded217236342e7d2d9185a56f2f003efb6d1e597bf`  
		Last Modified: Fri, 02 Sep 2022 05:05:14 GMT  
		Size: 75.0 MB (74995198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:814af5012b36d9eed06c9cac7ad085d72ce7030a89e9b46d7c8f5c6d74d5bc25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (385997135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835e9afd0c76cb727206ffdc1e255cb66a4ad1f768b4a044f6316e2a544b93c0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:38:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:39:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV ROS_DISTRO=melodic
# Wed, 03 Aug 2022 22:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:42:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:42:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:42:42 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:43:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:44:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:46:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad475a95b77752b25dc36bec810d7cc2000f86bc50ea57592b8f988605fc4c6`  
		Last Modified: Wed, 03 Aug 2022 23:06:53 GMT  
		Size: 840.0 KB (839977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76a2f1b035d0df7e2f785a3199e9e86fdeeda1c9f6087f594f2d8a42f0cfb`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 4.1 MB (4087975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acdc23d18c079581f3391d042b65fd7ae55d75333914fd8cdcd0b8acdd6bf10`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3a86db6f1e409fa1d0b2018d788c0539b214c365337f886b86db7e860ee482`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c58cc0918adb02a33e27d7ad4e74c5e0463844a26e99fb60557c3594324b5`  
		Last Modified: Wed, 03 Aug 2022 23:07:34 GMT  
		Size: 239.0 MB (239014439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e568816932729edf86ebafaaeb847af8bda6ade01fb926c6a121f6b825974`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23d14b221e943bfa66059662f80e5ae90e6e1f053ed424ca6b2a40c15876113`  
		Last Modified: Wed, 03 Aug 2022 23:07:57 GMT  
		Size: 54.7 MB (54720659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537d299c243ea0c73b05e8b607aa42ec071f847fbfa98d9ab5463a6594a04406`  
		Last Modified: Wed, 03 Aug 2022 23:07:46 GMT  
		Size: 283.1 KB (283112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d03bb1219b316469e8bd9f059ea35bbe07e5c60596349c1a2f46c2230f51e2`  
		Last Modified: Wed, 03 Aug 2022 23:08:02 GMT  
		Size: 64.7 MB (64743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a017f5b1831aed25ba8fa263279b616191b00173d0d95c4b20ade8026023c6b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.7 MB (411713079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fab7ccc0e2a24d05f9ac4c885d8e7249b5ed274c7312c5703daa04ce0fd0bd2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:58:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 05:58:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 05:58:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 05:58:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 05:58:48 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:00:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:00:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:00:19 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:01:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741c1db167ba98dcc4f0b1dce059664982999c77d7cad916a075711462e7e58d`  
		Last Modified: Fri, 02 Sep 2022 06:26:53 GMT  
		Size: 831.6 KB (831649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4f808c51f1cf44217d8ce4ebca03255e969acca4cf09dff77aee0d3f3a816d`  
		Last Modified: Fri, 02 Sep 2022 06:26:52 GMT  
		Size: 4.3 MB (4265983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19873eb8e73732ae72ef6128c3fa94f987527a5a1439d57eb398f1cb5f4df`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fea62807d8351d36c0b83cdd41872e4d80c976755fa7a501da8e7e7437ad6c`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181336855135b72b6bf5b30d7c1e5beebbdd63f1fe6c933ab551f4a196e800f1`  
		Last Modified: Fri, 02 Sep 2022 06:27:26 GMT  
		Size: 252.5 MB (252504641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284d05b44a890de734833cf20b5313f89437f66ee971f29d55252b3d63572a19`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5912bc4d8ce79891b6639473d128eac65e87986185897f1cc258c457ac8e7ca1`  
		Last Modified: Fri, 02 Sep 2022 06:27:46 GMT  
		Size: 63.1 MB (63088909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767c5618f004c047c357ca236bbcdb7d205c11b960f1d0d7e69a5b074923fe7`  
		Last Modified: Fri, 02 Sep 2022 06:27:37 GMT  
		Size: 284.7 KB (284651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bbb5ba813f9800cb0ccc8cc793a2a5a75588b1ba651ba7a58afd3b8c9f2115`  
		Last Modified: Fri, 02 Sep 2022 06:27:48 GMT  
		Size: 67.0 MB (67001363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:1462562db0edc62b40c7bf7aade03f17ff45b4e81288a4714aa654b5221ea9fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:6161bfe6f5130cd4a735c86853cf7938719faab46bf7598700c32d9e6c905c16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742863544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f193582ec5d8aa3650e7bb7af89868fd4265bcd8af0e4262805656156bf49a39`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:20:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 04:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:22:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:22:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:22:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:23:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:23:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc21f3c6df3e09da41edf5cd277be198a0b9ce9de84590bce7c7f8169fe8458`  
		Last Modified: Fri, 02 Sep 2022 05:04:14 GMT  
		Size: 4.9 MB (4873660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601897ffb3e3526f97b7f3ac57655aa3b636d8d501e997e89629b654dd7e8dc`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02d512a7003472763130f30478d4f0c5e440cc42c6e111764af77b527686d5`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a32123d45b8f75cdc98623e79fe3c15f9f2da76e2827622e844770c38afa4`  
		Last Modified: Fri, 02 Sep 2022 05:04:53 GMT  
		Size: 259.6 MB (259559627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abce6b68d4012a79d622c3088e409f52f46a4c2d57e7d45df885e9a566a052c`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0804aad7d24aedc9674dd262573672ffb24e77bd0b94b38774dd4c1344a65`  
		Last Modified: Fri, 02 Sep 2022 05:05:12 GMT  
		Size: 70.3 MB (70259712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4c705dfb136d0edfefa4b6ea486990b27430cb1acb7e7aa9c680225f5845c`  
		Last Modified: Fri, 02 Sep 2022 05:05:02 GMT  
		Size: 284.7 KB (284711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463d8179e60fd0676ccb9cded217236342e7d2d9185a56f2f003efb6d1e597bf`  
		Last Modified: Fri, 02 Sep 2022 05:05:14 GMT  
		Size: 75.0 MB (74995198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9ad2f398f5cff0abe5f19d6199b225ec6b2591d2450a4222f6d1b8210f9bbf`  
		Last Modified: Fri, 02 Sep 2022 05:06:25 GMT  
		Size: 305.3 MB (305347717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:fb56a30a42037799cccacc2d306c93fb5b70fb26c7f5bc8d6cde583f63b68b57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.0 MB (646041548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0a6500c512cffcafac3324bd92bbeb06210f4ed725fb52e531a98253a8241d9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:38:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:39:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV ROS_DISTRO=melodic
# Wed, 03 Aug 2022 22:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:42:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:42:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:42:42 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:43:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:44:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:46:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:52:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad475a95b77752b25dc36bec810d7cc2000f86bc50ea57592b8f988605fc4c6`  
		Last Modified: Wed, 03 Aug 2022 23:06:53 GMT  
		Size: 840.0 KB (839977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76a2f1b035d0df7e2f785a3199e9e86fdeeda1c9f6087f594f2d8a42f0cfb`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 4.1 MB (4087975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acdc23d18c079581f3391d042b65fd7ae55d75333914fd8cdcd0b8acdd6bf10`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3a86db6f1e409fa1d0b2018d788c0539b214c365337f886b86db7e860ee482`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c58cc0918adb02a33e27d7ad4e74c5e0463844a26e99fb60557c3594324b5`  
		Last Modified: Wed, 03 Aug 2022 23:07:34 GMT  
		Size: 239.0 MB (239014439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e568816932729edf86ebafaaeb847af8bda6ade01fb926c6a121f6b825974`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23d14b221e943bfa66059662f80e5ae90e6e1f053ed424ca6b2a40c15876113`  
		Last Modified: Wed, 03 Aug 2022 23:07:57 GMT  
		Size: 54.7 MB (54720659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537d299c243ea0c73b05e8b607aa42ec071f847fbfa98d9ab5463a6594a04406`  
		Last Modified: Wed, 03 Aug 2022 23:07:46 GMT  
		Size: 283.1 KB (283112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d03bb1219b316469e8bd9f059ea35bbe07e5c60596349c1a2f46c2230f51e2`  
		Last Modified: Wed, 03 Aug 2022 23:08:02 GMT  
		Size: 64.7 MB (64743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3a8af3711aa61966951251c2db1ff769876ceeb475fc27d25c223cb4a7d293`  
		Last Modified: Wed, 03 Aug 2022 23:09:15 GMT  
		Size: 260.0 MB (260044413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7b82c82ee1a0a4fa80e27e48388e742b0fabdf020389baf4cb65aa46c45e6842
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.2 MB (703157629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c365f5838312ab433bc5133b089b99c3385e55ebceeea554393361d25380876a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:58:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 05:58:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 05:58:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 05:58:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 05:58:48 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:00:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:00:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:00:19 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:01:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:03:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741c1db167ba98dcc4f0b1dce059664982999c77d7cad916a075711462e7e58d`  
		Last Modified: Fri, 02 Sep 2022 06:26:53 GMT  
		Size: 831.6 KB (831649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4f808c51f1cf44217d8ce4ebca03255e969acca4cf09dff77aee0d3f3a816d`  
		Last Modified: Fri, 02 Sep 2022 06:26:52 GMT  
		Size: 4.3 MB (4265983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19873eb8e73732ae72ef6128c3fa94f987527a5a1439d57eb398f1cb5f4df`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fea62807d8351d36c0b83cdd41872e4d80c976755fa7a501da8e7e7437ad6c`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181336855135b72b6bf5b30d7c1e5beebbdd63f1fe6c933ab551f4a196e800f1`  
		Last Modified: Fri, 02 Sep 2022 06:27:26 GMT  
		Size: 252.5 MB (252504641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284d05b44a890de734833cf20b5313f89437f66ee971f29d55252b3d63572a19`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5912bc4d8ce79891b6639473d128eac65e87986185897f1cc258c457ac8e7ca1`  
		Last Modified: Fri, 02 Sep 2022 06:27:46 GMT  
		Size: 63.1 MB (63088909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767c5618f004c047c357ca236bbcdb7d205c11b960f1d0d7e69a5b074923fe7`  
		Last Modified: Fri, 02 Sep 2022 06:27:37 GMT  
		Size: 284.7 KB (284651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bbb5ba813f9800cb0ccc8cc793a2a5a75588b1ba651ba7a58afd3b8c9f2115`  
		Last Modified: Fri, 02 Sep 2022 06:27:48 GMT  
		Size: 67.0 MB (67001363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bdfb0b91d2badff31d5194b03325f705f919c636ff3b578ea0d56c042d6556`  
		Last Modified: Fri, 02 Sep 2022 06:28:59 GMT  
		Size: 291.4 MB (291444550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:1462562db0edc62b40c7bf7aade03f17ff45b4e81288a4714aa654b5221ea9fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:6161bfe6f5130cd4a735c86853cf7938719faab46bf7598700c32d9e6c905c16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742863544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f193582ec5d8aa3650e7bb7af89868fd4265bcd8af0e4262805656156bf49a39`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:20:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 04:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:22:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:22:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:22:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:23:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:23:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc21f3c6df3e09da41edf5cd277be198a0b9ce9de84590bce7c7f8169fe8458`  
		Last Modified: Fri, 02 Sep 2022 05:04:14 GMT  
		Size: 4.9 MB (4873660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601897ffb3e3526f97b7f3ac57655aa3b636d8d501e997e89629b654dd7e8dc`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02d512a7003472763130f30478d4f0c5e440cc42c6e111764af77b527686d5`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a32123d45b8f75cdc98623e79fe3c15f9f2da76e2827622e844770c38afa4`  
		Last Modified: Fri, 02 Sep 2022 05:04:53 GMT  
		Size: 259.6 MB (259559627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abce6b68d4012a79d622c3088e409f52f46a4c2d57e7d45df885e9a566a052c`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0804aad7d24aedc9674dd262573672ffb24e77bd0b94b38774dd4c1344a65`  
		Last Modified: Fri, 02 Sep 2022 05:05:12 GMT  
		Size: 70.3 MB (70259712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4c705dfb136d0edfefa4b6ea486990b27430cb1acb7e7aa9c680225f5845c`  
		Last Modified: Fri, 02 Sep 2022 05:05:02 GMT  
		Size: 284.7 KB (284711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463d8179e60fd0676ccb9cded217236342e7d2d9185a56f2f003efb6d1e597bf`  
		Last Modified: Fri, 02 Sep 2022 05:05:14 GMT  
		Size: 75.0 MB (74995198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9ad2f398f5cff0abe5f19d6199b225ec6b2591d2450a4222f6d1b8210f9bbf`  
		Last Modified: Fri, 02 Sep 2022 05:06:25 GMT  
		Size: 305.3 MB (305347717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:fb56a30a42037799cccacc2d306c93fb5b70fb26c7f5bc8d6cde583f63b68b57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.0 MB (646041548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0a6500c512cffcafac3324bd92bbeb06210f4ed725fb52e531a98253a8241d9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:38:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:39:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV ROS_DISTRO=melodic
# Wed, 03 Aug 2022 22:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:42:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:42:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:42:42 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:43:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:44:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:46:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:52:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad475a95b77752b25dc36bec810d7cc2000f86bc50ea57592b8f988605fc4c6`  
		Last Modified: Wed, 03 Aug 2022 23:06:53 GMT  
		Size: 840.0 KB (839977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76a2f1b035d0df7e2f785a3199e9e86fdeeda1c9f6087f594f2d8a42f0cfb`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 4.1 MB (4087975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acdc23d18c079581f3391d042b65fd7ae55d75333914fd8cdcd0b8acdd6bf10`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3a86db6f1e409fa1d0b2018d788c0539b214c365337f886b86db7e860ee482`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c58cc0918adb02a33e27d7ad4e74c5e0463844a26e99fb60557c3594324b5`  
		Last Modified: Wed, 03 Aug 2022 23:07:34 GMT  
		Size: 239.0 MB (239014439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e568816932729edf86ebafaaeb847af8bda6ade01fb926c6a121f6b825974`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23d14b221e943bfa66059662f80e5ae90e6e1f053ed424ca6b2a40c15876113`  
		Last Modified: Wed, 03 Aug 2022 23:07:57 GMT  
		Size: 54.7 MB (54720659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537d299c243ea0c73b05e8b607aa42ec071f847fbfa98d9ab5463a6594a04406`  
		Last Modified: Wed, 03 Aug 2022 23:07:46 GMT  
		Size: 283.1 KB (283112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d03bb1219b316469e8bd9f059ea35bbe07e5c60596349c1a2f46c2230f51e2`  
		Last Modified: Wed, 03 Aug 2022 23:08:02 GMT  
		Size: 64.7 MB (64743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3a8af3711aa61966951251c2db1ff769876ceeb475fc27d25c223cb4a7d293`  
		Last Modified: Wed, 03 Aug 2022 23:09:15 GMT  
		Size: 260.0 MB (260044413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7b82c82ee1a0a4fa80e27e48388e742b0fabdf020389baf4cb65aa46c45e6842
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.2 MB (703157629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c365f5838312ab433bc5133b089b99c3385e55ebceeea554393361d25380876a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:58:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 05:58:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 05:58:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 05:58:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 05:58:48 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:00:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:00:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:00:19 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:01:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:03:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741c1db167ba98dcc4f0b1dce059664982999c77d7cad916a075711462e7e58d`  
		Last Modified: Fri, 02 Sep 2022 06:26:53 GMT  
		Size: 831.6 KB (831649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4f808c51f1cf44217d8ce4ebca03255e969acca4cf09dff77aee0d3f3a816d`  
		Last Modified: Fri, 02 Sep 2022 06:26:52 GMT  
		Size: 4.3 MB (4265983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19873eb8e73732ae72ef6128c3fa94f987527a5a1439d57eb398f1cb5f4df`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fea62807d8351d36c0b83cdd41872e4d80c976755fa7a501da8e7e7437ad6c`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181336855135b72b6bf5b30d7c1e5beebbdd63f1fe6c933ab551f4a196e800f1`  
		Last Modified: Fri, 02 Sep 2022 06:27:26 GMT  
		Size: 252.5 MB (252504641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284d05b44a890de734833cf20b5313f89437f66ee971f29d55252b3d63572a19`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5912bc4d8ce79891b6639473d128eac65e87986185897f1cc258c457ac8e7ca1`  
		Last Modified: Fri, 02 Sep 2022 06:27:46 GMT  
		Size: 63.1 MB (63088909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767c5618f004c047c357ca236bbcdb7d205c11b960f1d0d7e69a5b074923fe7`  
		Last Modified: Fri, 02 Sep 2022 06:27:37 GMT  
		Size: 284.7 KB (284651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bbb5ba813f9800cb0ccc8cc793a2a5a75588b1ba651ba7a58afd3b8c9f2115`  
		Last Modified: Fri, 02 Sep 2022 06:27:48 GMT  
		Size: 67.0 MB (67001363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bdfb0b91d2badff31d5194b03325f705f919c636ff3b578ea0d56c042d6556`  
		Last Modified: Fri, 02 Sep 2022 06:28:59 GMT  
		Size: 291.4 MB (291444550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:258d51fa572a77fd70a2bef486c07b8489bc86c35d54e72624dde9eb07a1b399
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:85bc4c3c605d67ba0ef9275c4750d9cf8af7bcb8a3b01be2a686cb56e570bd51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448601669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8721d889104c51a26ed1d5208079740f172ba6c73512808b54b32fa72fc2397`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:20:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 04:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:22:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:22:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:22:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:23:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:23:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:25:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc21f3c6df3e09da41edf5cd277be198a0b9ce9de84590bce7c7f8169fe8458`  
		Last Modified: Fri, 02 Sep 2022 05:04:14 GMT  
		Size: 4.9 MB (4873660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601897ffb3e3526f97b7f3ac57655aa3b636d8d501e997e89629b654dd7e8dc`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02d512a7003472763130f30478d4f0c5e440cc42c6e111764af77b527686d5`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a32123d45b8f75cdc98623e79fe3c15f9f2da76e2827622e844770c38afa4`  
		Last Modified: Fri, 02 Sep 2022 05:04:53 GMT  
		Size: 259.6 MB (259559627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abce6b68d4012a79d622c3088e409f52f46a4c2d57e7d45df885e9a566a052c`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0804aad7d24aedc9674dd262573672ffb24e77bd0b94b38774dd4c1344a65`  
		Last Modified: Fri, 02 Sep 2022 05:05:12 GMT  
		Size: 70.3 MB (70259712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4c705dfb136d0edfefa4b6ea486990b27430cb1acb7e7aa9c680225f5845c`  
		Last Modified: Fri, 02 Sep 2022 05:05:02 GMT  
		Size: 284.7 KB (284711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463d8179e60fd0676ccb9cded217236342e7d2d9185a56f2f003efb6d1e597bf`  
		Last Modified: Fri, 02 Sep 2022 05:05:14 GMT  
		Size: 75.0 MB (74995198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f95ccd28b67e6e24906599991ef70fb02811a4e3873615747bd8af8017f7bc`  
		Last Modified: Fri, 02 Sep 2022 05:05:28 GMT  
		Size: 11.1 MB (11085842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:7f4b7e824e2c2d884a5fb5a2c9b781342f4cf8aa705a8a43780f57b072fceb77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396120708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09ce3f49835d2c880946babd1f27d25bd83fed4169ab6f73ef3ed6972266945`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:38:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:39:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV ROS_DISTRO=melodic
# Wed, 03 Aug 2022 22:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:42:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:42:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:42:42 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:43:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:44:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:46:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:47:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad475a95b77752b25dc36bec810d7cc2000f86bc50ea57592b8f988605fc4c6`  
		Last Modified: Wed, 03 Aug 2022 23:06:53 GMT  
		Size: 840.0 KB (839977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76a2f1b035d0df7e2f785a3199e9e86fdeeda1c9f6087f594f2d8a42f0cfb`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 4.1 MB (4087975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acdc23d18c079581f3391d042b65fd7ae55d75333914fd8cdcd0b8acdd6bf10`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3a86db6f1e409fa1d0b2018d788c0539b214c365337f886b86db7e860ee482`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c58cc0918adb02a33e27d7ad4e74c5e0463844a26e99fb60557c3594324b5`  
		Last Modified: Wed, 03 Aug 2022 23:07:34 GMT  
		Size: 239.0 MB (239014439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e568816932729edf86ebafaaeb847af8bda6ade01fb926c6a121f6b825974`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23d14b221e943bfa66059662f80e5ae90e6e1f053ed424ca6b2a40c15876113`  
		Last Modified: Wed, 03 Aug 2022 23:07:57 GMT  
		Size: 54.7 MB (54720659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537d299c243ea0c73b05e8b607aa42ec071f847fbfa98d9ab5463a6594a04406`  
		Last Modified: Wed, 03 Aug 2022 23:07:46 GMT  
		Size: 283.1 KB (283112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d03bb1219b316469e8bd9f059ea35bbe07e5c60596349c1a2f46c2230f51e2`  
		Last Modified: Wed, 03 Aug 2022 23:08:02 GMT  
		Size: 64.7 MB (64743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a494ed3d310625a6aa0f4889bc59e46085f1933560b3cf30b478de3be02dae6`  
		Last Modified: Wed, 03 Aug 2022 23:08:20 GMT  
		Size: 10.1 MB (10123573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3dc563618f94c289ff4fb6380b08ac5e419824dd9ab05ee85824d9fda47a01de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.4 MB (422448964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f87df4ce0f85310e58f4b79d8592460a43aafc45d9dc8e8909fe84ced5eee8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:58:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 05:58:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 05:58:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 05:58:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 05:58:48 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:00:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:00:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:00:19 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:01:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:02:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741c1db167ba98dcc4f0b1dce059664982999c77d7cad916a075711462e7e58d`  
		Last Modified: Fri, 02 Sep 2022 06:26:53 GMT  
		Size: 831.6 KB (831649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4f808c51f1cf44217d8ce4ebca03255e969acca4cf09dff77aee0d3f3a816d`  
		Last Modified: Fri, 02 Sep 2022 06:26:52 GMT  
		Size: 4.3 MB (4265983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19873eb8e73732ae72ef6128c3fa94f987527a5a1439d57eb398f1cb5f4df`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fea62807d8351d36c0b83cdd41872e4d80c976755fa7a501da8e7e7437ad6c`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181336855135b72b6bf5b30d7c1e5beebbdd63f1fe6c933ab551f4a196e800f1`  
		Last Modified: Fri, 02 Sep 2022 06:27:26 GMT  
		Size: 252.5 MB (252504641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284d05b44a890de734833cf20b5313f89437f66ee971f29d55252b3d63572a19`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5912bc4d8ce79891b6639473d128eac65e87986185897f1cc258c457ac8e7ca1`  
		Last Modified: Fri, 02 Sep 2022 06:27:46 GMT  
		Size: 63.1 MB (63088909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767c5618f004c047c357ca236bbcdb7d205c11b960f1d0d7e69a5b074923fe7`  
		Last Modified: Fri, 02 Sep 2022 06:27:37 GMT  
		Size: 284.7 KB (284651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bbb5ba813f9800cb0ccc8cc793a2a5a75588b1ba651ba7a58afd3b8c9f2115`  
		Last Modified: Fri, 02 Sep 2022 06:27:48 GMT  
		Size: 67.0 MB (67001363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e000c44a6a1b7e651141833ad6b8b222dcb51bff6496e03dd8a4420a6836cb`  
		Last Modified: Fri, 02 Sep 2022 06:28:04 GMT  
		Size: 10.7 MB (10735885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:258d51fa572a77fd70a2bef486c07b8489bc86c35d54e72624dde9eb07a1b399
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:85bc4c3c605d67ba0ef9275c4750d9cf8af7bcb8a3b01be2a686cb56e570bd51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448601669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8721d889104c51a26ed1d5208079740f172ba6c73512808b54b32fa72fc2397`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:20:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 04:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:22:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:22:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:22:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:23:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:23:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:25:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc21f3c6df3e09da41edf5cd277be198a0b9ce9de84590bce7c7f8169fe8458`  
		Last Modified: Fri, 02 Sep 2022 05:04:14 GMT  
		Size: 4.9 MB (4873660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601897ffb3e3526f97b7f3ac57655aa3b636d8d501e997e89629b654dd7e8dc`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02d512a7003472763130f30478d4f0c5e440cc42c6e111764af77b527686d5`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a32123d45b8f75cdc98623e79fe3c15f9f2da76e2827622e844770c38afa4`  
		Last Modified: Fri, 02 Sep 2022 05:04:53 GMT  
		Size: 259.6 MB (259559627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abce6b68d4012a79d622c3088e409f52f46a4c2d57e7d45df885e9a566a052c`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0804aad7d24aedc9674dd262573672ffb24e77bd0b94b38774dd4c1344a65`  
		Last Modified: Fri, 02 Sep 2022 05:05:12 GMT  
		Size: 70.3 MB (70259712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4c705dfb136d0edfefa4b6ea486990b27430cb1acb7e7aa9c680225f5845c`  
		Last Modified: Fri, 02 Sep 2022 05:05:02 GMT  
		Size: 284.7 KB (284711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463d8179e60fd0676ccb9cded217236342e7d2d9185a56f2f003efb6d1e597bf`  
		Last Modified: Fri, 02 Sep 2022 05:05:14 GMT  
		Size: 75.0 MB (74995198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f95ccd28b67e6e24906599991ef70fb02811a4e3873615747bd8af8017f7bc`  
		Last Modified: Fri, 02 Sep 2022 05:05:28 GMT  
		Size: 11.1 MB (11085842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:7f4b7e824e2c2d884a5fb5a2c9b781342f4cf8aa705a8a43780f57b072fceb77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396120708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09ce3f49835d2c880946babd1f27d25bd83fed4169ab6f73ef3ed6972266945`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:38:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:39:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV ROS_DISTRO=melodic
# Wed, 03 Aug 2022 22:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:42:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:42:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:42:42 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:43:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:44:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:46:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:47:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad475a95b77752b25dc36bec810d7cc2000f86bc50ea57592b8f988605fc4c6`  
		Last Modified: Wed, 03 Aug 2022 23:06:53 GMT  
		Size: 840.0 KB (839977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76a2f1b035d0df7e2f785a3199e9e86fdeeda1c9f6087f594f2d8a42f0cfb`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 4.1 MB (4087975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acdc23d18c079581f3391d042b65fd7ae55d75333914fd8cdcd0b8acdd6bf10`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3a86db6f1e409fa1d0b2018d788c0539b214c365337f886b86db7e860ee482`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c58cc0918adb02a33e27d7ad4e74c5e0463844a26e99fb60557c3594324b5`  
		Last Modified: Wed, 03 Aug 2022 23:07:34 GMT  
		Size: 239.0 MB (239014439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e568816932729edf86ebafaaeb847af8bda6ade01fb926c6a121f6b825974`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23d14b221e943bfa66059662f80e5ae90e6e1f053ed424ca6b2a40c15876113`  
		Last Modified: Wed, 03 Aug 2022 23:07:57 GMT  
		Size: 54.7 MB (54720659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537d299c243ea0c73b05e8b607aa42ec071f847fbfa98d9ab5463a6594a04406`  
		Last Modified: Wed, 03 Aug 2022 23:07:46 GMT  
		Size: 283.1 KB (283112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d03bb1219b316469e8bd9f059ea35bbe07e5c60596349c1a2f46c2230f51e2`  
		Last Modified: Wed, 03 Aug 2022 23:08:02 GMT  
		Size: 64.7 MB (64743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a494ed3d310625a6aa0f4889bc59e46085f1933560b3cf30b478de3be02dae6`  
		Last Modified: Wed, 03 Aug 2022 23:08:20 GMT  
		Size: 10.1 MB (10123573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3dc563618f94c289ff4fb6380b08ac5e419824dd9ab05ee85824d9fda47a01de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.4 MB (422448964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f87df4ce0f85310e58f4b79d8592460a43aafc45d9dc8e8909fe84ced5eee8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:58:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 05:58:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 05:58:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 05:58:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 05:58:48 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:00:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:00:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:00:19 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:01:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:02:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741c1db167ba98dcc4f0b1dce059664982999c77d7cad916a075711462e7e58d`  
		Last Modified: Fri, 02 Sep 2022 06:26:53 GMT  
		Size: 831.6 KB (831649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4f808c51f1cf44217d8ce4ebca03255e969acca4cf09dff77aee0d3f3a816d`  
		Last Modified: Fri, 02 Sep 2022 06:26:52 GMT  
		Size: 4.3 MB (4265983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19873eb8e73732ae72ef6128c3fa94f987527a5a1439d57eb398f1cb5f4df`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fea62807d8351d36c0b83cdd41872e4d80c976755fa7a501da8e7e7437ad6c`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181336855135b72b6bf5b30d7c1e5beebbdd63f1fe6c933ab551f4a196e800f1`  
		Last Modified: Fri, 02 Sep 2022 06:27:26 GMT  
		Size: 252.5 MB (252504641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284d05b44a890de734833cf20b5313f89437f66ee971f29d55252b3d63572a19`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5912bc4d8ce79891b6639473d128eac65e87986185897f1cc258c457ac8e7ca1`  
		Last Modified: Fri, 02 Sep 2022 06:27:46 GMT  
		Size: 63.1 MB (63088909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767c5618f004c047c357ca236bbcdb7d205c11b960f1d0d7e69a5b074923fe7`  
		Last Modified: Fri, 02 Sep 2022 06:27:37 GMT  
		Size: 284.7 KB (284651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bbb5ba813f9800cb0ccc8cc793a2a5a75588b1ba651ba7a58afd3b8c9f2115`  
		Last Modified: Fri, 02 Sep 2022 06:27:48 GMT  
		Size: 67.0 MB (67001363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e000c44a6a1b7e651141833ad6b8b222dcb51bff6496e03dd8a4420a6836cb`  
		Last Modified: Fri, 02 Sep 2022 06:28:04 GMT  
		Size: 10.7 MB (10735885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:599c778f902462e7b2da29cb5ce052fd683cc30b3e17868a8bd373a6145f2bea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:e894f44bf088cc62986b1aae33d8a8ec96810c746194983ce48d373f28c2eb60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437515827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e77b7e42944fc41a062c94ba1e54f9bc75737c6f1ee3293947939145ea10318`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:20:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 04:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:22:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:22:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:22:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:23:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:23:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc21f3c6df3e09da41edf5cd277be198a0b9ce9de84590bce7c7f8169fe8458`  
		Last Modified: Fri, 02 Sep 2022 05:04:14 GMT  
		Size: 4.9 MB (4873660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601897ffb3e3526f97b7f3ac57655aa3b636d8d501e997e89629b654dd7e8dc`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02d512a7003472763130f30478d4f0c5e440cc42c6e111764af77b527686d5`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a32123d45b8f75cdc98623e79fe3c15f9f2da76e2827622e844770c38afa4`  
		Last Modified: Fri, 02 Sep 2022 05:04:53 GMT  
		Size: 259.6 MB (259559627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abce6b68d4012a79d622c3088e409f52f46a4c2d57e7d45df885e9a566a052c`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0804aad7d24aedc9674dd262573672ffb24e77bd0b94b38774dd4c1344a65`  
		Last Modified: Fri, 02 Sep 2022 05:05:12 GMT  
		Size: 70.3 MB (70259712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4c705dfb136d0edfefa4b6ea486990b27430cb1acb7e7aa9c680225f5845c`  
		Last Modified: Fri, 02 Sep 2022 05:05:02 GMT  
		Size: 284.7 KB (284711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463d8179e60fd0676ccb9cded217236342e7d2d9185a56f2f003efb6d1e597bf`  
		Last Modified: Fri, 02 Sep 2022 05:05:14 GMT  
		Size: 75.0 MB (74995198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:814af5012b36d9eed06c9cac7ad085d72ce7030a89e9b46d7c8f5c6d74d5bc25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (385997135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835e9afd0c76cb727206ffdc1e255cb66a4ad1f768b4a044f6316e2a544b93c0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:38:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:39:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV ROS_DISTRO=melodic
# Wed, 03 Aug 2022 22:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:42:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:42:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:42:42 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:43:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:44:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:46:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad475a95b77752b25dc36bec810d7cc2000f86bc50ea57592b8f988605fc4c6`  
		Last Modified: Wed, 03 Aug 2022 23:06:53 GMT  
		Size: 840.0 KB (839977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76a2f1b035d0df7e2f785a3199e9e86fdeeda1c9f6087f594f2d8a42f0cfb`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 4.1 MB (4087975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acdc23d18c079581f3391d042b65fd7ae55d75333914fd8cdcd0b8acdd6bf10`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3a86db6f1e409fa1d0b2018d788c0539b214c365337f886b86db7e860ee482`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c58cc0918adb02a33e27d7ad4e74c5e0463844a26e99fb60557c3594324b5`  
		Last Modified: Wed, 03 Aug 2022 23:07:34 GMT  
		Size: 239.0 MB (239014439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e568816932729edf86ebafaaeb847af8bda6ade01fb926c6a121f6b825974`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23d14b221e943bfa66059662f80e5ae90e6e1f053ed424ca6b2a40c15876113`  
		Last Modified: Wed, 03 Aug 2022 23:07:57 GMT  
		Size: 54.7 MB (54720659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537d299c243ea0c73b05e8b607aa42ec071f847fbfa98d9ab5463a6594a04406`  
		Last Modified: Wed, 03 Aug 2022 23:07:46 GMT  
		Size: 283.1 KB (283112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d03bb1219b316469e8bd9f059ea35bbe07e5c60596349c1a2f46c2230f51e2`  
		Last Modified: Wed, 03 Aug 2022 23:08:02 GMT  
		Size: 64.7 MB (64743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a017f5b1831aed25ba8fa263279b616191b00173d0d95c4b20ade8026023c6b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.7 MB (411713079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fab7ccc0e2a24d05f9ac4c885d8e7249b5ed274c7312c5703daa04ce0fd0bd2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:58:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 05:58:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 05:58:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 05:58:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 05:58:48 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:00:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:00:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:00:19 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:01:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741c1db167ba98dcc4f0b1dce059664982999c77d7cad916a075711462e7e58d`  
		Last Modified: Fri, 02 Sep 2022 06:26:53 GMT  
		Size: 831.6 KB (831649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4f808c51f1cf44217d8ce4ebca03255e969acca4cf09dff77aee0d3f3a816d`  
		Last Modified: Fri, 02 Sep 2022 06:26:52 GMT  
		Size: 4.3 MB (4265983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19873eb8e73732ae72ef6128c3fa94f987527a5a1439d57eb398f1cb5f4df`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fea62807d8351d36c0b83cdd41872e4d80c976755fa7a501da8e7e7437ad6c`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181336855135b72b6bf5b30d7c1e5beebbdd63f1fe6c933ab551f4a196e800f1`  
		Last Modified: Fri, 02 Sep 2022 06:27:26 GMT  
		Size: 252.5 MB (252504641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284d05b44a890de734833cf20b5313f89437f66ee971f29d55252b3d63572a19`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5912bc4d8ce79891b6639473d128eac65e87986185897f1cc258c457ac8e7ca1`  
		Last Modified: Fri, 02 Sep 2022 06:27:46 GMT  
		Size: 63.1 MB (63088909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767c5618f004c047c357ca236bbcdb7d205c11b960f1d0d7e69a5b074923fe7`  
		Last Modified: Fri, 02 Sep 2022 06:27:37 GMT  
		Size: 284.7 KB (284651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bbb5ba813f9800cb0ccc8cc793a2a5a75588b1ba651ba7a58afd3b8c9f2115`  
		Last Modified: Fri, 02 Sep 2022 06:27:48 GMT  
		Size: 67.0 MB (67001363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:599c778f902462e7b2da29cb5ce052fd683cc30b3e17868a8bd373a6145f2bea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:e894f44bf088cc62986b1aae33d8a8ec96810c746194983ce48d373f28c2eb60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437515827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e77b7e42944fc41a062c94ba1e54f9bc75737c6f1ee3293947939145ea10318`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:20:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 04:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:22:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:22:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:22:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:23:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:23:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc21f3c6df3e09da41edf5cd277be198a0b9ce9de84590bce7c7f8169fe8458`  
		Last Modified: Fri, 02 Sep 2022 05:04:14 GMT  
		Size: 4.9 MB (4873660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601897ffb3e3526f97b7f3ac57655aa3b636d8d501e997e89629b654dd7e8dc`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02d512a7003472763130f30478d4f0c5e440cc42c6e111764af77b527686d5`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a32123d45b8f75cdc98623e79fe3c15f9f2da76e2827622e844770c38afa4`  
		Last Modified: Fri, 02 Sep 2022 05:04:53 GMT  
		Size: 259.6 MB (259559627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abce6b68d4012a79d622c3088e409f52f46a4c2d57e7d45df885e9a566a052c`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0804aad7d24aedc9674dd262573672ffb24e77bd0b94b38774dd4c1344a65`  
		Last Modified: Fri, 02 Sep 2022 05:05:12 GMT  
		Size: 70.3 MB (70259712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4c705dfb136d0edfefa4b6ea486990b27430cb1acb7e7aa9c680225f5845c`  
		Last Modified: Fri, 02 Sep 2022 05:05:02 GMT  
		Size: 284.7 KB (284711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463d8179e60fd0676ccb9cded217236342e7d2d9185a56f2f003efb6d1e597bf`  
		Last Modified: Fri, 02 Sep 2022 05:05:14 GMT  
		Size: 75.0 MB (74995198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:814af5012b36d9eed06c9cac7ad085d72ce7030a89e9b46d7c8f5c6d74d5bc25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (385997135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835e9afd0c76cb727206ffdc1e255cb66a4ad1f768b4a044f6316e2a544b93c0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:38:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:39:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV ROS_DISTRO=melodic
# Wed, 03 Aug 2022 22:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:42:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:42:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:42:42 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:43:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:44:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:46:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad475a95b77752b25dc36bec810d7cc2000f86bc50ea57592b8f988605fc4c6`  
		Last Modified: Wed, 03 Aug 2022 23:06:53 GMT  
		Size: 840.0 KB (839977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76a2f1b035d0df7e2f785a3199e9e86fdeeda1c9f6087f594f2d8a42f0cfb`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 4.1 MB (4087975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acdc23d18c079581f3391d042b65fd7ae55d75333914fd8cdcd0b8acdd6bf10`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3a86db6f1e409fa1d0b2018d788c0539b214c365337f886b86db7e860ee482`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c58cc0918adb02a33e27d7ad4e74c5e0463844a26e99fb60557c3594324b5`  
		Last Modified: Wed, 03 Aug 2022 23:07:34 GMT  
		Size: 239.0 MB (239014439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e568816932729edf86ebafaaeb847af8bda6ade01fb926c6a121f6b825974`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23d14b221e943bfa66059662f80e5ae90e6e1f053ed424ca6b2a40c15876113`  
		Last Modified: Wed, 03 Aug 2022 23:07:57 GMT  
		Size: 54.7 MB (54720659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537d299c243ea0c73b05e8b607aa42ec071f847fbfa98d9ab5463a6594a04406`  
		Last Modified: Wed, 03 Aug 2022 23:07:46 GMT  
		Size: 283.1 KB (283112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d03bb1219b316469e8bd9f059ea35bbe07e5c60596349c1a2f46c2230f51e2`  
		Last Modified: Wed, 03 Aug 2022 23:08:02 GMT  
		Size: 64.7 MB (64743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a017f5b1831aed25ba8fa263279b616191b00173d0d95c4b20ade8026023c6b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.7 MB (411713079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fab7ccc0e2a24d05f9ac4c885d8e7249b5ed274c7312c5703daa04ce0fd0bd2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:58:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 05:58:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 05:58:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 05:58:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 05:58:48 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:00:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:00:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:00:19 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:01:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741c1db167ba98dcc4f0b1dce059664982999c77d7cad916a075711462e7e58d`  
		Last Modified: Fri, 02 Sep 2022 06:26:53 GMT  
		Size: 831.6 KB (831649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4f808c51f1cf44217d8ce4ebca03255e969acca4cf09dff77aee0d3f3a816d`  
		Last Modified: Fri, 02 Sep 2022 06:26:52 GMT  
		Size: 4.3 MB (4265983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19873eb8e73732ae72ef6128c3fa94f987527a5a1439d57eb398f1cb5f4df`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fea62807d8351d36c0b83cdd41872e4d80c976755fa7a501da8e7e7437ad6c`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181336855135b72b6bf5b30d7c1e5beebbdd63f1fe6c933ab551f4a196e800f1`  
		Last Modified: Fri, 02 Sep 2022 06:27:26 GMT  
		Size: 252.5 MB (252504641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284d05b44a890de734833cf20b5313f89437f66ee971f29d55252b3d63572a19`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5912bc4d8ce79891b6639473d128eac65e87986185897f1cc258c457ac8e7ca1`  
		Last Modified: Fri, 02 Sep 2022 06:27:46 GMT  
		Size: 63.1 MB (63088909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767c5618f004c047c357ca236bbcdb7d205c11b960f1d0d7e69a5b074923fe7`  
		Last Modified: Fri, 02 Sep 2022 06:27:37 GMT  
		Size: 284.7 KB (284651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bbb5ba813f9800cb0ccc8cc793a2a5a75588b1ba651ba7a58afd3b8c9f2115`  
		Last Modified: Fri, 02 Sep 2022 06:27:48 GMT  
		Size: 67.0 MB (67001363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:4d62d17a0c771eb97ef20669aeae1c2b363ca29b7f6d6bd79267a187f1dde4eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:9b669165378423e81a191798b5e52aa75e944399105596a518f4b552cd63afbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291976206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:379814066976db125a7e5d64cfcda1c2e9f57f003358ac3442eb1e117bae9d7a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:20:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 04:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:22:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:22:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:22:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc21f3c6df3e09da41edf5cd277be198a0b9ce9de84590bce7c7f8169fe8458`  
		Last Modified: Fri, 02 Sep 2022 05:04:14 GMT  
		Size: 4.9 MB (4873660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601897ffb3e3526f97b7f3ac57655aa3b636d8d501e997e89629b654dd7e8dc`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02d512a7003472763130f30478d4f0c5e440cc42c6e111764af77b527686d5`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a32123d45b8f75cdc98623e79fe3c15f9f2da76e2827622e844770c38afa4`  
		Last Modified: Fri, 02 Sep 2022 05:04:53 GMT  
		Size: 259.6 MB (259559627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abce6b68d4012a79d622c3088e409f52f46a4c2d57e7d45df885e9a566a052c`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:517a5cd34d4f76ea5bd0e123281d4ebaf06483d151b29d5852bcf1199d1462e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266249851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3807b97ce7468b1b2aedbfc07777530bf31cb68749123cd0ee0cf10c2c4f1ae6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:38:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:39:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV ROS_DISTRO=melodic
# Wed, 03 Aug 2022 22:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:42:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:42:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:42:42 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad475a95b77752b25dc36bec810d7cc2000f86bc50ea57592b8f988605fc4c6`  
		Last Modified: Wed, 03 Aug 2022 23:06:53 GMT  
		Size: 840.0 KB (839977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76a2f1b035d0df7e2f785a3199e9e86fdeeda1c9f6087f594f2d8a42f0cfb`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 4.1 MB (4087975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acdc23d18c079581f3391d042b65fd7ae55d75333914fd8cdcd0b8acdd6bf10`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3a86db6f1e409fa1d0b2018d788c0539b214c365337f886b86db7e860ee482`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c58cc0918adb02a33e27d7ad4e74c5e0463844a26e99fb60557c3594324b5`  
		Last Modified: Wed, 03 Aug 2022 23:07:34 GMT  
		Size: 239.0 MB (239014439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e568816932729edf86ebafaaeb847af8bda6ade01fb926c6a121f6b825974`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2edb6d2cfc7df7d81378db7ca5d7c02275aaab95ed9fa0157e17bb5478bcb154
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281338156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2206435ec70b97df1443b70f21da2ec487a4fbce004b232c1c1a9433acad2e4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:58:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 05:58:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 05:58:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 05:58:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 05:58:48 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:00:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:00:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:00:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741c1db167ba98dcc4f0b1dce059664982999c77d7cad916a075711462e7e58d`  
		Last Modified: Fri, 02 Sep 2022 06:26:53 GMT  
		Size: 831.6 KB (831649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4f808c51f1cf44217d8ce4ebca03255e969acca4cf09dff77aee0d3f3a816d`  
		Last Modified: Fri, 02 Sep 2022 06:26:52 GMT  
		Size: 4.3 MB (4265983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19873eb8e73732ae72ef6128c3fa94f987527a5a1439d57eb398f1cb5f4df`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fea62807d8351d36c0b83cdd41872e4d80c976755fa7a501da8e7e7437ad6c`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181336855135b72b6bf5b30d7c1e5beebbdd63f1fe6c933ab551f4a196e800f1`  
		Last Modified: Fri, 02 Sep 2022 06:27:26 GMT  
		Size: 252.5 MB (252504641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284d05b44a890de734833cf20b5313f89437f66ee971f29d55252b3d63572a19`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:4d62d17a0c771eb97ef20669aeae1c2b363ca29b7f6d6bd79267a187f1dde4eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:9b669165378423e81a191798b5e52aa75e944399105596a518f4b552cd63afbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291976206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:379814066976db125a7e5d64cfcda1c2e9f57f003358ac3442eb1e117bae9d7a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:20:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 04:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:22:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:22:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:22:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc21f3c6df3e09da41edf5cd277be198a0b9ce9de84590bce7c7f8169fe8458`  
		Last Modified: Fri, 02 Sep 2022 05:04:14 GMT  
		Size: 4.9 MB (4873660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601897ffb3e3526f97b7f3ac57655aa3b636d8d501e997e89629b654dd7e8dc`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02d512a7003472763130f30478d4f0c5e440cc42c6e111764af77b527686d5`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a32123d45b8f75cdc98623e79fe3c15f9f2da76e2827622e844770c38afa4`  
		Last Modified: Fri, 02 Sep 2022 05:04:53 GMT  
		Size: 259.6 MB (259559627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abce6b68d4012a79d622c3088e409f52f46a4c2d57e7d45df885e9a566a052c`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:517a5cd34d4f76ea5bd0e123281d4ebaf06483d151b29d5852bcf1199d1462e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266249851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3807b97ce7468b1b2aedbfc07777530bf31cb68749123cd0ee0cf10c2c4f1ae6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:38:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:39:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV ROS_DISTRO=melodic
# Wed, 03 Aug 2022 22:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:42:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:42:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:42:42 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad475a95b77752b25dc36bec810d7cc2000f86bc50ea57592b8f988605fc4c6`  
		Last Modified: Wed, 03 Aug 2022 23:06:53 GMT  
		Size: 840.0 KB (839977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76a2f1b035d0df7e2f785a3199e9e86fdeeda1c9f6087f594f2d8a42f0cfb`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 4.1 MB (4087975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acdc23d18c079581f3391d042b65fd7ae55d75333914fd8cdcd0b8acdd6bf10`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3a86db6f1e409fa1d0b2018d788c0539b214c365337f886b86db7e860ee482`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c58cc0918adb02a33e27d7ad4e74c5e0463844a26e99fb60557c3594324b5`  
		Last Modified: Wed, 03 Aug 2022 23:07:34 GMT  
		Size: 239.0 MB (239014439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e568816932729edf86ebafaaeb847af8bda6ade01fb926c6a121f6b825974`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2edb6d2cfc7df7d81378db7ca5d7c02275aaab95ed9fa0157e17bb5478bcb154
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281338156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2206435ec70b97df1443b70f21da2ec487a4fbce004b232c1c1a9433acad2e4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:58:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 05:58:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 05:58:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 05:58:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 05:58:48 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:00:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:00:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:00:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741c1db167ba98dcc4f0b1dce059664982999c77d7cad916a075711462e7e58d`  
		Last Modified: Fri, 02 Sep 2022 06:26:53 GMT  
		Size: 831.6 KB (831649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4f808c51f1cf44217d8ce4ebca03255e969acca4cf09dff77aee0d3f3a816d`  
		Last Modified: Fri, 02 Sep 2022 06:26:52 GMT  
		Size: 4.3 MB (4265983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19873eb8e73732ae72ef6128c3fa94f987527a5a1439d57eb398f1cb5f4df`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fea62807d8351d36c0b83cdd41872e4d80c976755fa7a501da8e7e7437ad6c`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181336855135b72b6bf5b30d7c1e5beebbdd63f1fe6c933ab551f4a196e800f1`  
		Last Modified: Fri, 02 Sep 2022 06:27:26 GMT  
		Size: 252.5 MB (252504641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284d05b44a890de734833cf20b5313f89437f66ee971f29d55252b3d63572a19`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:61be0eb69faf71dbe5dc943dbc06c569ecb4d64db02dc2468b9a85e1d7b3657c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:a3668b236d93abbfedcf72a51abc193842193459fdb8aac6b642ed95441a6cbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343151353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b356ccf86aa9679666fabf6c6ce440b45f40baf7f272adee0eca54f31d4d6b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:30:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:30:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 04:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:32:46 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:33:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:33:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e933af47665655d97d902ecb6d264063a041b2c12dfcbaf849a05672cafc9044`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1916d550484243d392ddc6fdca4ba34710bd3305a578bf9d241f2ad6d944c099`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d152bd7bb3b1335dd05a53828858de8ceab15c85e96fdc0181b2e38f72323b8`  
		Last Modified: Fri, 02 Sep 2022 05:07:05 GMT  
		Size: 177.0 MB (176996015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edc8aa6732f94d22820aa0f96400c620b51e015fa6a940c03e9b579f0de306f`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38aa1dd8b74095a973aa1b1fe9d7495fcbf895f954b66adbff905119d10103`  
		Last Modified: Fri, 02 Sep 2022 05:07:22 GMT  
		Size: 50.9 MB (50940098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5cec93c265dc40fb6eb4790e71c25ac877e2addb6eddf96377e4336554651e`  
		Last Modified: Fri, 02 Sep 2022 05:07:14 GMT  
		Size: 325.7 KB (325719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca383d78ab41bd8631ac0ef8afce8de1b461c6b95a74094926636a7d8ff9c57`  
		Last Modified: Fri, 02 Sep 2022 05:07:26 GMT  
		Size: 79.6 MB (79603671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:dc89df4c67ffb8e35dcb232a71956399e39b3575cfa1e8389e74e1d5a0782638
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289240180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c5a83264b759495b4caae5a5c49c6f2dbf31890cf1b28ffedbd7d55f94c0279`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:53:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:53:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 Aug 2022 22:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:55:11 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:56:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:56:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:57:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d345e3aeca1c4dd8930e961af9d46712aa474a7ce53acba4f54b4ff3b113a84`  
		Last Modified: Wed, 03 Aug 2022 23:09:30 GMT  
		Size: 1.2 MB (1181992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf40d14b8b7f81b4f192b1708fbdb0a57c3626f5b72be630a041c1f634f266`  
		Last Modified: Wed, 03 Aug 2022 23:09:28 GMT  
		Size: 4.7 MB (4676289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3223d85d87ee35ea3ab4535feef031631e281f3c617de4cdc218c4983c9b6f`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5bf7f51f5d7e24eec5395780a42aebd0c726cb0466dd5e0b2c492c6d0c84b3`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c66f511399e2f2993ed8fd014bb457c6d6a9483ae665aea0e9eb01fb0a54b4`  
		Last Modified: Wed, 03 Aug 2022 23:10:06 GMT  
		Size: 157.5 MB (157479986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa138f7b3214bda7dc2ae9534dff610b8c2a41d8de8dfb7c8a69ab5eba596887`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956f29112fb883f35fde1c1d67fc064ab659310ef5bc2f894fd7fabc7cb1b53`  
		Last Modified: Wed, 03 Aug 2022 23:10:25 GMT  
		Size: 40.5 MB (40505939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b4fa88c4ff97cf49d78a40c699333d1182e8a7a0cdb62a65b76e6d6ba39208`  
		Last Modified: Wed, 03 Aug 2022 23:10:18 GMT  
		Size: 323.5 KB (323517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f054c04c983a4aa345e62e3a2df78c234e061aab4b29b964612f3ff52473c`  
		Last Modified: Wed, 03 Aug 2022 23:10:30 GMT  
		Size: 60.5 MB (60480770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:986aa4972599a27a24d5fef240d4bbb3baa85e68212932eed5e984b1f6683628
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.2 MB (322166779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a94e2896051c439f0a9a4bb21c10b79700eb74d879d67d9ca855a477f7f94ca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:04:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:04:14 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:04:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:04:16 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 06:05:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:05:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:05:17 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:05:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14c9b385a2e2a1aaf2e3e0e96bb0ab19b0ae4bd1ba4df6e04bd247b310d5c2`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb230fc3fead8135d54463448100608dff8db563117ce648ff536d58028e043`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a441fbb85ca0fc9351965d962c26631f0c0fdd0a80a5de4349d0a2fe39cdad`  
		Last Modified: Fri, 02 Sep 2022 06:29:39 GMT  
		Size: 171.4 MB (171414641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cbf101495077c64a07b49123584c92c50e4eedbf37c6fe039a5c96c1a45fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351e164058f5f6b26f33ca86e472799ca95df650c8044c529338423424b38ea4`  
		Last Modified: Fri, 02 Sep 2022 06:29:56 GMT  
		Size: 45.0 MB (44988847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fcd9c3e7122e87ef29f417d198e443a1892d621f1fe005f9cbf9072b5d3b9`  
		Last Modified: Fri, 02 Sep 2022 06:29:50 GMT  
		Size: 325.7 KB (325657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65599a689993fa62149f8b2028498730ddd14125298b858124751013f37cdba4`  
		Last Modified: Fri, 02 Sep 2022 06:30:00 GMT  
		Size: 71.8 MB (71754873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:123f89ea553f7e6afe92d67ebc38ddd5660cca7c851c0cfcbd4406e856ace1cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:92a9a61a2bbca7538207c06e045a7a5e686090a54831516ffa488a491aa1c4ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.1 MB (835120913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:536572ffb5a95c08ca27649d9209f61d60a1f36a15acdb55bfb3efe0650d171d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:30:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:30:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 04:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:32:46 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:33:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:33:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:41:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e933af47665655d97d902ecb6d264063a041b2c12dfcbaf849a05672cafc9044`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1916d550484243d392ddc6fdca4ba34710bd3305a578bf9d241f2ad6d944c099`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d152bd7bb3b1335dd05a53828858de8ceab15c85e96fdc0181b2e38f72323b8`  
		Last Modified: Fri, 02 Sep 2022 05:07:05 GMT  
		Size: 177.0 MB (176996015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edc8aa6732f94d22820aa0f96400c620b51e015fa6a940c03e9b579f0de306f`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38aa1dd8b74095a973aa1b1fe9d7495fcbf895f954b66adbff905119d10103`  
		Last Modified: Fri, 02 Sep 2022 05:07:22 GMT  
		Size: 50.9 MB (50940098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5cec93c265dc40fb6eb4790e71c25ac877e2addb6eddf96377e4336554651e`  
		Last Modified: Fri, 02 Sep 2022 05:07:14 GMT  
		Size: 325.7 KB (325719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca383d78ab41bd8631ac0ef8afce8de1b461c6b95a74094926636a7d8ff9c57`  
		Last Modified: Fri, 02 Sep 2022 05:07:26 GMT  
		Size: 79.6 MB (79603671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec642114a0fb290bf0ad8660843fcd6f3653247c1aedf51d36e3b9afa30a2a4`  
		Last Modified: Fri, 02 Sep 2022 05:09:04 GMT  
		Size: 492.0 MB (491969560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:1ecaf8e232748957ac86a63221733c7593239f1c1f6e1f806933b288509f4c99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.1 MB (726125169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea4e067cd70525d9e125993cb33ef7c1d7b685b94254c7e68f9bd1e3f34d89f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:53:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:53:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 Aug 2022 22:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:55:11 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:56:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:56:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:57:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 23:05:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d345e3aeca1c4dd8930e961af9d46712aa474a7ce53acba4f54b4ff3b113a84`  
		Last Modified: Wed, 03 Aug 2022 23:09:30 GMT  
		Size: 1.2 MB (1181992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf40d14b8b7f81b4f192b1708fbdb0a57c3626f5b72be630a041c1f634f266`  
		Last Modified: Wed, 03 Aug 2022 23:09:28 GMT  
		Size: 4.7 MB (4676289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3223d85d87ee35ea3ab4535feef031631e281f3c617de4cdc218c4983c9b6f`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5bf7f51f5d7e24eec5395780a42aebd0c726cb0466dd5e0b2c492c6d0c84b3`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c66f511399e2f2993ed8fd014bb457c6d6a9483ae665aea0e9eb01fb0a54b4`  
		Last Modified: Wed, 03 Aug 2022 23:10:06 GMT  
		Size: 157.5 MB (157479986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa138f7b3214bda7dc2ae9534dff610b8c2a41d8de8dfb7c8a69ab5eba596887`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956f29112fb883f35fde1c1d67fc064ab659310ef5bc2f894fd7fabc7cb1b53`  
		Last Modified: Wed, 03 Aug 2022 23:10:25 GMT  
		Size: 40.5 MB (40505939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b4fa88c4ff97cf49d78a40c699333d1182e8a7a0cdb62a65b76e6d6ba39208`  
		Last Modified: Wed, 03 Aug 2022 23:10:18 GMT  
		Size: 323.5 KB (323517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f054c04c983a4aa345e62e3a2df78c234e061aab4b29b964612f3ff52473c`  
		Last Modified: Wed, 03 Aug 2022 23:10:30 GMT  
		Size: 60.5 MB (60480770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802d1642a23d0013e97d3851823d3d1d2bb88f1ffa90be40d87e65a988ea2a9a`  
		Last Modified: Wed, 03 Aug 2022 23:12:10 GMT  
		Size: 436.9 MB (436884989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3a23640f0502b7ce1a14a1ce2fb0ca734787b52dcce2179726207994db47b046
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.7 MB (784702327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18c06d8aac74677fc646cd57ac4f15d1436576e7f99961067ca2b0b864f39b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:04:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:04:14 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:04:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:04:16 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 06:05:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:05:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:05:17 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:05:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:08:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14c9b385a2e2a1aaf2e3e0e96bb0ab19b0ae4bd1ba4df6e04bd247b310d5c2`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb230fc3fead8135d54463448100608dff8db563117ce648ff536d58028e043`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a441fbb85ca0fc9351965d962c26631f0c0fdd0a80a5de4349d0a2fe39cdad`  
		Last Modified: Fri, 02 Sep 2022 06:29:39 GMT  
		Size: 171.4 MB (171414641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cbf101495077c64a07b49123584c92c50e4eedbf37c6fe039a5c96c1a45fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351e164058f5f6b26f33ca86e472799ca95df650c8044c529338423424b38ea4`  
		Last Modified: Fri, 02 Sep 2022 06:29:56 GMT  
		Size: 45.0 MB (44988847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fcd9c3e7122e87ef29f417d198e443a1892d621f1fe005f9cbf9072b5d3b9`  
		Last Modified: Fri, 02 Sep 2022 06:29:50 GMT  
		Size: 325.7 KB (325657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65599a689993fa62149f8b2028498730ddd14125298b858124751013f37cdba4`  
		Last Modified: Fri, 02 Sep 2022 06:30:00 GMT  
		Size: 71.8 MB (71754873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b396b7a3bfa745d7c175ab81e6fefdc70dca400b25af857523fb7351d8252a`  
		Last Modified: Fri, 02 Sep 2022 06:31:35 GMT  
		Size: 462.5 MB (462535548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:afd8ccf1909bb6cface65b28097fb1099c41d2543775444a5635f0ce4a51a4c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:97cbd624fa29bbb7b96ff26b8a56d64177ad5f70daac01c05374b03b3ad5f58f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.4 MB (951401294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9934f52c622a20cac28951203d192a341dc6bf5ca1390702b2c22c818448c29c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:10:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:10:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 23 Aug 2022 11:10:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 23 Aug 2022 11:10:45 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:10:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 23 Aug 2022 11:10:45 GMT
ENV ROS_DISTRO=noetic
# Tue, 23 Aug 2022 11:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:11:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 23 Aug 2022 11:11:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 23 Aug 2022 11:11:49 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:12:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:12:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 23 Aug 2022 11:12:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:15:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd91dd5198cc577c5556c7c5c335e0ea5701168d8c2ded40b83bc24be1434e47`  
		Last Modified: Tue, 23 Aug 2022 11:17:01 GMT  
		Size: 10.9 MB (10893537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385a586942561cc66fbd30195e87e96f1b39c6350f5ecd935dab71ef933e1bca`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3402e2486e536bf44469c2ce583b71937b7cbff76618e426dd63ed6b7dfe0cc5`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c2873f607da18c9f2623d952abd04118f7d0778f3599821850f1919eafc164`  
		Last Modified: Tue, 23 Aug 2022 11:17:33 GMT  
		Size: 239.2 MB (239186445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d17c4e21a19faebaa430ee698b7cb100d2e778f790784743bdc70da09436a41`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7245c288a141189c997601cc51df3c78474637e0eaaf193d9ff374f766648200`  
		Last Modified: Tue, 23 Aug 2022 11:17:55 GMT  
		Size: 86.6 MB (86569601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3ced040e753b4661b1383d3e5ed1eeb33533efbd4f2e5f6a9b9bd9fe4ca902`  
		Last Modified: Tue, 23 Aug 2022 11:17:42 GMT  
		Size: 319.4 KB (319418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0737249fff82a9ae2caa5144493e9d2fcf088027709fe87ee86f79726d1ae7fd`  
		Last Modified: Tue, 23 Aug 2022 11:17:52 GMT  
		Size: 76.0 MB (75976837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c173bb5a05c73c32307f7778ed744e43ef32a24abee76dcb9bed1c4f60562ea8`  
		Last Modified: Tue, 23 Aug 2022 11:19:25 GMT  
		Size: 488.0 MB (488012770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e9b3c1ce9dd2ed273198e7f47fdb4d01c140daec8afd44b1805c27bc38517c8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **867.7 MB (867666349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b035c99685d1be45df5e6768994c6926d03c9fdd19fe3087a1939619cc3e37c7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:18:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:18:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 23 Aug 2022 11:18:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 23 Aug 2022 11:18:57 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:18:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 23 Aug 2022 11:18:59 GMT
ENV ROS_DISTRO=noetic
# Tue, 23 Aug 2022 11:20:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:20:21 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 23 Aug 2022 11:20:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 23 Aug 2022 11:20:24 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:20:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:21:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 23 Aug 2022 11:21:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:25:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc5b8055a31acea8cf6858fb7058f9828cf856d7ca15408120754ef8e582e8b`  
		Last Modified: Tue, 23 Aug 2022 11:28:27 GMT  
		Size: 10.7 MB (10689268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3e051ec8c4f50bc9206c4036995d09b8baf8a208b4aae22a2deeb7a246a5f0`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3dbf6ff20222664e13d9f371430b5b76a850b135d2cd6876f8239ebf2cf26`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6b972b9d90022d411ed9be6a75b03629caf11045e410b85bf532d9b574973f`  
		Last Modified: Tue, 23 Aug 2022 11:28:56 GMT  
		Size: 184.4 MB (184373802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bebe4a80f1367e9d727dcccb4679e5590d80dd2a8d0b00100b06f21a5e20bc0`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97614d076b0337a5bf133b8ea0f63b2a64fd4907f6242d84556146524077b032`  
		Last Modified: Tue, 23 Aug 2022 11:29:14 GMT  
		Size: 84.4 MB (84370471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a86f0adf69a256428f0eb97e4d0a6ebb4c333ee833fa76731d8b0526eb88d5d`  
		Last Modified: Tue, 23 Aug 2022 11:29:04 GMT  
		Size: 319.4 KB (319361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a577fe3ce43ebe0d1f7719dc2286b8f2cead9743255d3f8f71caebb62632e29e`  
		Last Modified: Tue, 23 Aug 2022 11:29:13 GMT  
		Size: 73.9 MB (73865202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4ba63562a66f6afe3ebe16c242c26e8178e665b54612c145c479b1e9748026`  
		Last Modified: Tue, 23 Aug 2022 11:30:41 GMT  
		Size: 464.8 MB (464817808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:123f89ea553f7e6afe92d67ebc38ddd5660cca7c851c0cfcbd4406e856ace1cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:92a9a61a2bbca7538207c06e045a7a5e686090a54831516ffa488a491aa1c4ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.1 MB (835120913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:536572ffb5a95c08ca27649d9209f61d60a1f36a15acdb55bfb3efe0650d171d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:30:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:30:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 04:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:32:46 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:33:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:33:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:41:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e933af47665655d97d902ecb6d264063a041b2c12dfcbaf849a05672cafc9044`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1916d550484243d392ddc6fdca4ba34710bd3305a578bf9d241f2ad6d944c099`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d152bd7bb3b1335dd05a53828858de8ceab15c85e96fdc0181b2e38f72323b8`  
		Last Modified: Fri, 02 Sep 2022 05:07:05 GMT  
		Size: 177.0 MB (176996015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edc8aa6732f94d22820aa0f96400c620b51e015fa6a940c03e9b579f0de306f`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38aa1dd8b74095a973aa1b1fe9d7495fcbf895f954b66adbff905119d10103`  
		Last Modified: Fri, 02 Sep 2022 05:07:22 GMT  
		Size: 50.9 MB (50940098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5cec93c265dc40fb6eb4790e71c25ac877e2addb6eddf96377e4336554651e`  
		Last Modified: Fri, 02 Sep 2022 05:07:14 GMT  
		Size: 325.7 KB (325719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca383d78ab41bd8631ac0ef8afce8de1b461c6b95a74094926636a7d8ff9c57`  
		Last Modified: Fri, 02 Sep 2022 05:07:26 GMT  
		Size: 79.6 MB (79603671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec642114a0fb290bf0ad8660843fcd6f3653247c1aedf51d36e3b9afa30a2a4`  
		Last Modified: Fri, 02 Sep 2022 05:09:04 GMT  
		Size: 492.0 MB (491969560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:1ecaf8e232748957ac86a63221733c7593239f1c1f6e1f806933b288509f4c99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.1 MB (726125169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea4e067cd70525d9e125993cb33ef7c1d7b685b94254c7e68f9bd1e3f34d89f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:53:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:53:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 Aug 2022 22:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:55:11 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:56:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:56:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:57:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 23:05:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d345e3aeca1c4dd8930e961af9d46712aa474a7ce53acba4f54b4ff3b113a84`  
		Last Modified: Wed, 03 Aug 2022 23:09:30 GMT  
		Size: 1.2 MB (1181992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf40d14b8b7f81b4f192b1708fbdb0a57c3626f5b72be630a041c1f634f266`  
		Last Modified: Wed, 03 Aug 2022 23:09:28 GMT  
		Size: 4.7 MB (4676289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3223d85d87ee35ea3ab4535feef031631e281f3c617de4cdc218c4983c9b6f`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5bf7f51f5d7e24eec5395780a42aebd0c726cb0466dd5e0b2c492c6d0c84b3`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c66f511399e2f2993ed8fd014bb457c6d6a9483ae665aea0e9eb01fb0a54b4`  
		Last Modified: Wed, 03 Aug 2022 23:10:06 GMT  
		Size: 157.5 MB (157479986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa138f7b3214bda7dc2ae9534dff610b8c2a41d8de8dfb7c8a69ab5eba596887`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956f29112fb883f35fde1c1d67fc064ab659310ef5bc2f894fd7fabc7cb1b53`  
		Last Modified: Wed, 03 Aug 2022 23:10:25 GMT  
		Size: 40.5 MB (40505939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b4fa88c4ff97cf49d78a40c699333d1182e8a7a0cdb62a65b76e6d6ba39208`  
		Last Modified: Wed, 03 Aug 2022 23:10:18 GMT  
		Size: 323.5 KB (323517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f054c04c983a4aa345e62e3a2df78c234e061aab4b29b964612f3ff52473c`  
		Last Modified: Wed, 03 Aug 2022 23:10:30 GMT  
		Size: 60.5 MB (60480770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802d1642a23d0013e97d3851823d3d1d2bb88f1ffa90be40d87e65a988ea2a9a`  
		Last Modified: Wed, 03 Aug 2022 23:12:10 GMT  
		Size: 436.9 MB (436884989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3a23640f0502b7ce1a14a1ce2fb0ca734787b52dcce2179726207994db47b046
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.7 MB (784702327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18c06d8aac74677fc646cd57ac4f15d1436576e7f99961067ca2b0b864f39b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:04:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:04:14 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:04:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:04:16 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 06:05:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:05:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:05:17 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:05:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:08:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14c9b385a2e2a1aaf2e3e0e96bb0ab19b0ae4bd1ba4df6e04bd247b310d5c2`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb230fc3fead8135d54463448100608dff8db563117ce648ff536d58028e043`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a441fbb85ca0fc9351965d962c26631f0c0fdd0a80a5de4349d0a2fe39cdad`  
		Last Modified: Fri, 02 Sep 2022 06:29:39 GMT  
		Size: 171.4 MB (171414641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cbf101495077c64a07b49123584c92c50e4eedbf37c6fe039a5c96c1a45fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351e164058f5f6b26f33ca86e472799ca95df650c8044c529338423424b38ea4`  
		Last Modified: Fri, 02 Sep 2022 06:29:56 GMT  
		Size: 45.0 MB (44988847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fcd9c3e7122e87ef29f417d198e443a1892d621f1fe005f9cbf9072b5d3b9`  
		Last Modified: Fri, 02 Sep 2022 06:29:50 GMT  
		Size: 325.7 KB (325657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65599a689993fa62149f8b2028498730ddd14125298b858124751013f37cdba4`  
		Last Modified: Fri, 02 Sep 2022 06:30:00 GMT  
		Size: 71.8 MB (71754873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b396b7a3bfa745d7c175ab81e6fefdc70dca400b25af857523fb7351d8252a`  
		Last Modified: Fri, 02 Sep 2022 06:31:35 GMT  
		Size: 462.5 MB (462535548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:ed00f1c0e6c2f074587303dc200ef98cf93e6808b96bccd791a44263bf7f9701
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:669c18fe44b20f61149f51771c40553202d44d46ec86a74600eb1e7431000bd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359011850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d33234d459a19d3a4bbe5ae8699e82192f9a9f50eb461757a4dbee1be52429ab`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:30:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:30:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 04:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:32:46 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:33:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:33:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:35:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e933af47665655d97d902ecb6d264063a041b2c12dfcbaf849a05672cafc9044`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1916d550484243d392ddc6fdca4ba34710bd3305a578bf9d241f2ad6d944c099`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d152bd7bb3b1335dd05a53828858de8ceab15c85e96fdc0181b2e38f72323b8`  
		Last Modified: Fri, 02 Sep 2022 05:07:05 GMT  
		Size: 177.0 MB (176996015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edc8aa6732f94d22820aa0f96400c620b51e015fa6a940c03e9b579f0de306f`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38aa1dd8b74095a973aa1b1fe9d7495fcbf895f954b66adbff905119d10103`  
		Last Modified: Fri, 02 Sep 2022 05:07:22 GMT  
		Size: 50.9 MB (50940098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5cec93c265dc40fb6eb4790e71c25ac877e2addb6eddf96377e4336554651e`  
		Last Modified: Fri, 02 Sep 2022 05:07:14 GMT  
		Size: 325.7 KB (325719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca383d78ab41bd8631ac0ef8afce8de1b461c6b95a74094926636a7d8ff9c57`  
		Last Modified: Fri, 02 Sep 2022 05:07:26 GMT  
		Size: 79.6 MB (79603671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0626adf2cf42b6dad9a292e7d21a2c1206ef600a05e321e33d906aee3aa891cf`  
		Last Modified: Fri, 02 Sep 2022 05:07:41 GMT  
		Size: 15.9 MB (15860497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:d047da019eed0ae7d07f4483f4f6dca6ddb5aab8834d63bcee903ecff0073bc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303305191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6388f41565b185241b75e7dc046ca9f15971530341e6c9d8aabf93ee93145659`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:53:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:53:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 Aug 2022 22:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:55:11 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:56:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:56:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:57:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d345e3aeca1c4dd8930e961af9d46712aa474a7ce53acba4f54b4ff3b113a84`  
		Last Modified: Wed, 03 Aug 2022 23:09:30 GMT  
		Size: 1.2 MB (1181992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf40d14b8b7f81b4f192b1708fbdb0a57c3626f5b72be630a041c1f634f266`  
		Last Modified: Wed, 03 Aug 2022 23:09:28 GMT  
		Size: 4.7 MB (4676289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3223d85d87ee35ea3ab4535feef031631e281f3c617de4cdc218c4983c9b6f`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5bf7f51f5d7e24eec5395780a42aebd0c726cb0466dd5e0b2c492c6d0c84b3`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c66f511399e2f2993ed8fd014bb457c6d6a9483ae665aea0e9eb01fb0a54b4`  
		Last Modified: Wed, 03 Aug 2022 23:10:06 GMT  
		Size: 157.5 MB (157479986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa138f7b3214bda7dc2ae9534dff610b8c2a41d8de8dfb7c8a69ab5eba596887`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956f29112fb883f35fde1c1d67fc064ab659310ef5bc2f894fd7fabc7cb1b53`  
		Last Modified: Wed, 03 Aug 2022 23:10:25 GMT  
		Size: 40.5 MB (40505939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b4fa88c4ff97cf49d78a40c699333d1182e8a7a0cdb62a65b76e6d6ba39208`  
		Last Modified: Wed, 03 Aug 2022 23:10:18 GMT  
		Size: 323.5 KB (323517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f054c04c983a4aa345e62e3a2df78c234e061aab4b29b964612f3ff52473c`  
		Last Modified: Wed, 03 Aug 2022 23:10:30 GMT  
		Size: 60.5 MB (60480770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714bead958c0893197e557905b695ea7e2e9f9a621b7b00a14bc25d104d1e307`  
		Last Modified: Wed, 03 Aug 2022 23:10:48 GMT  
		Size: 14.1 MB (14065011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7115e6f5880c00e61f39bffe3417db74ca7d9d2c08fbf76d3693a0dd38cb54e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.6 MB (337615813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f84482c105f51b121ecf76fca749f92f777fd4925b639fa1eb780db6014cc9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:04:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:04:14 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:04:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:04:16 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 06:05:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:05:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:05:17 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:05:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:06:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14c9b385a2e2a1aaf2e3e0e96bb0ab19b0ae4bd1ba4df6e04bd247b310d5c2`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb230fc3fead8135d54463448100608dff8db563117ce648ff536d58028e043`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a441fbb85ca0fc9351965d962c26631f0c0fdd0a80a5de4349d0a2fe39cdad`  
		Last Modified: Fri, 02 Sep 2022 06:29:39 GMT  
		Size: 171.4 MB (171414641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cbf101495077c64a07b49123584c92c50e4eedbf37c6fe039a5c96c1a45fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351e164058f5f6b26f33ca86e472799ca95df650c8044c529338423424b38ea4`  
		Last Modified: Fri, 02 Sep 2022 06:29:56 GMT  
		Size: 45.0 MB (44988847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fcd9c3e7122e87ef29f417d198e443a1892d621f1fe005f9cbf9072b5d3b9`  
		Last Modified: Fri, 02 Sep 2022 06:29:50 GMT  
		Size: 325.7 KB (325657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65599a689993fa62149f8b2028498730ddd14125298b858124751013f37cdba4`  
		Last Modified: Fri, 02 Sep 2022 06:30:00 GMT  
		Size: 71.8 MB (71754873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18121c479bd23f9bed87b73dab18f777737e353710d6bc6fbea8ba53d4921f2e`  
		Last Modified: Fri, 02 Sep 2022 06:30:17 GMT  
		Size: 15.4 MB (15449034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:1d95973b3645afe08b3007d6b8f0111f7d0e2517dba58181323adf9cb45b1558
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:7956e83e77838e68d1587d3ef479c4cd0a188a4fb62c0e161ef14dc872c07c4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.8 MB (484837064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4760c478875c153123f1ae6782861cbb93a39312ce3b453fe25f12676ed92b4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:10:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:10:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 23 Aug 2022 11:10:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 23 Aug 2022 11:10:45 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:10:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 23 Aug 2022 11:10:45 GMT
ENV ROS_DISTRO=noetic
# Tue, 23 Aug 2022 11:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:11:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 23 Aug 2022 11:11:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 23 Aug 2022 11:11:49 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:12:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:12:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 23 Aug 2022 11:12:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:13:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd91dd5198cc577c5556c7c5c335e0ea5701168d8c2ded40b83bc24be1434e47`  
		Last Modified: Tue, 23 Aug 2022 11:17:01 GMT  
		Size: 10.9 MB (10893537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385a586942561cc66fbd30195e87e96f1b39c6350f5ecd935dab71ef933e1bca`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3402e2486e536bf44469c2ce583b71937b7cbff76618e426dd63ed6b7dfe0cc5`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c2873f607da18c9f2623d952abd04118f7d0778f3599821850f1919eafc164`  
		Last Modified: Tue, 23 Aug 2022 11:17:33 GMT  
		Size: 239.2 MB (239186445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d17c4e21a19faebaa430ee698b7cb100d2e778f790784743bdc70da09436a41`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7245c288a141189c997601cc51df3c78474637e0eaaf193d9ff374f766648200`  
		Last Modified: Tue, 23 Aug 2022 11:17:55 GMT  
		Size: 86.6 MB (86569601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3ced040e753b4661b1383d3e5ed1eeb33533efbd4f2e5f6a9b9bd9fe4ca902`  
		Last Modified: Tue, 23 Aug 2022 11:17:42 GMT  
		Size: 319.4 KB (319418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0737249fff82a9ae2caa5144493e9d2fcf088027709fe87ee86f79726d1ae7fd`  
		Last Modified: Tue, 23 Aug 2022 11:17:52 GMT  
		Size: 76.0 MB (75976837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a2c6bdee82b6f5b3558161c7d266c7601397cdce5456823e53e9f9d9841814`  
		Last Modified: Tue, 23 Aug 2022 11:18:04 GMT  
		Size: 21.4 MB (21448540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b1aac759bc9e577f5db35de92baf881e54af98a96df414359245b20d7c1d676c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.0 MB (423955218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc754b36f0fcd0f2a9690a792420df38b5c3060eb927369b9abc9df0e6c93b89`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:18:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:18:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 23 Aug 2022 11:18:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 23 Aug 2022 11:18:57 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:18:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 23 Aug 2022 11:18:59 GMT
ENV ROS_DISTRO=noetic
# Tue, 23 Aug 2022 11:20:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:20:21 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 23 Aug 2022 11:20:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 23 Aug 2022 11:20:24 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:20:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:21:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 23 Aug 2022 11:21:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:22:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc5b8055a31acea8cf6858fb7058f9828cf856d7ca15408120754ef8e582e8b`  
		Last Modified: Tue, 23 Aug 2022 11:28:27 GMT  
		Size: 10.7 MB (10689268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3e051ec8c4f50bc9206c4036995d09b8baf8a208b4aae22a2deeb7a246a5f0`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3dbf6ff20222664e13d9f371430b5b76a850b135d2cd6876f8239ebf2cf26`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6b972b9d90022d411ed9be6a75b03629caf11045e410b85bf532d9b574973f`  
		Last Modified: Tue, 23 Aug 2022 11:28:56 GMT  
		Size: 184.4 MB (184373802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bebe4a80f1367e9d727dcccb4679e5590d80dd2a8d0b00100b06f21a5e20bc0`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97614d076b0337a5bf133b8ea0f63b2a64fd4907f6242d84556146524077b032`  
		Last Modified: Tue, 23 Aug 2022 11:29:14 GMT  
		Size: 84.4 MB (84370471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a86f0adf69a256428f0eb97e4d0a6ebb4c333ee833fa76731d8b0526eb88d5d`  
		Last Modified: Tue, 23 Aug 2022 11:29:04 GMT  
		Size: 319.4 KB (319361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a577fe3ce43ebe0d1f7719dc2286b8f2cead9743255d3f8f71caebb62632e29e`  
		Last Modified: Tue, 23 Aug 2022 11:29:13 GMT  
		Size: 73.9 MB (73865202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d546ca9c14f09149deff55dacc44fd6006a70d77da691d40d69b36372a3c7f86`  
		Last Modified: Tue, 23 Aug 2022 11:29:25 GMT  
		Size: 21.1 MB (21106677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:ed00f1c0e6c2f074587303dc200ef98cf93e6808b96bccd791a44263bf7f9701
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:669c18fe44b20f61149f51771c40553202d44d46ec86a74600eb1e7431000bd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359011850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d33234d459a19d3a4bbe5ae8699e82192f9a9f50eb461757a4dbee1be52429ab`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:30:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:30:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 04:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:32:46 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:33:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:33:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:35:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e933af47665655d97d902ecb6d264063a041b2c12dfcbaf849a05672cafc9044`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1916d550484243d392ddc6fdca4ba34710bd3305a578bf9d241f2ad6d944c099`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d152bd7bb3b1335dd05a53828858de8ceab15c85e96fdc0181b2e38f72323b8`  
		Last Modified: Fri, 02 Sep 2022 05:07:05 GMT  
		Size: 177.0 MB (176996015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edc8aa6732f94d22820aa0f96400c620b51e015fa6a940c03e9b579f0de306f`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38aa1dd8b74095a973aa1b1fe9d7495fcbf895f954b66adbff905119d10103`  
		Last Modified: Fri, 02 Sep 2022 05:07:22 GMT  
		Size: 50.9 MB (50940098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5cec93c265dc40fb6eb4790e71c25ac877e2addb6eddf96377e4336554651e`  
		Last Modified: Fri, 02 Sep 2022 05:07:14 GMT  
		Size: 325.7 KB (325719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca383d78ab41bd8631ac0ef8afce8de1b461c6b95a74094926636a7d8ff9c57`  
		Last Modified: Fri, 02 Sep 2022 05:07:26 GMT  
		Size: 79.6 MB (79603671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0626adf2cf42b6dad9a292e7d21a2c1206ef600a05e321e33d906aee3aa891cf`  
		Last Modified: Fri, 02 Sep 2022 05:07:41 GMT  
		Size: 15.9 MB (15860497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:d047da019eed0ae7d07f4483f4f6dca6ddb5aab8834d63bcee903ecff0073bc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303305191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6388f41565b185241b75e7dc046ca9f15971530341e6c9d8aabf93ee93145659`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:53:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:53:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 Aug 2022 22:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:55:11 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:56:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:56:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:57:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d345e3aeca1c4dd8930e961af9d46712aa474a7ce53acba4f54b4ff3b113a84`  
		Last Modified: Wed, 03 Aug 2022 23:09:30 GMT  
		Size: 1.2 MB (1181992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf40d14b8b7f81b4f192b1708fbdb0a57c3626f5b72be630a041c1f634f266`  
		Last Modified: Wed, 03 Aug 2022 23:09:28 GMT  
		Size: 4.7 MB (4676289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3223d85d87ee35ea3ab4535feef031631e281f3c617de4cdc218c4983c9b6f`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5bf7f51f5d7e24eec5395780a42aebd0c726cb0466dd5e0b2c492c6d0c84b3`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c66f511399e2f2993ed8fd014bb457c6d6a9483ae665aea0e9eb01fb0a54b4`  
		Last Modified: Wed, 03 Aug 2022 23:10:06 GMT  
		Size: 157.5 MB (157479986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa138f7b3214bda7dc2ae9534dff610b8c2a41d8de8dfb7c8a69ab5eba596887`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956f29112fb883f35fde1c1d67fc064ab659310ef5bc2f894fd7fabc7cb1b53`  
		Last Modified: Wed, 03 Aug 2022 23:10:25 GMT  
		Size: 40.5 MB (40505939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b4fa88c4ff97cf49d78a40c699333d1182e8a7a0cdb62a65b76e6d6ba39208`  
		Last Modified: Wed, 03 Aug 2022 23:10:18 GMT  
		Size: 323.5 KB (323517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f054c04c983a4aa345e62e3a2df78c234e061aab4b29b964612f3ff52473c`  
		Last Modified: Wed, 03 Aug 2022 23:10:30 GMT  
		Size: 60.5 MB (60480770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714bead958c0893197e557905b695ea7e2e9f9a621b7b00a14bc25d104d1e307`  
		Last Modified: Wed, 03 Aug 2022 23:10:48 GMT  
		Size: 14.1 MB (14065011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7115e6f5880c00e61f39bffe3417db74ca7d9d2c08fbf76d3693a0dd38cb54e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.6 MB (337615813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f84482c105f51b121ecf76fca749f92f777fd4925b639fa1eb780db6014cc9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:04:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:04:14 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:04:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:04:16 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 06:05:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:05:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:05:17 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:05:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:06:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14c9b385a2e2a1aaf2e3e0e96bb0ab19b0ae4bd1ba4df6e04bd247b310d5c2`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb230fc3fead8135d54463448100608dff8db563117ce648ff536d58028e043`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a441fbb85ca0fc9351965d962c26631f0c0fdd0a80a5de4349d0a2fe39cdad`  
		Last Modified: Fri, 02 Sep 2022 06:29:39 GMT  
		Size: 171.4 MB (171414641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cbf101495077c64a07b49123584c92c50e4eedbf37c6fe039a5c96c1a45fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351e164058f5f6b26f33ca86e472799ca95df650c8044c529338423424b38ea4`  
		Last Modified: Fri, 02 Sep 2022 06:29:56 GMT  
		Size: 45.0 MB (44988847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fcd9c3e7122e87ef29f417d198e443a1892d621f1fe005f9cbf9072b5d3b9`  
		Last Modified: Fri, 02 Sep 2022 06:29:50 GMT  
		Size: 325.7 KB (325657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65599a689993fa62149f8b2028498730ddd14125298b858124751013f37cdba4`  
		Last Modified: Fri, 02 Sep 2022 06:30:00 GMT  
		Size: 71.8 MB (71754873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18121c479bd23f9bed87b73dab18f777737e353710d6bc6fbea8ba53d4921f2e`  
		Last Modified: Fri, 02 Sep 2022 06:30:17 GMT  
		Size: 15.4 MB (15449034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:61be0eb69faf71dbe5dc943dbc06c569ecb4d64db02dc2468b9a85e1d7b3657c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:a3668b236d93abbfedcf72a51abc193842193459fdb8aac6b642ed95441a6cbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343151353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b356ccf86aa9679666fabf6c6ce440b45f40baf7f272adee0eca54f31d4d6b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:30:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:30:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 04:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:32:46 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:33:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:33:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e933af47665655d97d902ecb6d264063a041b2c12dfcbaf849a05672cafc9044`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1916d550484243d392ddc6fdca4ba34710bd3305a578bf9d241f2ad6d944c099`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d152bd7bb3b1335dd05a53828858de8ceab15c85e96fdc0181b2e38f72323b8`  
		Last Modified: Fri, 02 Sep 2022 05:07:05 GMT  
		Size: 177.0 MB (176996015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edc8aa6732f94d22820aa0f96400c620b51e015fa6a940c03e9b579f0de306f`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38aa1dd8b74095a973aa1b1fe9d7495fcbf895f954b66adbff905119d10103`  
		Last Modified: Fri, 02 Sep 2022 05:07:22 GMT  
		Size: 50.9 MB (50940098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5cec93c265dc40fb6eb4790e71c25ac877e2addb6eddf96377e4336554651e`  
		Last Modified: Fri, 02 Sep 2022 05:07:14 GMT  
		Size: 325.7 KB (325719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca383d78ab41bd8631ac0ef8afce8de1b461c6b95a74094926636a7d8ff9c57`  
		Last Modified: Fri, 02 Sep 2022 05:07:26 GMT  
		Size: 79.6 MB (79603671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:dc89df4c67ffb8e35dcb232a71956399e39b3575cfa1e8389e74e1d5a0782638
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289240180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c5a83264b759495b4caae5a5c49c6f2dbf31890cf1b28ffedbd7d55f94c0279`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:53:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:53:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 Aug 2022 22:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:55:11 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:56:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:56:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:57:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d345e3aeca1c4dd8930e961af9d46712aa474a7ce53acba4f54b4ff3b113a84`  
		Last Modified: Wed, 03 Aug 2022 23:09:30 GMT  
		Size: 1.2 MB (1181992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf40d14b8b7f81b4f192b1708fbdb0a57c3626f5b72be630a041c1f634f266`  
		Last Modified: Wed, 03 Aug 2022 23:09:28 GMT  
		Size: 4.7 MB (4676289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3223d85d87ee35ea3ab4535feef031631e281f3c617de4cdc218c4983c9b6f`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5bf7f51f5d7e24eec5395780a42aebd0c726cb0466dd5e0b2c492c6d0c84b3`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c66f511399e2f2993ed8fd014bb457c6d6a9483ae665aea0e9eb01fb0a54b4`  
		Last Modified: Wed, 03 Aug 2022 23:10:06 GMT  
		Size: 157.5 MB (157479986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa138f7b3214bda7dc2ae9534dff610b8c2a41d8de8dfb7c8a69ab5eba596887`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956f29112fb883f35fde1c1d67fc064ab659310ef5bc2f894fd7fabc7cb1b53`  
		Last Modified: Wed, 03 Aug 2022 23:10:25 GMT  
		Size: 40.5 MB (40505939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b4fa88c4ff97cf49d78a40c699333d1182e8a7a0cdb62a65b76e6d6ba39208`  
		Last Modified: Wed, 03 Aug 2022 23:10:18 GMT  
		Size: 323.5 KB (323517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f054c04c983a4aa345e62e3a2df78c234e061aab4b29b964612f3ff52473c`  
		Last Modified: Wed, 03 Aug 2022 23:10:30 GMT  
		Size: 60.5 MB (60480770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:986aa4972599a27a24d5fef240d4bbb3baa85e68212932eed5e984b1f6683628
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.2 MB (322166779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a94e2896051c439f0a9a4bb21c10b79700eb74d879d67d9ca855a477f7f94ca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:04:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:04:14 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:04:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:04:16 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 06:05:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:05:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:05:17 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:05:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14c9b385a2e2a1aaf2e3e0e96bb0ab19b0ae4bd1ba4df6e04bd247b310d5c2`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb230fc3fead8135d54463448100608dff8db563117ce648ff536d58028e043`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a441fbb85ca0fc9351965d962c26631f0c0fdd0a80a5de4349d0a2fe39cdad`  
		Last Modified: Fri, 02 Sep 2022 06:29:39 GMT  
		Size: 171.4 MB (171414641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cbf101495077c64a07b49123584c92c50e4eedbf37c6fe039a5c96c1a45fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351e164058f5f6b26f33ca86e472799ca95df650c8044c529338423424b38ea4`  
		Last Modified: Fri, 02 Sep 2022 06:29:56 GMT  
		Size: 45.0 MB (44988847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fcd9c3e7122e87ef29f417d198e443a1892d621f1fe005f9cbf9072b5d3b9`  
		Last Modified: Fri, 02 Sep 2022 06:29:50 GMT  
		Size: 325.7 KB (325657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65599a689993fa62149f8b2028498730ddd14125298b858124751013f37cdba4`  
		Last Modified: Fri, 02 Sep 2022 06:30:00 GMT  
		Size: 71.8 MB (71754873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:460b5270d8efd9366df37679e97b7ff112e3fd9dd49e121c3b66d95a341e050d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:9b31f35802dbd4e2692766a1e4c26fb0455819e121512024c4d26fed8bf7bce0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.4 MB (463388524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe749cdeaebe2e2a4c64221e28a6de9e135c4e290c652a948c231ba1889cfb03`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:10:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:10:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 23 Aug 2022 11:10:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 23 Aug 2022 11:10:45 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:10:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 23 Aug 2022 11:10:45 GMT
ENV ROS_DISTRO=noetic
# Tue, 23 Aug 2022 11:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:11:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 23 Aug 2022 11:11:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 23 Aug 2022 11:11:49 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:12:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:12:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 23 Aug 2022 11:12:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd91dd5198cc577c5556c7c5c335e0ea5701168d8c2ded40b83bc24be1434e47`  
		Last Modified: Tue, 23 Aug 2022 11:17:01 GMT  
		Size: 10.9 MB (10893537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385a586942561cc66fbd30195e87e96f1b39c6350f5ecd935dab71ef933e1bca`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3402e2486e536bf44469c2ce583b71937b7cbff76618e426dd63ed6b7dfe0cc5`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c2873f607da18c9f2623d952abd04118f7d0778f3599821850f1919eafc164`  
		Last Modified: Tue, 23 Aug 2022 11:17:33 GMT  
		Size: 239.2 MB (239186445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d17c4e21a19faebaa430ee698b7cb100d2e778f790784743bdc70da09436a41`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7245c288a141189c997601cc51df3c78474637e0eaaf193d9ff374f766648200`  
		Last Modified: Tue, 23 Aug 2022 11:17:55 GMT  
		Size: 86.6 MB (86569601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3ced040e753b4661b1383d3e5ed1eeb33533efbd4f2e5f6a9b9bd9fe4ca902`  
		Last Modified: Tue, 23 Aug 2022 11:17:42 GMT  
		Size: 319.4 KB (319418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0737249fff82a9ae2caa5144493e9d2fcf088027709fe87ee86f79726d1ae7fd`  
		Last Modified: Tue, 23 Aug 2022 11:17:52 GMT  
		Size: 76.0 MB (75976837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:28c09a531af4f7df69d166a66ce447dae5c9390d17ee2a394f84640e8a68dc50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.8 MB (402848541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36620262bf72864e1023de7d7016850d3ea306b7222a6c6daa19dec3713f1025`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:18:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:18:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 23 Aug 2022 11:18:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 23 Aug 2022 11:18:57 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:18:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 23 Aug 2022 11:18:59 GMT
ENV ROS_DISTRO=noetic
# Tue, 23 Aug 2022 11:20:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:20:21 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 23 Aug 2022 11:20:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 23 Aug 2022 11:20:24 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:20:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:21:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 23 Aug 2022 11:21:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc5b8055a31acea8cf6858fb7058f9828cf856d7ca15408120754ef8e582e8b`  
		Last Modified: Tue, 23 Aug 2022 11:28:27 GMT  
		Size: 10.7 MB (10689268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3e051ec8c4f50bc9206c4036995d09b8baf8a208b4aae22a2deeb7a246a5f0`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3dbf6ff20222664e13d9f371430b5b76a850b135d2cd6876f8239ebf2cf26`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6b972b9d90022d411ed9be6a75b03629caf11045e410b85bf532d9b574973f`  
		Last Modified: Tue, 23 Aug 2022 11:28:56 GMT  
		Size: 184.4 MB (184373802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bebe4a80f1367e9d727dcccb4679e5590d80dd2a8d0b00100b06f21a5e20bc0`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97614d076b0337a5bf133b8ea0f63b2a64fd4907f6242d84556146524077b032`  
		Last Modified: Tue, 23 Aug 2022 11:29:14 GMT  
		Size: 84.4 MB (84370471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a86f0adf69a256428f0eb97e4d0a6ebb4c333ee833fa76731d8b0526eb88d5d`  
		Last Modified: Tue, 23 Aug 2022 11:29:04 GMT  
		Size: 319.4 KB (319361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a577fe3ce43ebe0d1f7719dc2286b8f2cead9743255d3f8f71caebb62632e29e`  
		Last Modified: Tue, 23 Aug 2022 11:29:13 GMT  
		Size: 73.9 MB (73865202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:61be0eb69faf71dbe5dc943dbc06c569ecb4d64db02dc2468b9a85e1d7b3657c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:a3668b236d93abbfedcf72a51abc193842193459fdb8aac6b642ed95441a6cbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343151353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b356ccf86aa9679666fabf6c6ce440b45f40baf7f272adee0eca54f31d4d6b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:30:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:30:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 04:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:32:46 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:33:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:33:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e933af47665655d97d902ecb6d264063a041b2c12dfcbaf849a05672cafc9044`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1916d550484243d392ddc6fdca4ba34710bd3305a578bf9d241f2ad6d944c099`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d152bd7bb3b1335dd05a53828858de8ceab15c85e96fdc0181b2e38f72323b8`  
		Last Modified: Fri, 02 Sep 2022 05:07:05 GMT  
		Size: 177.0 MB (176996015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edc8aa6732f94d22820aa0f96400c620b51e015fa6a940c03e9b579f0de306f`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38aa1dd8b74095a973aa1b1fe9d7495fcbf895f954b66adbff905119d10103`  
		Last Modified: Fri, 02 Sep 2022 05:07:22 GMT  
		Size: 50.9 MB (50940098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5cec93c265dc40fb6eb4790e71c25ac877e2addb6eddf96377e4336554651e`  
		Last Modified: Fri, 02 Sep 2022 05:07:14 GMT  
		Size: 325.7 KB (325719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca383d78ab41bd8631ac0ef8afce8de1b461c6b95a74094926636a7d8ff9c57`  
		Last Modified: Fri, 02 Sep 2022 05:07:26 GMT  
		Size: 79.6 MB (79603671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:dc89df4c67ffb8e35dcb232a71956399e39b3575cfa1e8389e74e1d5a0782638
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289240180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c5a83264b759495b4caae5a5c49c6f2dbf31890cf1b28ffedbd7d55f94c0279`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:53:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:53:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 Aug 2022 22:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:55:11 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:56:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:56:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:57:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d345e3aeca1c4dd8930e961af9d46712aa474a7ce53acba4f54b4ff3b113a84`  
		Last Modified: Wed, 03 Aug 2022 23:09:30 GMT  
		Size: 1.2 MB (1181992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf40d14b8b7f81b4f192b1708fbdb0a57c3626f5b72be630a041c1f634f266`  
		Last Modified: Wed, 03 Aug 2022 23:09:28 GMT  
		Size: 4.7 MB (4676289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3223d85d87ee35ea3ab4535feef031631e281f3c617de4cdc218c4983c9b6f`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5bf7f51f5d7e24eec5395780a42aebd0c726cb0466dd5e0b2c492c6d0c84b3`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c66f511399e2f2993ed8fd014bb457c6d6a9483ae665aea0e9eb01fb0a54b4`  
		Last Modified: Wed, 03 Aug 2022 23:10:06 GMT  
		Size: 157.5 MB (157479986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa138f7b3214bda7dc2ae9534dff610b8c2a41d8de8dfb7c8a69ab5eba596887`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956f29112fb883f35fde1c1d67fc064ab659310ef5bc2f894fd7fabc7cb1b53`  
		Last Modified: Wed, 03 Aug 2022 23:10:25 GMT  
		Size: 40.5 MB (40505939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b4fa88c4ff97cf49d78a40c699333d1182e8a7a0cdb62a65b76e6d6ba39208`  
		Last Modified: Wed, 03 Aug 2022 23:10:18 GMT  
		Size: 323.5 KB (323517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f054c04c983a4aa345e62e3a2df78c234e061aab4b29b964612f3ff52473c`  
		Last Modified: Wed, 03 Aug 2022 23:10:30 GMT  
		Size: 60.5 MB (60480770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:986aa4972599a27a24d5fef240d4bbb3baa85e68212932eed5e984b1f6683628
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.2 MB (322166779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a94e2896051c439f0a9a4bb21c10b79700eb74d879d67d9ca855a477f7f94ca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:04:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:04:14 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:04:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:04:16 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 06:05:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:05:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:05:17 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:05:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14c9b385a2e2a1aaf2e3e0e96bb0ab19b0ae4bd1ba4df6e04bd247b310d5c2`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb230fc3fead8135d54463448100608dff8db563117ce648ff536d58028e043`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a441fbb85ca0fc9351965d962c26631f0c0fdd0a80a5de4349d0a2fe39cdad`  
		Last Modified: Fri, 02 Sep 2022 06:29:39 GMT  
		Size: 171.4 MB (171414641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cbf101495077c64a07b49123584c92c50e4eedbf37c6fe039a5c96c1a45fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351e164058f5f6b26f33ca86e472799ca95df650c8044c529338423424b38ea4`  
		Last Modified: Fri, 02 Sep 2022 06:29:56 GMT  
		Size: 45.0 MB (44988847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fcd9c3e7122e87ef29f417d198e443a1892d621f1fe005f9cbf9072b5d3b9`  
		Last Modified: Fri, 02 Sep 2022 06:29:50 GMT  
		Size: 325.7 KB (325657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65599a689993fa62149f8b2028498730ddd14125298b858124751013f37cdba4`  
		Last Modified: Fri, 02 Sep 2022 06:30:00 GMT  
		Size: 71.8 MB (71754873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:0090af1a03e4f22eb7f7c755fce49915e8fe6dd810c91d85bda29381078f9913
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:15787f4244d2c4f18c65ff9f5e7aa63bad77a3174d734e44c5d2efe18ccedbf6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212281865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b851b252f464f1ba9e081c21053a32f21ce69a6ec8af25754576fe7b6efd082`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:30:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:30:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 04:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:32:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e933af47665655d97d902ecb6d264063a041b2c12dfcbaf849a05672cafc9044`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1916d550484243d392ddc6fdca4ba34710bd3305a578bf9d241f2ad6d944c099`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d152bd7bb3b1335dd05a53828858de8ceab15c85e96fdc0181b2e38f72323b8`  
		Last Modified: Fri, 02 Sep 2022 05:07:05 GMT  
		Size: 177.0 MB (176996015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edc8aa6732f94d22820aa0f96400c620b51e015fa6a940c03e9b579f0de306f`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:b627329429c292b2ec2942cf25941025bba74bdd29b28271ffa3758060d0ee56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187929954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7324654dea2b039973f3b058244c1f5bf15eb28690dbe2fd8426e09c3f10323`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:53:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:53:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 Aug 2022 22:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:55:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d345e3aeca1c4dd8930e961af9d46712aa474a7ce53acba4f54b4ff3b113a84`  
		Last Modified: Wed, 03 Aug 2022 23:09:30 GMT  
		Size: 1.2 MB (1181992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf40d14b8b7f81b4f192b1708fbdb0a57c3626f5b72be630a041c1f634f266`  
		Last Modified: Wed, 03 Aug 2022 23:09:28 GMT  
		Size: 4.7 MB (4676289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3223d85d87ee35ea3ab4535feef031631e281f3c617de4cdc218c4983c9b6f`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5bf7f51f5d7e24eec5395780a42aebd0c726cb0466dd5e0b2c492c6d0c84b3`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c66f511399e2f2993ed8fd014bb457c6d6a9483ae665aea0e9eb01fb0a54b4`  
		Last Modified: Wed, 03 Aug 2022 23:10:06 GMT  
		Size: 157.5 MB (157479986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa138f7b3214bda7dc2ae9534dff610b8c2a41d8de8dfb7c8a69ab5eba596887`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:00e70faeb51356ce872d636c80c7c9ce93b6e1dc20f59680610efb1fbf87de74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205097402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c635e1c1c52092c1d9870179723f781a11deaf43fa216482c654757887b1e05`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:04:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:04:14 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:04:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:04:16 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 06:05:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:05:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:05:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14c9b385a2e2a1aaf2e3e0e96bb0ab19b0ae4bd1ba4df6e04bd247b310d5c2`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb230fc3fead8135d54463448100608dff8db563117ce648ff536d58028e043`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a441fbb85ca0fc9351965d962c26631f0c0fdd0a80a5de4349d0a2fe39cdad`  
		Last Modified: Fri, 02 Sep 2022 06:29:39 GMT  
		Size: 171.4 MB (171414641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cbf101495077c64a07b49123584c92c50e4eedbf37c6fe039a5c96c1a45fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:2909b34c7b1c64431ca0f75bec7eda0857c4815c58da9e62d4858e2973582a75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:1a1d06b35677ea6f17b411b6bcb701c371187b5cde9933440638403a1a3f3a33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300522668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0366cedccb9e45dc41095871119e8aebed346194dab88db7bd95ba5f71e98c4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:10:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:10:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 23 Aug 2022 11:10:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 23 Aug 2022 11:10:45 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:10:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 23 Aug 2022 11:10:45 GMT
ENV ROS_DISTRO=noetic
# Tue, 23 Aug 2022 11:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:11:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 23 Aug 2022 11:11:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 23 Aug 2022 11:11:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd91dd5198cc577c5556c7c5c335e0ea5701168d8c2ded40b83bc24be1434e47`  
		Last Modified: Tue, 23 Aug 2022 11:17:01 GMT  
		Size: 10.9 MB (10893537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385a586942561cc66fbd30195e87e96f1b39c6350f5ecd935dab71ef933e1bca`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3402e2486e536bf44469c2ce583b71937b7cbff76618e426dd63ed6b7dfe0cc5`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c2873f607da18c9f2623d952abd04118f7d0778f3599821850f1919eafc164`  
		Last Modified: Tue, 23 Aug 2022 11:17:33 GMT  
		Size: 239.2 MB (239186445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d17c4e21a19faebaa430ee698b7cb100d2e778f790784743bdc70da09436a41`  
		Last Modified: Tue, 23 Aug 2022 11:16:59 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b8a2f95e3a3e173aaa2bb444bccdca8fc2e86c556b35596b039e7fccbbe9633b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244293507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89673ed8d38d107a06ec46cc1af47c271e78a4301bd71e7e62fcfa10850e23fb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:18:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:18:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 23 Aug 2022 11:18:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 23 Aug 2022 11:18:57 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:18:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 23 Aug 2022 11:18:59 GMT
ENV ROS_DISTRO=noetic
# Tue, 23 Aug 2022 11:20:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:20:21 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 23 Aug 2022 11:20:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 23 Aug 2022 11:20:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc5b8055a31acea8cf6858fb7058f9828cf856d7ca15408120754ef8e582e8b`  
		Last Modified: Tue, 23 Aug 2022 11:28:27 GMT  
		Size: 10.7 MB (10689268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3e051ec8c4f50bc9206c4036995d09b8baf8a208b4aae22a2deeb7a246a5f0`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3dbf6ff20222664e13d9f371430b5b76a850b135d2cd6876f8239ebf2cf26`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6b972b9d90022d411ed9be6a75b03629caf11045e410b85bf532d9b574973f`  
		Last Modified: Tue, 23 Aug 2022 11:28:56 GMT  
		Size: 184.4 MB (184373802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bebe4a80f1367e9d727dcccb4679e5590d80dd2a8d0b00100b06f21a5e20bc0`  
		Last Modified: Tue, 23 Aug 2022 11:28:25 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:0090af1a03e4f22eb7f7c755fce49915e8fe6dd810c91d85bda29381078f9913
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:15787f4244d2c4f18c65ff9f5e7aa63bad77a3174d734e44c5d2efe18ccedbf6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212281865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b851b252f464f1ba9e081c21053a32f21ce69a6ec8af25754576fe7b6efd082`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:30:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:30:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 04:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:32:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e933af47665655d97d902ecb6d264063a041b2c12dfcbaf849a05672cafc9044`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1916d550484243d392ddc6fdca4ba34710bd3305a578bf9d241f2ad6d944c099`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d152bd7bb3b1335dd05a53828858de8ceab15c85e96fdc0181b2e38f72323b8`  
		Last Modified: Fri, 02 Sep 2022 05:07:05 GMT  
		Size: 177.0 MB (176996015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edc8aa6732f94d22820aa0f96400c620b51e015fa6a940c03e9b579f0de306f`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:b627329429c292b2ec2942cf25941025bba74bdd29b28271ffa3758060d0ee56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187929954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7324654dea2b039973f3b058244c1f5bf15eb28690dbe2fd8426e09c3f10323`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:53:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:53:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 Aug 2022 22:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:55:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d345e3aeca1c4dd8930e961af9d46712aa474a7ce53acba4f54b4ff3b113a84`  
		Last Modified: Wed, 03 Aug 2022 23:09:30 GMT  
		Size: 1.2 MB (1181992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf40d14b8b7f81b4f192b1708fbdb0a57c3626f5b72be630a041c1f634f266`  
		Last Modified: Wed, 03 Aug 2022 23:09:28 GMT  
		Size: 4.7 MB (4676289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3223d85d87ee35ea3ab4535feef031631e281f3c617de4cdc218c4983c9b6f`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5bf7f51f5d7e24eec5395780a42aebd0c726cb0466dd5e0b2c492c6d0c84b3`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c66f511399e2f2993ed8fd014bb457c6d6a9483ae665aea0e9eb01fb0a54b4`  
		Last Modified: Wed, 03 Aug 2022 23:10:06 GMT  
		Size: 157.5 MB (157479986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa138f7b3214bda7dc2ae9534dff610b8c2a41d8de8dfb7c8a69ab5eba596887`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:00e70faeb51356ce872d636c80c7c9ce93b6e1dc20f59680610efb1fbf87de74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205097402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c635e1c1c52092c1d9870179723f781a11deaf43fa216482c654757887b1e05`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:04:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:04:14 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:04:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:04:16 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 06:05:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:05:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:05:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14c9b385a2e2a1aaf2e3e0e96bb0ab19b0ae4bd1ba4df6e04bd247b310d5c2`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb230fc3fead8135d54463448100608dff8db563117ce648ff536d58028e043`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a441fbb85ca0fc9351965d962c26631f0c0fdd0a80a5de4349d0a2fe39cdad`  
		Last Modified: Fri, 02 Sep 2022 06:29:39 GMT  
		Size: 171.4 MB (171414641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cbf101495077c64a07b49123584c92c50e4eedbf37c6fe039a5c96c1a45fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:e1b81803e71c64f9fb4a9465103d7d6e26acaf114ce724bca30ffda6a49bc521
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:7b4c586e54c27743aab2a47e40c9703663d5a9e8de1e08173aafbce70150359c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (262952620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223af4769b7faa40e705248499c92752b2b8291256bf897cda3f27d405b0fe59`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:59:53 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 05:00:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:00:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 05:00:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 05:01:07 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 05:01:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3dc50070b191638388b8a6f45838ba98380554ae338b31cc128a05d2395988`  
		Last Modified: Fri, 02 Sep 2022 05:14:57 GMT  
		Size: 106.2 MB (106166428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81258fb9cb69dfc99169ad3cb6e4fdf405255a94947c3080addd04660088d9`  
		Last Modified: Fri, 02 Sep 2022 05:14:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06230df102e423df05671bcf3524ba4a66b7948f791b968310ce88c3912d891b`  
		Last Modified: Fri, 02 Sep 2022 05:15:20 GMT  
		Size: 97.8 MB (97849361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fba9b08f3c34427866a17b95897c2bbf6d0ddaa0388e56fec786cc5e8b03e9`  
		Last Modified: Fri, 02 Sep 2022 05:15:07 GMT  
		Size: 280.9 KB (280936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8408c6380a2368a7fad097e912751c17f613c5e60923c6797b34c7146889011c`  
		Last Modified: Fri, 02 Sep 2022 05:15:06 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd491e285c840733c080cbbbbaaff463949c9101c61e114e1827f6c8bcac997`  
		Last Modified: Fri, 02 Sep 2022 05:15:10 GMT  
		Size: 23.2 MB (23221130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a9dcdf82e957bea076149139b3c6cdee66559f489613daa7903b56685f7f1aef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255169056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e9bd1d5dd1b3a26db2b810ff05f70c5869229f070eb096aab27f1e691324200`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:20:47 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 06:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:21:36 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:21:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:21:38 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:22:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:22:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:22:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:22:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57709850deb7ebb6da7e7913dd7f347b87d4aff6128c1297029b1764763a4c43`  
		Last Modified: Fri, 02 Sep 2022 06:37:27 GMT  
		Size: 103.9 MB (103880245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67b53a682dfe82f8a87e67d34d26e3a50eacc3e0bf38649a8b67d96c7e03ea`  
		Last Modified: Fri, 02 Sep 2022 06:37:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2a782d281bb90dd26f42ed3113a1e4d736c784ad27b4546669bca780ad66bd`  
		Last Modified: Fri, 02 Sep 2022 06:37:51 GMT  
		Size: 95.2 MB (95213961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf639d3046819cf6b3d082dad590518137fc54d4a308acc8f6545b8bb68ac366`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 280.9 KB (280888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f896ae4cec7dae8bae24fa69bc7c65810575491c2df60e45eebffad0fe8a61bb`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 2.4 KB (2355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819335435c465f7b44fe0db81c9fddd471a57234896c5daf09af9efb60a54319`  
		Last Modified: Fri, 02 Sep 2022 06:37:41 GMT  
		Size: 22.6 MB (22635152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:b9a0164ab06b4057b0fe1b3ccd1f9e42f219eca9f7e548ea477d507415963a5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:5da4c659ca33880dde2f1c81b6090f5fe36d146c2220ec69778c2a7553c46779
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1084630290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1e0191400b6a2d7a2b735a66b6136ebd11c56de6a117c0c9aa49d15c5964d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:59:53 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 05:00:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:00:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 05:00:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 05:01:07 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 05:01:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:03:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3dc50070b191638388b8a6f45838ba98380554ae338b31cc128a05d2395988`  
		Last Modified: Fri, 02 Sep 2022 05:14:57 GMT  
		Size: 106.2 MB (106166428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81258fb9cb69dfc99169ad3cb6e4fdf405255a94947c3080addd04660088d9`  
		Last Modified: Fri, 02 Sep 2022 05:14:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06230df102e423df05671bcf3524ba4a66b7948f791b968310ce88c3912d891b`  
		Last Modified: Fri, 02 Sep 2022 05:15:20 GMT  
		Size: 97.8 MB (97849361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fba9b08f3c34427866a17b95897c2bbf6d0ddaa0388e56fec786cc5e8b03e9`  
		Last Modified: Fri, 02 Sep 2022 05:15:07 GMT  
		Size: 280.9 KB (280936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8408c6380a2368a7fad097e912751c17f613c5e60923c6797b34c7146889011c`  
		Last Modified: Fri, 02 Sep 2022 05:15:06 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd491e285c840733c080cbbbbaaff463949c9101c61e114e1827f6c8bcac997`  
		Last Modified: Fri, 02 Sep 2022 05:15:10 GMT  
		Size: 23.2 MB (23221130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed4b59ab5f03f5776c1e0a48cdcd05a090c9d07c58d47bf3c3cdfafb3d497b0`  
		Last Modified: Fri, 02 Sep 2022 05:17:11 GMT  
		Size: 821.7 MB (821677670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:96eff54f23eca63101f9166eae6e3cd683bf0a757662e9d9fb0143c0c2fa38af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1034622591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aedba49e3b43e9c07e0d7e5213b7160e58d080cd86822a74c2968de9e4b531a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:20:47 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 06:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:21:36 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:21:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:21:38 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:22:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:22:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:22:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:22:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:25:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57709850deb7ebb6da7e7913dd7f347b87d4aff6128c1297029b1764763a4c43`  
		Last Modified: Fri, 02 Sep 2022 06:37:27 GMT  
		Size: 103.9 MB (103880245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67b53a682dfe82f8a87e67d34d26e3a50eacc3e0bf38649a8b67d96c7e03ea`  
		Last Modified: Fri, 02 Sep 2022 06:37:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2a782d281bb90dd26f42ed3113a1e4d736c784ad27b4546669bca780ad66bd`  
		Last Modified: Fri, 02 Sep 2022 06:37:51 GMT  
		Size: 95.2 MB (95213961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf639d3046819cf6b3d082dad590518137fc54d4a308acc8f6545b8bb68ac366`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 280.9 KB (280888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f896ae4cec7dae8bae24fa69bc7c65810575491c2df60e45eebffad0fe8a61bb`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 2.4 KB (2355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819335435c465f7b44fe0db81c9fddd471a57234896c5daf09af9efb60a54319`  
		Last Modified: Fri, 02 Sep 2022 06:37:41 GMT  
		Size: 22.6 MB (22635152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def99dc249ff5e9cd10748e4d1436c96551f2b8199c65a9659cc000ae4d0fedf`  
		Last Modified: Fri, 02 Sep 2022 06:39:40 GMT  
		Size: 779.5 MB (779453535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:b9a0164ab06b4057b0fe1b3ccd1f9e42f219eca9f7e548ea477d507415963a5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:5da4c659ca33880dde2f1c81b6090f5fe36d146c2220ec69778c2a7553c46779
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1084630290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1e0191400b6a2d7a2b735a66b6136ebd11c56de6a117c0c9aa49d15c5964d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:59:53 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 05:00:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:00:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 05:00:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 05:01:07 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 05:01:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:03:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3dc50070b191638388b8a6f45838ba98380554ae338b31cc128a05d2395988`  
		Last Modified: Fri, 02 Sep 2022 05:14:57 GMT  
		Size: 106.2 MB (106166428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81258fb9cb69dfc99169ad3cb6e4fdf405255a94947c3080addd04660088d9`  
		Last Modified: Fri, 02 Sep 2022 05:14:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06230df102e423df05671bcf3524ba4a66b7948f791b968310ce88c3912d891b`  
		Last Modified: Fri, 02 Sep 2022 05:15:20 GMT  
		Size: 97.8 MB (97849361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fba9b08f3c34427866a17b95897c2bbf6d0ddaa0388e56fec786cc5e8b03e9`  
		Last Modified: Fri, 02 Sep 2022 05:15:07 GMT  
		Size: 280.9 KB (280936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8408c6380a2368a7fad097e912751c17f613c5e60923c6797b34c7146889011c`  
		Last Modified: Fri, 02 Sep 2022 05:15:06 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd491e285c840733c080cbbbbaaff463949c9101c61e114e1827f6c8bcac997`  
		Last Modified: Fri, 02 Sep 2022 05:15:10 GMT  
		Size: 23.2 MB (23221130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed4b59ab5f03f5776c1e0a48cdcd05a090c9d07c58d47bf3c3cdfafb3d497b0`  
		Last Modified: Fri, 02 Sep 2022 05:17:11 GMT  
		Size: 821.7 MB (821677670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:96eff54f23eca63101f9166eae6e3cd683bf0a757662e9d9fb0143c0c2fa38af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1034622591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aedba49e3b43e9c07e0d7e5213b7160e58d080cd86822a74c2968de9e4b531a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:20:47 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 06:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:21:36 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:21:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:21:38 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:22:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:22:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:22:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:22:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:25:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57709850deb7ebb6da7e7913dd7f347b87d4aff6128c1297029b1764763a4c43`  
		Last Modified: Fri, 02 Sep 2022 06:37:27 GMT  
		Size: 103.9 MB (103880245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67b53a682dfe82f8a87e67d34d26e3a50eacc3e0bf38649a8b67d96c7e03ea`  
		Last Modified: Fri, 02 Sep 2022 06:37:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2a782d281bb90dd26f42ed3113a1e4d736c784ad27b4546669bca780ad66bd`  
		Last Modified: Fri, 02 Sep 2022 06:37:51 GMT  
		Size: 95.2 MB (95213961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf639d3046819cf6b3d082dad590518137fc54d4a308acc8f6545b8bb68ac366`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 280.9 KB (280888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f896ae4cec7dae8bae24fa69bc7c65810575491c2df60e45eebffad0fe8a61bb`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 2.4 KB (2355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819335435c465f7b44fe0db81c9fddd471a57234896c5daf09af9efb60a54319`  
		Last Modified: Fri, 02 Sep 2022 06:37:41 GMT  
		Size: 22.6 MB (22635152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def99dc249ff5e9cd10748e4d1436c96551f2b8199c65a9659cc000ae4d0fedf`  
		Last Modified: Fri, 02 Sep 2022 06:39:40 GMT  
		Size: 779.5 MB (779453535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:e1b81803e71c64f9fb4a9465103d7d6e26acaf114ce724bca30ffda6a49bc521
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:7b4c586e54c27743aab2a47e40c9703663d5a9e8de1e08173aafbce70150359c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (262952620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223af4769b7faa40e705248499c92752b2b8291256bf897cda3f27d405b0fe59`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:59:53 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 05:00:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:00:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 05:00:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 05:01:07 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 05:01:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3dc50070b191638388b8a6f45838ba98380554ae338b31cc128a05d2395988`  
		Last Modified: Fri, 02 Sep 2022 05:14:57 GMT  
		Size: 106.2 MB (106166428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81258fb9cb69dfc99169ad3cb6e4fdf405255a94947c3080addd04660088d9`  
		Last Modified: Fri, 02 Sep 2022 05:14:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06230df102e423df05671bcf3524ba4a66b7948f791b968310ce88c3912d891b`  
		Last Modified: Fri, 02 Sep 2022 05:15:20 GMT  
		Size: 97.8 MB (97849361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fba9b08f3c34427866a17b95897c2bbf6d0ddaa0388e56fec786cc5e8b03e9`  
		Last Modified: Fri, 02 Sep 2022 05:15:07 GMT  
		Size: 280.9 KB (280936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8408c6380a2368a7fad097e912751c17f613c5e60923c6797b34c7146889011c`  
		Last Modified: Fri, 02 Sep 2022 05:15:06 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd491e285c840733c080cbbbbaaff463949c9101c61e114e1827f6c8bcac997`  
		Last Modified: Fri, 02 Sep 2022 05:15:10 GMT  
		Size: 23.2 MB (23221130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a9dcdf82e957bea076149139b3c6cdee66559f489613daa7903b56685f7f1aef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255169056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e9bd1d5dd1b3a26db2b810ff05f70c5869229f070eb096aab27f1e691324200`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:20:47 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 06:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:21:36 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:21:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:21:38 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:22:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:22:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:22:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:22:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57709850deb7ebb6da7e7913dd7f347b87d4aff6128c1297029b1764763a4c43`  
		Last Modified: Fri, 02 Sep 2022 06:37:27 GMT  
		Size: 103.9 MB (103880245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67b53a682dfe82f8a87e67d34d26e3a50eacc3e0bf38649a8b67d96c7e03ea`  
		Last Modified: Fri, 02 Sep 2022 06:37:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2a782d281bb90dd26f42ed3113a1e4d736c784ad27b4546669bca780ad66bd`  
		Last Modified: Fri, 02 Sep 2022 06:37:51 GMT  
		Size: 95.2 MB (95213961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf639d3046819cf6b3d082dad590518137fc54d4a308acc8f6545b8bb68ac366`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 280.9 KB (280888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f896ae4cec7dae8bae24fa69bc7c65810575491c2df60e45eebffad0fe8a61bb`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 2.4 KB (2355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819335435c465f7b44fe0db81c9fddd471a57234896c5daf09af9efb60a54319`  
		Last Modified: Fri, 02 Sep 2022 06:37:41 GMT  
		Size: 22.6 MB (22635152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:e1b81803e71c64f9fb4a9465103d7d6e26acaf114ce724bca30ffda6a49bc521
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:7b4c586e54c27743aab2a47e40c9703663d5a9e8de1e08173aafbce70150359c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (262952620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223af4769b7faa40e705248499c92752b2b8291256bf897cda3f27d405b0fe59`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:59:53 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 05:00:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:00:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 05:00:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 05:01:07 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 05:01:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3dc50070b191638388b8a6f45838ba98380554ae338b31cc128a05d2395988`  
		Last Modified: Fri, 02 Sep 2022 05:14:57 GMT  
		Size: 106.2 MB (106166428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81258fb9cb69dfc99169ad3cb6e4fdf405255a94947c3080addd04660088d9`  
		Last Modified: Fri, 02 Sep 2022 05:14:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06230df102e423df05671bcf3524ba4a66b7948f791b968310ce88c3912d891b`  
		Last Modified: Fri, 02 Sep 2022 05:15:20 GMT  
		Size: 97.8 MB (97849361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fba9b08f3c34427866a17b95897c2bbf6d0ddaa0388e56fec786cc5e8b03e9`  
		Last Modified: Fri, 02 Sep 2022 05:15:07 GMT  
		Size: 280.9 KB (280936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8408c6380a2368a7fad097e912751c17f613c5e60923c6797b34c7146889011c`  
		Last Modified: Fri, 02 Sep 2022 05:15:06 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd491e285c840733c080cbbbbaaff463949c9101c61e114e1827f6c8bcac997`  
		Last Modified: Fri, 02 Sep 2022 05:15:10 GMT  
		Size: 23.2 MB (23221130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a9dcdf82e957bea076149139b3c6cdee66559f489613daa7903b56685f7f1aef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255169056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e9bd1d5dd1b3a26db2b810ff05f70c5869229f070eb096aab27f1e691324200`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:20:47 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 06:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:21:36 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:21:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:21:38 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:22:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:22:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:22:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:22:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57709850deb7ebb6da7e7913dd7f347b87d4aff6128c1297029b1764763a4c43`  
		Last Modified: Fri, 02 Sep 2022 06:37:27 GMT  
		Size: 103.9 MB (103880245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67b53a682dfe82f8a87e67d34d26e3a50eacc3e0bf38649a8b67d96c7e03ea`  
		Last Modified: Fri, 02 Sep 2022 06:37:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2a782d281bb90dd26f42ed3113a1e4d736c784ad27b4546669bca780ad66bd`  
		Last Modified: Fri, 02 Sep 2022 06:37:51 GMT  
		Size: 95.2 MB (95213961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf639d3046819cf6b3d082dad590518137fc54d4a308acc8f6545b8bb68ac366`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 280.9 KB (280888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f896ae4cec7dae8bae24fa69bc7c65810575491c2df60e45eebffad0fe8a61bb`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 2.4 KB (2355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819335435c465f7b44fe0db81c9fddd471a57234896c5daf09af9efb60a54319`  
		Last Modified: Fri, 02 Sep 2022 06:37:41 GMT  
		Size: 22.6 MB (22635152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:a43512359d6bb4b4cb13c018421d51af7f2da784da6a5dca1d18fb9f610f9641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:62b636750693d82af6038d86ef97419fe9b50715b452f8f5629fbff16916cd82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141598742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a06b95e4ada0c24e36fd8a8f9f13030fe23ea7867e50f915a0829bfddd89e5d4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:59:53 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 05:00:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:00:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 05:00:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3dc50070b191638388b8a6f45838ba98380554ae338b31cc128a05d2395988`  
		Last Modified: Fri, 02 Sep 2022 05:14:57 GMT  
		Size: 106.2 MB (106166428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81258fb9cb69dfc99169ad3cb6e4fdf405255a94947c3080addd04660088d9`  
		Last Modified: Fri, 02 Sep 2022 05:14:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b17fedbb473fb50f4e28ae046b8a279b6c7219b56300afc94bf4f24224eb4640
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (137036700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8302d02ce0698a6abda67eeeeb5c09dde3e47a0326483c19f08f3993f1ed40ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:20:47 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 06:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:21:36 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:21:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:21:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57709850deb7ebb6da7e7913dd7f347b87d4aff6128c1297029b1764763a4c43`  
		Last Modified: Fri, 02 Sep 2022 06:37:27 GMT  
		Size: 103.9 MB (103880245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67b53a682dfe82f8a87e67d34d26e3a50eacc3e0bf38649a8b67d96c7e03ea`  
		Last Modified: Fri, 02 Sep 2022 06:37:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:a43512359d6bb4b4cb13c018421d51af7f2da784da6a5dca1d18fb9f610f9641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:62b636750693d82af6038d86ef97419fe9b50715b452f8f5629fbff16916cd82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141598742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a06b95e4ada0c24e36fd8a8f9f13030fe23ea7867e50f915a0829bfddd89e5d4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:59:53 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 05:00:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:00:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 05:00:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3dc50070b191638388b8a6f45838ba98380554ae338b31cc128a05d2395988`  
		Last Modified: Fri, 02 Sep 2022 05:14:57 GMT  
		Size: 106.2 MB (106166428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81258fb9cb69dfc99169ad3cb6e4fdf405255a94947c3080addd04660088d9`  
		Last Modified: Fri, 02 Sep 2022 05:14:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b17fedbb473fb50f4e28ae046b8a279b6c7219b56300afc94bf4f24224eb4640
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (137036700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8302d02ce0698a6abda67eeeeb5c09dde3e47a0326483c19f08f3993f1ed40ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:20:47 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 06:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:21:36 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:21:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:21:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57709850deb7ebb6da7e7913dd7f347b87d4aff6128c1297029b1764763a4c43`  
		Last Modified: Fri, 02 Sep 2022 06:37:27 GMT  
		Size: 103.9 MB (103880245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67b53a682dfe82f8a87e67d34d26e3a50eacc3e0bf38649a8b67d96c7e03ea`  
		Last Modified: Fri, 02 Sep 2022 06:37:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
