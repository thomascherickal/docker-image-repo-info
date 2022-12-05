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
$ docker pull ros@sha256:02ba160fa839b96ba6acb22a554190c4743285cdc17745e28c0f13585b10c345
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:2a2cb6ec4fa94c8405549a3ba868f1be8e7cc9ba3530bf9909f1d7517fc33acd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250910730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79dc804c68414a56e2bc462fd1705c10a1815d04042c72e88ced0971e695f5b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 07:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:26:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:26:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:26:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:27:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:27:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:27:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 07:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122af75c69e965a1d4b50e964ea95ec60ddd9997347536d0e79ecf1dc96f8e4d`  
		Last Modified: Tue, 25 Oct 2022 07:59:22 GMT  
		Size: 120.4 MB (120353945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fb29cc59034ebd9df4a3ddc0a423888144631e3a1e4b4cffff2ce4396d52ed`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5fb36af82e519ef989f9d9107e767f04c18c153572130e0f6c3a343ebb0ce0`  
		Last Modified: Tue, 25 Oct 2022 07:59:43 GMT  
		Size: 73.3 MB (73325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837655cef3c4cc06788fbad7c6df8a77081a39d3392b8bafed1ea74c35a302e3`  
		Last Modified: Tue, 25 Oct 2022 07:59:32 GMT  
		Size: 269.4 KB (269364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb41d05e0bd11afe16ecfcf7ef668e3908835201cc94fa813d0bf7783c3ba24f`  
		Last Modified: Tue, 25 Oct 2022 07:59:31 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f073c138f041e9b85ff0ddae19609c388a359370280ec72e5d549f73206c8`  
		Last Modified: Tue, 25 Oct 2022 07:59:35 GMT  
		Size: 21.7 MB (21663794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1814ed410f2086291253ecfb6ae7f91372772eeae0dce2bdfe0a5be0164af52b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226763797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5022b17e9054bde6a86e41848695fea694d49265ee919d449400104fe721b737`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 21:34:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:35:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:35:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:35:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:35:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:36:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:36:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 21:36:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1125e614642ae08f414585e39268e20619496243391fc14223c48efb76567fe`  
		Last Modified: Tue, 25 Oct 2022 22:06:20 GMT  
		Size: 104.5 MB (104549412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3257e5f004cfece29d48f51619b6b61a55c530aa1ecbc38e1be4208caa2ae368`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414db4c36b110ea6ec637828a4983215f3c8120f5113c6b8a1b1e7b63d490652`  
		Last Modified: Tue, 25 Oct 2022 22:06:39 GMT  
		Size: 67.7 MB (67673997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29c8a2e8faff52e903b8c6eb0d283754c1de2db5a4f0fa1c50542d8ed3bf757`  
		Last Modified: Tue, 25 Oct 2022 22:06:31 GMT  
		Size: 269.4 KB (269368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650fa392d56bb2a49e8e5ceaea16096752cb2cddfae87d9cf1a6193b59b1da7a`  
		Last Modified: Tue, 25 Oct 2022 22:06:30 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cee9901e31fd356db4bc05acd8610220bec8ba0ced72c5658083ba9b7e4d51`  
		Last Modified: Tue, 25 Oct 2022 22:06:34 GMT  
		Size: 20.4 MB (20372962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:02ba160fa839b96ba6acb22a554190c4743285cdc17745e28c0f13585b10c345
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:2a2cb6ec4fa94c8405549a3ba868f1be8e7cc9ba3530bf9909f1d7517fc33acd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250910730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79dc804c68414a56e2bc462fd1705c10a1815d04042c72e88ced0971e695f5b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 07:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:26:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:26:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:26:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:27:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:27:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:27:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 07:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122af75c69e965a1d4b50e964ea95ec60ddd9997347536d0e79ecf1dc96f8e4d`  
		Last Modified: Tue, 25 Oct 2022 07:59:22 GMT  
		Size: 120.4 MB (120353945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fb29cc59034ebd9df4a3ddc0a423888144631e3a1e4b4cffff2ce4396d52ed`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5fb36af82e519ef989f9d9107e767f04c18c153572130e0f6c3a343ebb0ce0`  
		Last Modified: Tue, 25 Oct 2022 07:59:43 GMT  
		Size: 73.3 MB (73325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837655cef3c4cc06788fbad7c6df8a77081a39d3392b8bafed1ea74c35a302e3`  
		Last Modified: Tue, 25 Oct 2022 07:59:32 GMT  
		Size: 269.4 KB (269364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb41d05e0bd11afe16ecfcf7ef668e3908835201cc94fa813d0bf7783c3ba24f`  
		Last Modified: Tue, 25 Oct 2022 07:59:31 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f073c138f041e9b85ff0ddae19609c388a359370280ec72e5d549f73206c8`  
		Last Modified: Tue, 25 Oct 2022 07:59:35 GMT  
		Size: 21.7 MB (21663794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1814ed410f2086291253ecfb6ae7f91372772eeae0dce2bdfe0a5be0164af52b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226763797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5022b17e9054bde6a86e41848695fea694d49265ee919d449400104fe721b737`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 21:34:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:35:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:35:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:35:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:35:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:36:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:36:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 21:36:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1125e614642ae08f414585e39268e20619496243391fc14223c48efb76567fe`  
		Last Modified: Tue, 25 Oct 2022 22:06:20 GMT  
		Size: 104.5 MB (104549412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3257e5f004cfece29d48f51619b6b61a55c530aa1ecbc38e1be4208caa2ae368`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414db4c36b110ea6ec637828a4983215f3c8120f5113c6b8a1b1e7b63d490652`  
		Last Modified: Tue, 25 Oct 2022 22:06:39 GMT  
		Size: 67.7 MB (67673997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29c8a2e8faff52e903b8c6eb0d283754c1de2db5a4f0fa1c50542d8ed3bf757`  
		Last Modified: Tue, 25 Oct 2022 22:06:31 GMT  
		Size: 269.4 KB (269368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650fa392d56bb2a49e8e5ceaea16096752cb2cddfae87d9cf1a6193b59b1da7a`  
		Last Modified: Tue, 25 Oct 2022 22:06:30 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cee9901e31fd356db4bc05acd8610220bec8ba0ced72c5658083ba9b7e4d51`  
		Last Modified: Tue, 25 Oct 2022 22:06:34 GMT  
		Size: 20.4 MB (20372962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:02ba160fa839b96ba6acb22a554190c4743285cdc17745e28c0f13585b10c345
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:2a2cb6ec4fa94c8405549a3ba868f1be8e7cc9ba3530bf9909f1d7517fc33acd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250910730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79dc804c68414a56e2bc462fd1705c10a1815d04042c72e88ced0971e695f5b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 07:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:26:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:26:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:26:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:27:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:27:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:27:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 07:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122af75c69e965a1d4b50e964ea95ec60ddd9997347536d0e79ecf1dc96f8e4d`  
		Last Modified: Tue, 25 Oct 2022 07:59:22 GMT  
		Size: 120.4 MB (120353945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fb29cc59034ebd9df4a3ddc0a423888144631e3a1e4b4cffff2ce4396d52ed`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5fb36af82e519ef989f9d9107e767f04c18c153572130e0f6c3a343ebb0ce0`  
		Last Modified: Tue, 25 Oct 2022 07:59:43 GMT  
		Size: 73.3 MB (73325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837655cef3c4cc06788fbad7c6df8a77081a39d3392b8bafed1ea74c35a302e3`  
		Last Modified: Tue, 25 Oct 2022 07:59:32 GMT  
		Size: 269.4 KB (269364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb41d05e0bd11afe16ecfcf7ef668e3908835201cc94fa813d0bf7783c3ba24f`  
		Last Modified: Tue, 25 Oct 2022 07:59:31 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f073c138f041e9b85ff0ddae19609c388a359370280ec72e5d549f73206c8`  
		Last Modified: Tue, 25 Oct 2022 07:59:35 GMT  
		Size: 21.7 MB (21663794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1814ed410f2086291253ecfb6ae7f91372772eeae0dce2bdfe0a5be0164af52b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226763797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5022b17e9054bde6a86e41848695fea694d49265ee919d449400104fe721b737`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 21:34:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:35:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:35:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:35:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:35:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:36:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:36:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 21:36:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1125e614642ae08f414585e39268e20619496243391fc14223c48efb76567fe`  
		Last Modified: Tue, 25 Oct 2022 22:06:20 GMT  
		Size: 104.5 MB (104549412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3257e5f004cfece29d48f51619b6b61a55c530aa1ecbc38e1be4208caa2ae368`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414db4c36b110ea6ec637828a4983215f3c8120f5113c6b8a1b1e7b63d490652`  
		Last Modified: Tue, 25 Oct 2022 22:06:39 GMT  
		Size: 67.7 MB (67673997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29c8a2e8faff52e903b8c6eb0d283754c1de2db5a4f0fa1c50542d8ed3bf757`  
		Last Modified: Tue, 25 Oct 2022 22:06:31 GMT  
		Size: 269.4 KB (269368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650fa392d56bb2a49e8e5ceaea16096752cb2cddfae87d9cf1a6193b59b1da7a`  
		Last Modified: Tue, 25 Oct 2022 22:06:30 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cee9901e31fd356db4bc05acd8610220bec8ba0ced72c5658083ba9b7e4d51`  
		Last Modified: Tue, 25 Oct 2022 22:06:34 GMT  
		Size: 20.4 MB (20372962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:03528d3871764da0c6cee24e7baaeee8562c4ba3e90debfae5746ecd42ac82ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:87d8f4e045ca908ea1e9fc36cd58992b068c2243cd417af51df28015cae361c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155649379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f133e19ba781eb57466f334011e632c7258cb020aa4bd3f02210dc2724fc2f68`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 07:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:26:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:26:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:26:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122af75c69e965a1d4b50e964ea95ec60ddd9997347536d0e79ecf1dc96f8e4d`  
		Last Modified: Tue, 25 Oct 2022 07:59:22 GMT  
		Size: 120.4 MB (120353945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fb29cc59034ebd9df4a3ddc0a423888144631e3a1e4b4cffff2ce4396d52ed`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:14b37ec2f8cb57f1f948ddcb5dde6683ad4fed9db0365ff2ba990b3008ede6e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138445026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aaad4dee75eed93cc82b94029a2a7353ef3d2e022f002a56599f1750b75818a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 21:34:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:35:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:35:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:35:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1125e614642ae08f414585e39268e20619496243391fc14223c48efb76567fe`  
		Last Modified: Tue, 25 Oct 2022 22:06:20 GMT  
		Size: 104.5 MB (104549412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3257e5f004cfece29d48f51619b6b61a55c530aa1ecbc38e1be4208caa2ae368`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:03528d3871764da0c6cee24e7baaeee8562c4ba3e90debfae5746ecd42ac82ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:87d8f4e045ca908ea1e9fc36cd58992b068c2243cd417af51df28015cae361c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155649379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f133e19ba781eb57466f334011e632c7258cb020aa4bd3f02210dc2724fc2f68`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 07:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:26:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:26:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:26:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122af75c69e965a1d4b50e964ea95ec60ddd9997347536d0e79ecf1dc96f8e4d`  
		Last Modified: Tue, 25 Oct 2022 07:59:22 GMT  
		Size: 120.4 MB (120353945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fb29cc59034ebd9df4a3ddc0a423888144631e3a1e4b4cffff2ce4396d52ed`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:14b37ec2f8cb57f1f948ddcb5dde6683ad4fed9db0365ff2ba990b3008ede6e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138445026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aaad4dee75eed93cc82b94029a2a7353ef3d2e022f002a56599f1750b75818a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 21:34:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:35:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:35:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:35:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1125e614642ae08f414585e39268e20619496243391fc14223c48efb76567fe`  
		Last Modified: Tue, 25 Oct 2022 22:06:20 GMT  
		Size: 104.5 MB (104549412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3257e5f004cfece29d48f51619b6b61a55c530aa1ecbc38e1be4208caa2ae368`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:eb124a55056240f1cf593d767a41cd98f6de7d61dd4bcb40a54e45e85c46ebfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:7f3fea5f773eae8cc5ec19ac4b187c6ccdea246ebdde5f2f5cd15f0465925125
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349021297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c8ff5e9ab7d12eeafd7fb87cd290b6726657253eb5dbe4bb616f9f967713d75`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 07:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:26:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:26:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:26:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:27:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:27:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:27:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 07:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:28:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:28:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:28:12 GMT
ENV ROS1_DISTRO=noetic
# Tue, 25 Oct 2022 07:28:13 GMT
ENV ROS2_DISTRO=foxy
# Mon, 05 Dec 2022 20:57:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 20:57:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 20:57:49 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122af75c69e965a1d4b50e964ea95ec60ddd9997347536d0e79ecf1dc96f8e4d`  
		Last Modified: Tue, 25 Oct 2022 07:59:22 GMT  
		Size: 120.4 MB (120353945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fb29cc59034ebd9df4a3ddc0a423888144631e3a1e4b4cffff2ce4396d52ed`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5fb36af82e519ef989f9d9107e767f04c18c153572130e0f6c3a343ebb0ce0`  
		Last Modified: Tue, 25 Oct 2022 07:59:43 GMT  
		Size: 73.3 MB (73325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837655cef3c4cc06788fbad7c6df8a77081a39d3392b8bafed1ea74c35a302e3`  
		Last Modified: Tue, 25 Oct 2022 07:59:32 GMT  
		Size: 269.4 KB (269364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb41d05e0bd11afe16ecfcf7ef668e3908835201cc94fa813d0bf7783c3ba24f`  
		Last Modified: Tue, 25 Oct 2022 07:59:31 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f073c138f041e9b85ff0ddae19609c388a359370280ec72e5d549f73206c8`  
		Last Modified: Tue, 25 Oct 2022 07:59:35 GMT  
		Size: 21.7 MB (21663794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b18f13baebbb1e3f7ffc35466142e70d5913b88c27a49f5e5dbb9eab829e68e`  
		Last Modified: Tue, 25 Oct 2022 07:59:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff282c273773346a09f274c19f2310cf509f62c59ff80bf3c1831cb16577d048`  
		Last Modified: Tue, 25 Oct 2022 07:59:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7492531b55c893da637e0b9a8f32fd40679b4ab77d58bfbc77ecb53265a828ed`  
		Last Modified: Mon, 05 Dec 2022 21:00:12 GMT  
		Size: 76.4 MB (76436034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f615b827f5f8848516ff25f22a3e90207468b673fc217f1b93f4d34e2a4c9b`  
		Last Modified: Mon, 05 Dec 2022 21:00:04 GMT  
		Size: 21.7 MB (21673906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1709860875b5f1bb148d0068110d834fe3213c70e9b8737b2814fc0a01874645`  
		Last Modified: Mon, 05 Dec 2022 20:59:57 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7cf0d5c6ba9866cdc208048aa6a8637c2ab70997d91b7728eafafb40610fd2fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317586189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430a6894eca1853128c921cba5b2b2d2190ac62a856f619df8f706668cb643d4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 21:34:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:35:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:35:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:35:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:35:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:36:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:36:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 21:36:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:37:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:37:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:37:06 GMT
ENV ROS1_DISTRO=noetic
# Tue, 25 Oct 2022 21:37:06 GMT
ENV ROS2_DISTRO=foxy
# Tue, 25 Oct 2022 21:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:38:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:38:38 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1125e614642ae08f414585e39268e20619496243391fc14223c48efb76567fe`  
		Last Modified: Tue, 25 Oct 2022 22:06:20 GMT  
		Size: 104.5 MB (104549412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3257e5f004cfece29d48f51619b6b61a55c530aa1ecbc38e1be4208caa2ae368`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414db4c36b110ea6ec637828a4983215f3c8120f5113c6b8a1b1e7b63d490652`  
		Last Modified: Tue, 25 Oct 2022 22:06:39 GMT  
		Size: 67.7 MB (67673997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29c8a2e8faff52e903b8c6eb0d283754c1de2db5a4f0fa1c50542d8ed3bf757`  
		Last Modified: Tue, 25 Oct 2022 22:06:31 GMT  
		Size: 269.4 KB (269368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650fa392d56bb2a49e8e5ceaea16096752cb2cddfae87d9cf1a6193b59b1da7a`  
		Last Modified: Tue, 25 Oct 2022 22:06:30 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cee9901e31fd356db4bc05acd8610220bec8ba0ced72c5658083ba9b7e4d51`  
		Last Modified: Tue, 25 Oct 2022 22:06:34 GMT  
		Size: 20.4 MB (20372962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf5433e7c9e061f27cf48f334ed9ad7cc4a5ae501c1b108833008725972b866`  
		Last Modified: Tue, 25 Oct 2022 22:06:53 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb74af6d3b5c37adef97f1fd6e95e116863e798184de223195cd2bed8dcbeba2`  
		Last Modified: Tue, 25 Oct 2022 22:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f420526906050934cc358b07ad0fc7eb75f00fb532e634a89120c99fa12c4b`  
		Last Modified: Tue, 25 Oct 2022 22:07:09 GMT  
		Size: 76.5 MB (76498135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e83da535cea3510c390e46cacfb76f7c2e44b10a2a3f2a9cdeb3588df562d1`  
		Last Modified: Tue, 25 Oct 2022 22:06:56 GMT  
		Size: 14.3 MB (14323630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82106a27fefc9b7d0614542f8d3d1ca6771cf9006d3fb2a6d280abc49a689f17`  
		Last Modified: Tue, 25 Oct 2022 22:06:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:eb124a55056240f1cf593d767a41cd98f6de7d61dd4bcb40a54e45e85c46ebfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:7f3fea5f773eae8cc5ec19ac4b187c6ccdea246ebdde5f2f5cd15f0465925125
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349021297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c8ff5e9ab7d12eeafd7fb87cd290b6726657253eb5dbe4bb616f9f967713d75`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 07:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:26:27 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:26:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:26:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:27:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:27:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:27:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 07:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:28:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:28:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:28:12 GMT
ENV ROS1_DISTRO=noetic
# Tue, 25 Oct 2022 07:28:13 GMT
ENV ROS2_DISTRO=foxy
# Mon, 05 Dec 2022 20:57:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 20:57:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 20:57:49 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122af75c69e965a1d4b50e964ea95ec60ddd9997347536d0e79ecf1dc96f8e4d`  
		Last Modified: Tue, 25 Oct 2022 07:59:22 GMT  
		Size: 120.4 MB (120353945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fb29cc59034ebd9df4a3ddc0a423888144631e3a1e4b4cffff2ce4396d52ed`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5fb36af82e519ef989f9d9107e767f04c18c153572130e0f6c3a343ebb0ce0`  
		Last Modified: Tue, 25 Oct 2022 07:59:43 GMT  
		Size: 73.3 MB (73325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837655cef3c4cc06788fbad7c6df8a77081a39d3392b8bafed1ea74c35a302e3`  
		Last Modified: Tue, 25 Oct 2022 07:59:32 GMT  
		Size: 269.4 KB (269364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb41d05e0bd11afe16ecfcf7ef668e3908835201cc94fa813d0bf7783c3ba24f`  
		Last Modified: Tue, 25 Oct 2022 07:59:31 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f073c138f041e9b85ff0ddae19609c388a359370280ec72e5d549f73206c8`  
		Last Modified: Tue, 25 Oct 2022 07:59:35 GMT  
		Size: 21.7 MB (21663794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b18f13baebbb1e3f7ffc35466142e70d5913b88c27a49f5e5dbb9eab829e68e`  
		Last Modified: Tue, 25 Oct 2022 07:59:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff282c273773346a09f274c19f2310cf509f62c59ff80bf3c1831cb16577d048`  
		Last Modified: Tue, 25 Oct 2022 07:59:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7492531b55c893da637e0b9a8f32fd40679b4ab77d58bfbc77ecb53265a828ed`  
		Last Modified: Mon, 05 Dec 2022 21:00:12 GMT  
		Size: 76.4 MB (76436034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f615b827f5f8848516ff25f22a3e90207468b673fc217f1b93f4d34e2a4c9b`  
		Last Modified: Mon, 05 Dec 2022 21:00:04 GMT  
		Size: 21.7 MB (21673906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1709860875b5f1bb148d0068110d834fe3213c70e9b8737b2814fc0a01874645`  
		Last Modified: Mon, 05 Dec 2022 20:59:57 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7cf0d5c6ba9866cdc208048aa6a8637c2ab70997d91b7728eafafb40610fd2fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317586189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430a6894eca1853128c921cba5b2b2d2190ac62a856f619df8f706668cb643d4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV ROS_DISTRO=foxy
# Tue, 25 Oct 2022 21:34:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:35:02 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:35:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:35:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:35:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:36:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:36:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 21:36:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:37:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:37:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:37:06 GMT
ENV ROS1_DISTRO=noetic
# Tue, 25 Oct 2022 21:37:06 GMT
ENV ROS2_DISTRO=foxy
# Tue, 25 Oct 2022 21:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:38:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:38:38 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1125e614642ae08f414585e39268e20619496243391fc14223c48efb76567fe`  
		Last Modified: Tue, 25 Oct 2022 22:06:20 GMT  
		Size: 104.5 MB (104549412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3257e5f004cfece29d48f51619b6b61a55c530aa1ecbc38e1be4208caa2ae368`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414db4c36b110ea6ec637828a4983215f3c8120f5113c6b8a1b1e7b63d490652`  
		Last Modified: Tue, 25 Oct 2022 22:06:39 GMT  
		Size: 67.7 MB (67673997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29c8a2e8faff52e903b8c6eb0d283754c1de2db5a4f0fa1c50542d8ed3bf757`  
		Last Modified: Tue, 25 Oct 2022 22:06:31 GMT  
		Size: 269.4 KB (269368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650fa392d56bb2a49e8e5ceaea16096752cb2cddfae87d9cf1a6193b59b1da7a`  
		Last Modified: Tue, 25 Oct 2022 22:06:30 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cee9901e31fd356db4bc05acd8610220bec8ba0ced72c5658083ba9b7e4d51`  
		Last Modified: Tue, 25 Oct 2022 22:06:34 GMT  
		Size: 20.4 MB (20372962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf5433e7c9e061f27cf48f334ed9ad7cc4a5ae501c1b108833008725972b866`  
		Last Modified: Tue, 25 Oct 2022 22:06:53 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb74af6d3b5c37adef97f1fd6e95e116863e798184de223195cd2bed8dcbeba2`  
		Last Modified: Tue, 25 Oct 2022 22:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f420526906050934cc358b07ad0fc7eb75f00fb532e634a89120c99fa12c4b`  
		Last Modified: Tue, 25 Oct 2022 22:07:09 GMT  
		Size: 76.5 MB (76498135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e83da535cea3510c390e46cacfb76f7c2e44b10a2a3f2a9cdeb3588df562d1`  
		Last Modified: Tue, 25 Oct 2022 22:06:56 GMT  
		Size: 14.3 MB (14323630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82106a27fefc9b7d0614542f8d3d1ca6771cf9006d3fb2a6d280abc49a689f17`  
		Last Modified: Tue, 25 Oct 2022 22:06:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:a97603c10c099c7ea5df2f160c27bc91152964daae0e620157c6afc5a283830c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:569696e5621fad056b14672265a27fb12507999bba8a6d8dcf332d16e6a2dad1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234891739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9da8c152231c267d0724f107b91d186a7da80f21ae25d40984d9b4ce79d3985f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:29:48 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 07:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:30:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:30:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:30:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:31:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:31:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:31:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 07:31:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c34379670d69cf7211d3babcb41e5d7851c837e47be70bf7e93d4c243031e3`  
		Last Modified: Tue, 25 Oct 2022 08:00:51 GMT  
		Size: 103.9 MB (103894975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4200c5a3f7cd026b35c4c14ddd08ce81b9a8286688a9d195b89dd005dac72263`  
		Last Modified: Tue, 25 Oct 2022 08:00:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7f5b5c701916838562eb61ea9d238d42ecdcf4603217d5f36de002d875373`  
		Last Modified: Tue, 25 Oct 2022 08:01:15 GMT  
		Size: 73.3 MB (73280543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066dfb5edf358837c3acdfe4765a62b10a0588d5ee88a202f18c6decb245a6c4`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 279.6 KB (279618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81213e1334be0f25c6545b79677786f9e06c1aaea8a510b21195f4dc08b6ecac`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c4d1072c5bb0b70378dd5a649ff6468e2763e77a087f95fa4e934dfa18632e`  
		Last Modified: Tue, 25 Oct 2022 08:01:06 GMT  
		Size: 22.1 MB (22138749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:25bf046ff522cf774f874b6261fc95bc68c878db7d76f30646ecf896643d5739
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223597053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a74627c6271f818124d2fb9c79689c1b0fee39c740f2a0a6559bddf5791274e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:38:42 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 21:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:18 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:39:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:39:18 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:39:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:39:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 21:39:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17eb1844923f36e5d0264c722bf583eee704a021a2a142476d6eca76b79c5df`  
		Last Modified: Tue, 25 Oct 2022 22:07:38 GMT  
		Size: 100.3 MB (100323992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ba2f0772bc1a1a3faed0480a753c5b8806b0e6bd948fd32b6a7b378dea751`  
		Last Modified: Tue, 25 Oct 2022 22:07:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb15d0de8d57e94728781ae793ebb9c47da6af6d21a8a38c4506decc8066b63`  
		Last Modified: Tue, 25 Oct 2022 22:07:56 GMT  
		Size: 67.6 MB (67619873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7674f0c0caa8655a1368b99f006f9efd6c9309ac5fb7eb7aa609b2b0e9ceb`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 279.6 KB (279608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f136bdb9a4de4a69c2fd48d4558581abb495390dbb234332d4e4feecccbc78`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 2.4 KB (2431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5041645cebe7017ddeab3344686c7feca135348dedf51a23c6c4595ba1d2e826`  
		Last Modified: Tue, 25 Oct 2022 22:07:51 GMT  
		Size: 21.5 MB (21475535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:a97603c10c099c7ea5df2f160c27bc91152964daae0e620157c6afc5a283830c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:569696e5621fad056b14672265a27fb12507999bba8a6d8dcf332d16e6a2dad1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234891739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9da8c152231c267d0724f107b91d186a7da80f21ae25d40984d9b4ce79d3985f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:29:48 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 07:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:30:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:30:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:30:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:31:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:31:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:31:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 07:31:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c34379670d69cf7211d3babcb41e5d7851c837e47be70bf7e93d4c243031e3`  
		Last Modified: Tue, 25 Oct 2022 08:00:51 GMT  
		Size: 103.9 MB (103894975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4200c5a3f7cd026b35c4c14ddd08ce81b9a8286688a9d195b89dd005dac72263`  
		Last Modified: Tue, 25 Oct 2022 08:00:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7f5b5c701916838562eb61ea9d238d42ecdcf4603217d5f36de002d875373`  
		Last Modified: Tue, 25 Oct 2022 08:01:15 GMT  
		Size: 73.3 MB (73280543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066dfb5edf358837c3acdfe4765a62b10a0588d5ee88a202f18c6decb245a6c4`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 279.6 KB (279618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81213e1334be0f25c6545b79677786f9e06c1aaea8a510b21195f4dc08b6ecac`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c4d1072c5bb0b70378dd5a649ff6468e2763e77a087f95fa4e934dfa18632e`  
		Last Modified: Tue, 25 Oct 2022 08:01:06 GMT  
		Size: 22.1 MB (22138749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:25bf046ff522cf774f874b6261fc95bc68c878db7d76f30646ecf896643d5739
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223597053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a74627c6271f818124d2fb9c79689c1b0fee39c740f2a0a6559bddf5791274e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:38:42 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 21:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:18 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:39:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:39:18 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:39:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:39:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 21:39:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17eb1844923f36e5d0264c722bf583eee704a021a2a142476d6eca76b79c5df`  
		Last Modified: Tue, 25 Oct 2022 22:07:38 GMT  
		Size: 100.3 MB (100323992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ba2f0772bc1a1a3faed0480a753c5b8806b0e6bd948fd32b6a7b378dea751`  
		Last Modified: Tue, 25 Oct 2022 22:07:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb15d0de8d57e94728781ae793ebb9c47da6af6d21a8a38c4506decc8066b63`  
		Last Modified: Tue, 25 Oct 2022 22:07:56 GMT  
		Size: 67.6 MB (67619873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7674f0c0caa8655a1368b99f006f9efd6c9309ac5fb7eb7aa609b2b0e9ceb`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 279.6 KB (279608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f136bdb9a4de4a69c2fd48d4558581abb495390dbb234332d4e4feecccbc78`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 2.4 KB (2431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5041645cebe7017ddeab3344686c7feca135348dedf51a23c6c4595ba1d2e826`  
		Last Modified: Tue, 25 Oct 2022 22:07:51 GMT  
		Size: 21.5 MB (21475535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:a97603c10c099c7ea5df2f160c27bc91152964daae0e620157c6afc5a283830c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:569696e5621fad056b14672265a27fb12507999bba8a6d8dcf332d16e6a2dad1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234891739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9da8c152231c267d0724f107b91d186a7da80f21ae25d40984d9b4ce79d3985f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:29:48 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 07:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:30:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:30:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:30:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:31:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:31:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:31:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 07:31:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c34379670d69cf7211d3babcb41e5d7851c837e47be70bf7e93d4c243031e3`  
		Last Modified: Tue, 25 Oct 2022 08:00:51 GMT  
		Size: 103.9 MB (103894975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4200c5a3f7cd026b35c4c14ddd08ce81b9a8286688a9d195b89dd005dac72263`  
		Last Modified: Tue, 25 Oct 2022 08:00:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7f5b5c701916838562eb61ea9d238d42ecdcf4603217d5f36de002d875373`  
		Last Modified: Tue, 25 Oct 2022 08:01:15 GMT  
		Size: 73.3 MB (73280543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066dfb5edf358837c3acdfe4765a62b10a0588d5ee88a202f18c6decb245a6c4`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 279.6 KB (279618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81213e1334be0f25c6545b79677786f9e06c1aaea8a510b21195f4dc08b6ecac`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c4d1072c5bb0b70378dd5a649ff6468e2763e77a087f95fa4e934dfa18632e`  
		Last Modified: Tue, 25 Oct 2022 08:01:06 GMT  
		Size: 22.1 MB (22138749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:25bf046ff522cf774f874b6261fc95bc68c878db7d76f30646ecf896643d5739
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223597053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a74627c6271f818124d2fb9c79689c1b0fee39c740f2a0a6559bddf5791274e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:38:42 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 21:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:18 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:39:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:39:18 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:39:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:39:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 21:39:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17eb1844923f36e5d0264c722bf583eee704a021a2a142476d6eca76b79c5df`  
		Last Modified: Tue, 25 Oct 2022 22:07:38 GMT  
		Size: 100.3 MB (100323992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ba2f0772bc1a1a3faed0480a753c5b8806b0e6bd948fd32b6a7b378dea751`  
		Last Modified: Tue, 25 Oct 2022 22:07:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb15d0de8d57e94728781ae793ebb9c47da6af6d21a8a38c4506decc8066b63`  
		Last Modified: Tue, 25 Oct 2022 22:07:56 GMT  
		Size: 67.6 MB (67619873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7674f0c0caa8655a1368b99f006f9efd6c9309ac5fb7eb7aa609b2b0e9ceb`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 279.6 KB (279608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f136bdb9a4de4a69c2fd48d4558581abb495390dbb234332d4e4feecccbc78`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 2.4 KB (2431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5041645cebe7017ddeab3344686c7feca135348dedf51a23c6c4595ba1d2e826`  
		Last Modified: Tue, 25 Oct 2022 22:07:51 GMT  
		Size: 21.5 MB (21475535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:5fb1cbfdc5deeaea48407ba875002bf1cd93c858d911c9f7572e9808eb064eec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:92e1833b32530d7a5e8f72ebb1d0bffa7c492fc1d1ba6137b107f8df2c94f264
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.2 MB (139190409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9c7553e926bb17363c98f4a1766d20d7e6c10c4b439a1b3746eb1010493a86`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:29:48 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 07:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:30:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:30:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:30:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c34379670d69cf7211d3babcb41e5d7851c837e47be70bf7e93d4c243031e3`  
		Last Modified: Tue, 25 Oct 2022 08:00:51 GMT  
		Size: 103.9 MB (103894975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4200c5a3f7cd026b35c4c14ddd08ce81b9a8286688a9d195b89dd005dac72263`  
		Last Modified: Tue, 25 Oct 2022 08:00:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4d315d3003b7dfae479bc9208a5291cc9dae3cb455776c6fa52b0292dcaca2e4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134219606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f40c6313db5ac3b043e637e86bfae908df34d52dcd7c520ebf9c975de69eaf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:38:42 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 21:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:18 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:39:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:39:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17eb1844923f36e5d0264c722bf583eee704a021a2a142476d6eca76b79c5df`  
		Last Modified: Tue, 25 Oct 2022 22:07:38 GMT  
		Size: 100.3 MB (100323992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ba2f0772bc1a1a3faed0480a753c5b8806b0e6bd948fd32b6a7b378dea751`  
		Last Modified: Tue, 25 Oct 2022 22:07:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:5fb1cbfdc5deeaea48407ba875002bf1cd93c858d911c9f7572e9808eb064eec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:92e1833b32530d7a5e8f72ebb1d0bffa7c492fc1d1ba6137b107f8df2c94f264
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.2 MB (139190409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9c7553e926bb17363c98f4a1766d20d7e6c10c4b439a1b3746eb1010493a86`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:29:48 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 07:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:30:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:30:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:30:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c34379670d69cf7211d3babcb41e5d7851c837e47be70bf7e93d4c243031e3`  
		Last Modified: Tue, 25 Oct 2022 08:00:51 GMT  
		Size: 103.9 MB (103894975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4200c5a3f7cd026b35c4c14ddd08ce81b9a8286688a9d195b89dd005dac72263`  
		Last Modified: Tue, 25 Oct 2022 08:00:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4d315d3003b7dfae479bc9208a5291cc9dae3cb455776c6fa52b0292dcaca2e4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134219606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f40c6313db5ac3b043e637e86bfae908df34d52dcd7c520ebf9c975de69eaf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:38:42 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 21:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:18 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:39:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:39:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17eb1844923f36e5d0264c722bf583eee704a021a2a142476d6eca76b79c5df`  
		Last Modified: Tue, 25 Oct 2022 22:07:38 GMT  
		Size: 100.3 MB (100323992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ba2f0772bc1a1a3faed0480a753c5b8806b0e6bd948fd32b6a7b378dea751`  
		Last Modified: Tue, 25 Oct 2022 22:07:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:6b0c6cefcd881ed29f19c1f1af64f1e15743469c3d06637ac631535954bedbc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:bab22323a0214f5fa9cafb98e00fa71861f9c2d57b95aa087b2ef20eed7bbd43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.1 MB (330069416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5eb59b1f887e3059879623790ea7d4208917f30f8f460b74e07257048e2eb4d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:29:48 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 07:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:30:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:30:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:30:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:31:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:31:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:31:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 07:31:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:31:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:31:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:31:37 GMT
ENV ROS1_DISTRO=noetic
# Tue, 25 Oct 2022 07:31:37 GMT
ENV ROS2_DISTRO=galactic
# Mon, 05 Dec 2022 20:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 20:58:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 20:58:40 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c34379670d69cf7211d3babcb41e5d7851c837e47be70bf7e93d4c243031e3`  
		Last Modified: Tue, 25 Oct 2022 08:00:51 GMT  
		Size: 103.9 MB (103894975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4200c5a3f7cd026b35c4c14ddd08ce81b9a8286688a9d195b89dd005dac72263`  
		Last Modified: Tue, 25 Oct 2022 08:00:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7f5b5c701916838562eb61ea9d238d42ecdcf4603217d5f36de002d875373`  
		Last Modified: Tue, 25 Oct 2022 08:01:15 GMT  
		Size: 73.3 MB (73280543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066dfb5edf358837c3acdfe4765a62b10a0588d5ee88a202f18c6decb245a6c4`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 279.6 KB (279618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81213e1334be0f25c6545b79677786f9e06c1aaea8a510b21195f4dc08b6ecac`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c4d1072c5bb0b70378dd5a649ff6468e2763e77a087f95fa4e934dfa18632e`  
		Last Modified: Tue, 25 Oct 2022 08:01:06 GMT  
		Size: 22.1 MB (22138749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f8c44f31c8de7186a01b87fd4516c3397f99b9cd341f36f8cd884940d852be`  
		Last Modified: Tue, 25 Oct 2022 08:01:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08eb43ea9a6ec61bf6c97f1d126b6a349c84449712c18182f9bc67d4229193fe`  
		Last Modified: Tue, 25 Oct 2022 08:01:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee3bddad4ed426da9149f801e402c4e7b31092b050e28307f810faf15566d5d`  
		Last Modified: Mon, 05 Dec 2022 21:00:40 GMT  
		Size: 78.7 MB (78711799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52095e933e87e6b024c09ed3e6e8b75ed3ad78be4bb04827964a51d673b3d05b`  
		Last Modified: Mon, 05 Dec 2022 21:00:27 GMT  
		Size: 16.5 MB (16465249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658f01ec3401ce6e030e463e354d30073b745fc73a48c21d33f508e2b92e230c`  
		Last Modified: Mon, 05 Dec 2022 21:00:24 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:136867129b348b9ec08c706aa4705f734dd30b83f456847c0b548c6d6676bf26
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.3 MB (318258712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0422b9f009f34723daed7887d2deed414853709402a9d3a2f3cd23ccc15f4852`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:38:42 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 21:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:18 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:39:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:39:18 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:39:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:39:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 21:39:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:39:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:39:58 GMT
ENV ROS1_DISTRO=noetic
# Tue, 25 Oct 2022 21:39:58 GMT
ENV ROS2_DISTRO=galactic
# Tue, 25 Oct 2022 21:40:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:40:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:40:27 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17eb1844923f36e5d0264c722bf583eee704a021a2a142476d6eca76b79c5df`  
		Last Modified: Tue, 25 Oct 2022 22:07:38 GMT  
		Size: 100.3 MB (100323992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ba2f0772bc1a1a3faed0480a753c5b8806b0e6bd948fd32b6a7b378dea751`  
		Last Modified: Tue, 25 Oct 2022 22:07:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb15d0de8d57e94728781ae793ebb9c47da6af6d21a8a38c4506decc8066b63`  
		Last Modified: Tue, 25 Oct 2022 22:07:56 GMT  
		Size: 67.6 MB (67619873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7674f0c0caa8655a1368b99f006f9efd6c9309ac5fb7eb7aa609b2b0e9ceb`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 279.6 KB (279608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f136bdb9a4de4a69c2fd48d4558581abb495390dbb234332d4e4feecccbc78`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 2.4 KB (2431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5041645cebe7017ddeab3344686c7feca135348dedf51a23c6c4595ba1d2e826`  
		Last Modified: Tue, 25 Oct 2022 22:07:51 GMT  
		Size: 21.5 MB (21475535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e7a424e7ef0057fa34db63d0489365de499500ef3615cbd982ee78c0b4e674`  
		Last Modified: Tue, 25 Oct 2022 22:08:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f618329feb5073887e7596cff8d8ad3752efb4da04ddb54e58b0b42f535cda`  
		Last Modified: Tue, 25 Oct 2022 22:08:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d91e78ebff825fe8eb15f5361c4d83e75f0d88cb7e0975e4abbee79e5207c62`  
		Last Modified: Tue, 25 Oct 2022 22:08:26 GMT  
		Size: 78.7 MB (78674318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7426775b2e38908cbea672ba093ff3be1b9856e7eba27eb415ca1132e0839238`  
		Last Modified: Tue, 25 Oct 2022 22:08:12 GMT  
		Size: 16.0 MB (15986715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfa625e83a588d3f3b2bc6c4cbdf8f9e30a8af255a45ba262d8e8c83c8f3878`  
		Last Modified: Tue, 25 Oct 2022 22:08:09 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:6b0c6cefcd881ed29f19c1f1af64f1e15743469c3d06637ac631535954bedbc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:bab22323a0214f5fa9cafb98e00fa71861f9c2d57b95aa087b2ef20eed7bbd43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.1 MB (330069416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5eb59b1f887e3059879623790ea7d4208917f30f8f460b74e07257048e2eb4d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:24:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 07:24:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:29:48 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 07:30:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:30:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 07:30:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:30:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:31:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:31:09 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:31:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 07:31:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:31:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:31:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:31:37 GMT
ENV ROS1_DISTRO=noetic
# Tue, 25 Oct 2022 07:31:37 GMT
ENV ROS2_DISTRO=galactic
# Mon, 05 Dec 2022 20:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 20:58:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 20:58:40 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0589eb768011f6ff991de1d9b06aa08cf9992361dcd95dcbbd19cab6f9367571`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6d7365895cad17027328617908a6ed236d9972fefa6c1bf5af11b3b35ecb35`  
		Last Modified: Tue, 25 Oct 2022 07:59:00 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c34379670d69cf7211d3babcb41e5d7851c837e47be70bf7e93d4c243031e3`  
		Last Modified: Tue, 25 Oct 2022 08:00:51 GMT  
		Size: 103.9 MB (103894975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4200c5a3f7cd026b35c4c14ddd08ce81b9a8286688a9d195b89dd005dac72263`  
		Last Modified: Tue, 25 Oct 2022 08:00:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7f5b5c701916838562eb61ea9d238d42ecdcf4603217d5f36de002d875373`  
		Last Modified: Tue, 25 Oct 2022 08:01:15 GMT  
		Size: 73.3 MB (73280543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066dfb5edf358837c3acdfe4765a62b10a0588d5ee88a202f18c6decb245a6c4`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 279.6 KB (279618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81213e1334be0f25c6545b79677786f9e06c1aaea8a510b21195f4dc08b6ecac`  
		Last Modified: Tue, 25 Oct 2022 08:01:01 GMT  
		Size: 2.4 KB (2420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c4d1072c5bb0b70378dd5a649ff6468e2763e77a087f95fa4e934dfa18632e`  
		Last Modified: Tue, 25 Oct 2022 08:01:06 GMT  
		Size: 22.1 MB (22138749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f8c44f31c8de7186a01b87fd4516c3397f99b9cd341f36f8cd884940d852be`  
		Last Modified: Tue, 25 Oct 2022 08:01:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08eb43ea9a6ec61bf6c97f1d126b6a349c84449712c18182f9bc67d4229193fe`  
		Last Modified: Tue, 25 Oct 2022 08:01:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee3bddad4ed426da9149f801e402c4e7b31092b050e28307f810faf15566d5d`  
		Last Modified: Mon, 05 Dec 2022 21:00:40 GMT  
		Size: 78.7 MB (78711799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52095e933e87e6b024c09ed3e6e8b75ed3ad78be4bb04827964a51d673b3d05b`  
		Last Modified: Mon, 05 Dec 2022 21:00:27 GMT  
		Size: 16.5 MB (16465249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658f01ec3401ce6e030e463e354d30073b745fc73a48c21d33f508e2b92e230c`  
		Last Modified: Mon, 05 Dec 2022 21:00:24 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:136867129b348b9ec08c706aa4705f734dd30b83f456847c0b548c6d6676bf26
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.3 MB (318258712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0422b9f009f34723daed7887d2deed414853709402a9d3a2f3cd23ccc15f4852`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:33:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 25 Oct 2022 21:33:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:33:06 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:38:42 GMT
ENV ROS_DISTRO=galactic
# Tue, 25 Oct 2022 21:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:18 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 25 Oct 2022 21:39:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:39:18 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:39:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:39:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 25 Oct 2022 21:39:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:39:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:39:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:39:58 GMT
ENV ROS1_DISTRO=noetic
# Tue, 25 Oct 2022 21:39:58 GMT
ENV ROS2_DISTRO=galactic
# Tue, 25 Oct 2022 21:40:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:40:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:40:27 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bf249399bc0440c14b3771796a8a9749b00b8b1f768beabb4bf65173978661`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95e1d715258f8932e6718ed06a1eb17a823b5bb14f27e1ca7cead6b3cdb64a`  
		Last Modified: Tue, 25 Oct 2022 22:06:02 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17eb1844923f36e5d0264c722bf583eee704a021a2a142476d6eca76b79c5df`  
		Last Modified: Tue, 25 Oct 2022 22:07:38 GMT  
		Size: 100.3 MB (100323992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ba2f0772bc1a1a3faed0480a753c5b8806b0e6bd948fd32b6a7b378dea751`  
		Last Modified: Tue, 25 Oct 2022 22:07:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb15d0de8d57e94728781ae793ebb9c47da6af6d21a8a38c4506decc8066b63`  
		Last Modified: Tue, 25 Oct 2022 22:07:56 GMT  
		Size: 67.6 MB (67619873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e7674f0c0caa8655a1368b99f006f9efd6c9309ac5fb7eb7aa609b2b0e9ceb`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 279.6 KB (279608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f136bdb9a4de4a69c2fd48d4558581abb495390dbb234332d4e4feecccbc78`  
		Last Modified: Tue, 25 Oct 2022 22:07:47 GMT  
		Size: 2.4 KB (2431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5041645cebe7017ddeab3344686c7feca135348dedf51a23c6c4595ba1d2e826`  
		Last Modified: Tue, 25 Oct 2022 22:07:51 GMT  
		Size: 21.5 MB (21475535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e7a424e7ef0057fa34db63d0489365de499500ef3615cbd982ee78c0b4e674`  
		Last Modified: Tue, 25 Oct 2022 22:08:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f618329feb5073887e7596cff8d8ad3752efb4da04ddb54e58b0b42f535cda`  
		Last Modified: Tue, 25 Oct 2022 22:08:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d91e78ebff825fe8eb15f5361c4d83e75f0d88cb7e0975e4abbee79e5207c62`  
		Last Modified: Tue, 25 Oct 2022 22:08:26 GMT  
		Size: 78.7 MB (78674318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7426775b2e38908cbea672ba093ff3be1b9856e7eba27eb415ca1132e0839238`  
		Last Modified: Tue, 25 Oct 2022 22:08:12 GMT  
		Size: 16.0 MB (15986715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfa625e83a588d3f3b2bc6c4cbdf8f9e30a8af255a45ba262d8e8c83c8f3878`  
		Last Modified: Tue, 25 Oct 2022 22:08:09 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble`

```console
$ docker pull ros@sha256:4fa7f4421a72e4623b9f580b28cc8669207c72fc4b2e887bad3d564b37939552
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:9bf1a5b14fd9b2266178a5b95667fa2d8e861d335fdc9a0cdd7daf074f5939b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262837012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c144c1e970a33e387b79eb5588ae795fb1539a2de1d6a04750b10231258a960d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:07:16 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:08:48 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:08:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:08:49 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:09:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:09:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:10:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74da46ef266f8ba534cb4dde37c2da0e270d1df1225aa78548cd0ab2b59ebd3a`  
		Last Modified: Wed, 02 Nov 2022 19:24:52 GMT  
		Size: 106.2 MB (106223087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed47f73c5e60922a92b32f660f99c0fb408f814b243dc7de94ace2dee1f33a09`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0402bce15ac4ac00a43cf4b18e2406e71314ceaf39a5cc92ca1357413f87c029`  
		Last Modified: Wed, 02 Nov 2022 19:25:16 GMT  
		Size: 97.9 MB (97876837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10a5da761f7db56ec4aa72c2922ceb8350bd90d044c31e8a21e0b1ccd7ec81`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 295.6 KB (295632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74417cdbd164d16f1389679e94d83364890a14a1a7ec5ebaa726f5da444cc413`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 2.4 KB (2435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a9a4846b9f36feace908e6ce30cb0f05300da3e6854bb9b812dbbeb046f1de`  
		Last Modified: Wed, 02 Nov 2022 19:25:06 GMT  
		Size: 23.0 MB (23008159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5dcca810d0528bb38f274a1490eb803f4c87c0f33c071d05b72eb3d336c43888
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.5 MB (255534260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2de556a740eb984e38e40b39bebcfb8c41d76603a7f4e16761e928f4c755edf3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:23:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:23:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:23:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:23:07 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:23:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:24:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:24:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:24:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae686679d19077688e7d06954e6e0f6754ffebb1e29ca823f62e08f8bd45825`  
		Last Modified: Wed, 02 Nov 2022 19:39:54 GMT  
		Size: 104.0 MB (103974109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9d5bd38521973ce8aaca4d8a7e6412e7d953b8984efc2bc83877aa3d1ac27c`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470c91ae91f6f95613901a50063d68e3cff7271aa2bd22ee31e103e1a87a7b99`  
		Last Modified: Wed, 02 Nov 2022 19:40:16 GMT  
		Size: 95.5 MB (95469195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70e807f120abf970bc2df136833c1349c7c57acf3d33be8789ba4bf1f48945`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 295.6 KB (295631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6600ecdf5a14f5c94bd2a8d429da5e7f68adc291f97eb186d6be36d67d25fd3f`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba103933cf30b26056f7a3af3942ec5f3bf5f7360286f5bd562e7c6f77ade7`  
		Last Modified: Wed, 02 Nov 2022 19:40:08 GMT  
		Size: 22.4 MB (22433366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:ac3f7889fdfdcf027f34abb11e9877299d1c61008a01f641108e9a507464651c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:6cece840f8ab66e08a8441fda758b54ce0590b7a3d6c489ef3c1c199f37cbc75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1087026281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744864ebb3d7a1ee57c570755836fca4e05255db935d6d14c3fa687f4e33a43a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:07:16 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:08:48 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:08:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:08:49 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:09:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:09:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:10:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:19:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74da46ef266f8ba534cb4dde37c2da0e270d1df1225aa78548cd0ab2b59ebd3a`  
		Last Modified: Wed, 02 Nov 2022 19:24:52 GMT  
		Size: 106.2 MB (106223087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed47f73c5e60922a92b32f660f99c0fb408f814b243dc7de94ace2dee1f33a09`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0402bce15ac4ac00a43cf4b18e2406e71314ceaf39a5cc92ca1357413f87c029`  
		Last Modified: Wed, 02 Nov 2022 19:25:16 GMT  
		Size: 97.9 MB (97876837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10a5da761f7db56ec4aa72c2922ceb8350bd90d044c31e8a21e0b1ccd7ec81`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 295.6 KB (295632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74417cdbd164d16f1389679e94d83364890a14a1a7ec5ebaa726f5da444cc413`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 2.4 KB (2435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a9a4846b9f36feace908e6ce30cb0f05300da3e6854bb9b812dbbeb046f1de`  
		Last Modified: Wed, 02 Nov 2022 19:25:06 GMT  
		Size: 23.0 MB (23008159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbb23d15116fa49a9d59cbb6c218515aa6a2e585336a615e7a883ce3f9d62e`  
		Last Modified: Wed, 02 Nov 2022 19:27:11 GMT  
		Size: 824.2 MB (824189269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3fa3f8ab67a14b79335870436bb911797aa9e7d5211c5b029b4ec7ab7b62d183
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1037296258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c4073b7bfc849f242b1217083741adfc92ae66f58cc5896ec62b19a892febf3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:23:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:23:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:23:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:23:07 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:23:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:24:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:24:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:24:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:34:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae686679d19077688e7d06954e6e0f6754ffebb1e29ca823f62e08f8bd45825`  
		Last Modified: Wed, 02 Nov 2022 19:39:54 GMT  
		Size: 104.0 MB (103974109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9d5bd38521973ce8aaca4d8a7e6412e7d953b8984efc2bc83877aa3d1ac27c`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470c91ae91f6f95613901a50063d68e3cff7271aa2bd22ee31e103e1a87a7b99`  
		Last Modified: Wed, 02 Nov 2022 19:40:16 GMT  
		Size: 95.5 MB (95469195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70e807f120abf970bc2df136833c1349c7c57acf3d33be8789ba4bf1f48945`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 295.6 KB (295631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6600ecdf5a14f5c94bd2a8d429da5e7f68adc291f97eb186d6be36d67d25fd3f`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba103933cf30b26056f7a3af3942ec5f3bf5f7360286f5bd562e7c6f77ade7`  
		Last Modified: Wed, 02 Nov 2022 19:40:08 GMT  
		Size: 22.4 MB (22433366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e613da958a036d1dbb30de715173a4d739ce9a27293f153af44007015cd2052`  
		Last Modified: Wed, 02 Nov 2022 19:41:47 GMT  
		Size: 781.8 MB (781761998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:ac3f7889fdfdcf027f34abb11e9877299d1c61008a01f641108e9a507464651c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:6cece840f8ab66e08a8441fda758b54ce0590b7a3d6c489ef3c1c199f37cbc75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1087026281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744864ebb3d7a1ee57c570755836fca4e05255db935d6d14c3fa687f4e33a43a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:07:16 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:08:48 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:08:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:08:49 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:09:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:09:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:10:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:19:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74da46ef266f8ba534cb4dde37c2da0e270d1df1225aa78548cd0ab2b59ebd3a`  
		Last Modified: Wed, 02 Nov 2022 19:24:52 GMT  
		Size: 106.2 MB (106223087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed47f73c5e60922a92b32f660f99c0fb408f814b243dc7de94ace2dee1f33a09`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0402bce15ac4ac00a43cf4b18e2406e71314ceaf39a5cc92ca1357413f87c029`  
		Last Modified: Wed, 02 Nov 2022 19:25:16 GMT  
		Size: 97.9 MB (97876837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10a5da761f7db56ec4aa72c2922ceb8350bd90d044c31e8a21e0b1ccd7ec81`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 295.6 KB (295632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74417cdbd164d16f1389679e94d83364890a14a1a7ec5ebaa726f5da444cc413`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 2.4 KB (2435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a9a4846b9f36feace908e6ce30cb0f05300da3e6854bb9b812dbbeb046f1de`  
		Last Modified: Wed, 02 Nov 2022 19:25:06 GMT  
		Size: 23.0 MB (23008159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbb23d15116fa49a9d59cbb6c218515aa6a2e585336a615e7a883ce3f9d62e`  
		Last Modified: Wed, 02 Nov 2022 19:27:11 GMT  
		Size: 824.2 MB (824189269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3fa3f8ab67a14b79335870436bb911797aa9e7d5211c5b029b4ec7ab7b62d183
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1037296258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c4073b7bfc849f242b1217083741adfc92ae66f58cc5896ec62b19a892febf3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:23:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:23:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:23:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:23:07 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:23:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:24:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:24:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:24:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:34:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae686679d19077688e7d06954e6e0f6754ffebb1e29ca823f62e08f8bd45825`  
		Last Modified: Wed, 02 Nov 2022 19:39:54 GMT  
		Size: 104.0 MB (103974109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9d5bd38521973ce8aaca4d8a7e6412e7d953b8984efc2bc83877aa3d1ac27c`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470c91ae91f6f95613901a50063d68e3cff7271aa2bd22ee31e103e1a87a7b99`  
		Last Modified: Wed, 02 Nov 2022 19:40:16 GMT  
		Size: 95.5 MB (95469195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70e807f120abf970bc2df136833c1349c7c57acf3d33be8789ba4bf1f48945`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 295.6 KB (295631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6600ecdf5a14f5c94bd2a8d429da5e7f68adc291f97eb186d6be36d67d25fd3f`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba103933cf30b26056f7a3af3942ec5f3bf5f7360286f5bd562e7c6f77ade7`  
		Last Modified: Wed, 02 Nov 2022 19:40:08 GMT  
		Size: 22.4 MB (22433366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e613da958a036d1dbb30de715173a4d739ce9a27293f153af44007015cd2052`  
		Last Modified: Wed, 02 Nov 2022 19:41:47 GMT  
		Size: 781.8 MB (781761998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:4fa7f4421a72e4623b9f580b28cc8669207c72fc4b2e887bad3d564b37939552
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:9bf1a5b14fd9b2266178a5b95667fa2d8e861d335fdc9a0cdd7daf074f5939b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262837012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c144c1e970a33e387b79eb5588ae795fb1539a2de1d6a04750b10231258a960d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:07:16 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:08:48 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:08:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:08:49 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:09:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:09:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:10:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74da46ef266f8ba534cb4dde37c2da0e270d1df1225aa78548cd0ab2b59ebd3a`  
		Last Modified: Wed, 02 Nov 2022 19:24:52 GMT  
		Size: 106.2 MB (106223087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed47f73c5e60922a92b32f660f99c0fb408f814b243dc7de94ace2dee1f33a09`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0402bce15ac4ac00a43cf4b18e2406e71314ceaf39a5cc92ca1357413f87c029`  
		Last Modified: Wed, 02 Nov 2022 19:25:16 GMT  
		Size: 97.9 MB (97876837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10a5da761f7db56ec4aa72c2922ceb8350bd90d044c31e8a21e0b1ccd7ec81`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 295.6 KB (295632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74417cdbd164d16f1389679e94d83364890a14a1a7ec5ebaa726f5da444cc413`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 2.4 KB (2435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a9a4846b9f36feace908e6ce30cb0f05300da3e6854bb9b812dbbeb046f1de`  
		Last Modified: Wed, 02 Nov 2022 19:25:06 GMT  
		Size: 23.0 MB (23008159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5dcca810d0528bb38f274a1490eb803f4c87c0f33c071d05b72eb3d336c43888
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.5 MB (255534260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2de556a740eb984e38e40b39bebcfb8c41d76603a7f4e16761e928f4c755edf3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:23:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:23:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:23:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:23:07 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:23:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:24:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:24:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:24:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae686679d19077688e7d06954e6e0f6754ffebb1e29ca823f62e08f8bd45825`  
		Last Modified: Wed, 02 Nov 2022 19:39:54 GMT  
		Size: 104.0 MB (103974109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9d5bd38521973ce8aaca4d8a7e6412e7d953b8984efc2bc83877aa3d1ac27c`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470c91ae91f6f95613901a50063d68e3cff7271aa2bd22ee31e103e1a87a7b99`  
		Last Modified: Wed, 02 Nov 2022 19:40:16 GMT  
		Size: 95.5 MB (95469195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70e807f120abf970bc2df136833c1349c7c57acf3d33be8789ba4bf1f48945`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 295.6 KB (295631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6600ecdf5a14f5c94bd2a8d429da5e7f68adc291f97eb186d6be36d67d25fd3f`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba103933cf30b26056f7a3af3942ec5f3bf5f7360286f5bd562e7c6f77ade7`  
		Last Modified: Wed, 02 Nov 2022 19:40:08 GMT  
		Size: 22.4 MB (22433366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:4fa7f4421a72e4623b9f580b28cc8669207c72fc4b2e887bad3d564b37939552
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:9bf1a5b14fd9b2266178a5b95667fa2d8e861d335fdc9a0cdd7daf074f5939b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262837012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c144c1e970a33e387b79eb5588ae795fb1539a2de1d6a04750b10231258a960d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:07:16 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:08:48 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:08:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:08:49 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:09:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:09:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:10:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74da46ef266f8ba534cb4dde37c2da0e270d1df1225aa78548cd0ab2b59ebd3a`  
		Last Modified: Wed, 02 Nov 2022 19:24:52 GMT  
		Size: 106.2 MB (106223087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed47f73c5e60922a92b32f660f99c0fb408f814b243dc7de94ace2dee1f33a09`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0402bce15ac4ac00a43cf4b18e2406e71314ceaf39a5cc92ca1357413f87c029`  
		Last Modified: Wed, 02 Nov 2022 19:25:16 GMT  
		Size: 97.9 MB (97876837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10a5da761f7db56ec4aa72c2922ceb8350bd90d044c31e8a21e0b1ccd7ec81`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 295.6 KB (295632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74417cdbd164d16f1389679e94d83364890a14a1a7ec5ebaa726f5da444cc413`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 2.4 KB (2435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a9a4846b9f36feace908e6ce30cb0f05300da3e6854bb9b812dbbeb046f1de`  
		Last Modified: Wed, 02 Nov 2022 19:25:06 GMT  
		Size: 23.0 MB (23008159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5dcca810d0528bb38f274a1490eb803f4c87c0f33c071d05b72eb3d336c43888
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.5 MB (255534260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2de556a740eb984e38e40b39bebcfb8c41d76603a7f4e16761e928f4c755edf3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:23:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:23:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:23:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:23:07 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:23:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:24:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:24:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:24:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae686679d19077688e7d06954e6e0f6754ffebb1e29ca823f62e08f8bd45825`  
		Last Modified: Wed, 02 Nov 2022 19:39:54 GMT  
		Size: 104.0 MB (103974109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9d5bd38521973ce8aaca4d8a7e6412e7d953b8984efc2bc83877aa3d1ac27c`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470c91ae91f6f95613901a50063d68e3cff7271aa2bd22ee31e103e1a87a7b99`  
		Last Modified: Wed, 02 Nov 2022 19:40:16 GMT  
		Size: 95.5 MB (95469195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70e807f120abf970bc2df136833c1349c7c57acf3d33be8789ba4bf1f48945`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 295.6 KB (295631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6600ecdf5a14f5c94bd2a8d429da5e7f68adc291f97eb186d6be36d67d25fd3f`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba103933cf30b26056f7a3af3942ec5f3bf5f7360286f5bd562e7c6f77ade7`  
		Last Modified: Wed, 02 Nov 2022 19:40:08 GMT  
		Size: 22.4 MB (22433366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:6acf4ee414eb55e96cc3e02534357c0101c64b7ee81ed1ab02efc703d1bb314f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:ef150a962ad2b2bfe7dc29f22bc3eb784a041d3a0f374117d9a841780a55ee16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141653949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0cc72a40bf88f4527d256cdd115504d89e5e9c58f64683588332e63cdef1b6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:07:16 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:08:48 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:08:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:08:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74da46ef266f8ba534cb4dde37c2da0e270d1df1225aa78548cd0ab2b59ebd3a`  
		Last Modified: Wed, 02 Nov 2022 19:24:52 GMT  
		Size: 106.2 MB (106223087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed47f73c5e60922a92b32f660f99c0fb408f814b243dc7de94ace2dee1f33a09`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c5ff981860c2649a53c87d612b762dfcca19dde2f45fffc719bc73f7e4a94abf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137333659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447465179f02058eab9bbb39d630e187e25c9f7819b918ddd8de8a0c10aeaf52`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:23:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:23:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:23:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:23:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae686679d19077688e7d06954e6e0f6754ffebb1e29ca823f62e08f8bd45825`  
		Last Modified: Wed, 02 Nov 2022 19:39:54 GMT  
		Size: 104.0 MB (103974109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9d5bd38521973ce8aaca4d8a7e6412e7d953b8984efc2bc83877aa3d1ac27c`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:6acf4ee414eb55e96cc3e02534357c0101c64b7ee81ed1ab02efc703d1bb314f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:ef150a962ad2b2bfe7dc29f22bc3eb784a041d3a0f374117d9a841780a55ee16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141653949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0cc72a40bf88f4527d256cdd115504d89e5e9c58f64683588332e63cdef1b6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:07:16 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:08:48 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:08:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:08:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74da46ef266f8ba534cb4dde37c2da0e270d1df1225aa78548cd0ab2b59ebd3a`  
		Last Modified: Wed, 02 Nov 2022 19:24:52 GMT  
		Size: 106.2 MB (106223087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed47f73c5e60922a92b32f660f99c0fb408f814b243dc7de94ace2dee1f33a09`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c5ff981860c2649a53c87d612b762dfcca19dde2f45fffc719bc73f7e4a94abf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137333659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447465179f02058eab9bbb39d630e187e25c9f7819b918ddd8de8a0c10aeaf52`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:23:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:23:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:23:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:23:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae686679d19077688e7d06954e6e0f6754ffebb1e29ca823f62e08f8bd45825`  
		Last Modified: Wed, 02 Nov 2022 19:39:54 GMT  
		Size: 104.0 MB (103974109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9d5bd38521973ce8aaca4d8a7e6412e7d953b8984efc2bc83877aa3d1ac27c`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:4fa7f4421a72e4623b9f580b28cc8669207c72fc4b2e887bad3d564b37939552
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:9bf1a5b14fd9b2266178a5b95667fa2d8e861d335fdc9a0cdd7daf074f5939b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262837012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c144c1e970a33e387b79eb5588ae795fb1539a2de1d6a04750b10231258a960d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:07:16 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:08:48 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:08:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:08:49 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:09:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:09:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:10:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74da46ef266f8ba534cb4dde37c2da0e270d1df1225aa78548cd0ab2b59ebd3a`  
		Last Modified: Wed, 02 Nov 2022 19:24:52 GMT  
		Size: 106.2 MB (106223087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed47f73c5e60922a92b32f660f99c0fb408f814b243dc7de94ace2dee1f33a09`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0402bce15ac4ac00a43cf4b18e2406e71314ceaf39a5cc92ca1357413f87c029`  
		Last Modified: Wed, 02 Nov 2022 19:25:16 GMT  
		Size: 97.9 MB (97876837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10a5da761f7db56ec4aa72c2922ceb8350bd90d044c31e8a21e0b1ccd7ec81`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 295.6 KB (295632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74417cdbd164d16f1389679e94d83364890a14a1a7ec5ebaa726f5da444cc413`  
		Last Modified: Wed, 02 Nov 2022 19:25:02 GMT  
		Size: 2.4 KB (2435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a9a4846b9f36feace908e6ce30cb0f05300da3e6854bb9b812dbbeb046f1de`  
		Last Modified: Wed, 02 Nov 2022 19:25:06 GMT  
		Size: 23.0 MB (23008159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5dcca810d0528bb38f274a1490eb803f4c87c0f33c071d05b72eb3d336c43888
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.5 MB (255534260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2de556a740eb984e38e40b39bebcfb8c41d76603a7f4e16761e928f4c755edf3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV ROS_DISTRO=humble
# Wed, 02 Nov 2022 19:23:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:23:07 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:23:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:23:07 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:23:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:24:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:24:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:24:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae686679d19077688e7d06954e6e0f6754ffebb1e29ca823f62e08f8bd45825`  
		Last Modified: Wed, 02 Nov 2022 19:39:54 GMT  
		Size: 104.0 MB (103974109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9d5bd38521973ce8aaca4d8a7e6412e7d953b8984efc2bc83877aa3d1ac27c`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470c91ae91f6f95613901a50063d68e3cff7271aa2bd22ee31e103e1a87a7b99`  
		Last Modified: Wed, 02 Nov 2022 19:40:16 GMT  
		Size: 95.5 MB (95469195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70e807f120abf970bc2df136833c1349c7c57acf3d33be8789ba4bf1f48945`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 295.6 KB (295631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6600ecdf5a14f5c94bd2a8d429da5e7f68adc291f97eb186d6be36d67d25fd3f`  
		Last Modified: Wed, 02 Nov 2022 19:40:05 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba103933cf30b26056f7a3af3942ec5f3bf5f7360286f5bd562e7c6f77ade7`  
		Last Modified: Wed, 02 Nov 2022 19:40:08 GMT  
		Size: 22.4 MB (22433366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:82cf50229c1d12addba6dc05124dde705cb4839e96349fc9a1cae01632655d61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:a7201ea28800aff6b84b5fc7ab4fd80b61bc58dc006b9c2cdca6ec7be32cf6ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437538991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898998df3ed57ef16b7e130a5148adf56b94754f794c70d6f6b5c670eb939dbf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:51:42 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 06:51:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 06:55:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:55:51 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 06:55:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 06:55:51 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:56:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:56:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 06:58:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955214fb5b152d9d9fa8ce9a39b19a4e6e8ea487bc617e76c0b7b33e1881bc`  
		Last Modified: Tue, 25 Oct 2022 07:50:06 GMT  
		Size: 831.1 KB (831118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389880aa1534b94319b44ef0d7e8e52ae108ec326dc1efe1cf0e4e749a4190a`  
		Last Modified: Tue, 25 Oct 2022 07:50:04 GMT  
		Size: 4.9 MB (4877285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db68a36d4b9f8fa036da9f0c51e74b6d27dffd9d39317f42638ee84b29322668`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b325e4aad15f84b511f749de8e3b84dc88f98909bbfdd1961ac0e84f7d273f16`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ad76754b2b5a9699fc604ac8d1393dd3d6dfe21df82c8e930da67ffd6f6708`  
		Last Modified: Tue, 25 Oct 2022 07:50:52 GMT  
		Size: 259.6 MB (259567997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1318baf5e3f70ccdc707f97c58bf69e65917aadaa98ec26b67d1d2695572fa`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb834ce8392143178e871793c61a9bd2ac4e34031627b0f8d8453a1f1d836a1`  
		Last Modified: Tue, 25 Oct 2022 07:51:13 GMT  
		Size: 70.3 MB (70260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874278d4c37ef6d13abdb486dd6dfd9900b104ad68492eb5ba5df13c5c947b37`  
		Last Modified: Tue, 25 Oct 2022 07:51:03 GMT  
		Size: 289.2 KB (289160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5236595b9f2b064d0593cf222d04423eaa11b12eaa5c8e78974d822f22c23287`  
		Last Modified: Tue, 25 Oct 2022 07:51:19 GMT  
		Size: 75.0 MB (74998649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:12aab43566b2071488b4aa92c00718564fe9c214f1b5140d79c64f6c26f3941c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386028472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3609bfe5658aa0d47a0912a5414796fe5cb3657ef0bdaf25459f273c316bde`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:51 GMT
ADD file:577e89b09dccbe472d77fc02945d56a9eac3a24e20bf618c45074becfa1f49c9 in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 18:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV ROS_DISTRO=melodic
# Wed, 02 Nov 2022 19:00:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:00:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:00:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:00:23 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:01:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8cba8250122e011a113a9792b4a631b34b2aa89453e4c04090586d85464707de`  
		Last Modified: Tue, 25 Oct 2022 03:09:09 GMT  
		Size: 22.3 MB (22306283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc908b61f80477ac7791402bccbdb66903da21a17218a82598c6b5d68b42504a`  
		Last Modified: Wed, 02 Nov 2022 19:25:26 GMT  
		Size: 829.9 KB (829874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee3c131e9ae3f02652725609817aa7aeadca2d8f2d76a59d7f9264eb44e557`  
		Last Modified: Wed, 02 Nov 2022 19:25:24 GMT  
		Size: 4.1 MB (4088339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aa1a282fea46d652eaad9c87154fc787260798454ff685efa0b9f014e80211`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae6ce0e1086d82b010d3b4800835ad5cee4b4cda373a532b7915921440aaf0b`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f5c438d3cc55ffe5c481e73e0f1ee6d6ad654caa476e58a5d57c522aed267`  
		Last Modified: Wed, 02 Nov 2022 19:26:05 GMT  
		Size: 239.0 MB (239043717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fada99ba68d64cf8bce10f31ba55521c25aabf87e21a948e348c0a63ea5033`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a77d2db7252005f29e5e658434aba2b5cfd8639d128908ee57489ca6cf2818`  
		Last Modified: Wed, 02 Nov 2022 19:26:26 GMT  
		Size: 54.7 MB (54722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23db9ba1443d202279569a7e761c1cec59c0e4a55c78221b3592790683ee9f`  
		Last Modified: Wed, 02 Nov 2022 19:26:17 GMT  
		Size: 288.9 KB (288944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5d7c0964f9677840ae3fa2177c3b580272f045ba8413a33f8523d8f5a6edb9`  
		Last Modified: Wed, 02 Nov 2022 19:26:30 GMT  
		Size: 64.7 MB (64747387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a3bc1386512161551014d974ef7a92ab093f9740745a129aaf585129950f409a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412168880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9021aea3f107f10bf15a3e04d0ebc412e3119eea741be23df0d0b94c222f3b7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 20:56:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 20:57:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 21:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:01:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:01:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:01:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:02:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:02:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716808bd159516452cc1fc4db13d26965a5ea97f8fd507504f2abbd039e6b49d`  
		Last Modified: Tue, 25 Oct 2022 21:59:17 GMT  
		Size: 832.1 KB (832133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba094397f1fa2e72e998a82343d0614edda5257c98110b93a24af381630d3d31`  
		Last Modified: Tue, 25 Oct 2022 21:59:16 GMT  
		Size: 4.5 MB (4461373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282853d155ba0f593cc03d8773b2943181fe800a9fd446c6f8e70272937f7b9`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8dfb3f0f683701a85906157d325487eef9df7b6c559e3789449d02a6141051`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20849d29bb87d6b2a985fcc31e046ea130cae04137e9d346ad8322cab86170`  
		Last Modified: Tue, 25 Oct 2022 21:59:49 GMT  
		Size: 252.5 MB (252526710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90dfe4568d11bee7e54df662800278a22a50ea4a63904f366d46a49ee17f6a4`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f778aa7fa96e398ee7887d76161f1c151b67c7d0888a48c9512e86d37ba7c532`  
		Last Modified: Tue, 25 Oct 2022 22:00:07 GMT  
		Size: 63.1 MB (63091592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da590a11132a9292f690e41ddd35c007c4ad4da0e52655fad6f6ef220d97f9b7`  
		Last Modified: Tue, 25 Oct 2022 22:00:00 GMT  
		Size: 289.2 KB (289154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cb1026663e1c31e2f46024240399e38da1fd0da606460b86316cba8196c55a`  
		Last Modified: Tue, 25 Oct 2022 22:00:11 GMT  
		Size: 67.2 MB (67230215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:503650c03fbf09a2d51e36c710df66eac2f179eda19e089b48aac4e11196a505
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:760356bd129ecac893a2c56afe72c845c57258ec8d238e58be69eef50afcce0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742894003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0abbf16914f8244ac1927554743a188b63ed7ab5c73d268af3cce4073bf7d27`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:51:42 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 06:51:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 06:55:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:55:51 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 06:55:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 06:55:51 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:56:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:56:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 06:58:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955214fb5b152d9d9fa8ce9a39b19a4e6e8ea487bc617e76c0b7b33e1881bc`  
		Last Modified: Tue, 25 Oct 2022 07:50:06 GMT  
		Size: 831.1 KB (831118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389880aa1534b94319b44ef0d7e8e52ae108ec326dc1efe1cf0e4e749a4190a`  
		Last Modified: Tue, 25 Oct 2022 07:50:04 GMT  
		Size: 4.9 MB (4877285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db68a36d4b9f8fa036da9f0c51e74b6d27dffd9d39317f42638ee84b29322668`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b325e4aad15f84b511f749de8e3b84dc88f98909bbfdd1961ac0e84f7d273f16`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ad76754b2b5a9699fc604ac8d1393dd3d6dfe21df82c8e930da67ffd6f6708`  
		Last Modified: Tue, 25 Oct 2022 07:50:52 GMT  
		Size: 259.6 MB (259567997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1318baf5e3f70ccdc707f97c58bf69e65917aadaa98ec26b67d1d2695572fa`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb834ce8392143178e871793c61a9bd2ac4e34031627b0f8d8453a1f1d836a1`  
		Last Modified: Tue, 25 Oct 2022 07:51:13 GMT  
		Size: 70.3 MB (70260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874278d4c37ef6d13abdb486dd6dfd9900b104ad68492eb5ba5df13c5c947b37`  
		Last Modified: Tue, 25 Oct 2022 07:51:03 GMT  
		Size: 289.2 KB (289160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5236595b9f2b064d0593cf222d04423eaa11b12eaa5c8e78974d822f22c23287`  
		Last Modified: Tue, 25 Oct 2022 07:51:19 GMT  
		Size: 75.0 MB (74998649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5938790ff52815fa00897b4584fc3cff933821fac6b497b443f30e51552f900e`  
		Last Modified: Tue, 25 Oct 2022 07:52:42 GMT  
		Size: 305.4 MB (305355012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:a49df305bd76d5d92fadc23d79457f61892cc149bf7cd0af60cc8141cf975775
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.1 MB (646054655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:391e22eb9322f5990536c89ffb271fe4e105bca8527a4a8d25fe9831e4c78a34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:51 GMT
ADD file:577e89b09dccbe472d77fc02945d56a9eac3a24e20bf618c45074becfa1f49c9 in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 18:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV ROS_DISTRO=melodic
# Wed, 02 Nov 2022 19:00:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:00:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:00:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:00:23 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:01:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:09:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8cba8250122e011a113a9792b4a631b34b2aa89453e4c04090586d85464707de`  
		Last Modified: Tue, 25 Oct 2022 03:09:09 GMT  
		Size: 22.3 MB (22306283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc908b61f80477ac7791402bccbdb66903da21a17218a82598c6b5d68b42504a`  
		Last Modified: Wed, 02 Nov 2022 19:25:26 GMT  
		Size: 829.9 KB (829874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee3c131e9ae3f02652725609817aa7aeadca2d8f2d76a59d7f9264eb44e557`  
		Last Modified: Wed, 02 Nov 2022 19:25:24 GMT  
		Size: 4.1 MB (4088339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aa1a282fea46d652eaad9c87154fc787260798454ff685efa0b9f014e80211`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae6ce0e1086d82b010d3b4800835ad5cee4b4cda373a532b7915921440aaf0b`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f5c438d3cc55ffe5c481e73e0f1ee6d6ad654caa476e58a5d57c522aed267`  
		Last Modified: Wed, 02 Nov 2022 19:26:05 GMT  
		Size: 239.0 MB (239043717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fada99ba68d64cf8bce10f31ba55521c25aabf87e21a948e348c0a63ea5033`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a77d2db7252005f29e5e658434aba2b5cfd8639d128908ee57489ca6cf2818`  
		Last Modified: Wed, 02 Nov 2022 19:26:26 GMT  
		Size: 54.7 MB (54722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23db9ba1443d202279569a7e761c1cec59c0e4a55c78221b3592790683ee9f`  
		Last Modified: Wed, 02 Nov 2022 19:26:17 GMT  
		Size: 288.9 KB (288944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5d7c0964f9677840ae3fa2177c3b580272f045ba8413a33f8523d8f5a6edb9`  
		Last Modified: Wed, 02 Nov 2022 19:26:30 GMT  
		Size: 64.7 MB (64747387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e3dd07ae35371b865a646b287af96ae1cd851398f92a933bca32fe22f0596e`  
		Last Modified: Wed, 02 Nov 2022 19:27:46 GMT  
		Size: 260.0 MB (260026183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7809a857fa2d5937dd531dc6039e24134bba59233db5ed5d3120cc50f20f2f93
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.8 MB (703837400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e338d4cfe1123c4dd3b263398b0d267137e181241fc40cd1a6fb767ffe3dd78`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 20:56:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 20:57:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 21:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:01:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:01:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:01:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:02:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:02:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:10:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716808bd159516452cc1fc4db13d26965a5ea97f8fd507504f2abbd039e6b49d`  
		Last Modified: Tue, 25 Oct 2022 21:59:17 GMT  
		Size: 832.1 KB (832133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba094397f1fa2e72e998a82343d0614edda5257c98110b93a24af381630d3d31`  
		Last Modified: Tue, 25 Oct 2022 21:59:16 GMT  
		Size: 4.5 MB (4461373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282853d155ba0f593cc03d8773b2943181fe800a9fd446c6f8e70272937f7b9`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8dfb3f0f683701a85906157d325487eef9df7b6c559e3789449d02a6141051`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20849d29bb87d6b2a985fcc31e046ea130cae04137e9d346ad8322cab86170`  
		Last Modified: Tue, 25 Oct 2022 21:59:49 GMT  
		Size: 252.5 MB (252526710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90dfe4568d11bee7e54df662800278a22a50ea4a63904f366d46a49ee17f6a4`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f778aa7fa96e398ee7887d76161f1c151b67c7d0888a48c9512e86d37ba7c532`  
		Last Modified: Tue, 25 Oct 2022 22:00:07 GMT  
		Size: 63.1 MB (63091592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da590a11132a9292f690e41ddd35c007c4ad4da0e52655fad6f6ef220d97f9b7`  
		Last Modified: Tue, 25 Oct 2022 22:00:00 GMT  
		Size: 289.2 KB (289154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cb1026663e1c31e2f46024240399e38da1fd0da606460b86316cba8196c55a`  
		Last Modified: Tue, 25 Oct 2022 22:00:11 GMT  
		Size: 67.2 MB (67230215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d15817f04bd3a686b3a1d656bf22fa94a4a7522e64e30e5d667807bf05b3051`  
		Last Modified: Tue, 25 Oct 2022 22:01:14 GMT  
		Size: 291.7 MB (291668520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:503650c03fbf09a2d51e36c710df66eac2f179eda19e089b48aac4e11196a505
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:760356bd129ecac893a2c56afe72c845c57258ec8d238e58be69eef50afcce0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742894003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0abbf16914f8244ac1927554743a188b63ed7ab5c73d268af3cce4073bf7d27`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:51:42 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 06:51:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 06:55:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:55:51 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 06:55:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 06:55:51 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:56:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:56:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 06:58:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955214fb5b152d9d9fa8ce9a39b19a4e6e8ea487bc617e76c0b7b33e1881bc`  
		Last Modified: Tue, 25 Oct 2022 07:50:06 GMT  
		Size: 831.1 KB (831118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389880aa1534b94319b44ef0d7e8e52ae108ec326dc1efe1cf0e4e749a4190a`  
		Last Modified: Tue, 25 Oct 2022 07:50:04 GMT  
		Size: 4.9 MB (4877285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db68a36d4b9f8fa036da9f0c51e74b6d27dffd9d39317f42638ee84b29322668`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b325e4aad15f84b511f749de8e3b84dc88f98909bbfdd1961ac0e84f7d273f16`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ad76754b2b5a9699fc604ac8d1393dd3d6dfe21df82c8e930da67ffd6f6708`  
		Last Modified: Tue, 25 Oct 2022 07:50:52 GMT  
		Size: 259.6 MB (259567997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1318baf5e3f70ccdc707f97c58bf69e65917aadaa98ec26b67d1d2695572fa`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb834ce8392143178e871793c61a9bd2ac4e34031627b0f8d8453a1f1d836a1`  
		Last Modified: Tue, 25 Oct 2022 07:51:13 GMT  
		Size: 70.3 MB (70260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874278d4c37ef6d13abdb486dd6dfd9900b104ad68492eb5ba5df13c5c947b37`  
		Last Modified: Tue, 25 Oct 2022 07:51:03 GMT  
		Size: 289.2 KB (289160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5236595b9f2b064d0593cf222d04423eaa11b12eaa5c8e78974d822f22c23287`  
		Last Modified: Tue, 25 Oct 2022 07:51:19 GMT  
		Size: 75.0 MB (74998649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5938790ff52815fa00897b4584fc3cff933821fac6b497b443f30e51552f900e`  
		Last Modified: Tue, 25 Oct 2022 07:52:42 GMT  
		Size: 305.4 MB (305355012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:a49df305bd76d5d92fadc23d79457f61892cc149bf7cd0af60cc8141cf975775
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.1 MB (646054655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:391e22eb9322f5990536c89ffb271fe4e105bca8527a4a8d25fe9831e4c78a34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:51 GMT
ADD file:577e89b09dccbe472d77fc02945d56a9eac3a24e20bf618c45074becfa1f49c9 in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 18:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV ROS_DISTRO=melodic
# Wed, 02 Nov 2022 19:00:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:00:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:00:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:00:23 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:01:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:09:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8cba8250122e011a113a9792b4a631b34b2aa89453e4c04090586d85464707de`  
		Last Modified: Tue, 25 Oct 2022 03:09:09 GMT  
		Size: 22.3 MB (22306283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc908b61f80477ac7791402bccbdb66903da21a17218a82598c6b5d68b42504a`  
		Last Modified: Wed, 02 Nov 2022 19:25:26 GMT  
		Size: 829.9 KB (829874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee3c131e9ae3f02652725609817aa7aeadca2d8f2d76a59d7f9264eb44e557`  
		Last Modified: Wed, 02 Nov 2022 19:25:24 GMT  
		Size: 4.1 MB (4088339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aa1a282fea46d652eaad9c87154fc787260798454ff685efa0b9f014e80211`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae6ce0e1086d82b010d3b4800835ad5cee4b4cda373a532b7915921440aaf0b`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f5c438d3cc55ffe5c481e73e0f1ee6d6ad654caa476e58a5d57c522aed267`  
		Last Modified: Wed, 02 Nov 2022 19:26:05 GMT  
		Size: 239.0 MB (239043717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fada99ba68d64cf8bce10f31ba55521c25aabf87e21a948e348c0a63ea5033`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a77d2db7252005f29e5e658434aba2b5cfd8639d128908ee57489ca6cf2818`  
		Last Modified: Wed, 02 Nov 2022 19:26:26 GMT  
		Size: 54.7 MB (54722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23db9ba1443d202279569a7e761c1cec59c0e4a55c78221b3592790683ee9f`  
		Last Modified: Wed, 02 Nov 2022 19:26:17 GMT  
		Size: 288.9 KB (288944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5d7c0964f9677840ae3fa2177c3b580272f045ba8413a33f8523d8f5a6edb9`  
		Last Modified: Wed, 02 Nov 2022 19:26:30 GMT  
		Size: 64.7 MB (64747387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e3dd07ae35371b865a646b287af96ae1cd851398f92a933bca32fe22f0596e`  
		Last Modified: Wed, 02 Nov 2022 19:27:46 GMT  
		Size: 260.0 MB (260026183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7809a857fa2d5937dd531dc6039e24134bba59233db5ed5d3120cc50f20f2f93
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.8 MB (703837400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e338d4cfe1123c4dd3b263398b0d267137e181241fc40cd1a6fb767ffe3dd78`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 20:56:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 20:57:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 21:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:01:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:01:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:01:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:02:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:02:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:10:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716808bd159516452cc1fc4db13d26965a5ea97f8fd507504f2abbd039e6b49d`  
		Last Modified: Tue, 25 Oct 2022 21:59:17 GMT  
		Size: 832.1 KB (832133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba094397f1fa2e72e998a82343d0614edda5257c98110b93a24af381630d3d31`  
		Last Modified: Tue, 25 Oct 2022 21:59:16 GMT  
		Size: 4.5 MB (4461373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282853d155ba0f593cc03d8773b2943181fe800a9fd446c6f8e70272937f7b9`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8dfb3f0f683701a85906157d325487eef9df7b6c559e3789449d02a6141051`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20849d29bb87d6b2a985fcc31e046ea130cae04137e9d346ad8322cab86170`  
		Last Modified: Tue, 25 Oct 2022 21:59:49 GMT  
		Size: 252.5 MB (252526710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90dfe4568d11bee7e54df662800278a22a50ea4a63904f366d46a49ee17f6a4`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f778aa7fa96e398ee7887d76161f1c151b67c7d0888a48c9512e86d37ba7c532`  
		Last Modified: Tue, 25 Oct 2022 22:00:07 GMT  
		Size: 63.1 MB (63091592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da590a11132a9292f690e41ddd35c007c4ad4da0e52655fad6f6ef220d97f9b7`  
		Last Modified: Tue, 25 Oct 2022 22:00:00 GMT  
		Size: 289.2 KB (289154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cb1026663e1c31e2f46024240399e38da1fd0da606460b86316cba8196c55a`  
		Last Modified: Tue, 25 Oct 2022 22:00:11 GMT  
		Size: 67.2 MB (67230215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d15817f04bd3a686b3a1d656bf22fa94a4a7522e64e30e5d667807bf05b3051`  
		Last Modified: Tue, 25 Oct 2022 22:01:14 GMT  
		Size: 291.7 MB (291668520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:9ed05c1b82301331bd41fdbed05477892f9d4c0167faac144fa139ba4201d8ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:7fb936bf3f4c1f768981550fbafaa6e7b7b43f00d4d95b05798c4f78962cb349
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448624983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56880250050883f30db34a14ba89363854f201ded84b8f75d95611f26b8a787`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:51:42 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 06:51:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 06:55:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:55:51 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 06:55:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 06:55:51 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:56:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:56:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 06:58:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:58:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955214fb5b152d9d9fa8ce9a39b19a4e6e8ea487bc617e76c0b7b33e1881bc`  
		Last Modified: Tue, 25 Oct 2022 07:50:06 GMT  
		Size: 831.1 KB (831118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389880aa1534b94319b44ef0d7e8e52ae108ec326dc1efe1cf0e4e749a4190a`  
		Last Modified: Tue, 25 Oct 2022 07:50:04 GMT  
		Size: 4.9 MB (4877285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db68a36d4b9f8fa036da9f0c51e74b6d27dffd9d39317f42638ee84b29322668`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b325e4aad15f84b511f749de8e3b84dc88f98909bbfdd1961ac0e84f7d273f16`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ad76754b2b5a9699fc604ac8d1393dd3d6dfe21df82c8e930da67ffd6f6708`  
		Last Modified: Tue, 25 Oct 2022 07:50:52 GMT  
		Size: 259.6 MB (259567997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1318baf5e3f70ccdc707f97c58bf69e65917aadaa98ec26b67d1d2695572fa`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb834ce8392143178e871793c61a9bd2ac4e34031627b0f8d8453a1f1d836a1`  
		Last Modified: Tue, 25 Oct 2022 07:51:13 GMT  
		Size: 70.3 MB (70260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874278d4c37ef6d13abdb486dd6dfd9900b104ad68492eb5ba5df13c5c947b37`  
		Last Modified: Tue, 25 Oct 2022 07:51:03 GMT  
		Size: 289.2 KB (289160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5236595b9f2b064d0593cf222d04423eaa11b12eaa5c8e78974d822f22c23287`  
		Last Modified: Tue, 25 Oct 2022 07:51:19 GMT  
		Size: 75.0 MB (74998649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04787df350a9858b29dcd5d866d17be1b134ac05697019c51a96201ec3a86463`  
		Last Modified: Tue, 25 Oct 2022 07:51:34 GMT  
		Size: 11.1 MB (11085992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:60bce79ba350d9a7744bd3b91b55eb70f15c117d0ac4caf01c2050e0f91d29e4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396150904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a74fb4f5eae084f0a2dfd86d39793b94478c263531f90387a4b2b49623a9195`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:51 GMT
ADD file:577e89b09dccbe472d77fc02945d56a9eac3a24e20bf618c45074becfa1f49c9 in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 18:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV ROS_DISTRO=melodic
# Wed, 02 Nov 2022 19:00:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:00:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:00:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:00:23 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:01:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8cba8250122e011a113a9792b4a631b34b2aa89453e4c04090586d85464707de`  
		Last Modified: Tue, 25 Oct 2022 03:09:09 GMT  
		Size: 22.3 MB (22306283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc908b61f80477ac7791402bccbdb66903da21a17218a82598c6b5d68b42504a`  
		Last Modified: Wed, 02 Nov 2022 19:25:26 GMT  
		Size: 829.9 KB (829874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee3c131e9ae3f02652725609817aa7aeadca2d8f2d76a59d7f9264eb44e557`  
		Last Modified: Wed, 02 Nov 2022 19:25:24 GMT  
		Size: 4.1 MB (4088339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aa1a282fea46d652eaad9c87154fc787260798454ff685efa0b9f014e80211`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae6ce0e1086d82b010d3b4800835ad5cee4b4cda373a532b7915921440aaf0b`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f5c438d3cc55ffe5c481e73e0f1ee6d6ad654caa476e58a5d57c522aed267`  
		Last Modified: Wed, 02 Nov 2022 19:26:05 GMT  
		Size: 239.0 MB (239043717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fada99ba68d64cf8bce10f31ba55521c25aabf87e21a948e348c0a63ea5033`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a77d2db7252005f29e5e658434aba2b5cfd8639d128908ee57489ca6cf2818`  
		Last Modified: Wed, 02 Nov 2022 19:26:26 GMT  
		Size: 54.7 MB (54722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23db9ba1443d202279569a7e761c1cec59c0e4a55c78221b3592790683ee9f`  
		Last Modified: Wed, 02 Nov 2022 19:26:17 GMT  
		Size: 288.9 KB (288944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5d7c0964f9677840ae3fa2177c3b580272f045ba8413a33f8523d8f5a6edb9`  
		Last Modified: Wed, 02 Nov 2022 19:26:30 GMT  
		Size: 64.7 MB (64747387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc2220575faa963a59498a58cd42d5586c34cd46ab64242b92384017653c6a6`  
		Last Modified: Wed, 02 Nov 2022 19:26:49 GMT  
		Size: 10.1 MB (10122432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2826cb95ef557c971ab9ff9e05ac0d9bf8e5803e9fcab9c4ea183188916e8899
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422909619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6553320dee30456380867da2c2c527fe0a5dcf416fa8f246f11a3c100295005a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 20:56:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 20:57:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 21:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:01:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:01:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:01:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:02:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:02:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:04:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716808bd159516452cc1fc4db13d26965a5ea97f8fd507504f2abbd039e6b49d`  
		Last Modified: Tue, 25 Oct 2022 21:59:17 GMT  
		Size: 832.1 KB (832133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba094397f1fa2e72e998a82343d0614edda5257c98110b93a24af381630d3d31`  
		Last Modified: Tue, 25 Oct 2022 21:59:16 GMT  
		Size: 4.5 MB (4461373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282853d155ba0f593cc03d8773b2943181fe800a9fd446c6f8e70272937f7b9`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8dfb3f0f683701a85906157d325487eef9df7b6c559e3789449d02a6141051`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20849d29bb87d6b2a985fcc31e046ea130cae04137e9d346ad8322cab86170`  
		Last Modified: Tue, 25 Oct 2022 21:59:49 GMT  
		Size: 252.5 MB (252526710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90dfe4568d11bee7e54df662800278a22a50ea4a63904f366d46a49ee17f6a4`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f778aa7fa96e398ee7887d76161f1c151b67c7d0888a48c9512e86d37ba7c532`  
		Last Modified: Tue, 25 Oct 2022 22:00:07 GMT  
		Size: 63.1 MB (63091592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da590a11132a9292f690e41ddd35c007c4ad4da0e52655fad6f6ef220d97f9b7`  
		Last Modified: Tue, 25 Oct 2022 22:00:00 GMT  
		Size: 289.2 KB (289154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cb1026663e1c31e2f46024240399e38da1fd0da606460b86316cba8196c55a`  
		Last Modified: Tue, 25 Oct 2022 22:00:11 GMT  
		Size: 67.2 MB (67230215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3212a29689ef6acf47341018b771b6536b1f595d3096d92409420d7bce7996`  
		Last Modified: Tue, 25 Oct 2022 22:00:25 GMT  
		Size: 10.7 MB (10740739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:9ed05c1b82301331bd41fdbed05477892f9d4c0167faac144fa139ba4201d8ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:7fb936bf3f4c1f768981550fbafaa6e7b7b43f00d4d95b05798c4f78962cb349
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448624983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56880250050883f30db34a14ba89363854f201ded84b8f75d95611f26b8a787`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:51:42 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 06:51:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 06:55:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:55:51 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 06:55:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 06:55:51 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:56:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:56:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 06:58:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:58:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955214fb5b152d9d9fa8ce9a39b19a4e6e8ea487bc617e76c0b7b33e1881bc`  
		Last Modified: Tue, 25 Oct 2022 07:50:06 GMT  
		Size: 831.1 KB (831118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389880aa1534b94319b44ef0d7e8e52ae108ec326dc1efe1cf0e4e749a4190a`  
		Last Modified: Tue, 25 Oct 2022 07:50:04 GMT  
		Size: 4.9 MB (4877285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db68a36d4b9f8fa036da9f0c51e74b6d27dffd9d39317f42638ee84b29322668`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b325e4aad15f84b511f749de8e3b84dc88f98909bbfdd1961ac0e84f7d273f16`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ad76754b2b5a9699fc604ac8d1393dd3d6dfe21df82c8e930da67ffd6f6708`  
		Last Modified: Tue, 25 Oct 2022 07:50:52 GMT  
		Size: 259.6 MB (259567997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1318baf5e3f70ccdc707f97c58bf69e65917aadaa98ec26b67d1d2695572fa`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb834ce8392143178e871793c61a9bd2ac4e34031627b0f8d8453a1f1d836a1`  
		Last Modified: Tue, 25 Oct 2022 07:51:13 GMT  
		Size: 70.3 MB (70260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874278d4c37ef6d13abdb486dd6dfd9900b104ad68492eb5ba5df13c5c947b37`  
		Last Modified: Tue, 25 Oct 2022 07:51:03 GMT  
		Size: 289.2 KB (289160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5236595b9f2b064d0593cf222d04423eaa11b12eaa5c8e78974d822f22c23287`  
		Last Modified: Tue, 25 Oct 2022 07:51:19 GMT  
		Size: 75.0 MB (74998649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04787df350a9858b29dcd5d866d17be1b134ac05697019c51a96201ec3a86463`  
		Last Modified: Tue, 25 Oct 2022 07:51:34 GMT  
		Size: 11.1 MB (11085992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:60bce79ba350d9a7744bd3b91b55eb70f15c117d0ac4caf01c2050e0f91d29e4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396150904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a74fb4f5eae084f0a2dfd86d39793b94478c263531f90387a4b2b49623a9195`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:51 GMT
ADD file:577e89b09dccbe472d77fc02945d56a9eac3a24e20bf618c45074becfa1f49c9 in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 18:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV ROS_DISTRO=melodic
# Wed, 02 Nov 2022 19:00:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:00:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:00:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:00:23 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:01:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8cba8250122e011a113a9792b4a631b34b2aa89453e4c04090586d85464707de`  
		Last Modified: Tue, 25 Oct 2022 03:09:09 GMT  
		Size: 22.3 MB (22306283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc908b61f80477ac7791402bccbdb66903da21a17218a82598c6b5d68b42504a`  
		Last Modified: Wed, 02 Nov 2022 19:25:26 GMT  
		Size: 829.9 KB (829874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee3c131e9ae3f02652725609817aa7aeadca2d8f2d76a59d7f9264eb44e557`  
		Last Modified: Wed, 02 Nov 2022 19:25:24 GMT  
		Size: 4.1 MB (4088339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aa1a282fea46d652eaad9c87154fc787260798454ff685efa0b9f014e80211`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae6ce0e1086d82b010d3b4800835ad5cee4b4cda373a532b7915921440aaf0b`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f5c438d3cc55ffe5c481e73e0f1ee6d6ad654caa476e58a5d57c522aed267`  
		Last Modified: Wed, 02 Nov 2022 19:26:05 GMT  
		Size: 239.0 MB (239043717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fada99ba68d64cf8bce10f31ba55521c25aabf87e21a948e348c0a63ea5033`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a77d2db7252005f29e5e658434aba2b5cfd8639d128908ee57489ca6cf2818`  
		Last Modified: Wed, 02 Nov 2022 19:26:26 GMT  
		Size: 54.7 MB (54722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23db9ba1443d202279569a7e761c1cec59c0e4a55c78221b3592790683ee9f`  
		Last Modified: Wed, 02 Nov 2022 19:26:17 GMT  
		Size: 288.9 KB (288944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5d7c0964f9677840ae3fa2177c3b580272f045ba8413a33f8523d8f5a6edb9`  
		Last Modified: Wed, 02 Nov 2022 19:26:30 GMT  
		Size: 64.7 MB (64747387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc2220575faa963a59498a58cd42d5586c34cd46ab64242b92384017653c6a6`  
		Last Modified: Wed, 02 Nov 2022 19:26:49 GMT  
		Size: 10.1 MB (10122432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2826cb95ef557c971ab9ff9e05ac0d9bf8e5803e9fcab9c4ea183188916e8899
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422909619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6553320dee30456380867da2c2c527fe0a5dcf416fa8f246f11a3c100295005a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 20:56:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 20:57:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 21:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:01:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:01:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:01:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:02:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:02:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:04:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716808bd159516452cc1fc4db13d26965a5ea97f8fd507504f2abbd039e6b49d`  
		Last Modified: Tue, 25 Oct 2022 21:59:17 GMT  
		Size: 832.1 KB (832133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba094397f1fa2e72e998a82343d0614edda5257c98110b93a24af381630d3d31`  
		Last Modified: Tue, 25 Oct 2022 21:59:16 GMT  
		Size: 4.5 MB (4461373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282853d155ba0f593cc03d8773b2943181fe800a9fd446c6f8e70272937f7b9`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8dfb3f0f683701a85906157d325487eef9df7b6c559e3789449d02a6141051`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20849d29bb87d6b2a985fcc31e046ea130cae04137e9d346ad8322cab86170`  
		Last Modified: Tue, 25 Oct 2022 21:59:49 GMT  
		Size: 252.5 MB (252526710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90dfe4568d11bee7e54df662800278a22a50ea4a63904f366d46a49ee17f6a4`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f778aa7fa96e398ee7887d76161f1c151b67c7d0888a48c9512e86d37ba7c532`  
		Last Modified: Tue, 25 Oct 2022 22:00:07 GMT  
		Size: 63.1 MB (63091592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da590a11132a9292f690e41ddd35c007c4ad4da0e52655fad6f6ef220d97f9b7`  
		Last Modified: Tue, 25 Oct 2022 22:00:00 GMT  
		Size: 289.2 KB (289154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cb1026663e1c31e2f46024240399e38da1fd0da606460b86316cba8196c55a`  
		Last Modified: Tue, 25 Oct 2022 22:00:11 GMT  
		Size: 67.2 MB (67230215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3212a29689ef6acf47341018b771b6536b1f595d3096d92409420d7bce7996`  
		Last Modified: Tue, 25 Oct 2022 22:00:25 GMT  
		Size: 10.7 MB (10740739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:82cf50229c1d12addba6dc05124dde705cb4839e96349fc9a1cae01632655d61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:a7201ea28800aff6b84b5fc7ab4fd80b61bc58dc006b9c2cdca6ec7be32cf6ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437538991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898998df3ed57ef16b7e130a5148adf56b94754f794c70d6f6b5c670eb939dbf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:51:42 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 06:51:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 06:55:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:55:51 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 06:55:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 06:55:51 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:56:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:56:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 06:58:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955214fb5b152d9d9fa8ce9a39b19a4e6e8ea487bc617e76c0b7b33e1881bc`  
		Last Modified: Tue, 25 Oct 2022 07:50:06 GMT  
		Size: 831.1 KB (831118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389880aa1534b94319b44ef0d7e8e52ae108ec326dc1efe1cf0e4e749a4190a`  
		Last Modified: Tue, 25 Oct 2022 07:50:04 GMT  
		Size: 4.9 MB (4877285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db68a36d4b9f8fa036da9f0c51e74b6d27dffd9d39317f42638ee84b29322668`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b325e4aad15f84b511f749de8e3b84dc88f98909bbfdd1961ac0e84f7d273f16`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ad76754b2b5a9699fc604ac8d1393dd3d6dfe21df82c8e930da67ffd6f6708`  
		Last Modified: Tue, 25 Oct 2022 07:50:52 GMT  
		Size: 259.6 MB (259567997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1318baf5e3f70ccdc707f97c58bf69e65917aadaa98ec26b67d1d2695572fa`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb834ce8392143178e871793c61a9bd2ac4e34031627b0f8d8453a1f1d836a1`  
		Last Modified: Tue, 25 Oct 2022 07:51:13 GMT  
		Size: 70.3 MB (70260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874278d4c37ef6d13abdb486dd6dfd9900b104ad68492eb5ba5df13c5c947b37`  
		Last Modified: Tue, 25 Oct 2022 07:51:03 GMT  
		Size: 289.2 KB (289160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5236595b9f2b064d0593cf222d04423eaa11b12eaa5c8e78974d822f22c23287`  
		Last Modified: Tue, 25 Oct 2022 07:51:19 GMT  
		Size: 75.0 MB (74998649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:12aab43566b2071488b4aa92c00718564fe9c214f1b5140d79c64f6c26f3941c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386028472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3609bfe5658aa0d47a0912a5414796fe5cb3657ef0bdaf25459f273c316bde`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:51 GMT
ADD file:577e89b09dccbe472d77fc02945d56a9eac3a24e20bf618c45074becfa1f49c9 in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 18:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV ROS_DISTRO=melodic
# Wed, 02 Nov 2022 19:00:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:00:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:00:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:00:23 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:01:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8cba8250122e011a113a9792b4a631b34b2aa89453e4c04090586d85464707de`  
		Last Modified: Tue, 25 Oct 2022 03:09:09 GMT  
		Size: 22.3 MB (22306283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc908b61f80477ac7791402bccbdb66903da21a17218a82598c6b5d68b42504a`  
		Last Modified: Wed, 02 Nov 2022 19:25:26 GMT  
		Size: 829.9 KB (829874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee3c131e9ae3f02652725609817aa7aeadca2d8f2d76a59d7f9264eb44e557`  
		Last Modified: Wed, 02 Nov 2022 19:25:24 GMT  
		Size: 4.1 MB (4088339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aa1a282fea46d652eaad9c87154fc787260798454ff685efa0b9f014e80211`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae6ce0e1086d82b010d3b4800835ad5cee4b4cda373a532b7915921440aaf0b`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f5c438d3cc55ffe5c481e73e0f1ee6d6ad654caa476e58a5d57c522aed267`  
		Last Modified: Wed, 02 Nov 2022 19:26:05 GMT  
		Size: 239.0 MB (239043717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fada99ba68d64cf8bce10f31ba55521c25aabf87e21a948e348c0a63ea5033`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a77d2db7252005f29e5e658434aba2b5cfd8639d128908ee57489ca6cf2818`  
		Last Modified: Wed, 02 Nov 2022 19:26:26 GMT  
		Size: 54.7 MB (54722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23db9ba1443d202279569a7e761c1cec59c0e4a55c78221b3592790683ee9f`  
		Last Modified: Wed, 02 Nov 2022 19:26:17 GMT  
		Size: 288.9 KB (288944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5d7c0964f9677840ae3fa2177c3b580272f045ba8413a33f8523d8f5a6edb9`  
		Last Modified: Wed, 02 Nov 2022 19:26:30 GMT  
		Size: 64.7 MB (64747387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a3bc1386512161551014d974ef7a92ab093f9740745a129aaf585129950f409a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412168880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9021aea3f107f10bf15a3e04d0ebc412e3119eea741be23df0d0b94c222f3b7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 20:56:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 20:57:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 21:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:01:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:01:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:01:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:02:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:02:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716808bd159516452cc1fc4db13d26965a5ea97f8fd507504f2abbd039e6b49d`  
		Last Modified: Tue, 25 Oct 2022 21:59:17 GMT  
		Size: 832.1 KB (832133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba094397f1fa2e72e998a82343d0614edda5257c98110b93a24af381630d3d31`  
		Last Modified: Tue, 25 Oct 2022 21:59:16 GMT  
		Size: 4.5 MB (4461373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282853d155ba0f593cc03d8773b2943181fe800a9fd446c6f8e70272937f7b9`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8dfb3f0f683701a85906157d325487eef9df7b6c559e3789449d02a6141051`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20849d29bb87d6b2a985fcc31e046ea130cae04137e9d346ad8322cab86170`  
		Last Modified: Tue, 25 Oct 2022 21:59:49 GMT  
		Size: 252.5 MB (252526710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90dfe4568d11bee7e54df662800278a22a50ea4a63904f366d46a49ee17f6a4`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f778aa7fa96e398ee7887d76161f1c151b67c7d0888a48c9512e86d37ba7c532`  
		Last Modified: Tue, 25 Oct 2022 22:00:07 GMT  
		Size: 63.1 MB (63091592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da590a11132a9292f690e41ddd35c007c4ad4da0e52655fad6f6ef220d97f9b7`  
		Last Modified: Tue, 25 Oct 2022 22:00:00 GMT  
		Size: 289.2 KB (289154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cb1026663e1c31e2f46024240399e38da1fd0da606460b86316cba8196c55a`  
		Last Modified: Tue, 25 Oct 2022 22:00:11 GMT  
		Size: 67.2 MB (67230215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:82cf50229c1d12addba6dc05124dde705cb4839e96349fc9a1cae01632655d61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:a7201ea28800aff6b84b5fc7ab4fd80b61bc58dc006b9c2cdca6ec7be32cf6ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437538991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898998df3ed57ef16b7e130a5148adf56b94754f794c70d6f6b5c670eb939dbf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:51:42 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 06:51:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 06:55:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:55:51 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 06:55:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 06:55:51 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:56:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:56:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 06:58:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955214fb5b152d9d9fa8ce9a39b19a4e6e8ea487bc617e76c0b7b33e1881bc`  
		Last Modified: Tue, 25 Oct 2022 07:50:06 GMT  
		Size: 831.1 KB (831118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389880aa1534b94319b44ef0d7e8e52ae108ec326dc1efe1cf0e4e749a4190a`  
		Last Modified: Tue, 25 Oct 2022 07:50:04 GMT  
		Size: 4.9 MB (4877285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db68a36d4b9f8fa036da9f0c51e74b6d27dffd9d39317f42638ee84b29322668`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b325e4aad15f84b511f749de8e3b84dc88f98909bbfdd1961ac0e84f7d273f16`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ad76754b2b5a9699fc604ac8d1393dd3d6dfe21df82c8e930da67ffd6f6708`  
		Last Modified: Tue, 25 Oct 2022 07:50:52 GMT  
		Size: 259.6 MB (259567997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1318baf5e3f70ccdc707f97c58bf69e65917aadaa98ec26b67d1d2695572fa`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb834ce8392143178e871793c61a9bd2ac4e34031627b0f8d8453a1f1d836a1`  
		Last Modified: Tue, 25 Oct 2022 07:51:13 GMT  
		Size: 70.3 MB (70260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874278d4c37ef6d13abdb486dd6dfd9900b104ad68492eb5ba5df13c5c947b37`  
		Last Modified: Tue, 25 Oct 2022 07:51:03 GMT  
		Size: 289.2 KB (289160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5236595b9f2b064d0593cf222d04423eaa11b12eaa5c8e78974d822f22c23287`  
		Last Modified: Tue, 25 Oct 2022 07:51:19 GMT  
		Size: 75.0 MB (74998649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:12aab43566b2071488b4aa92c00718564fe9c214f1b5140d79c64f6c26f3941c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386028472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3609bfe5658aa0d47a0912a5414796fe5cb3657ef0bdaf25459f273c316bde`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:51 GMT
ADD file:577e89b09dccbe472d77fc02945d56a9eac3a24e20bf618c45074becfa1f49c9 in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 18:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV ROS_DISTRO=melodic
# Wed, 02 Nov 2022 19:00:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:00:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:00:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:00:23 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:01:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:01:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8cba8250122e011a113a9792b4a631b34b2aa89453e4c04090586d85464707de`  
		Last Modified: Tue, 25 Oct 2022 03:09:09 GMT  
		Size: 22.3 MB (22306283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc908b61f80477ac7791402bccbdb66903da21a17218a82598c6b5d68b42504a`  
		Last Modified: Wed, 02 Nov 2022 19:25:26 GMT  
		Size: 829.9 KB (829874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee3c131e9ae3f02652725609817aa7aeadca2d8f2d76a59d7f9264eb44e557`  
		Last Modified: Wed, 02 Nov 2022 19:25:24 GMT  
		Size: 4.1 MB (4088339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aa1a282fea46d652eaad9c87154fc787260798454ff685efa0b9f014e80211`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae6ce0e1086d82b010d3b4800835ad5cee4b4cda373a532b7915921440aaf0b`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f5c438d3cc55ffe5c481e73e0f1ee6d6ad654caa476e58a5d57c522aed267`  
		Last Modified: Wed, 02 Nov 2022 19:26:05 GMT  
		Size: 239.0 MB (239043717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fada99ba68d64cf8bce10f31ba55521c25aabf87e21a948e348c0a63ea5033`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a77d2db7252005f29e5e658434aba2b5cfd8639d128908ee57489ca6cf2818`  
		Last Modified: Wed, 02 Nov 2022 19:26:26 GMT  
		Size: 54.7 MB (54722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23db9ba1443d202279569a7e761c1cec59c0e4a55c78221b3592790683ee9f`  
		Last Modified: Wed, 02 Nov 2022 19:26:17 GMT  
		Size: 288.9 KB (288944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5d7c0964f9677840ae3fa2177c3b580272f045ba8413a33f8523d8f5a6edb9`  
		Last Modified: Wed, 02 Nov 2022 19:26:30 GMT  
		Size: 64.7 MB (64747387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a3bc1386512161551014d974ef7a92ab093f9740745a129aaf585129950f409a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412168880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9021aea3f107f10bf15a3e04d0ebc412e3119eea741be23df0d0b94c222f3b7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 20:56:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 20:57:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 21:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:01:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:01:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:01:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:02:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:02:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716808bd159516452cc1fc4db13d26965a5ea97f8fd507504f2abbd039e6b49d`  
		Last Modified: Tue, 25 Oct 2022 21:59:17 GMT  
		Size: 832.1 KB (832133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba094397f1fa2e72e998a82343d0614edda5257c98110b93a24af381630d3d31`  
		Last Modified: Tue, 25 Oct 2022 21:59:16 GMT  
		Size: 4.5 MB (4461373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282853d155ba0f593cc03d8773b2943181fe800a9fd446c6f8e70272937f7b9`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8dfb3f0f683701a85906157d325487eef9df7b6c559e3789449d02a6141051`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20849d29bb87d6b2a985fcc31e046ea130cae04137e9d346ad8322cab86170`  
		Last Modified: Tue, 25 Oct 2022 21:59:49 GMT  
		Size: 252.5 MB (252526710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90dfe4568d11bee7e54df662800278a22a50ea4a63904f366d46a49ee17f6a4`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f778aa7fa96e398ee7887d76161f1c151b67c7d0888a48c9512e86d37ba7c532`  
		Last Modified: Tue, 25 Oct 2022 22:00:07 GMT  
		Size: 63.1 MB (63091592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da590a11132a9292f690e41ddd35c007c4ad4da0e52655fad6f6ef220d97f9b7`  
		Last Modified: Tue, 25 Oct 2022 22:00:00 GMT  
		Size: 289.2 KB (289154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cb1026663e1c31e2f46024240399e38da1fd0da606460b86316cba8196c55a`  
		Last Modified: Tue, 25 Oct 2022 22:00:11 GMT  
		Size: 67.2 MB (67230215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:0c8cefbabb0989e6275d39204d6870081328f1ebecb7e98120d4bd26dde288b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:4823a905ffe0b3e7d527d857d533d78fc707ace416fed369a38da35f98b535bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291990746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b750019b37ee79ded291459fd57709578c21c1a3c552e25109bf1f41e0d8dd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:51:42 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 06:51:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 06:55:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:55:51 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 06:55:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 06:55:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955214fb5b152d9d9fa8ce9a39b19a4e6e8ea487bc617e76c0b7b33e1881bc`  
		Last Modified: Tue, 25 Oct 2022 07:50:06 GMT  
		Size: 831.1 KB (831118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389880aa1534b94319b44ef0d7e8e52ae108ec326dc1efe1cf0e4e749a4190a`  
		Last Modified: Tue, 25 Oct 2022 07:50:04 GMT  
		Size: 4.9 MB (4877285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db68a36d4b9f8fa036da9f0c51e74b6d27dffd9d39317f42638ee84b29322668`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b325e4aad15f84b511f749de8e3b84dc88f98909bbfdd1961ac0e84f7d273f16`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ad76754b2b5a9699fc604ac8d1393dd3d6dfe21df82c8e930da67ffd6f6708`  
		Last Modified: Tue, 25 Oct 2022 07:50:52 GMT  
		Size: 259.6 MB (259567997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1318baf5e3f70ccdc707f97c58bf69e65917aadaa98ec26b67d1d2695572fa`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:bbd7b447f9cf8b49ad310d76b2bff2616e87a6de7852f1e55ac80326049d6e49
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266270060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f3190352c0dc0d38e5f26baf1dc74914b046d2230d28e95df71cc15bc25f2c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:51 GMT
ADD file:577e89b09dccbe472d77fc02945d56a9eac3a24e20bf618c45074becfa1f49c9 in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 18:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV ROS_DISTRO=melodic
# Wed, 02 Nov 2022 19:00:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:00:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:00:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:00:23 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8cba8250122e011a113a9792b4a631b34b2aa89453e4c04090586d85464707de`  
		Last Modified: Tue, 25 Oct 2022 03:09:09 GMT  
		Size: 22.3 MB (22306283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc908b61f80477ac7791402bccbdb66903da21a17218a82598c6b5d68b42504a`  
		Last Modified: Wed, 02 Nov 2022 19:25:26 GMT  
		Size: 829.9 KB (829874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee3c131e9ae3f02652725609817aa7aeadca2d8f2d76a59d7f9264eb44e557`  
		Last Modified: Wed, 02 Nov 2022 19:25:24 GMT  
		Size: 4.1 MB (4088339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aa1a282fea46d652eaad9c87154fc787260798454ff685efa0b9f014e80211`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae6ce0e1086d82b010d3b4800835ad5cee4b4cda373a532b7915921440aaf0b`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f5c438d3cc55ffe5c481e73e0f1ee6d6ad654caa476e58a5d57c522aed267`  
		Last Modified: Wed, 02 Nov 2022 19:26:05 GMT  
		Size: 239.0 MB (239043717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fada99ba68d64cf8bce10f31ba55521c25aabf87e21a948e348c0a63ea5033`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0c361609706c9aee43282132738b66d3471f861629c71d8d949be9738ad6bb87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281557919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c264a0eff7c5acbeca6ee4599d1de01b6c8d56f44c806d6564b60b2ee5d0fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 20:56:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 20:57:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 21:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:01:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:01:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:01:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716808bd159516452cc1fc4db13d26965a5ea97f8fd507504f2abbd039e6b49d`  
		Last Modified: Tue, 25 Oct 2022 21:59:17 GMT  
		Size: 832.1 KB (832133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba094397f1fa2e72e998a82343d0614edda5257c98110b93a24af381630d3d31`  
		Last Modified: Tue, 25 Oct 2022 21:59:16 GMT  
		Size: 4.5 MB (4461373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282853d155ba0f593cc03d8773b2943181fe800a9fd446c6f8e70272937f7b9`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8dfb3f0f683701a85906157d325487eef9df7b6c559e3789449d02a6141051`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20849d29bb87d6b2a985fcc31e046ea130cae04137e9d346ad8322cab86170`  
		Last Modified: Tue, 25 Oct 2022 21:59:49 GMT  
		Size: 252.5 MB (252526710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90dfe4568d11bee7e54df662800278a22a50ea4a63904f366d46a49ee17f6a4`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:0c8cefbabb0989e6275d39204d6870081328f1ebecb7e98120d4bd26dde288b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:4823a905ffe0b3e7d527d857d533d78fc707ace416fed369a38da35f98b535bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291990746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b750019b37ee79ded291459fd57709578c21c1a3c552e25109bf1f41e0d8dd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:51:42 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:51:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 06:51:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 06:51:58 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 06:55:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:55:51 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 06:55:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 06:55:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955214fb5b152d9d9fa8ce9a39b19a4e6e8ea487bc617e76c0b7b33e1881bc`  
		Last Modified: Tue, 25 Oct 2022 07:50:06 GMT  
		Size: 831.1 KB (831118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389880aa1534b94319b44ef0d7e8e52ae108ec326dc1efe1cf0e4e749a4190a`  
		Last Modified: Tue, 25 Oct 2022 07:50:04 GMT  
		Size: 4.9 MB (4877285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db68a36d4b9f8fa036da9f0c51e74b6d27dffd9d39317f42638ee84b29322668`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b325e4aad15f84b511f749de8e3b84dc88f98909bbfdd1961ac0e84f7d273f16`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ad76754b2b5a9699fc604ac8d1393dd3d6dfe21df82c8e930da67ffd6f6708`  
		Last Modified: Tue, 25 Oct 2022 07:50:52 GMT  
		Size: 259.6 MB (259567997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1318baf5e3f70ccdc707f97c58bf69e65917aadaa98ec26b67d1d2695572fa`  
		Last Modified: Tue, 25 Oct 2022 07:50:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:bbd7b447f9cf8b49ad310d76b2bff2616e87a6de7852f1e55ac80326049d6e49
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266270060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f3190352c0dc0d38e5f26baf1dc74914b046d2230d28e95df71cc15bc25f2c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:06:51 GMT
ADD file:577e89b09dccbe472d77fc02945d56a9eac3a24e20bf618c45074becfa1f49c9 in / 
# Tue, 25 Oct 2022 03:06:52 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:55:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 18:55:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 18:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 18:55:59 GMT
ENV ROS_DISTRO=melodic
# Wed, 02 Nov 2022 19:00:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:00:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:00:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:00:23 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8cba8250122e011a113a9792b4a631b34b2aa89453e4c04090586d85464707de`  
		Last Modified: Tue, 25 Oct 2022 03:09:09 GMT  
		Size: 22.3 MB (22306283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc908b61f80477ac7791402bccbdb66903da21a17218a82598c6b5d68b42504a`  
		Last Modified: Wed, 02 Nov 2022 19:25:26 GMT  
		Size: 829.9 KB (829874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee3c131e9ae3f02652725609817aa7aeadca2d8f2d76a59d7f9264eb44e557`  
		Last Modified: Wed, 02 Nov 2022 19:25:24 GMT  
		Size: 4.1 MB (4088339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aa1a282fea46d652eaad9c87154fc787260798454ff685efa0b9f014e80211`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae6ce0e1086d82b010d3b4800835ad5cee4b4cda373a532b7915921440aaf0b`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f5c438d3cc55ffe5c481e73e0f1ee6d6ad654caa476e58a5d57c522aed267`  
		Last Modified: Wed, 02 Nov 2022 19:26:05 GMT  
		Size: 239.0 MB (239043717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fada99ba68d64cf8bce10f31ba55521c25aabf87e21a948e348c0a63ea5033`  
		Last Modified: Wed, 02 Nov 2022 19:25:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0c361609706c9aee43282132738b66d3471f861629c71d8d949be9738ad6bb87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281557919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c264a0eff7c5acbeca6ee4599d1de01b6c8d56f44c806d6564b60b2ee5d0fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 20:56:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:56:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 20:57:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 20:57:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 25 Oct 2022 21:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:01:22 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:01:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:01:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716808bd159516452cc1fc4db13d26965a5ea97f8fd507504f2abbd039e6b49d`  
		Last Modified: Tue, 25 Oct 2022 21:59:17 GMT  
		Size: 832.1 KB (832133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba094397f1fa2e72e998a82343d0614edda5257c98110b93a24af381630d3d31`  
		Last Modified: Tue, 25 Oct 2022 21:59:16 GMT  
		Size: 4.5 MB (4461373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282853d155ba0f593cc03d8773b2943181fe800a9fd446c6f8e70272937f7b9`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8dfb3f0f683701a85906157d325487eef9df7b6c559e3789449d02a6141051`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20849d29bb87d6b2a985fcc31e046ea130cae04137e9d346ad8322cab86170`  
		Last Modified: Tue, 25 Oct 2022 21:59:49 GMT  
		Size: 252.5 MB (252526710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90dfe4568d11bee7e54df662800278a22a50ea4a63904f366d46a49ee17f6a4`  
		Last Modified: Tue, 25 Oct 2022 21:59:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:ab5d0ba8771862f65925511a61f212c7623e8b020d05fd391611b6071e0e43c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:34cbfe55d811fe7c57add8b3d6f01ba9c209258ef1b4029cec5118dcd21e358f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343179990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d6d7ab7e066ec3cc62a3c2bfe041ba6a0a444f0b66da68886d72c1906c5004a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:04:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 07:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:07:31 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 07:07:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:07:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:08:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:08:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcba2703cc13554dd6ac252966be0f9f0a9d6e79ee879b5e0289457bc632f55`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c617320b8300618f53ec135b976c7f3a733354c5ef799b7c969108d82a8509f8`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065fe084d225480619420eb81fce25e1ea4e12e4f4b95002773742fc0e01d67`  
		Last Modified: Tue, 25 Oct 2022 07:53:37 GMT  
		Size: 177.0 MB (177008909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f66f6a9e5d5690a6fcd01f03ca5ef0146410fa911f6fccb17d73db1bbec814`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcd60406762b57a7de1c5c937562c8a145da66c5f0d5716f70f5c5ae115ab71`  
		Last Modified: Tue, 25 Oct 2022 07:53:56 GMT  
		Size: 50.9 MB (50940379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb29d90361859f6ac155a32b08124b4fecb3b64649f15b68b7d6b59f22d70d4`  
		Last Modified: Tue, 25 Oct 2022 07:53:47 GMT  
		Size: 332.1 KB (332101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055f4ec67f38d1b1c161894d68208d46a4d5822664774d4554aaf150f243341c`  
		Last Modified: Tue, 25 Oct 2022 07:54:01 GMT  
		Size: 79.6 MB (79603171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:c79509ab582f5fbaa979bbcf48f28ee81addc3e04aa6d5eb23e6035c0b84ec11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289252155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc2eb6984a475649e76658947d772c7f43483529829f3b6fee85f4111a8417d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:00 GMT
ADD file:0e30b9fd980776c745b113ac234367069202f461c4d888acb3225ccc0aa75385 in / 
# Tue, 25 Oct 2022 03:07:02 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 19:10:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Nov 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:13:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:13:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:13:08 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88411d40226eb74e038e5d2cbedefbd7555c34298ed687d1073cf87740fab694`  
		Last Modified: Tue, 25 Oct 2022 03:09:28 GMT  
		Size: 24.6 MB (24588786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4980d48be3296f50c2eb7a1ed914910fd03228f6827e76761e4f91e855c274`  
		Last Modified: Wed, 02 Nov 2022 19:28:01 GMT  
		Size: 1.2 MB (1162277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df80e53990143d250cd2cfc257128e21ad7900fea8655f90dc73db497ee70d`  
		Last Modified: Wed, 02 Nov 2022 19:27:59 GMT  
		Size: 4.7 MB (4678939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c8d46e4b38edb3ed3b546e70c15759ea848a90835313ff76420f5f6236f4d`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631c1eea769a3bb413e8b9acee2ba43d03ca28ba9f352402a1f438929797bf8`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0f2b9e1046c08b089ef7de2e729e4fe4a931f878eb337e38e38b21f05d7466`  
		Last Modified: Wed, 02 Nov 2022 19:28:32 GMT  
		Size: 157.5 MB (157499042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723fb85ab5877cb1c8a4c5404244e3ae35339f14585e9fc0cf6ea7edbd98e744`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d36e628b562012ce5558f6c1874f3d6cd0986636f5fed29a2a12443ff5843e`  
		Last Modified: Wed, 02 Nov 2022 19:28:51 GMT  
		Size: 40.5 MB (40506752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bb6ea983ee09f27ab55355b62ddd57de03cc019997304ca3c7557a61368083`  
		Last Modified: Wed, 02 Nov 2022 19:28:45 GMT  
		Size: 332.8 KB (332813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f5efd84d9c10fd339e85aeef8d785c40cc233d921959b11cd7b991b49b6e3c`  
		Last Modified: Wed, 02 Nov 2022 19:28:56 GMT  
		Size: 60.5 MB (60481135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:01d2a5693cbb33946e8b06971fe471d2fb165267fdbcb711dabe777d24337749
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322853760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8198d039a3796669f31af0d2cd9fe7c58a960e811af29f1768be002666b9167a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:11:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 21:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:14:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:14:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:14:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:15:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:15:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7354b266abeda9b5bfbca97ad1c6887d2a277d69ff8c607591a279459548ac7`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d614279c49f19055c903676e10afd41c8a3cd40f35d8b708fb499f7b5eeb965f`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c1b3c16d04da075eb127cecb646f3fbb43b07575ac781c7f670ca3f1885796`  
		Last Modified: Tue, 25 Oct 2022 22:01:55 GMT  
		Size: 171.4 MB (171447425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ac303ffe5e80a8c48e68fb479034e19261f5b6990dd5100bc6ddb1c7cd38ff`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4148c35466d56fca5bdd1144c7cc49f7c57ff22d51ce5c197995f215040f68d6`  
		Last Modified: Tue, 25 Oct 2022 22:02:11 GMT  
		Size: 45.2 MB (45204375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b385026becc2dcce049f0ab39c7d58c6459f28965efe78e7ee77336f82328a45`  
		Last Modified: Tue, 25 Oct 2022 22:02:05 GMT  
		Size: 332.1 KB (332102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d152eaa0a13418a883f576ea85d8893f1cdcafe87fc965ff14ee47fd4e076e7`  
		Last Modified: Tue, 25 Oct 2022 22:02:14 GMT  
		Size: 72.0 MB (71974237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:336a02bd77a55cc242eda416a251baca9d22d2374a0b353bfde166a3d84b53f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:cbbb6aa7e54b07b867ea1c6fefab9c1bd83f795f6e3a30a499c0a1f595db15c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.1 MB (835147503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d806f6ce0fd63436af5228a1d9a4209bb5f7f8de53205864e5319df8784e227`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:04:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 07:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:07:31 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 07:07:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:07:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:08:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:08:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:16:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcba2703cc13554dd6ac252966be0f9f0a9d6e79ee879b5e0289457bc632f55`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c617320b8300618f53ec135b976c7f3a733354c5ef799b7c969108d82a8509f8`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065fe084d225480619420eb81fce25e1ea4e12e4f4b95002773742fc0e01d67`  
		Last Modified: Tue, 25 Oct 2022 07:53:37 GMT  
		Size: 177.0 MB (177008909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f66f6a9e5d5690a6fcd01f03ca5ef0146410fa911f6fccb17d73db1bbec814`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcd60406762b57a7de1c5c937562c8a145da66c5f0d5716f70f5c5ae115ab71`  
		Last Modified: Tue, 25 Oct 2022 07:53:56 GMT  
		Size: 50.9 MB (50940379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb29d90361859f6ac155a32b08124b4fecb3b64649f15b68b7d6b59f22d70d4`  
		Last Modified: Tue, 25 Oct 2022 07:53:47 GMT  
		Size: 332.1 KB (332101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055f4ec67f38d1b1c161894d68208d46a4d5822664774d4554aaf150f243341c`  
		Last Modified: Tue, 25 Oct 2022 07:54:01 GMT  
		Size: 79.6 MB (79603171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96304f40d98ec3ee8f481818e18af495a0d8da05d780423f6da8294be3c5fcc1`  
		Last Modified: Tue, 25 Oct 2022 07:55:56 GMT  
		Size: 492.0 MB (491967513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:fc4e7314da161bef9b3589fddb7888ce44e929562292ccd970cde66a3d6a42ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.1 MB (726133078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab00ab59e29b7eb8379c2c7b0b877f8c907697572a4243edfe93f98fd3b43c41`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:00 GMT
ADD file:0e30b9fd980776c745b113ac234367069202f461c4d888acb3225ccc0aa75385 in / 
# Tue, 25 Oct 2022 03:07:02 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 19:10:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Nov 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:13:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:13:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:13:08 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:24:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88411d40226eb74e038e5d2cbedefbd7555c34298ed687d1073cf87740fab694`  
		Last Modified: Tue, 25 Oct 2022 03:09:28 GMT  
		Size: 24.6 MB (24588786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4980d48be3296f50c2eb7a1ed914910fd03228f6827e76761e4f91e855c274`  
		Last Modified: Wed, 02 Nov 2022 19:28:01 GMT  
		Size: 1.2 MB (1162277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df80e53990143d250cd2cfc257128e21ad7900fea8655f90dc73db497ee70d`  
		Last Modified: Wed, 02 Nov 2022 19:27:59 GMT  
		Size: 4.7 MB (4678939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c8d46e4b38edb3ed3b546e70c15759ea848a90835313ff76420f5f6236f4d`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631c1eea769a3bb413e8b9acee2ba43d03ca28ba9f352402a1f438929797bf8`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0f2b9e1046c08b089ef7de2e729e4fe4a931f878eb337e38e38b21f05d7466`  
		Last Modified: Wed, 02 Nov 2022 19:28:32 GMT  
		Size: 157.5 MB (157499042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723fb85ab5877cb1c8a4c5404244e3ae35339f14585e9fc0cf6ea7edbd98e744`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d36e628b562012ce5558f6c1874f3d6cd0986636f5fed29a2a12443ff5843e`  
		Last Modified: Wed, 02 Nov 2022 19:28:51 GMT  
		Size: 40.5 MB (40506752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bb6ea983ee09f27ab55355b62ddd57de03cc019997304ca3c7557a61368083`  
		Last Modified: Wed, 02 Nov 2022 19:28:45 GMT  
		Size: 332.8 KB (332813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f5efd84d9c10fd339e85aeef8d785c40cc233d921959b11cd7b991b49b6e3c`  
		Last Modified: Wed, 02 Nov 2022 19:28:56 GMT  
		Size: 60.5 MB (60481135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e159464b5134248b87ac0740d2aad50f36d410b1b2708cf289da16ad3ded0`  
		Last Modified: Wed, 02 Nov 2022 19:30:40 GMT  
		Size: 436.9 MB (436880923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a56e4c46dd57c138947ba191f82579cbebc7bc8be157b4afdc98279d0c2824a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.4 MB (785391798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e9ded839737165910ae71f3043672969d898b0aea25743168af6643850474c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:11:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 21:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:14:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:14:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:14:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:15:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:15:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:25:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7354b266abeda9b5bfbca97ad1c6887d2a277d69ff8c607591a279459548ac7`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d614279c49f19055c903676e10afd41c8a3cd40f35d8b708fb499f7b5eeb965f`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c1b3c16d04da075eb127cecb646f3fbb43b07575ac781c7f670ca3f1885796`  
		Last Modified: Tue, 25 Oct 2022 22:01:55 GMT  
		Size: 171.4 MB (171447425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ac303ffe5e80a8c48e68fb479034e19261f5b6990dd5100bc6ddb1c7cd38ff`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4148c35466d56fca5bdd1144c7cc49f7c57ff22d51ce5c197995f215040f68d6`  
		Last Modified: Tue, 25 Oct 2022 22:02:11 GMT  
		Size: 45.2 MB (45204375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b385026becc2dcce049f0ab39c7d58c6459f28965efe78e7ee77336f82328a45`  
		Last Modified: Tue, 25 Oct 2022 22:02:05 GMT  
		Size: 332.1 KB (332102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d152eaa0a13418a883f576ea85d8893f1cdcafe87fc965ff14ee47fd4e076e7`  
		Last Modified: Tue, 25 Oct 2022 22:02:14 GMT  
		Size: 72.0 MB (71974237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aa43327036965b93b120edc9468bb69de8263d58440de8ffc83cab8e59a269`  
		Last Modified: Tue, 25 Oct 2022 22:03:38 GMT  
		Size: 462.5 MB (462538038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:bacb377deeeb32940dc529634d22297630d6ef930e109bcbebbdd91a4788e867
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:3f430bdda79b5222464a15daa64d5225206b11326df98b7bae9861548183fdbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.1 MB (951139855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77653b5d1e9b5d88058239b1aebe5dfb81ab1d095ba7163a1c9b303ba382d0ea`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:09:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:09:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 15 Nov 2022 14:09:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 15 Nov 2022 14:09:11 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 14:09:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 Nov 2022 14:09:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 15 Nov 2022 14:10:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:10:38 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 15 Nov 2022 14:10:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 15 Nov 2022 14:10:38 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:11:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:11:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 15 Nov 2022 14:11:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050e80b3f85a5310349e1ba47f11fe807f2c447d5358f6207db81eb48fb2b5e1`  
		Last Modified: Tue, 15 Nov 2022 14:17:21 GMT  
		Size: 10.9 MB (10896874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d8bcd08342a708663e781db1d732df0583ec7e20a6545afe34e2db45c681f3`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6992da17af56fed0afceb107f48e33fb328ce20f2c086147f7025f9db0333d9e`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21027d057c2994560e78eb41d5b87a4472dbd12f943e76faa7c63fd554351677`  
		Last Modified: Tue, 15 Nov 2022 14:17:52 GMT  
		Size: 239.2 MB (239196483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11a9ed5ead225330619570c47bef0fb905868ad736d096e89862a1d2b514a4f`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f31d494c64a80d7def3cfd48da2a51be60eece07dd4e1e3e5610b4d7010478`  
		Last Modified: Tue, 15 Nov 2022 14:18:11 GMT  
		Size: 86.6 MB (86584973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85acc3837ea20ae7ab209c27727e989114bdddabf07c2d35414e82256ad4f785`  
		Last Modified: Tue, 15 Nov 2022 14:17:59 GMT  
		Size: 328.1 KB (328123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a668996e7d023b897fe956d678fbf3f0c0d5044f4418a2ca81cbef8d33120734`  
		Last Modified: Tue, 15 Nov 2022 14:18:10 GMT  
		Size: 76.0 MB (75977768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffcf2e951c7569c8c9bd788863547adcb4a6da74df144775af539eeb2a00faf`  
		Last Modified: Tue, 15 Nov 2022 14:19:47 GMT  
		Size: 487.7 MB (487704400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:51f295d08ae7049af488c3566afdf4eaf1808f48cbbf0e13372dcf648719d1eb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **867.9 MB (867923270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:063b3fd49c9e7939e1bf9e38abefed9332646a1810671c9d78df659b2ae6fee7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 11:01:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:01:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 15 Nov 2022 11:01:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 15 Nov 2022 11:01:16 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 11:01:16 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 Nov 2022 11:01:16 GMT
ENV ROS_DISTRO=noetic
# Tue, 15 Nov 2022 11:02:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:02:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 15 Nov 2022 11:02:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 15 Nov 2022 11:02:39 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 11:03:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:03:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 15 Nov 2022 11:03:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:08:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0d6aa77dc7e3e6cb404ca839ffe05429dc865c6f53f61d199627cddc197c0a`  
		Last Modified: Tue, 15 Nov 2022 11:09:47 GMT  
		Size: 10.9 MB (10902568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3955f704bc1936a82d8f59acffc7b268f5b37cb949b1eae1f51ddb2efb63f8c9`  
		Last Modified: Tue, 15 Nov 2022 11:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eb3e975face0a771cbbe4d7fcbaecd10a64dc2553cc0d0d405eabcd005d5a8`  
		Last Modified: Tue, 15 Nov 2022 11:09:46 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0a529ecc45627e8b17f5c8845fa00a9cca8cd87cfa9629ee2b23196501416`  
		Last Modified: Tue, 15 Nov 2022 11:10:09 GMT  
		Size: 184.4 MB (184381056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039cb484dc03fe448fd378fdeeb38fa7aed48361105571b0a99aa20163544cb`  
		Last Modified: Tue, 15 Nov 2022 11:09:45 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa787bdebdd6e7b0820bb59f70b63ad6b222698c18f8d4208b31ee8f12f781b`  
		Last Modified: Tue, 15 Nov 2022 11:10:34 GMT  
		Size: 84.4 MB (84371231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cd46bf0af5382b66346d8967c0d9de11e028d2ce44b491452432b6375130e2`  
		Last Modified: Tue, 15 Nov 2022 11:10:25 GMT  
		Size: 328.1 KB (328125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3658fda8fc78decc2782203a4a0a9905242d6c87dee1c0526a27dd719748b7`  
		Last Modified: Tue, 15 Nov 2022 11:10:33 GMT  
		Size: 74.1 MB (74089671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f87870f8806433cc50c810132b756fb2c58ebfe0ad8d40e5e16cf1e1d16975b`  
		Last Modified: Tue, 15 Nov 2022 11:11:40 GMT  
		Size: 464.6 MB (464614420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:336a02bd77a55cc242eda416a251baca9d22d2374a0b353bfde166a3d84b53f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:cbbb6aa7e54b07b867ea1c6fefab9c1bd83f795f6e3a30a499c0a1f595db15c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.1 MB (835147503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d806f6ce0fd63436af5228a1d9a4209bb5f7f8de53205864e5319df8784e227`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:04:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 07:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:07:31 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 07:07:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:07:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:08:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:08:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:16:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcba2703cc13554dd6ac252966be0f9f0a9d6e79ee879b5e0289457bc632f55`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c617320b8300618f53ec135b976c7f3a733354c5ef799b7c969108d82a8509f8`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065fe084d225480619420eb81fce25e1ea4e12e4f4b95002773742fc0e01d67`  
		Last Modified: Tue, 25 Oct 2022 07:53:37 GMT  
		Size: 177.0 MB (177008909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f66f6a9e5d5690a6fcd01f03ca5ef0146410fa911f6fccb17d73db1bbec814`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcd60406762b57a7de1c5c937562c8a145da66c5f0d5716f70f5c5ae115ab71`  
		Last Modified: Tue, 25 Oct 2022 07:53:56 GMT  
		Size: 50.9 MB (50940379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb29d90361859f6ac155a32b08124b4fecb3b64649f15b68b7d6b59f22d70d4`  
		Last Modified: Tue, 25 Oct 2022 07:53:47 GMT  
		Size: 332.1 KB (332101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055f4ec67f38d1b1c161894d68208d46a4d5822664774d4554aaf150f243341c`  
		Last Modified: Tue, 25 Oct 2022 07:54:01 GMT  
		Size: 79.6 MB (79603171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96304f40d98ec3ee8f481818e18af495a0d8da05d780423f6da8294be3c5fcc1`  
		Last Modified: Tue, 25 Oct 2022 07:55:56 GMT  
		Size: 492.0 MB (491967513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:fc4e7314da161bef9b3589fddb7888ce44e929562292ccd970cde66a3d6a42ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.1 MB (726133078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab00ab59e29b7eb8379c2c7b0b877f8c907697572a4243edfe93f98fd3b43c41`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:00 GMT
ADD file:0e30b9fd980776c745b113ac234367069202f461c4d888acb3225ccc0aa75385 in / 
# Tue, 25 Oct 2022 03:07:02 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 19:10:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Nov 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:13:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:13:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:13:08 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:24:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88411d40226eb74e038e5d2cbedefbd7555c34298ed687d1073cf87740fab694`  
		Last Modified: Tue, 25 Oct 2022 03:09:28 GMT  
		Size: 24.6 MB (24588786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4980d48be3296f50c2eb7a1ed914910fd03228f6827e76761e4f91e855c274`  
		Last Modified: Wed, 02 Nov 2022 19:28:01 GMT  
		Size: 1.2 MB (1162277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df80e53990143d250cd2cfc257128e21ad7900fea8655f90dc73db497ee70d`  
		Last Modified: Wed, 02 Nov 2022 19:27:59 GMT  
		Size: 4.7 MB (4678939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c8d46e4b38edb3ed3b546e70c15759ea848a90835313ff76420f5f6236f4d`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631c1eea769a3bb413e8b9acee2ba43d03ca28ba9f352402a1f438929797bf8`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0f2b9e1046c08b089ef7de2e729e4fe4a931f878eb337e38e38b21f05d7466`  
		Last Modified: Wed, 02 Nov 2022 19:28:32 GMT  
		Size: 157.5 MB (157499042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723fb85ab5877cb1c8a4c5404244e3ae35339f14585e9fc0cf6ea7edbd98e744`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d36e628b562012ce5558f6c1874f3d6cd0986636f5fed29a2a12443ff5843e`  
		Last Modified: Wed, 02 Nov 2022 19:28:51 GMT  
		Size: 40.5 MB (40506752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bb6ea983ee09f27ab55355b62ddd57de03cc019997304ca3c7557a61368083`  
		Last Modified: Wed, 02 Nov 2022 19:28:45 GMT  
		Size: 332.8 KB (332813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f5efd84d9c10fd339e85aeef8d785c40cc233d921959b11cd7b991b49b6e3c`  
		Last Modified: Wed, 02 Nov 2022 19:28:56 GMT  
		Size: 60.5 MB (60481135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e159464b5134248b87ac0740d2aad50f36d410b1b2708cf289da16ad3ded0`  
		Last Modified: Wed, 02 Nov 2022 19:30:40 GMT  
		Size: 436.9 MB (436880923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a56e4c46dd57c138947ba191f82579cbebc7bc8be157b4afdc98279d0c2824a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.4 MB (785391798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e9ded839737165910ae71f3043672969d898b0aea25743168af6643850474c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:11:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 21:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:14:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:14:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:14:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:15:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:15:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:25:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7354b266abeda9b5bfbca97ad1c6887d2a277d69ff8c607591a279459548ac7`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d614279c49f19055c903676e10afd41c8a3cd40f35d8b708fb499f7b5eeb965f`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c1b3c16d04da075eb127cecb646f3fbb43b07575ac781c7f670ca3f1885796`  
		Last Modified: Tue, 25 Oct 2022 22:01:55 GMT  
		Size: 171.4 MB (171447425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ac303ffe5e80a8c48e68fb479034e19261f5b6990dd5100bc6ddb1c7cd38ff`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4148c35466d56fca5bdd1144c7cc49f7c57ff22d51ce5c197995f215040f68d6`  
		Last Modified: Tue, 25 Oct 2022 22:02:11 GMT  
		Size: 45.2 MB (45204375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b385026becc2dcce049f0ab39c7d58c6459f28965efe78e7ee77336f82328a45`  
		Last Modified: Tue, 25 Oct 2022 22:02:05 GMT  
		Size: 332.1 KB (332102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d152eaa0a13418a883f576ea85d8893f1cdcafe87fc965ff14ee47fd4e076e7`  
		Last Modified: Tue, 25 Oct 2022 22:02:14 GMT  
		Size: 72.0 MB (71974237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aa43327036965b93b120edc9468bb69de8263d58440de8ffc83cab8e59a269`  
		Last Modified: Tue, 25 Oct 2022 22:03:38 GMT  
		Size: 462.5 MB (462538038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:dec52d670aead774ba5906310da12fd28a68080c44578e6062762b7ce7cb76ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:f2cb64c09356a71a17270f40ae8e9d42d242509547d47b395d46e04fbfaa5c93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359041151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aae48c851939de656e19f202234d0491e2bf82aa82870ab8070c404b34a0bda`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:04:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 07:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:07:31 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 07:07:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:07:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:08:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:08:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:10:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcba2703cc13554dd6ac252966be0f9f0a9d6e79ee879b5e0289457bc632f55`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c617320b8300618f53ec135b976c7f3a733354c5ef799b7c969108d82a8509f8`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065fe084d225480619420eb81fce25e1ea4e12e4f4b95002773742fc0e01d67`  
		Last Modified: Tue, 25 Oct 2022 07:53:37 GMT  
		Size: 177.0 MB (177008909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f66f6a9e5d5690a6fcd01f03ca5ef0146410fa911f6fccb17d73db1bbec814`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcd60406762b57a7de1c5c937562c8a145da66c5f0d5716f70f5c5ae115ab71`  
		Last Modified: Tue, 25 Oct 2022 07:53:56 GMT  
		Size: 50.9 MB (50940379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb29d90361859f6ac155a32b08124b4fecb3b64649f15b68b7d6b59f22d70d4`  
		Last Modified: Tue, 25 Oct 2022 07:53:47 GMT  
		Size: 332.1 KB (332101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055f4ec67f38d1b1c161894d68208d46a4d5822664774d4554aaf150f243341c`  
		Last Modified: Tue, 25 Oct 2022 07:54:01 GMT  
		Size: 79.6 MB (79603171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a67e64bc6cfc11803ed4fdb948911a3d1d22b6f40e7ed61cd815d62c050a4fc`  
		Last Modified: Tue, 25 Oct 2022 07:54:17 GMT  
		Size: 15.9 MB (15861161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:3f776a6cc9ad8ec3c64b0118d5d2b8918e544fbf1b757849998c2abfd5fd2a2a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303318474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe35d649eccf626ca98db067e0a14b9e1db741b83c309d322c069d6ea628019`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:00 GMT
ADD file:0e30b9fd980776c745b113ac234367069202f461c4d888acb3225ccc0aa75385 in / 
# Tue, 25 Oct 2022 03:07:02 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 19:10:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Nov 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:13:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:13:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:13:08 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:16:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88411d40226eb74e038e5d2cbedefbd7555c34298ed687d1073cf87740fab694`  
		Last Modified: Tue, 25 Oct 2022 03:09:28 GMT  
		Size: 24.6 MB (24588786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4980d48be3296f50c2eb7a1ed914910fd03228f6827e76761e4f91e855c274`  
		Last Modified: Wed, 02 Nov 2022 19:28:01 GMT  
		Size: 1.2 MB (1162277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df80e53990143d250cd2cfc257128e21ad7900fea8655f90dc73db497ee70d`  
		Last Modified: Wed, 02 Nov 2022 19:27:59 GMT  
		Size: 4.7 MB (4678939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c8d46e4b38edb3ed3b546e70c15759ea848a90835313ff76420f5f6236f4d`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631c1eea769a3bb413e8b9acee2ba43d03ca28ba9f352402a1f438929797bf8`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0f2b9e1046c08b089ef7de2e729e4fe4a931f878eb337e38e38b21f05d7466`  
		Last Modified: Wed, 02 Nov 2022 19:28:32 GMT  
		Size: 157.5 MB (157499042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723fb85ab5877cb1c8a4c5404244e3ae35339f14585e9fc0cf6ea7edbd98e744`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d36e628b562012ce5558f6c1874f3d6cd0986636f5fed29a2a12443ff5843e`  
		Last Modified: Wed, 02 Nov 2022 19:28:51 GMT  
		Size: 40.5 MB (40506752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bb6ea983ee09f27ab55355b62ddd57de03cc019997304ca3c7557a61368083`  
		Last Modified: Wed, 02 Nov 2022 19:28:45 GMT  
		Size: 332.8 KB (332813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f5efd84d9c10fd339e85aeef8d785c40cc233d921959b11cd7b991b49b6e3c`  
		Last Modified: Wed, 02 Nov 2022 19:28:56 GMT  
		Size: 60.5 MB (60481135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb0840c62f958906360caf24fcd6f69712d87d2c678c220aedb409e746faa24`  
		Last Modified: Wed, 02 Nov 2022 19:29:15 GMT  
		Size: 14.1 MB (14066319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:35c0807c3a9674796b7ff7b819fbd159fc13f69dc3034a817a170c98c29ebee6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338307578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eb6fdbc1a68f4521e7fb3e4b2a4c8d83f26b47cd5b4233095f12c3dd95ec6a1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:11:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 21:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:14:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:14:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:14:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:15:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:15:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:17:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7354b266abeda9b5bfbca97ad1c6887d2a277d69ff8c607591a279459548ac7`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d614279c49f19055c903676e10afd41c8a3cd40f35d8b708fb499f7b5eeb965f`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c1b3c16d04da075eb127cecb646f3fbb43b07575ac781c7f670ca3f1885796`  
		Last Modified: Tue, 25 Oct 2022 22:01:55 GMT  
		Size: 171.4 MB (171447425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ac303ffe5e80a8c48e68fb479034e19261f5b6990dd5100bc6ddb1c7cd38ff`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4148c35466d56fca5bdd1144c7cc49f7c57ff22d51ce5c197995f215040f68d6`  
		Last Modified: Tue, 25 Oct 2022 22:02:11 GMT  
		Size: 45.2 MB (45204375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b385026becc2dcce049f0ab39c7d58c6459f28965efe78e7ee77336f82328a45`  
		Last Modified: Tue, 25 Oct 2022 22:02:05 GMT  
		Size: 332.1 KB (332102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d152eaa0a13418a883f576ea85d8893f1cdcafe87fc965ff14ee47fd4e076e7`  
		Last Modified: Tue, 25 Oct 2022 22:02:14 GMT  
		Size: 72.0 MB (71974237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1ae12efe38c9f33d969d096b063141edbfda6df668fbb72467712d72e825b5`  
		Last Modified: Tue, 25 Oct 2022 22:02:29 GMT  
		Size: 15.5 MB (15453818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:4dffb51fe745dc708ef5407b8140f974f4529c60ad913b0b20ce7be0755fcf6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:6d3fa1e52d72f2aac6b3c1826851bdb6f90ed09ca3de75193011b27bba91a1c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.6 MB (484586435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:446f46aefa1703d9998d518113860d4b021674eaab91d1cac01a7b6f8cbf7d05`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:09:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:09:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 15 Nov 2022 14:09:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 15 Nov 2022 14:09:11 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 14:09:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 Nov 2022 14:09:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 15 Nov 2022 14:10:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:10:38 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 15 Nov 2022 14:10:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 15 Nov 2022 14:10:38 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:11:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:11:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 15 Nov 2022 14:11:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:12:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050e80b3f85a5310349e1ba47f11fe807f2c447d5358f6207db81eb48fb2b5e1`  
		Last Modified: Tue, 15 Nov 2022 14:17:21 GMT  
		Size: 10.9 MB (10896874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d8bcd08342a708663e781db1d732df0583ec7e20a6545afe34e2db45c681f3`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6992da17af56fed0afceb107f48e33fb328ce20f2c086147f7025f9db0333d9e`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21027d057c2994560e78eb41d5b87a4472dbd12f943e76faa7c63fd554351677`  
		Last Modified: Tue, 15 Nov 2022 14:17:52 GMT  
		Size: 239.2 MB (239196483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11a9ed5ead225330619570c47bef0fb905868ad736d096e89862a1d2b514a4f`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f31d494c64a80d7def3cfd48da2a51be60eece07dd4e1e3e5610b4d7010478`  
		Last Modified: Tue, 15 Nov 2022 14:18:11 GMT  
		Size: 86.6 MB (86584973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85acc3837ea20ae7ab209c27727e989114bdddabf07c2d35414e82256ad4f785`  
		Last Modified: Tue, 15 Nov 2022 14:17:59 GMT  
		Size: 328.1 KB (328123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a668996e7d023b897fe956d678fbf3f0c0d5044f4418a2ca81cbef8d33120734`  
		Last Modified: Tue, 15 Nov 2022 14:18:10 GMT  
		Size: 76.0 MB (75977768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3647ddcb7b7cca26b8abd4c96e174ed1fcaf9e7072eb7e3e58c6bd94ef00c82a`  
		Last Modified: Tue, 15 Nov 2022 14:18:26 GMT  
		Size: 21.2 MB (21150980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6f306e83d45a83ae93754835c3eec4ef2457c3c74a656d18b08e2a6153ca04ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.1 MB (424121361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550c834ac3286574f74c3276903dbd1035ba34279beb2948f5e8ce36b56f06a3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 11:01:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:01:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 15 Nov 2022 11:01:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 15 Nov 2022 11:01:16 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 11:01:16 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 Nov 2022 11:01:16 GMT
ENV ROS_DISTRO=noetic
# Tue, 15 Nov 2022 11:02:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:02:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 15 Nov 2022 11:02:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 15 Nov 2022 11:02:39 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 11:03:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:03:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 15 Nov 2022 11:03:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:04:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0d6aa77dc7e3e6cb404ca839ffe05429dc865c6f53f61d199627cddc197c0a`  
		Last Modified: Tue, 15 Nov 2022 11:09:47 GMT  
		Size: 10.9 MB (10902568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3955f704bc1936a82d8f59acffc7b268f5b37cb949b1eae1f51ddb2efb63f8c9`  
		Last Modified: Tue, 15 Nov 2022 11:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eb3e975face0a771cbbe4d7fcbaecd10a64dc2553cc0d0d405eabcd005d5a8`  
		Last Modified: Tue, 15 Nov 2022 11:09:46 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0a529ecc45627e8b17f5c8845fa00a9cca8cd87cfa9629ee2b23196501416`  
		Last Modified: Tue, 15 Nov 2022 11:10:09 GMT  
		Size: 184.4 MB (184381056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039cb484dc03fe448fd378fdeeb38fa7aed48361105571b0a99aa20163544cb`  
		Last Modified: Tue, 15 Nov 2022 11:09:45 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa787bdebdd6e7b0820bb59f70b63ad6b222698c18f8d4208b31ee8f12f781b`  
		Last Modified: Tue, 15 Nov 2022 11:10:34 GMT  
		Size: 84.4 MB (84371231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cd46bf0af5382b66346d8967c0d9de11e028d2ce44b491452432b6375130e2`  
		Last Modified: Tue, 15 Nov 2022 11:10:25 GMT  
		Size: 328.1 KB (328125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3658fda8fc78decc2782203a4a0a9905242d6c87dee1c0526a27dd719748b7`  
		Last Modified: Tue, 15 Nov 2022 11:10:33 GMT  
		Size: 74.1 MB (74089671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b20af995e6bd2a2e18ead3083d8bfcf90d71f630f10c06d1da58fabd959e54d`  
		Last Modified: Tue, 15 Nov 2022 11:10:43 GMT  
		Size: 20.8 MB (20812511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:dec52d670aead774ba5906310da12fd28a68080c44578e6062762b7ce7cb76ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:f2cb64c09356a71a17270f40ae8e9d42d242509547d47b395d46e04fbfaa5c93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359041151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aae48c851939de656e19f202234d0491e2bf82aa82870ab8070c404b34a0bda`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:04:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 07:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:07:31 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 07:07:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:07:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:08:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:08:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:10:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcba2703cc13554dd6ac252966be0f9f0a9d6e79ee879b5e0289457bc632f55`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c617320b8300618f53ec135b976c7f3a733354c5ef799b7c969108d82a8509f8`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065fe084d225480619420eb81fce25e1ea4e12e4f4b95002773742fc0e01d67`  
		Last Modified: Tue, 25 Oct 2022 07:53:37 GMT  
		Size: 177.0 MB (177008909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f66f6a9e5d5690a6fcd01f03ca5ef0146410fa911f6fccb17d73db1bbec814`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcd60406762b57a7de1c5c937562c8a145da66c5f0d5716f70f5c5ae115ab71`  
		Last Modified: Tue, 25 Oct 2022 07:53:56 GMT  
		Size: 50.9 MB (50940379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb29d90361859f6ac155a32b08124b4fecb3b64649f15b68b7d6b59f22d70d4`  
		Last Modified: Tue, 25 Oct 2022 07:53:47 GMT  
		Size: 332.1 KB (332101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055f4ec67f38d1b1c161894d68208d46a4d5822664774d4554aaf150f243341c`  
		Last Modified: Tue, 25 Oct 2022 07:54:01 GMT  
		Size: 79.6 MB (79603171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a67e64bc6cfc11803ed4fdb948911a3d1d22b6f40e7ed61cd815d62c050a4fc`  
		Last Modified: Tue, 25 Oct 2022 07:54:17 GMT  
		Size: 15.9 MB (15861161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:3f776a6cc9ad8ec3c64b0118d5d2b8918e544fbf1b757849998c2abfd5fd2a2a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303318474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe35d649eccf626ca98db067e0a14b9e1db741b83c309d322c069d6ea628019`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:00 GMT
ADD file:0e30b9fd980776c745b113ac234367069202f461c4d888acb3225ccc0aa75385 in / 
# Tue, 25 Oct 2022 03:07:02 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 19:10:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Nov 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:13:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:13:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:13:08 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:16:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88411d40226eb74e038e5d2cbedefbd7555c34298ed687d1073cf87740fab694`  
		Last Modified: Tue, 25 Oct 2022 03:09:28 GMT  
		Size: 24.6 MB (24588786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4980d48be3296f50c2eb7a1ed914910fd03228f6827e76761e4f91e855c274`  
		Last Modified: Wed, 02 Nov 2022 19:28:01 GMT  
		Size: 1.2 MB (1162277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df80e53990143d250cd2cfc257128e21ad7900fea8655f90dc73db497ee70d`  
		Last Modified: Wed, 02 Nov 2022 19:27:59 GMT  
		Size: 4.7 MB (4678939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c8d46e4b38edb3ed3b546e70c15759ea848a90835313ff76420f5f6236f4d`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631c1eea769a3bb413e8b9acee2ba43d03ca28ba9f352402a1f438929797bf8`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0f2b9e1046c08b089ef7de2e729e4fe4a931f878eb337e38e38b21f05d7466`  
		Last Modified: Wed, 02 Nov 2022 19:28:32 GMT  
		Size: 157.5 MB (157499042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723fb85ab5877cb1c8a4c5404244e3ae35339f14585e9fc0cf6ea7edbd98e744`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d36e628b562012ce5558f6c1874f3d6cd0986636f5fed29a2a12443ff5843e`  
		Last Modified: Wed, 02 Nov 2022 19:28:51 GMT  
		Size: 40.5 MB (40506752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bb6ea983ee09f27ab55355b62ddd57de03cc019997304ca3c7557a61368083`  
		Last Modified: Wed, 02 Nov 2022 19:28:45 GMT  
		Size: 332.8 KB (332813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f5efd84d9c10fd339e85aeef8d785c40cc233d921959b11cd7b991b49b6e3c`  
		Last Modified: Wed, 02 Nov 2022 19:28:56 GMT  
		Size: 60.5 MB (60481135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb0840c62f958906360caf24fcd6f69712d87d2c678c220aedb409e746faa24`  
		Last Modified: Wed, 02 Nov 2022 19:29:15 GMT  
		Size: 14.1 MB (14066319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:35c0807c3a9674796b7ff7b819fbd159fc13f69dc3034a817a170c98c29ebee6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338307578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eb6fdbc1a68f4521e7fb3e4b2a4c8d83f26b47cd5b4233095f12c3dd95ec6a1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:11:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 21:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:14:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:14:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:14:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:15:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:15:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:17:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7354b266abeda9b5bfbca97ad1c6887d2a277d69ff8c607591a279459548ac7`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d614279c49f19055c903676e10afd41c8a3cd40f35d8b708fb499f7b5eeb965f`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c1b3c16d04da075eb127cecb646f3fbb43b07575ac781c7f670ca3f1885796`  
		Last Modified: Tue, 25 Oct 2022 22:01:55 GMT  
		Size: 171.4 MB (171447425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ac303ffe5e80a8c48e68fb479034e19261f5b6990dd5100bc6ddb1c7cd38ff`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4148c35466d56fca5bdd1144c7cc49f7c57ff22d51ce5c197995f215040f68d6`  
		Last Modified: Tue, 25 Oct 2022 22:02:11 GMT  
		Size: 45.2 MB (45204375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b385026becc2dcce049f0ab39c7d58c6459f28965efe78e7ee77336f82328a45`  
		Last Modified: Tue, 25 Oct 2022 22:02:05 GMT  
		Size: 332.1 KB (332102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d152eaa0a13418a883f576ea85d8893f1cdcafe87fc965ff14ee47fd4e076e7`  
		Last Modified: Tue, 25 Oct 2022 22:02:14 GMT  
		Size: 72.0 MB (71974237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1ae12efe38c9f33d969d096b063141edbfda6df668fbb72467712d72e825b5`  
		Last Modified: Tue, 25 Oct 2022 22:02:29 GMT  
		Size: 15.5 MB (15453818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:ab5d0ba8771862f65925511a61f212c7623e8b020d05fd391611b6071e0e43c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:34cbfe55d811fe7c57add8b3d6f01ba9c209258ef1b4029cec5118dcd21e358f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343179990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d6d7ab7e066ec3cc62a3c2bfe041ba6a0a444f0b66da68886d72c1906c5004a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:04:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 07:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:07:31 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 07:07:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:07:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:08:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:08:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcba2703cc13554dd6ac252966be0f9f0a9d6e79ee879b5e0289457bc632f55`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c617320b8300618f53ec135b976c7f3a733354c5ef799b7c969108d82a8509f8`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065fe084d225480619420eb81fce25e1ea4e12e4f4b95002773742fc0e01d67`  
		Last Modified: Tue, 25 Oct 2022 07:53:37 GMT  
		Size: 177.0 MB (177008909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f66f6a9e5d5690a6fcd01f03ca5ef0146410fa911f6fccb17d73db1bbec814`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcd60406762b57a7de1c5c937562c8a145da66c5f0d5716f70f5c5ae115ab71`  
		Last Modified: Tue, 25 Oct 2022 07:53:56 GMT  
		Size: 50.9 MB (50940379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb29d90361859f6ac155a32b08124b4fecb3b64649f15b68b7d6b59f22d70d4`  
		Last Modified: Tue, 25 Oct 2022 07:53:47 GMT  
		Size: 332.1 KB (332101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055f4ec67f38d1b1c161894d68208d46a4d5822664774d4554aaf150f243341c`  
		Last Modified: Tue, 25 Oct 2022 07:54:01 GMT  
		Size: 79.6 MB (79603171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:c79509ab582f5fbaa979bbcf48f28ee81addc3e04aa6d5eb23e6035c0b84ec11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289252155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc2eb6984a475649e76658947d772c7f43483529829f3b6fee85f4111a8417d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:00 GMT
ADD file:0e30b9fd980776c745b113ac234367069202f461c4d888acb3225ccc0aa75385 in / 
# Tue, 25 Oct 2022 03:07:02 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 19:10:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Nov 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:13:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:13:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:13:08 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88411d40226eb74e038e5d2cbedefbd7555c34298ed687d1073cf87740fab694`  
		Last Modified: Tue, 25 Oct 2022 03:09:28 GMT  
		Size: 24.6 MB (24588786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4980d48be3296f50c2eb7a1ed914910fd03228f6827e76761e4f91e855c274`  
		Last Modified: Wed, 02 Nov 2022 19:28:01 GMT  
		Size: 1.2 MB (1162277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df80e53990143d250cd2cfc257128e21ad7900fea8655f90dc73db497ee70d`  
		Last Modified: Wed, 02 Nov 2022 19:27:59 GMT  
		Size: 4.7 MB (4678939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c8d46e4b38edb3ed3b546e70c15759ea848a90835313ff76420f5f6236f4d`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631c1eea769a3bb413e8b9acee2ba43d03ca28ba9f352402a1f438929797bf8`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0f2b9e1046c08b089ef7de2e729e4fe4a931f878eb337e38e38b21f05d7466`  
		Last Modified: Wed, 02 Nov 2022 19:28:32 GMT  
		Size: 157.5 MB (157499042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723fb85ab5877cb1c8a4c5404244e3ae35339f14585e9fc0cf6ea7edbd98e744`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d36e628b562012ce5558f6c1874f3d6cd0986636f5fed29a2a12443ff5843e`  
		Last Modified: Wed, 02 Nov 2022 19:28:51 GMT  
		Size: 40.5 MB (40506752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bb6ea983ee09f27ab55355b62ddd57de03cc019997304ca3c7557a61368083`  
		Last Modified: Wed, 02 Nov 2022 19:28:45 GMT  
		Size: 332.8 KB (332813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f5efd84d9c10fd339e85aeef8d785c40cc233d921959b11cd7b991b49b6e3c`  
		Last Modified: Wed, 02 Nov 2022 19:28:56 GMT  
		Size: 60.5 MB (60481135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:01d2a5693cbb33946e8b06971fe471d2fb165267fdbcb711dabe777d24337749
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322853760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8198d039a3796669f31af0d2cd9fe7c58a960e811af29f1768be002666b9167a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:11:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 21:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:14:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:14:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:14:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:15:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:15:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7354b266abeda9b5bfbca97ad1c6887d2a277d69ff8c607591a279459548ac7`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d614279c49f19055c903676e10afd41c8a3cd40f35d8b708fb499f7b5eeb965f`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c1b3c16d04da075eb127cecb646f3fbb43b07575ac781c7f670ca3f1885796`  
		Last Modified: Tue, 25 Oct 2022 22:01:55 GMT  
		Size: 171.4 MB (171447425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ac303ffe5e80a8c48e68fb479034e19261f5b6990dd5100bc6ddb1c7cd38ff`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4148c35466d56fca5bdd1144c7cc49f7c57ff22d51ce5c197995f215040f68d6`  
		Last Modified: Tue, 25 Oct 2022 22:02:11 GMT  
		Size: 45.2 MB (45204375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b385026becc2dcce049f0ab39c7d58c6459f28965efe78e7ee77336f82328a45`  
		Last Modified: Tue, 25 Oct 2022 22:02:05 GMT  
		Size: 332.1 KB (332102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d152eaa0a13418a883f576ea85d8893f1cdcafe87fc965ff14ee47fd4e076e7`  
		Last Modified: Tue, 25 Oct 2022 22:02:14 GMT  
		Size: 72.0 MB (71974237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:35e0569ca7632a92dccc890a4478d82c465e5fd0b5844f2848fe8660a3e9f43a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:5b7dbb570a50046a24060a29f6b82eae8a184245c2ffbf75d59b6312c886a0f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.4 MB (463435455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d20e65a81a353d8f5b56c64f2252c3e63eb5ee3d665ba80c39a4390fc5a1b0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:09:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:09:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 15 Nov 2022 14:09:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 15 Nov 2022 14:09:11 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 14:09:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 Nov 2022 14:09:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 15 Nov 2022 14:10:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:10:38 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 15 Nov 2022 14:10:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 15 Nov 2022 14:10:38 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:11:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:11:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 15 Nov 2022 14:11:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050e80b3f85a5310349e1ba47f11fe807f2c447d5358f6207db81eb48fb2b5e1`  
		Last Modified: Tue, 15 Nov 2022 14:17:21 GMT  
		Size: 10.9 MB (10896874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d8bcd08342a708663e781db1d732df0583ec7e20a6545afe34e2db45c681f3`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6992da17af56fed0afceb107f48e33fb328ce20f2c086147f7025f9db0333d9e`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21027d057c2994560e78eb41d5b87a4472dbd12f943e76faa7c63fd554351677`  
		Last Modified: Tue, 15 Nov 2022 14:17:52 GMT  
		Size: 239.2 MB (239196483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11a9ed5ead225330619570c47bef0fb905868ad736d096e89862a1d2b514a4f`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f31d494c64a80d7def3cfd48da2a51be60eece07dd4e1e3e5610b4d7010478`  
		Last Modified: Tue, 15 Nov 2022 14:18:11 GMT  
		Size: 86.6 MB (86584973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85acc3837ea20ae7ab209c27727e989114bdddabf07c2d35414e82256ad4f785`  
		Last Modified: Tue, 15 Nov 2022 14:17:59 GMT  
		Size: 328.1 KB (328123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a668996e7d023b897fe956d678fbf3f0c0d5044f4418a2ca81cbef8d33120734`  
		Last Modified: Tue, 15 Nov 2022 14:18:10 GMT  
		Size: 76.0 MB (75977768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9561816b27e097de3ee1a77c73b9edb4355e9a8c4bde39a73e528dcacb554ab8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403308850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ad3fb65c6943de5f18393313e09415393b2b7205bb131b6226908c01b00b3d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 11:01:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:01:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 15 Nov 2022 11:01:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 15 Nov 2022 11:01:16 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 11:01:16 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 Nov 2022 11:01:16 GMT
ENV ROS_DISTRO=noetic
# Tue, 15 Nov 2022 11:02:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:02:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 15 Nov 2022 11:02:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 15 Nov 2022 11:02:39 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 11:03:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:03:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 15 Nov 2022 11:03:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0d6aa77dc7e3e6cb404ca839ffe05429dc865c6f53f61d199627cddc197c0a`  
		Last Modified: Tue, 15 Nov 2022 11:09:47 GMT  
		Size: 10.9 MB (10902568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3955f704bc1936a82d8f59acffc7b268f5b37cb949b1eae1f51ddb2efb63f8c9`  
		Last Modified: Tue, 15 Nov 2022 11:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eb3e975face0a771cbbe4d7fcbaecd10a64dc2553cc0d0d405eabcd005d5a8`  
		Last Modified: Tue, 15 Nov 2022 11:09:46 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0a529ecc45627e8b17f5c8845fa00a9cca8cd87cfa9629ee2b23196501416`  
		Last Modified: Tue, 15 Nov 2022 11:10:09 GMT  
		Size: 184.4 MB (184381056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039cb484dc03fe448fd378fdeeb38fa7aed48361105571b0a99aa20163544cb`  
		Last Modified: Tue, 15 Nov 2022 11:09:45 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa787bdebdd6e7b0820bb59f70b63ad6b222698c18f8d4208b31ee8f12f781b`  
		Last Modified: Tue, 15 Nov 2022 11:10:34 GMT  
		Size: 84.4 MB (84371231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cd46bf0af5382b66346d8967c0d9de11e028d2ce44b491452432b6375130e2`  
		Last Modified: Tue, 15 Nov 2022 11:10:25 GMT  
		Size: 328.1 KB (328125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3658fda8fc78decc2782203a4a0a9905242d6c87dee1c0526a27dd719748b7`  
		Last Modified: Tue, 15 Nov 2022 11:10:33 GMT  
		Size: 74.1 MB (74089671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:ab5d0ba8771862f65925511a61f212c7623e8b020d05fd391611b6071e0e43c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:34cbfe55d811fe7c57add8b3d6f01ba9c209258ef1b4029cec5118dcd21e358f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343179990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d6d7ab7e066ec3cc62a3c2bfe041ba6a0a444f0b66da68886d72c1906c5004a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:04:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 07:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:07:31 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 07:07:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:07:31 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:08:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:08:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 07:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcba2703cc13554dd6ac252966be0f9f0a9d6e79ee879b5e0289457bc632f55`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c617320b8300618f53ec135b976c7f3a733354c5ef799b7c969108d82a8509f8`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065fe084d225480619420eb81fce25e1ea4e12e4f4b95002773742fc0e01d67`  
		Last Modified: Tue, 25 Oct 2022 07:53:37 GMT  
		Size: 177.0 MB (177008909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f66f6a9e5d5690a6fcd01f03ca5ef0146410fa911f6fccb17d73db1bbec814`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcd60406762b57a7de1c5c937562c8a145da66c5f0d5716f70f5c5ae115ab71`  
		Last Modified: Tue, 25 Oct 2022 07:53:56 GMT  
		Size: 50.9 MB (50940379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb29d90361859f6ac155a32b08124b4fecb3b64649f15b68b7d6b59f22d70d4`  
		Last Modified: Tue, 25 Oct 2022 07:53:47 GMT  
		Size: 332.1 KB (332101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055f4ec67f38d1b1c161894d68208d46a4d5822664774d4554aaf150f243341c`  
		Last Modified: Tue, 25 Oct 2022 07:54:01 GMT  
		Size: 79.6 MB (79603171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:c79509ab582f5fbaa979bbcf48f28ee81addc3e04aa6d5eb23e6035c0b84ec11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289252155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc2eb6984a475649e76658947d772c7f43483529829f3b6fee85f4111a8417d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:00 GMT
ADD file:0e30b9fd980776c745b113ac234367069202f461c4d888acb3225ccc0aa75385 in / 
# Tue, 25 Oct 2022 03:07:02 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 19:10:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Nov 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:13:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:13:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:13:08 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:13:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:14:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88411d40226eb74e038e5d2cbedefbd7555c34298ed687d1073cf87740fab694`  
		Last Modified: Tue, 25 Oct 2022 03:09:28 GMT  
		Size: 24.6 MB (24588786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4980d48be3296f50c2eb7a1ed914910fd03228f6827e76761e4f91e855c274`  
		Last Modified: Wed, 02 Nov 2022 19:28:01 GMT  
		Size: 1.2 MB (1162277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df80e53990143d250cd2cfc257128e21ad7900fea8655f90dc73db497ee70d`  
		Last Modified: Wed, 02 Nov 2022 19:27:59 GMT  
		Size: 4.7 MB (4678939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c8d46e4b38edb3ed3b546e70c15759ea848a90835313ff76420f5f6236f4d`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631c1eea769a3bb413e8b9acee2ba43d03ca28ba9f352402a1f438929797bf8`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0f2b9e1046c08b089ef7de2e729e4fe4a931f878eb337e38e38b21f05d7466`  
		Last Modified: Wed, 02 Nov 2022 19:28:32 GMT  
		Size: 157.5 MB (157499042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723fb85ab5877cb1c8a4c5404244e3ae35339f14585e9fc0cf6ea7edbd98e744`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d36e628b562012ce5558f6c1874f3d6cd0986636f5fed29a2a12443ff5843e`  
		Last Modified: Wed, 02 Nov 2022 19:28:51 GMT  
		Size: 40.5 MB (40506752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bb6ea983ee09f27ab55355b62ddd57de03cc019997304ca3c7557a61368083`  
		Last Modified: Wed, 02 Nov 2022 19:28:45 GMT  
		Size: 332.8 KB (332813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f5efd84d9c10fd339e85aeef8d785c40cc233d921959b11cd7b991b49b6e3c`  
		Last Modified: Wed, 02 Nov 2022 19:28:56 GMT  
		Size: 60.5 MB (60481135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:01d2a5693cbb33946e8b06971fe471d2fb165267fdbcb711dabe777d24337749
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322853760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8198d039a3796669f31af0d2cd9fe7c58a960e811af29f1768be002666b9167a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:11:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 21:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:14:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:14:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:14:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:15:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:15:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 25 Oct 2022 21:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7354b266abeda9b5bfbca97ad1c6887d2a277d69ff8c607591a279459548ac7`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d614279c49f19055c903676e10afd41c8a3cd40f35d8b708fb499f7b5eeb965f`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c1b3c16d04da075eb127cecb646f3fbb43b07575ac781c7f670ca3f1885796`  
		Last Modified: Tue, 25 Oct 2022 22:01:55 GMT  
		Size: 171.4 MB (171447425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ac303ffe5e80a8c48e68fb479034e19261f5b6990dd5100bc6ddb1c7cd38ff`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4148c35466d56fca5bdd1144c7cc49f7c57ff22d51ce5c197995f215040f68d6`  
		Last Modified: Tue, 25 Oct 2022 22:02:11 GMT  
		Size: 45.2 MB (45204375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b385026becc2dcce049f0ab39c7d58c6459f28965efe78e7ee77336f82328a45`  
		Last Modified: Tue, 25 Oct 2022 22:02:05 GMT  
		Size: 332.1 KB (332102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d152eaa0a13418a883f576ea85d8893f1cdcafe87fc965ff14ee47fd4e076e7`  
		Last Modified: Tue, 25 Oct 2022 22:02:14 GMT  
		Size: 72.0 MB (71974237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:919be2ca31dd98c79d06f52204d11aa73b941d2783120d5022a67edcb5413a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:846f250f6dd222e44ee17b7f871875e20abd569082de6299b1d3fb89b4a60ee9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212304339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c78d80b5cf8bf8109d294a84172eb5bc1f718d08607ed579e63932bac8cfa9d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:04:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 07:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:07:31 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 07:07:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:07:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcba2703cc13554dd6ac252966be0f9f0a9d6e79ee879b5e0289457bc632f55`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c617320b8300618f53ec135b976c7f3a733354c5ef799b7c969108d82a8509f8`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065fe084d225480619420eb81fce25e1ea4e12e4f4b95002773742fc0e01d67`  
		Last Modified: Tue, 25 Oct 2022 07:53:37 GMT  
		Size: 177.0 MB (177008909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f66f6a9e5d5690a6fcd01f03ca5ef0146410fa911f6fccb17d73db1bbec814`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:d03d5be56966be242366663ce72f7847e52b47e8cca431bd854719a62a1365c4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187931455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f738e1bcf90c08d1919e239f46f0ff98ed35d40acf8b01064230e5d3c49ec6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:00 GMT
ADD file:0e30b9fd980776c745b113ac234367069202f461c4d888acb3225ccc0aa75385 in / 
# Tue, 25 Oct 2022 03:07:02 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 19:10:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Nov 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:13:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:13:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:13:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:88411d40226eb74e038e5d2cbedefbd7555c34298ed687d1073cf87740fab694`  
		Last Modified: Tue, 25 Oct 2022 03:09:28 GMT  
		Size: 24.6 MB (24588786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4980d48be3296f50c2eb7a1ed914910fd03228f6827e76761e4f91e855c274`  
		Last Modified: Wed, 02 Nov 2022 19:28:01 GMT  
		Size: 1.2 MB (1162277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df80e53990143d250cd2cfc257128e21ad7900fea8655f90dc73db497ee70d`  
		Last Modified: Wed, 02 Nov 2022 19:27:59 GMT  
		Size: 4.7 MB (4678939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c8d46e4b38edb3ed3b546e70c15759ea848a90835313ff76420f5f6236f4d`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631c1eea769a3bb413e8b9acee2ba43d03ca28ba9f352402a1f438929797bf8`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0f2b9e1046c08b089ef7de2e729e4fe4a931f878eb337e38e38b21f05d7466`  
		Last Modified: Wed, 02 Nov 2022 19:28:32 GMT  
		Size: 157.5 MB (157499042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723fb85ab5877cb1c8a4c5404244e3ae35339f14585e9fc0cf6ea7edbd98e744`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:89a530ed26b46eee46941dbadbb46db7466d5e5ce9d18d067dc815b0d3052467
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.3 MB (205343046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cbd10085e3bd8e389031b83d712cb3a42365b13f88c647a9ee795d92151879d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:11:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 21:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:14:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:14:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:14:39 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7354b266abeda9b5bfbca97ad1c6887d2a277d69ff8c607591a279459548ac7`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d614279c49f19055c903676e10afd41c8a3cd40f35d8b708fb499f7b5eeb965f`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c1b3c16d04da075eb127cecb646f3fbb43b07575ac781c7f670ca3f1885796`  
		Last Modified: Tue, 25 Oct 2022 22:01:55 GMT  
		Size: 171.4 MB (171447425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ac303ffe5e80a8c48e68fb479034e19261f5b6990dd5100bc6ddb1c7cd38ff`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:9045252f47d753b9c47a51705a8fc37dfecff1a9a1dd381d1b0b82f28f76755e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:8b3fb34c9d4df88d9042412d63874e2ae0fe54ec178a8008c4ec4ddc6486a8c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300544591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c29052fbf7fa34dfacad78c4fdc8353c75a7a67398e94d107a429525479a76e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:09:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:09:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 15 Nov 2022 14:09:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 15 Nov 2022 14:09:11 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 14:09:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 Nov 2022 14:09:11 GMT
ENV ROS_DISTRO=noetic
# Tue, 15 Nov 2022 14:10:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:10:38 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 15 Nov 2022 14:10:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 15 Nov 2022 14:10:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050e80b3f85a5310349e1ba47f11fe807f2c447d5358f6207db81eb48fb2b5e1`  
		Last Modified: Tue, 15 Nov 2022 14:17:21 GMT  
		Size: 10.9 MB (10896874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d8bcd08342a708663e781db1d732df0583ec7e20a6545afe34e2db45c681f3`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6992da17af56fed0afceb107f48e33fb328ce20f2c086147f7025f9db0333d9e`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21027d057c2994560e78eb41d5b87a4472dbd12f943e76faa7c63fd554351677`  
		Last Modified: Tue, 15 Nov 2022 14:17:52 GMT  
		Size: 239.2 MB (239196483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11a9ed5ead225330619570c47bef0fb905868ad736d096e89862a1d2b514a4f`  
		Last Modified: Tue, 15 Nov 2022 14:17:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ea0e03de4581586ce6d534f9e6fc2c2bf8e50a50168b9b0afb57d3fbe4f7582d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244519823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65702135bd10e5f317ce9f171437335f2de36dbf8ab6a4ba4da9465bdefaaffa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 11:01:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:01:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 15 Nov 2022 11:01:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 15 Nov 2022 11:01:16 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 11:01:16 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 Nov 2022 11:01:16 GMT
ENV ROS_DISTRO=noetic
# Tue, 15 Nov 2022 11:02:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:02:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 15 Nov 2022 11:02:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 15 Nov 2022 11:02:39 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0d6aa77dc7e3e6cb404ca839ffe05429dc865c6f53f61d199627cddc197c0a`  
		Last Modified: Tue, 15 Nov 2022 11:09:47 GMT  
		Size: 10.9 MB (10902568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3955f704bc1936a82d8f59acffc7b268f5b37cb949b1eae1f51ddb2efb63f8c9`  
		Last Modified: Tue, 15 Nov 2022 11:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eb3e975face0a771cbbe4d7fcbaecd10a64dc2553cc0d0d405eabcd005d5a8`  
		Last Modified: Tue, 15 Nov 2022 11:09:46 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0a529ecc45627e8b17f5c8845fa00a9cca8cd87cfa9629ee2b23196501416`  
		Last Modified: Tue, 15 Nov 2022 11:10:09 GMT  
		Size: 184.4 MB (184381056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039cb484dc03fe448fd378fdeeb38fa7aed48361105571b0a99aa20163544cb`  
		Last Modified: Tue, 15 Nov 2022 11:09:45 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:919be2ca31dd98c79d06f52204d11aa73b941d2783120d5022a67edcb5413a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:846f250f6dd222e44ee17b7f871875e20abd569082de6299b1d3fb89b4a60ee9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212304339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c78d80b5cf8bf8109d294a84172eb5bc1f718d08607ed579e63932bac8cfa9d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:04:29 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:04:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 07:04:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 07:04:54 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 07:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:07:31 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 07:07:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 07:07:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ff4b427f850657d03c70299694b020567ea6ea793e6e9113bc123ebe18aaf4`  
		Last Modified: Tue, 25 Oct 2022 07:52:57 GMT  
		Size: 1.2 MB (1163883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472155f6e6612bc976b4f23b2fbc13373ddcbbd7414f6b13ba9a6c11e853ec9b`  
		Last Modified: Tue, 25 Oct 2022 07:52:55 GMT  
		Size: 5.6 MB (5551301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcba2703cc13554dd6ac252966be0f9f0a9d6e79ee879b5e0289457bc632f55`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c617320b8300618f53ec135b976c7f3a733354c5ef799b7c969108d82a8509f8`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065fe084d225480619420eb81fce25e1ea4e12e4f4b95002773742fc0e01d67`  
		Last Modified: Tue, 25 Oct 2022 07:53:37 GMT  
		Size: 177.0 MB (177008909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f66f6a9e5d5690a6fcd01f03ca5ef0146410fa911f6fccb17d73db1bbec814`  
		Last Modified: Tue, 25 Oct 2022 07:52:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:d03d5be56966be242366663ce72f7847e52b47e8cca431bd854719a62a1365c4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187931455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f738e1bcf90c08d1919e239f46f0ff98ed35d40acf8b01064230e5d3c49ec6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:00 GMT
ADD file:0e30b9fd980776c745b113ac234367069202f461c4d888acb3225ccc0aa75385 in / 
# Tue, 25 Oct 2022 03:07:02 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:09:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:10:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 02 Nov 2022 19:10:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:10:12 GMT
ENV ROS_DISTRO=noetic
# Wed, 02 Nov 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:13:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 02 Nov 2022 19:13:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:13:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:88411d40226eb74e038e5d2cbedefbd7555c34298ed687d1073cf87740fab694`  
		Last Modified: Tue, 25 Oct 2022 03:09:28 GMT  
		Size: 24.6 MB (24588786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4980d48be3296f50c2eb7a1ed914910fd03228f6827e76761e4f91e855c274`  
		Last Modified: Wed, 02 Nov 2022 19:28:01 GMT  
		Size: 1.2 MB (1162277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df80e53990143d250cd2cfc257128e21ad7900fea8655f90dc73db497ee70d`  
		Last Modified: Wed, 02 Nov 2022 19:27:59 GMT  
		Size: 4.7 MB (4678939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c8d46e4b38edb3ed3b546e70c15759ea848a90835313ff76420f5f6236f4d`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631c1eea769a3bb413e8b9acee2ba43d03ca28ba9f352402a1f438929797bf8`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0f2b9e1046c08b089ef7de2e729e4fe4a931f878eb337e38e38b21f05d7466`  
		Last Modified: Wed, 02 Nov 2022 19:28:32 GMT  
		Size: 157.5 MB (157499042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723fb85ab5877cb1c8a4c5404244e3ae35339f14585e9fc0cf6ea7edbd98e744`  
		Last Modified: Wed, 02 Nov 2022 19:27:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:89a530ed26b46eee46941dbadbb46db7466d5e5ce9d18d067dc815b0d3052467
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.3 MB (205343046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cbd10085e3bd8e389031b83d712cb3a42365b13f88c647a9ee795d92151879d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 21:11:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:11:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 25 Oct 2022 21:11:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 25 Oct 2022 21:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV LC_ALL=C.UTF-8
# Tue, 25 Oct 2022 21:11:43 GMT
ENV ROS_DISTRO=noetic
# Tue, 25 Oct 2022 21:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 21:14:39 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 25 Oct 2022 21:14:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 25 Oct 2022 21:14:39 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9660e190ed5a21f6a47fc8cfa949892297824fc48480ba11a5119f126a25b4`  
		Last Modified: Tue, 25 Oct 2022 22:01:28 GMT  
		Size: 1.2 MB (1165046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b01fcd3ecd6496f537d89e10c06e3e8b4c184964ea86d849208d9347132cde`  
		Last Modified: Tue, 25 Oct 2022 22:01:26 GMT  
		Size: 5.5 MB (5532164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7354b266abeda9b5bfbca97ad1c6887d2a277d69ff8c607591a279459548ac7`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d614279c49f19055c903676e10afd41c8a3cd40f35d8b708fb499f7b5eeb965f`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c1b3c16d04da075eb127cecb646f3fbb43b07575ac781c7f670ca3f1885796`  
		Last Modified: Tue, 25 Oct 2022 22:01:55 GMT  
		Size: 171.4 MB (171447425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ac303ffe5e80a8c48e68fb479034e19261f5b6990dd5100bc6ddb1c7cd38ff`  
		Last Modified: Tue, 25 Oct 2022 22:01:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:52e537f081689f869e17eba032a5823026460f47629f95bc67e21a5e56c2efc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:9430a7637ae4815caed41d87692b703632da64fd1a8de7ac44b5c199a12e2ac1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263218750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3dfdf0214d49e84f92358bad18d5930aff35bc4535ba77dcc7a86f7de754d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:19:39 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:20:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:20:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:20:22 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:20:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:20:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:21:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11614817332af0948a51dccc0ac2fec8909f110de95b78985b29b8c3f7e970c1`  
		Last Modified: Wed, 02 Nov 2022 19:27:43 GMT  
		Size: 106.4 MB (106391794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0fa3a122b2ab87848b5d17fb2971645d70a05f26186dd83469908b5fc2782c9`  
		Last Modified: Wed, 02 Nov 2022 19:27:26 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c81e1547a26a3218c2267d44cb59398accac32565a64a6526e08ec328e7c02`  
		Last Modified: Wed, 02 Nov 2022 19:28:07 GMT  
		Size: 97.9 MB (97877379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858964a9bd3e2e8940d46dbde3c2ce321709ef75f592a61f57a5ca4e07fa2831`  
		Last Modified: Wed, 02 Nov 2022 19:27:53 GMT  
		Size: 289.4 KB (289400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0640f0773691621eb15edf8ccd1698f345f1b4699b5af20ff717c88bb98c9829`  
		Last Modified: Wed, 02 Nov 2022 19:27:53 GMT  
		Size: 2.4 KB (2428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed0d6a369f889af68dd4862416c0e68f68a9969b60471cce35083066e2f6016`  
		Last Modified: Wed, 02 Nov 2022 19:27:57 GMT  
		Size: 23.2 MB (23226886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a5945b491de4196efdef4843bba371f59e23bddde4204fff13e47ea8ee3df733
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255895077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f918a8ac17e4a8d5361a811437447bf16e701d3f1ca9971a0fe15934797a771`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:35:10 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:35:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:35:46 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:35:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:35:46 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:36:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:36:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:36:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe01c46c01bb82aca483b1c908f1f744fbf5f514d7bc29127dc2d13c92c43fd`  
		Last Modified: Wed, 02 Nov 2022 19:42:12 GMT  
		Size: 104.1 MB (104124486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b03d2faf31fcaa3607b8d6642d0d7aebc0c888fc741c6b7477337a853bbe199`  
		Last Modified: Wed, 02 Nov 2022 19:41:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b049aee909eee07c3fa6b0c4f58011d3c0b7fe37b557f63a4d7e9478d6426c`  
		Last Modified: Wed, 02 Nov 2022 19:42:35 GMT  
		Size: 95.5 MB (95469657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8551cbc2119bf668a98a498c06abc19d631c957ccee72b943b0e777f8d753d5`  
		Last Modified: Wed, 02 Nov 2022 19:42:22 GMT  
		Size: 289.4 KB (289398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972484bf36906e4dd12b81cac9aa26295bd1d13f6838fab80ff0e64f43087fe`  
		Last Modified: Wed, 02 Nov 2022 19:42:22 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541b9210000350e8829f8d302124c9abcadadb3cfe9864f3e7a31501dbe09394`  
		Last Modified: Wed, 02 Nov 2022 19:42:25 GMT  
		Size: 22.6 MB (22649561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:d79ccd7561dcacb4b4fa66ca6e7ee080ff1007589e08d752dd6f1689b068df2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:c707693a17cb1202f7d3b768375b47a05a0b094774da0232c28521a08f8d3f7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1088044067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6945dfdc6002b8534b26426c1e357864873a77407d82cd9b9eeb4e39ea43ba39`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:19:39 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:20:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:20:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:20:22 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:20:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:20:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:21:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:23:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11614817332af0948a51dccc0ac2fec8909f110de95b78985b29b8c3f7e970c1`  
		Last Modified: Wed, 02 Nov 2022 19:27:43 GMT  
		Size: 106.4 MB (106391794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0fa3a122b2ab87848b5d17fb2971645d70a05f26186dd83469908b5fc2782c9`  
		Last Modified: Wed, 02 Nov 2022 19:27:26 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c81e1547a26a3218c2267d44cb59398accac32565a64a6526e08ec328e7c02`  
		Last Modified: Wed, 02 Nov 2022 19:28:07 GMT  
		Size: 97.9 MB (97877379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858964a9bd3e2e8940d46dbde3c2ce321709ef75f592a61f57a5ca4e07fa2831`  
		Last Modified: Wed, 02 Nov 2022 19:27:53 GMT  
		Size: 289.4 KB (289400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0640f0773691621eb15edf8ccd1698f345f1b4699b5af20ff717c88bb98c9829`  
		Last Modified: Wed, 02 Nov 2022 19:27:53 GMT  
		Size: 2.4 KB (2428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed0d6a369f889af68dd4862416c0e68f68a9969b60471cce35083066e2f6016`  
		Last Modified: Wed, 02 Nov 2022 19:27:57 GMT  
		Size: 23.2 MB (23226886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7436de3271fc8bff591a3ebe7e1b4aa8f00c58b5b3eef5caff71c6f00296aa91`  
		Last Modified: Wed, 02 Nov 2022 19:29:58 GMT  
		Size: 824.8 MB (824825317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:063df331521058ec5e22196b792af1de98131252038c2bafffd7549eec23fbd1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1038299070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86dea3bee71f251642e1c5303029eabc420bcaf8bf30b36f3c2caa7b6f1417e3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:35:10 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:35:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:35:46 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:35:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:35:46 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:36:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:36:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:36:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:38:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe01c46c01bb82aca483b1c908f1f744fbf5f514d7bc29127dc2d13c92c43fd`  
		Last Modified: Wed, 02 Nov 2022 19:42:12 GMT  
		Size: 104.1 MB (104124486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b03d2faf31fcaa3607b8d6642d0d7aebc0c888fc741c6b7477337a853bbe199`  
		Last Modified: Wed, 02 Nov 2022 19:41:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b049aee909eee07c3fa6b0c4f58011d3c0b7fe37b557f63a4d7e9478d6426c`  
		Last Modified: Wed, 02 Nov 2022 19:42:35 GMT  
		Size: 95.5 MB (95469657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8551cbc2119bf668a98a498c06abc19d631c957ccee72b943b0e777f8d753d5`  
		Last Modified: Wed, 02 Nov 2022 19:42:22 GMT  
		Size: 289.4 KB (289398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972484bf36906e4dd12b81cac9aa26295bd1d13f6838fab80ff0e64f43087fe`  
		Last Modified: Wed, 02 Nov 2022 19:42:22 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541b9210000350e8829f8d302124c9abcadadb3cfe9864f3e7a31501dbe09394`  
		Last Modified: Wed, 02 Nov 2022 19:42:25 GMT  
		Size: 22.6 MB (22649561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab469ceb2c33ece432bce9e4ff984d91168e47ced17780485b30a39c0e2e6911`  
		Last Modified: Wed, 02 Nov 2022 19:43:59 GMT  
		Size: 782.4 MB (782403993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:d79ccd7561dcacb4b4fa66ca6e7ee080ff1007589e08d752dd6f1689b068df2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:c707693a17cb1202f7d3b768375b47a05a0b094774da0232c28521a08f8d3f7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1088044067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6945dfdc6002b8534b26426c1e357864873a77407d82cd9b9eeb4e39ea43ba39`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:19:39 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:20:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:20:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:20:22 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:20:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:20:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:21:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:23:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11614817332af0948a51dccc0ac2fec8909f110de95b78985b29b8c3f7e970c1`  
		Last Modified: Wed, 02 Nov 2022 19:27:43 GMT  
		Size: 106.4 MB (106391794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0fa3a122b2ab87848b5d17fb2971645d70a05f26186dd83469908b5fc2782c9`  
		Last Modified: Wed, 02 Nov 2022 19:27:26 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c81e1547a26a3218c2267d44cb59398accac32565a64a6526e08ec328e7c02`  
		Last Modified: Wed, 02 Nov 2022 19:28:07 GMT  
		Size: 97.9 MB (97877379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858964a9bd3e2e8940d46dbde3c2ce321709ef75f592a61f57a5ca4e07fa2831`  
		Last Modified: Wed, 02 Nov 2022 19:27:53 GMT  
		Size: 289.4 KB (289400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0640f0773691621eb15edf8ccd1698f345f1b4699b5af20ff717c88bb98c9829`  
		Last Modified: Wed, 02 Nov 2022 19:27:53 GMT  
		Size: 2.4 KB (2428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed0d6a369f889af68dd4862416c0e68f68a9969b60471cce35083066e2f6016`  
		Last Modified: Wed, 02 Nov 2022 19:27:57 GMT  
		Size: 23.2 MB (23226886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7436de3271fc8bff591a3ebe7e1b4aa8f00c58b5b3eef5caff71c6f00296aa91`  
		Last Modified: Wed, 02 Nov 2022 19:29:58 GMT  
		Size: 824.8 MB (824825317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:063df331521058ec5e22196b792af1de98131252038c2bafffd7549eec23fbd1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1038299070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86dea3bee71f251642e1c5303029eabc420bcaf8bf30b36f3c2caa7b6f1417e3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:35:10 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:35:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:35:46 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:35:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:35:46 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:36:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:36:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:36:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:38:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe01c46c01bb82aca483b1c908f1f744fbf5f514d7bc29127dc2d13c92c43fd`  
		Last Modified: Wed, 02 Nov 2022 19:42:12 GMT  
		Size: 104.1 MB (104124486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b03d2faf31fcaa3607b8d6642d0d7aebc0c888fc741c6b7477337a853bbe199`  
		Last Modified: Wed, 02 Nov 2022 19:41:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b049aee909eee07c3fa6b0c4f58011d3c0b7fe37b557f63a4d7e9478d6426c`  
		Last Modified: Wed, 02 Nov 2022 19:42:35 GMT  
		Size: 95.5 MB (95469657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8551cbc2119bf668a98a498c06abc19d631c957ccee72b943b0e777f8d753d5`  
		Last Modified: Wed, 02 Nov 2022 19:42:22 GMT  
		Size: 289.4 KB (289398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972484bf36906e4dd12b81cac9aa26295bd1d13f6838fab80ff0e64f43087fe`  
		Last Modified: Wed, 02 Nov 2022 19:42:22 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541b9210000350e8829f8d302124c9abcadadb3cfe9864f3e7a31501dbe09394`  
		Last Modified: Wed, 02 Nov 2022 19:42:25 GMT  
		Size: 22.6 MB (22649561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab469ceb2c33ece432bce9e4ff984d91168e47ced17780485b30a39c0e2e6911`  
		Last Modified: Wed, 02 Nov 2022 19:43:59 GMT  
		Size: 782.4 MB (782403993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:52e537f081689f869e17eba032a5823026460f47629f95bc67e21a5e56c2efc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:9430a7637ae4815caed41d87692b703632da64fd1a8de7ac44b5c199a12e2ac1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263218750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3dfdf0214d49e84f92358bad18d5930aff35bc4535ba77dcc7a86f7de754d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:19:39 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:20:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:20:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:20:22 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:20:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:20:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:21:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11614817332af0948a51dccc0ac2fec8909f110de95b78985b29b8c3f7e970c1`  
		Last Modified: Wed, 02 Nov 2022 19:27:43 GMT  
		Size: 106.4 MB (106391794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0fa3a122b2ab87848b5d17fb2971645d70a05f26186dd83469908b5fc2782c9`  
		Last Modified: Wed, 02 Nov 2022 19:27:26 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c81e1547a26a3218c2267d44cb59398accac32565a64a6526e08ec328e7c02`  
		Last Modified: Wed, 02 Nov 2022 19:28:07 GMT  
		Size: 97.9 MB (97877379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858964a9bd3e2e8940d46dbde3c2ce321709ef75f592a61f57a5ca4e07fa2831`  
		Last Modified: Wed, 02 Nov 2022 19:27:53 GMT  
		Size: 289.4 KB (289400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0640f0773691621eb15edf8ccd1698f345f1b4699b5af20ff717c88bb98c9829`  
		Last Modified: Wed, 02 Nov 2022 19:27:53 GMT  
		Size: 2.4 KB (2428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed0d6a369f889af68dd4862416c0e68f68a9969b60471cce35083066e2f6016`  
		Last Modified: Wed, 02 Nov 2022 19:27:57 GMT  
		Size: 23.2 MB (23226886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a5945b491de4196efdef4843bba371f59e23bddde4204fff13e47ea8ee3df733
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255895077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f918a8ac17e4a8d5361a811437447bf16e701d3f1ca9971a0fe15934797a771`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:35:10 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:35:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:35:46 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:35:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:35:46 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:36:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:36:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:36:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe01c46c01bb82aca483b1c908f1f744fbf5f514d7bc29127dc2d13c92c43fd`  
		Last Modified: Wed, 02 Nov 2022 19:42:12 GMT  
		Size: 104.1 MB (104124486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b03d2faf31fcaa3607b8d6642d0d7aebc0c888fc741c6b7477337a853bbe199`  
		Last Modified: Wed, 02 Nov 2022 19:41:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b049aee909eee07c3fa6b0c4f58011d3c0b7fe37b557f63a4d7e9478d6426c`  
		Last Modified: Wed, 02 Nov 2022 19:42:35 GMT  
		Size: 95.5 MB (95469657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8551cbc2119bf668a98a498c06abc19d631c957ccee72b943b0e777f8d753d5`  
		Last Modified: Wed, 02 Nov 2022 19:42:22 GMT  
		Size: 289.4 KB (289398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972484bf36906e4dd12b81cac9aa26295bd1d13f6838fab80ff0e64f43087fe`  
		Last Modified: Wed, 02 Nov 2022 19:42:22 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541b9210000350e8829f8d302124c9abcadadb3cfe9864f3e7a31501dbe09394`  
		Last Modified: Wed, 02 Nov 2022 19:42:25 GMT  
		Size: 22.6 MB (22649561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:52e537f081689f869e17eba032a5823026460f47629f95bc67e21a5e56c2efc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:9430a7637ae4815caed41d87692b703632da64fd1a8de7ac44b5c199a12e2ac1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263218750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3dfdf0214d49e84f92358bad18d5930aff35bc4535ba77dcc7a86f7de754d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:19:39 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:20:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:20:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:20:22 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:20:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:20:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:21:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11614817332af0948a51dccc0ac2fec8909f110de95b78985b29b8c3f7e970c1`  
		Last Modified: Wed, 02 Nov 2022 19:27:43 GMT  
		Size: 106.4 MB (106391794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0fa3a122b2ab87848b5d17fb2971645d70a05f26186dd83469908b5fc2782c9`  
		Last Modified: Wed, 02 Nov 2022 19:27:26 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c81e1547a26a3218c2267d44cb59398accac32565a64a6526e08ec328e7c02`  
		Last Modified: Wed, 02 Nov 2022 19:28:07 GMT  
		Size: 97.9 MB (97877379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858964a9bd3e2e8940d46dbde3c2ce321709ef75f592a61f57a5ca4e07fa2831`  
		Last Modified: Wed, 02 Nov 2022 19:27:53 GMT  
		Size: 289.4 KB (289400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0640f0773691621eb15edf8ccd1698f345f1b4699b5af20ff717c88bb98c9829`  
		Last Modified: Wed, 02 Nov 2022 19:27:53 GMT  
		Size: 2.4 KB (2428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed0d6a369f889af68dd4862416c0e68f68a9969b60471cce35083066e2f6016`  
		Last Modified: Wed, 02 Nov 2022 19:27:57 GMT  
		Size: 23.2 MB (23226886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a5945b491de4196efdef4843bba371f59e23bddde4204fff13e47ea8ee3df733
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255895077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f918a8ac17e4a8d5361a811437447bf16e701d3f1ca9971a0fe15934797a771`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:35:10 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:35:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:35:46 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:35:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:35:46 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:36:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:36:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Nov 2022 19:36:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 02 Nov 2022 19:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe01c46c01bb82aca483b1c908f1f744fbf5f514d7bc29127dc2d13c92c43fd`  
		Last Modified: Wed, 02 Nov 2022 19:42:12 GMT  
		Size: 104.1 MB (104124486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b03d2faf31fcaa3607b8d6642d0d7aebc0c888fc741c6b7477337a853bbe199`  
		Last Modified: Wed, 02 Nov 2022 19:41:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b049aee909eee07c3fa6b0c4f58011d3c0b7fe37b557f63a4d7e9478d6426c`  
		Last Modified: Wed, 02 Nov 2022 19:42:35 GMT  
		Size: 95.5 MB (95469657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8551cbc2119bf668a98a498c06abc19d631c957ccee72b943b0e777f8d753d5`  
		Last Modified: Wed, 02 Nov 2022 19:42:22 GMT  
		Size: 289.4 KB (289398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972484bf36906e4dd12b81cac9aa26295bd1d13f6838fab80ff0e64f43087fe`  
		Last Modified: Wed, 02 Nov 2022 19:42:22 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541b9210000350e8829f8d302124c9abcadadb3cfe9864f3e7a31501dbe09394`  
		Last Modified: Wed, 02 Nov 2022 19:42:25 GMT  
		Size: 22.6 MB (22649561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:09462aee0815a4e78b9b755769d805e2f999b5d94e6aad4a958dfa1859627894
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:300f09c7c4c4922805309d27bf9ce31cce8c69de2d4b5b5fe89a781fcdd65a2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141822657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dfe26daf1d7246d5e5a14976e6508af0276c90382fbef5b92acfa3905df1100`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:19:39 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:20:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:20:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:20:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11614817332af0948a51dccc0ac2fec8909f110de95b78985b29b8c3f7e970c1`  
		Last Modified: Wed, 02 Nov 2022 19:27:43 GMT  
		Size: 106.4 MB (106391794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0fa3a122b2ab87848b5d17fb2971645d70a05f26186dd83469908b5fc2782c9`  
		Last Modified: Wed, 02 Nov 2022 19:27:26 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2fa82fc9712adf8939173b6b69926b5de8f62637b57115f0089595207ddeaae6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137484035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ce525d434486e5df407554c6885b5814dfade488b61e23111b16235fa6d910`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:35:10 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:35:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:35:46 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:35:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:35:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe01c46c01bb82aca483b1c908f1f744fbf5f514d7bc29127dc2d13c92c43fd`  
		Last Modified: Wed, 02 Nov 2022 19:42:12 GMT  
		Size: 104.1 MB (104124486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b03d2faf31fcaa3607b8d6642d0d7aebc0c888fc741c6b7477337a853bbe199`  
		Last Modified: Wed, 02 Nov 2022 19:41:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:09462aee0815a4e78b9b755769d805e2f999b5d94e6aad4a958dfa1859627894
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:300f09c7c4c4922805309d27bf9ce31cce8c69de2d4b5b5fe89a781fcdd65a2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141822657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dfe26daf1d7246d5e5a14976e6508af0276c90382fbef5b92acfa3905df1100`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:07:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:07:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:07:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:19:39 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:20:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:20:21 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:20:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:20:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e309791760cb897f78d6ecdca3ecfa35842379a8f68578fae97e3ed231487`  
		Last Modified: Wed, 02 Nov 2022 19:24:38 GMT  
		Size: 1.2 MB (1174801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1968667a68200295ab81fbbe7a340eefffe28e7765ccce0ac08e4e840058f`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 3.8 MB (3828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ba109583179b86f91d9cef7488e67ac530a78c620ebe127cde962b001e8bf`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00beac66efa2733f4c56752491978562f4fd073a619736ec1ee66f17d44324c7`  
		Last Modified: Wed, 02 Nov 2022 19:24:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11614817332af0948a51dccc0ac2fec8909f110de95b78985b29b8c3f7e970c1`  
		Last Modified: Wed, 02 Nov 2022 19:27:43 GMT  
		Size: 106.4 MB (106391794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0fa3a122b2ab87848b5d17fb2971645d70a05f26186dd83469908b5fc2782c9`  
		Last Modified: Wed, 02 Nov 2022 19:27:26 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2fa82fc9712adf8939173b6b69926b5de8f62637b57115f0089595207ddeaae6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137484035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ce525d434486e5df407554c6885b5814dfade488b61e23111b16235fa6d910`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:21:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:21:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Nov 2022 19:21:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LANG=C.UTF-8
# Wed, 02 Nov 2022 19:21:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Nov 2022 19:35:10 GMT
ENV ROS_DISTRO=rolling
# Wed, 02 Nov 2022 19:35:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:35:46 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 02 Nov 2022 19:35:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Nov 2022 19:35:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11760287344b02d03930af87d27c6b9dc1acc8842adc4df018fbc979edafe07e`  
		Last Modified: Wed, 02 Nov 2022 19:39:41 GMT  
		Size: 1.2 MB (1175024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57286bbac2dc9c1c64117272c5610b0ccabf76c64c0d83ada53661e5bd6c7235`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 3.8 MB (3799957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe77194dbcb3cb1b9324930f565438ef05948cba7bb01a453e85a976f50cb1f`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeeadbd7d6fc1cd7ec48cf66192a01ee8304012593c12a1aaa6934e051205a1`  
		Last Modified: Wed, 02 Nov 2022 19:39:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe01c46c01bb82aca483b1c908f1f744fbf5f514d7bc29127dc2d13c92c43fd`  
		Last Modified: Wed, 02 Nov 2022 19:42:12 GMT  
		Size: 104.1 MB (104124486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b03d2faf31fcaa3607b8d6642d0d7aebc0c888fc741c6b7477337a853bbe199`  
		Last Modified: Wed, 02 Nov 2022 19:41:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
