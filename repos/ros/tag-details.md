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
$ docker pull ros@sha256:0c0e69ff71d21bff3a263c54143a60ea28ecebe24e3c01fdcfc642f883088914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:c6c4dcdcdba4646d8a6bebd6448625ed80cb18d8f1cae85e21a55a7e3d7ffec2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236641898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df65e6ff4c8f4ed1107f086582df71878afcbeb8d71e39214959ca5517adda77`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV ROS_DISTRO=foxy
# Tue, 27 Jul 2021 01:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:03:15 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:03:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:03:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:04:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:04:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:04:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e1e6579146c6323e3e1408e11008ac77c4d5c5ed8e5943332bc7254a56a5`  
		Last Modified: Tue, 27 Jul 2021 01:17:18 GMT  
		Size: 120.0 MB (119974774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88662ced653f598458e0c89695b0fb9e3e8bce9259f6efed11574a8f7ae220f5`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588ff9fb226bda0f04608743623449eccc27c7cc333932238b83bb7ec32398ea`  
		Last Modified: Tue, 27 Jul 2021 01:17:40 GMT  
		Size: 70.8 MB (70843719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a912ea800775dd8e48e78dac7555405832fcd4ad530eeae4cc976ba08ed32dbf`  
		Last Modified: Tue, 27 Jul 2021 01:17:30 GMT  
		Size: 238.5 KB (238478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b8c908ab26db0ef9598ff88bf38a1008a48fa6cc4f426e318321c589e254b4`  
		Last Modified: Tue, 27 Jul 2021 01:17:29 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ba81eeaf2f769cfb5f06e3b9de2651d04e9927d713613e7e5e7f86afbdba4`  
		Last Modified: Tue, 27 Jul 2021 01:17:32 GMT  
		Size: 10.3 MB (10282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cdcae8270776ec90508842a8c4507bb33cdc7d4214929a81086e14995baaca01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212758009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55fb2a38e2f521cb18fcad29f129d0d60d00ccfff4b77004a8f8f5c0e8dc4d75`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV ROS_DISTRO=foxy
# Mon, 26 Jul 2021 23:08:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:09:00 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:09:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:09:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:09:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99638d27524b744be6c72b148745cecbd30fce62732e56202509249a739f015`  
		Last Modified: Mon, 26 Jul 2021 23:24:01 GMT  
		Size: 104.2 MB (104166106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0795de1605d5236fe906b0103be795fd0d5906337ac8e1219ab8680fc286d6cc`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9212adaf308df7200d272b55747b777ee4c3f69fd8c33ed43a8cff46b456bcc`  
		Last Modified: Mon, 26 Jul 2021 23:24:25 GMT  
		Size: 65.2 MB (65183893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31858964d3495f929c4fbd43404976dce2b87c812a4a25b1a0c2c83dd29fddd`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 238.5 KB (238481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c120cd143733715303fadf97c47bb4fc1cb0590feeb076c32ccfe7258ac90b`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28758a874a9f9821a0fabd399ffae95818ddd755930e5b479087a3bd9b77b272`  
		Last Modified: Mon, 26 Jul 2021 23:24:16 GMT  
		Size: 9.3 MB (9298707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:0c0e69ff71d21bff3a263c54143a60ea28ecebe24e3c01fdcfc642f883088914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:c6c4dcdcdba4646d8a6bebd6448625ed80cb18d8f1cae85e21a55a7e3d7ffec2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236641898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df65e6ff4c8f4ed1107f086582df71878afcbeb8d71e39214959ca5517adda77`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV ROS_DISTRO=foxy
# Tue, 27 Jul 2021 01:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:03:15 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:03:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:03:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:04:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:04:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:04:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e1e6579146c6323e3e1408e11008ac77c4d5c5ed8e5943332bc7254a56a5`  
		Last Modified: Tue, 27 Jul 2021 01:17:18 GMT  
		Size: 120.0 MB (119974774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88662ced653f598458e0c89695b0fb9e3e8bce9259f6efed11574a8f7ae220f5`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588ff9fb226bda0f04608743623449eccc27c7cc333932238b83bb7ec32398ea`  
		Last Modified: Tue, 27 Jul 2021 01:17:40 GMT  
		Size: 70.8 MB (70843719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a912ea800775dd8e48e78dac7555405832fcd4ad530eeae4cc976ba08ed32dbf`  
		Last Modified: Tue, 27 Jul 2021 01:17:30 GMT  
		Size: 238.5 KB (238478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b8c908ab26db0ef9598ff88bf38a1008a48fa6cc4f426e318321c589e254b4`  
		Last Modified: Tue, 27 Jul 2021 01:17:29 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ba81eeaf2f769cfb5f06e3b9de2651d04e9927d713613e7e5e7f86afbdba4`  
		Last Modified: Tue, 27 Jul 2021 01:17:32 GMT  
		Size: 10.3 MB (10282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cdcae8270776ec90508842a8c4507bb33cdc7d4214929a81086e14995baaca01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212758009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55fb2a38e2f521cb18fcad29f129d0d60d00ccfff4b77004a8f8f5c0e8dc4d75`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV ROS_DISTRO=foxy
# Mon, 26 Jul 2021 23:08:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:09:00 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:09:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:09:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:09:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99638d27524b744be6c72b148745cecbd30fce62732e56202509249a739f015`  
		Last Modified: Mon, 26 Jul 2021 23:24:01 GMT  
		Size: 104.2 MB (104166106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0795de1605d5236fe906b0103be795fd0d5906337ac8e1219ab8680fc286d6cc`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9212adaf308df7200d272b55747b777ee4c3f69fd8c33ed43a8cff46b456bcc`  
		Last Modified: Mon, 26 Jul 2021 23:24:25 GMT  
		Size: 65.2 MB (65183893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31858964d3495f929c4fbd43404976dce2b87c812a4a25b1a0c2c83dd29fddd`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 238.5 KB (238481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c120cd143733715303fadf97c47bb4fc1cb0590feeb076c32ccfe7258ac90b`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28758a874a9f9821a0fabd399ffae95818ddd755930e5b479087a3bd9b77b272`  
		Last Modified: Mon, 26 Jul 2021 23:24:16 GMT  
		Size: 9.3 MB (9298707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:0c0e69ff71d21bff3a263c54143a60ea28ecebe24e3c01fdcfc642f883088914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:c6c4dcdcdba4646d8a6bebd6448625ed80cb18d8f1cae85e21a55a7e3d7ffec2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236641898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df65e6ff4c8f4ed1107f086582df71878afcbeb8d71e39214959ca5517adda77`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV ROS_DISTRO=foxy
# Tue, 27 Jul 2021 01:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:03:15 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:03:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:03:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:04:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:04:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:04:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e1e6579146c6323e3e1408e11008ac77c4d5c5ed8e5943332bc7254a56a5`  
		Last Modified: Tue, 27 Jul 2021 01:17:18 GMT  
		Size: 120.0 MB (119974774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88662ced653f598458e0c89695b0fb9e3e8bce9259f6efed11574a8f7ae220f5`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588ff9fb226bda0f04608743623449eccc27c7cc333932238b83bb7ec32398ea`  
		Last Modified: Tue, 27 Jul 2021 01:17:40 GMT  
		Size: 70.8 MB (70843719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a912ea800775dd8e48e78dac7555405832fcd4ad530eeae4cc976ba08ed32dbf`  
		Last Modified: Tue, 27 Jul 2021 01:17:30 GMT  
		Size: 238.5 KB (238478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b8c908ab26db0ef9598ff88bf38a1008a48fa6cc4f426e318321c589e254b4`  
		Last Modified: Tue, 27 Jul 2021 01:17:29 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ba81eeaf2f769cfb5f06e3b9de2651d04e9927d713613e7e5e7f86afbdba4`  
		Last Modified: Tue, 27 Jul 2021 01:17:32 GMT  
		Size: 10.3 MB (10282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cdcae8270776ec90508842a8c4507bb33cdc7d4214929a81086e14995baaca01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212758009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55fb2a38e2f521cb18fcad29f129d0d60d00ccfff4b77004a8f8f5c0e8dc4d75`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV ROS_DISTRO=foxy
# Mon, 26 Jul 2021 23:08:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:09:00 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:09:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:09:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:09:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99638d27524b744be6c72b148745cecbd30fce62732e56202509249a739f015`  
		Last Modified: Mon, 26 Jul 2021 23:24:01 GMT  
		Size: 104.2 MB (104166106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0795de1605d5236fe906b0103be795fd0d5906337ac8e1219ab8680fc286d6cc`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9212adaf308df7200d272b55747b777ee4c3f69fd8c33ed43a8cff46b456bcc`  
		Last Modified: Mon, 26 Jul 2021 23:24:25 GMT  
		Size: 65.2 MB (65183893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31858964d3495f929c4fbd43404976dce2b87c812a4a25b1a0c2c83dd29fddd`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 238.5 KB (238481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c120cd143733715303fadf97c47bb4fc1cb0590feeb076c32ccfe7258ac90b`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28758a874a9f9821a0fabd399ffae95818ddd755930e5b479087a3bd9b77b272`  
		Last Modified: Mon, 26 Jul 2021 23:24:16 GMT  
		Size: 9.3 MB (9298707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:eab9b11a845016bee4638f3414a05b8ded6d6aedd04b5bc6dd97d328e0686828
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:683ba2918ce69e5a9601828f8f0391af5a2bcc2dca4343f9d25454e361453575
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155274668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15b928b800f2e72749a36214430a363fdcd8e269b7956906b3a97a5728fc34af`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV ROS_DISTRO=foxy
# Tue, 27 Jul 2021 01:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:03:15 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:03:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:03:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e1e6579146c6323e3e1408e11008ac77c4d5c5ed8e5943332bc7254a56a5`  
		Last Modified: Tue, 27 Jul 2021 01:17:18 GMT  
		Size: 120.0 MB (119974774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88662ced653f598458e0c89695b0fb9e3e8bce9259f6efed11574a8f7ae220f5`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c4be163773f08ea2e728544988ebf8ef9545de979f9ad9a0124558d0ab537e2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138034880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5e7fc093ea6760870f1da1a83c5881f5a7c7192e05c3da54fe689c2e96670c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV ROS_DISTRO=foxy
# Mon, 26 Jul 2021 23:08:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:09:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99638d27524b744be6c72b148745cecbd30fce62732e56202509249a739f015`  
		Last Modified: Mon, 26 Jul 2021 23:24:01 GMT  
		Size: 104.2 MB (104166106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0795de1605d5236fe906b0103be795fd0d5906337ac8e1219ab8680fc286d6cc`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:eab9b11a845016bee4638f3414a05b8ded6d6aedd04b5bc6dd97d328e0686828
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:683ba2918ce69e5a9601828f8f0391af5a2bcc2dca4343f9d25454e361453575
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155274668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15b928b800f2e72749a36214430a363fdcd8e269b7956906b3a97a5728fc34af`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV ROS_DISTRO=foxy
# Tue, 27 Jul 2021 01:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:03:15 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:03:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:03:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e1e6579146c6323e3e1408e11008ac77c4d5c5ed8e5943332bc7254a56a5`  
		Last Modified: Tue, 27 Jul 2021 01:17:18 GMT  
		Size: 120.0 MB (119974774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88662ced653f598458e0c89695b0fb9e3e8bce9259f6efed11574a8f7ae220f5`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c4be163773f08ea2e728544988ebf8ef9545de979f9ad9a0124558d0ab537e2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138034880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5e7fc093ea6760870f1da1a83c5881f5a7c7192e05c3da54fe689c2e96670c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV ROS_DISTRO=foxy
# Mon, 26 Jul 2021 23:08:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:09:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99638d27524b744be6c72b148745cecbd30fce62732e56202509249a739f015`  
		Last Modified: Mon, 26 Jul 2021 23:24:01 GMT  
		Size: 104.2 MB (104166106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0795de1605d5236fe906b0103be795fd0d5906337ac8e1219ab8680fc286d6cc`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:1eac0797ab9b5c85378d7bbdf17d4db3199b7f437b001c17ccbbe5ded7c0ad00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:ef32e4aab556e47f966d7f47f8a0be2b2a4fc87430d768aad7a8278d21fbf7ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.5 MB (345507825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0de2bd00b710b309f04b3b8aece716e377b986ae69afa53efb7b861e4a96966`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV ROS_DISTRO=foxy
# Tue, 27 Jul 2021 01:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:03:15 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:03:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:03:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:04:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:04:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:04:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:04:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:04:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:04:34 GMT
ENV ROS1_DISTRO=noetic
# Tue, 27 Jul 2021 01:04:34 GMT
ENV ROS2_DISTRO=foxy
# Tue, 27 Jul 2021 01:05:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:05:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:05:29 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e1e6579146c6323e3e1408e11008ac77c4d5c5ed8e5943332bc7254a56a5`  
		Last Modified: Tue, 27 Jul 2021 01:17:18 GMT  
		Size: 120.0 MB (119974774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88662ced653f598458e0c89695b0fb9e3e8bce9259f6efed11574a8f7ae220f5`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588ff9fb226bda0f04608743623449eccc27c7cc333932238b83bb7ec32398ea`  
		Last Modified: Tue, 27 Jul 2021 01:17:40 GMT  
		Size: 70.8 MB (70843719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a912ea800775dd8e48e78dac7555405832fcd4ad530eeae4cc976ba08ed32dbf`  
		Last Modified: Tue, 27 Jul 2021 01:17:30 GMT  
		Size: 238.5 KB (238478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b8c908ab26db0ef9598ff88bf38a1008a48fa6cc4f426e318321c589e254b4`  
		Last Modified: Tue, 27 Jul 2021 01:17:29 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ba81eeaf2f769cfb5f06e3b9de2651d04e9927d713613e7e5e7f86afbdba4`  
		Last Modified: Tue, 27 Jul 2021 01:17:32 GMT  
		Size: 10.3 MB (10282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1506323a6748382badefb23bfb9e1426f36effd5b82d16d2694254e19f54c03d`  
		Last Modified: Tue, 27 Jul 2021 01:17:59 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94de0348dafb927ad69bfc28f49be82b04b67c489cbe28bbc61baca8fbd39aeb`  
		Last Modified: Tue, 27 Jul 2021 01:17:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b47f0b815bcd2eccc5fb521011a383e33f7df3c2e30dd4d21b5eff73327010`  
		Last Modified: Tue, 27 Jul 2021 01:18:14 GMT  
		Size: 76.1 MB (76130117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdf772cea424f27ffc6c8f44f4a54a1dc80fda4e2b8743d45cbf23f2de229f8`  
		Last Modified: Tue, 27 Jul 2021 01:18:05 GMT  
		Size: 32.7 MB (32735183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9353bf32a09ff870393a278312567b5a5dfcc62266e8569b44819c45946d61`  
		Last Modified: Tue, 27 Jul 2021 01:17:59 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d597d5e7c208683e0f65b765d88df852a350ac74f749753a26335733657316bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (314030519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72880d992a4585224fda3bda11e0f3afe8f4491229781d73bd198496f292b92f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV ROS_DISTRO=foxy
# Mon, 26 Jul 2021 23:08:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:09:00 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:09:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:09:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:09:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:09:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:09:53 GMT
ENV ROS1_DISTRO=noetic
# Mon, 26 Jul 2021 23:09:53 GMT
ENV ROS2_DISTRO=foxy
# Mon, 26 Jul 2021 23:10:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:10:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:10:36 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99638d27524b744be6c72b148745cecbd30fce62732e56202509249a739f015`  
		Last Modified: Mon, 26 Jul 2021 23:24:01 GMT  
		Size: 104.2 MB (104166106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0795de1605d5236fe906b0103be795fd0d5906337ac8e1219ab8680fc286d6cc`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9212adaf308df7200d272b55747b777ee4c3f69fd8c33ed43a8cff46b456bcc`  
		Last Modified: Mon, 26 Jul 2021 23:24:25 GMT  
		Size: 65.2 MB (65183893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31858964d3495f929c4fbd43404976dce2b87c812a4a25b1a0c2c83dd29fddd`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 238.5 KB (238481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c120cd143733715303fadf97c47bb4fc1cb0590feeb076c32ccfe7258ac90b`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28758a874a9f9821a0fabd399ffae95818ddd755930e5b479087a3bd9b77b272`  
		Last Modified: Mon, 26 Jul 2021 23:24:16 GMT  
		Size: 9.3 MB (9298707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56248d6b9a01933af094d8757699870aa609465d4792cfd4e0336e2c7e26161a`  
		Last Modified: Mon, 26 Jul 2021 23:24:51 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a54c8d0b154ce4292783bb78ca5f06e3b98159d11a7c15f87c7f371031021`  
		Last Modified: Mon, 26 Jul 2021 23:24:47 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd615e8d8979e0faeed49833a47290b5855be669fd01bcacb56a7412c847bf52`  
		Last Modified: Mon, 26 Jul 2021 23:25:09 GMT  
		Size: 76.2 MB (76162720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d6e1650f37b0d617071d14fbfffac08300c16ab3d0bd4b79239545bac4a29`  
		Last Modified: Mon, 26 Jul 2021 23:24:51 GMT  
		Size: 25.1 MB (25109167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f4006067a03d7813622e41f0d355ebfc4a95c87751a77c4ecd33a9824c42a`  
		Last Modified: Mon, 26 Jul 2021 23:24:47 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:1eac0797ab9b5c85378d7bbdf17d4db3199b7f437b001c17ccbbe5ded7c0ad00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:ef32e4aab556e47f966d7f47f8a0be2b2a4fc87430d768aad7a8278d21fbf7ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.5 MB (345507825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0de2bd00b710b309f04b3b8aece716e377b986ae69afa53efb7b861e4a96966`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV ROS_DISTRO=foxy
# Tue, 27 Jul 2021 01:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:03:15 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:03:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:03:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:04:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:04:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:04:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:04:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:04:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:04:34 GMT
ENV ROS1_DISTRO=noetic
# Tue, 27 Jul 2021 01:04:34 GMT
ENV ROS2_DISTRO=foxy
# Tue, 27 Jul 2021 01:05:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:05:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:05:29 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e1e6579146c6323e3e1408e11008ac77c4d5c5ed8e5943332bc7254a56a5`  
		Last Modified: Tue, 27 Jul 2021 01:17:18 GMT  
		Size: 120.0 MB (119974774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88662ced653f598458e0c89695b0fb9e3e8bce9259f6efed11574a8f7ae220f5`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588ff9fb226bda0f04608743623449eccc27c7cc333932238b83bb7ec32398ea`  
		Last Modified: Tue, 27 Jul 2021 01:17:40 GMT  
		Size: 70.8 MB (70843719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a912ea800775dd8e48e78dac7555405832fcd4ad530eeae4cc976ba08ed32dbf`  
		Last Modified: Tue, 27 Jul 2021 01:17:30 GMT  
		Size: 238.5 KB (238478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b8c908ab26db0ef9598ff88bf38a1008a48fa6cc4f426e318321c589e254b4`  
		Last Modified: Tue, 27 Jul 2021 01:17:29 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ba81eeaf2f769cfb5f06e3b9de2651d04e9927d713613e7e5e7f86afbdba4`  
		Last Modified: Tue, 27 Jul 2021 01:17:32 GMT  
		Size: 10.3 MB (10282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1506323a6748382badefb23bfb9e1426f36effd5b82d16d2694254e19f54c03d`  
		Last Modified: Tue, 27 Jul 2021 01:17:59 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94de0348dafb927ad69bfc28f49be82b04b67c489cbe28bbc61baca8fbd39aeb`  
		Last Modified: Tue, 27 Jul 2021 01:17:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b47f0b815bcd2eccc5fb521011a383e33f7df3c2e30dd4d21b5eff73327010`  
		Last Modified: Tue, 27 Jul 2021 01:18:14 GMT  
		Size: 76.1 MB (76130117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdf772cea424f27ffc6c8f44f4a54a1dc80fda4e2b8743d45cbf23f2de229f8`  
		Last Modified: Tue, 27 Jul 2021 01:18:05 GMT  
		Size: 32.7 MB (32735183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9353bf32a09ff870393a278312567b5a5dfcc62266e8569b44819c45946d61`  
		Last Modified: Tue, 27 Jul 2021 01:17:59 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d597d5e7c208683e0f65b765d88df852a350ac74f749753a26335733657316bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (314030519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72880d992a4585224fda3bda11e0f3afe8f4491229781d73bd198496f292b92f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV ROS_DISTRO=foxy
# Mon, 26 Jul 2021 23:08:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:09:00 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:09:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:09:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:09:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:09:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:09:53 GMT
ENV ROS1_DISTRO=noetic
# Mon, 26 Jul 2021 23:09:53 GMT
ENV ROS2_DISTRO=foxy
# Mon, 26 Jul 2021 23:10:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:10:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:10:36 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99638d27524b744be6c72b148745cecbd30fce62732e56202509249a739f015`  
		Last Modified: Mon, 26 Jul 2021 23:24:01 GMT  
		Size: 104.2 MB (104166106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0795de1605d5236fe906b0103be795fd0d5906337ac8e1219ab8680fc286d6cc`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9212adaf308df7200d272b55747b777ee4c3f69fd8c33ed43a8cff46b456bcc`  
		Last Modified: Mon, 26 Jul 2021 23:24:25 GMT  
		Size: 65.2 MB (65183893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31858964d3495f929c4fbd43404976dce2b87c812a4a25b1a0c2c83dd29fddd`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 238.5 KB (238481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c120cd143733715303fadf97c47bb4fc1cb0590feeb076c32ccfe7258ac90b`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28758a874a9f9821a0fabd399ffae95818ddd755930e5b479087a3bd9b77b272`  
		Last Modified: Mon, 26 Jul 2021 23:24:16 GMT  
		Size: 9.3 MB (9298707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56248d6b9a01933af094d8757699870aa609465d4792cfd4e0336e2c7e26161a`  
		Last Modified: Mon, 26 Jul 2021 23:24:51 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1a54c8d0b154ce4292783bb78ca5f06e3b98159d11a7c15f87c7f371031021`  
		Last Modified: Mon, 26 Jul 2021 23:24:47 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd615e8d8979e0faeed49833a47290b5855be669fd01bcacb56a7412c847bf52`  
		Last Modified: Mon, 26 Jul 2021 23:25:09 GMT  
		Size: 76.2 MB (76162720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d6e1650f37b0d617071d14fbfffac08300c16ab3d0bd4b79239545bac4a29`  
		Last Modified: Mon, 26 Jul 2021 23:24:51 GMT  
		Size: 25.1 MB (25109167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f4006067a03d7813622e41f0d355ebfc4a95c87751a77c4ecd33a9824c42a`  
		Last Modified: Mon, 26 Jul 2021 23:24:47 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:4b910e1df0882cb5aad51a9b87ff8695d762ee9e232927da22bd6e1d79ee9ee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:4d93293885527a8e099ba1d2e46b0f4540e78221490712adb30202e21c6278df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232069450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5776753f405d865e9853cfe70424e5cf92af3b3944c4c09533e41651a5aaaa4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:05:32 GMT
ENV ROS_DISTRO=galactic
# Tue, 27 Jul 2021 01:06:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:17 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:06:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:06:17 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:06:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:06:48 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698085f1b967a89a6f46a3ab27fbf0926f76b483b0843140c750e906cdbce36e`  
		Last Modified: Tue, 27 Jul 2021 01:18:43 GMT  
		Size: 103.6 MB (103633085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66de36d29cf49a4bbc2b20c3f5795f7d9c972b6c03fbfef58203d93014aab22`  
		Last Modified: Tue, 27 Jul 2021 01:18:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71385bc5f93112c08888184a0254508d98eb9c547e40f70af98924d3c7f7b735`  
		Last Modified: Tue, 27 Jul 2021 01:19:05 GMT  
		Size: 70.8 MB (70797407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6f08ba387a09b78071f694d7eb0fb4774c732d8bbeba44462bd43acc75d78f`  
		Last Modified: Tue, 27 Jul 2021 01:18:55 GMT  
		Size: 241.2 KB (241230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7990cf09456775859f728e71494b2adcec01b46fdbcda5a418970af90f5e5056`  
		Last Modified: Tue, 27 Jul 2021 01:18:55 GMT  
		Size: 2.0 KB (2026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23344c0439abccd2d4aff93d7e57f3697c56daad83902005a615a0e70e52a77c`  
		Last Modified: Tue, 27 Jul 2021 01:18:59 GMT  
		Size: 22.1 MB (22095808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:24914fea9b0162e326a242c6d5c993b63b27b7d8d630a1bbcc5cc773c114cb76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220716917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bac817d14f263a2045024f8fc69ed3b890e28a7de11711ef0a898b87ff8bbe2d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:10:43 GMT
ENV ROS_DISTRO=galactic
# Mon, 26 Jul 2021 23:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:11:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:11:26 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:11:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:12:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:12:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c0afa8948e130f316bf6e937a5009c86752b46a86110f2b0bc050963acae9a`  
		Last Modified: Mon, 26 Jul 2021 23:25:46 GMT  
		Size: 100.0 MB (100035926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacb211dd1e150cea7c549393186087c461f9055c1497d2fe1171b9b691a56e`  
		Last Modified: Mon, 26 Jul 2021 23:25:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791686871dcac1c755586850b4b34680c90d1a22eb2fb8e973797fa74ca00c`  
		Last Modified: Mon, 26 Jul 2021 23:26:11 GMT  
		Size: 65.1 MB (65138081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d6d89ff94a2c5bbf11ff673f6a8858ec987cf4c3a45ea8fadd495dbe19ebd4`  
		Last Modified: Mon, 26 Jul 2021 23:26:00 GMT  
		Size: 241.2 KB (241224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c0ee3348df19f1250bbf9b003b99c2eb1cdf51ca057364dae79d5e43ab5826`  
		Last Modified: Mon, 26 Jul 2021 23:25:59 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16deeb0c1f27f0ac61db069ece93545b39dd8ef8228c0d6e410445dfc02730f3`  
		Last Modified: Mon, 26 Jul 2021 23:26:04 GMT  
		Size: 21.4 MB (21430859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:4b910e1df0882cb5aad51a9b87ff8695d762ee9e232927da22bd6e1d79ee9ee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:4d93293885527a8e099ba1d2e46b0f4540e78221490712adb30202e21c6278df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232069450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5776753f405d865e9853cfe70424e5cf92af3b3944c4c09533e41651a5aaaa4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:05:32 GMT
ENV ROS_DISTRO=galactic
# Tue, 27 Jul 2021 01:06:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:17 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:06:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:06:17 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:06:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:06:48 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698085f1b967a89a6f46a3ab27fbf0926f76b483b0843140c750e906cdbce36e`  
		Last Modified: Tue, 27 Jul 2021 01:18:43 GMT  
		Size: 103.6 MB (103633085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66de36d29cf49a4bbc2b20c3f5795f7d9c972b6c03fbfef58203d93014aab22`  
		Last Modified: Tue, 27 Jul 2021 01:18:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71385bc5f93112c08888184a0254508d98eb9c547e40f70af98924d3c7f7b735`  
		Last Modified: Tue, 27 Jul 2021 01:19:05 GMT  
		Size: 70.8 MB (70797407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6f08ba387a09b78071f694d7eb0fb4774c732d8bbeba44462bd43acc75d78f`  
		Last Modified: Tue, 27 Jul 2021 01:18:55 GMT  
		Size: 241.2 KB (241230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7990cf09456775859f728e71494b2adcec01b46fdbcda5a418970af90f5e5056`  
		Last Modified: Tue, 27 Jul 2021 01:18:55 GMT  
		Size: 2.0 KB (2026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23344c0439abccd2d4aff93d7e57f3697c56daad83902005a615a0e70e52a77c`  
		Last Modified: Tue, 27 Jul 2021 01:18:59 GMT  
		Size: 22.1 MB (22095808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:24914fea9b0162e326a242c6d5c993b63b27b7d8d630a1bbcc5cc773c114cb76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220716917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bac817d14f263a2045024f8fc69ed3b890e28a7de11711ef0a898b87ff8bbe2d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:10:43 GMT
ENV ROS_DISTRO=galactic
# Mon, 26 Jul 2021 23:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:11:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:11:26 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:11:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:12:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:12:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c0afa8948e130f316bf6e937a5009c86752b46a86110f2b0bc050963acae9a`  
		Last Modified: Mon, 26 Jul 2021 23:25:46 GMT  
		Size: 100.0 MB (100035926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacb211dd1e150cea7c549393186087c461f9055c1497d2fe1171b9b691a56e`  
		Last Modified: Mon, 26 Jul 2021 23:25:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791686871dcac1c755586850b4b34680c90d1a22eb2fb8e973797fa74ca00c`  
		Last Modified: Mon, 26 Jul 2021 23:26:11 GMT  
		Size: 65.1 MB (65138081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d6d89ff94a2c5bbf11ff673f6a8858ec987cf4c3a45ea8fadd495dbe19ebd4`  
		Last Modified: Mon, 26 Jul 2021 23:26:00 GMT  
		Size: 241.2 KB (241224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c0ee3348df19f1250bbf9b003b99c2eb1cdf51ca057364dae79d5e43ab5826`  
		Last Modified: Mon, 26 Jul 2021 23:25:59 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16deeb0c1f27f0ac61db069ece93545b39dd8ef8228c0d6e410445dfc02730f3`  
		Last Modified: Mon, 26 Jul 2021 23:26:04 GMT  
		Size: 21.4 MB (21430859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:4b910e1df0882cb5aad51a9b87ff8695d762ee9e232927da22bd6e1d79ee9ee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:4d93293885527a8e099ba1d2e46b0f4540e78221490712adb30202e21c6278df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232069450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5776753f405d865e9853cfe70424e5cf92af3b3944c4c09533e41651a5aaaa4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:05:32 GMT
ENV ROS_DISTRO=galactic
# Tue, 27 Jul 2021 01:06:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:17 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:06:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:06:17 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:06:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:06:48 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698085f1b967a89a6f46a3ab27fbf0926f76b483b0843140c750e906cdbce36e`  
		Last Modified: Tue, 27 Jul 2021 01:18:43 GMT  
		Size: 103.6 MB (103633085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66de36d29cf49a4bbc2b20c3f5795f7d9c972b6c03fbfef58203d93014aab22`  
		Last Modified: Tue, 27 Jul 2021 01:18:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71385bc5f93112c08888184a0254508d98eb9c547e40f70af98924d3c7f7b735`  
		Last Modified: Tue, 27 Jul 2021 01:19:05 GMT  
		Size: 70.8 MB (70797407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6f08ba387a09b78071f694d7eb0fb4774c732d8bbeba44462bd43acc75d78f`  
		Last Modified: Tue, 27 Jul 2021 01:18:55 GMT  
		Size: 241.2 KB (241230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7990cf09456775859f728e71494b2adcec01b46fdbcda5a418970af90f5e5056`  
		Last Modified: Tue, 27 Jul 2021 01:18:55 GMT  
		Size: 2.0 KB (2026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23344c0439abccd2d4aff93d7e57f3697c56daad83902005a615a0e70e52a77c`  
		Last Modified: Tue, 27 Jul 2021 01:18:59 GMT  
		Size: 22.1 MB (22095808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:24914fea9b0162e326a242c6d5c993b63b27b7d8d630a1bbcc5cc773c114cb76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220716917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bac817d14f263a2045024f8fc69ed3b890e28a7de11711ef0a898b87ff8bbe2d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:10:43 GMT
ENV ROS_DISTRO=galactic
# Mon, 26 Jul 2021 23:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:11:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:11:26 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:11:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:12:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:12:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c0afa8948e130f316bf6e937a5009c86752b46a86110f2b0bc050963acae9a`  
		Last Modified: Mon, 26 Jul 2021 23:25:46 GMT  
		Size: 100.0 MB (100035926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacb211dd1e150cea7c549393186087c461f9055c1497d2fe1171b9b691a56e`  
		Last Modified: Mon, 26 Jul 2021 23:25:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791686871dcac1c755586850b4b34680c90d1a22eb2fb8e973797fa74ca00c`  
		Last Modified: Mon, 26 Jul 2021 23:26:11 GMT  
		Size: 65.1 MB (65138081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d6d89ff94a2c5bbf11ff673f6a8858ec987cf4c3a45ea8fadd495dbe19ebd4`  
		Last Modified: Mon, 26 Jul 2021 23:26:00 GMT  
		Size: 241.2 KB (241224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c0ee3348df19f1250bbf9b003b99c2eb1cdf51ca057364dae79d5e43ab5826`  
		Last Modified: Mon, 26 Jul 2021 23:25:59 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16deeb0c1f27f0ac61db069ece93545b39dd8ef8228c0d6e410445dfc02730f3`  
		Last Modified: Mon, 26 Jul 2021 23:26:04 GMT  
		Size: 21.4 MB (21430859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:692688917540052463916bb462853ab5f59b6fd3aed63aa6a0f367a4661862e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:232f4e33bd2c038a0c3a6eb10ae85cf9f051e079f6cb6b82f0a0146962120770
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138932979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c8bff07074d08c5e567030f617963bfbafa60010f72fea266cca3224238726`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:05:32 GMT
ENV ROS_DISTRO=galactic
# Tue, 27 Jul 2021 01:06:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:17 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:06:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:06:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698085f1b967a89a6f46a3ab27fbf0926f76b483b0843140c750e906cdbce36e`  
		Last Modified: Tue, 27 Jul 2021 01:18:43 GMT  
		Size: 103.6 MB (103633085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66de36d29cf49a4bbc2b20c3f5795f7d9c972b6c03fbfef58203d93014aab22`  
		Last Modified: Tue, 27 Jul 2021 01:18:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:42dacce98ba7958c04074a346997d440649f8c9734f0783092e749fe7b8781b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133904699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9379a018281708a6750c342fefa573be49224176d3a1b7c51d67948fb6fc0e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:10:43 GMT
ENV ROS_DISTRO=galactic
# Mon, 26 Jul 2021 23:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:11:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:11:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c0afa8948e130f316bf6e937a5009c86752b46a86110f2b0bc050963acae9a`  
		Last Modified: Mon, 26 Jul 2021 23:25:46 GMT  
		Size: 100.0 MB (100035926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacb211dd1e150cea7c549393186087c461f9055c1497d2fe1171b9b691a56e`  
		Last Modified: Mon, 26 Jul 2021 23:25:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:692688917540052463916bb462853ab5f59b6fd3aed63aa6a0f367a4661862e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:232f4e33bd2c038a0c3a6eb10ae85cf9f051e079f6cb6b82f0a0146962120770
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138932979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c8bff07074d08c5e567030f617963bfbafa60010f72fea266cca3224238726`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:05:32 GMT
ENV ROS_DISTRO=galactic
# Tue, 27 Jul 2021 01:06:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:17 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:06:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:06:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698085f1b967a89a6f46a3ab27fbf0926f76b483b0843140c750e906cdbce36e`  
		Last Modified: Tue, 27 Jul 2021 01:18:43 GMT  
		Size: 103.6 MB (103633085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66de36d29cf49a4bbc2b20c3f5795f7d9c972b6c03fbfef58203d93014aab22`  
		Last Modified: Tue, 27 Jul 2021 01:18:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:42dacce98ba7958c04074a346997d440649f8c9734f0783092e749fe7b8781b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133904699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9379a018281708a6750c342fefa573be49224176d3a1b7c51d67948fb6fc0e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:10:43 GMT
ENV ROS_DISTRO=galactic
# Mon, 26 Jul 2021 23:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:11:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:11:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c0afa8948e130f316bf6e937a5009c86752b46a86110f2b0bc050963acae9a`  
		Last Modified: Mon, 26 Jul 2021 23:25:46 GMT  
		Size: 100.0 MB (100035926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacb211dd1e150cea7c549393186087c461f9055c1497d2fe1171b9b691a56e`  
		Last Modified: Mon, 26 Jul 2021 23:25:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:0c839a314cd5819355c488d30401827225f533f128c790365cfd0e0939cb2f3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:3cfba0166cb37b1a2e2b252102343ed7bd265bae34092826d2b39e0664275208
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.8 MB (326842374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb19318f478c5ad3deebb1767360a541c56af0014dd542003565bd5e3e24bf1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:05:32 GMT
ENV ROS_DISTRO=galactic
# Tue, 27 Jul 2021 01:06:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:17 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:06:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:06:17 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:06:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:06:48 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:07:14 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:07:15 GMT
ENV ROS1_DISTRO=noetic
# Tue, 27 Jul 2021 01:07:16 GMT
ENV ROS2_DISTRO=galactic
# Tue, 27 Jul 2021 01:07:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:07:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:07:49 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698085f1b967a89a6f46a3ab27fbf0926f76b483b0843140c750e906cdbce36e`  
		Last Modified: Tue, 27 Jul 2021 01:18:43 GMT  
		Size: 103.6 MB (103633085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66de36d29cf49a4bbc2b20c3f5795f7d9c972b6c03fbfef58203d93014aab22`  
		Last Modified: Tue, 27 Jul 2021 01:18:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71385bc5f93112c08888184a0254508d98eb9c547e40f70af98924d3c7f7b735`  
		Last Modified: Tue, 27 Jul 2021 01:19:05 GMT  
		Size: 70.8 MB (70797407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6f08ba387a09b78071f694d7eb0fb4774c732d8bbeba44462bd43acc75d78f`  
		Last Modified: Tue, 27 Jul 2021 01:18:55 GMT  
		Size: 241.2 KB (241230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7990cf09456775859f728e71494b2adcec01b46fdbcda5a418970af90f5e5056`  
		Last Modified: Tue, 27 Jul 2021 01:18:55 GMT  
		Size: 2.0 KB (2026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23344c0439abccd2d4aff93d7e57f3697c56daad83902005a615a0e70e52a77c`  
		Last Modified: Tue, 27 Jul 2021 01:18:59 GMT  
		Size: 22.1 MB (22095808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14520e7f4d5e7abaa150d713df486bd446780cf35343d659c964a116fb83314d`  
		Last Modified: Tue, 27 Jul 2021 01:19:20 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89be30453f2f44b3a020e5ec2bfe5b2c6da662ed820f295c10522d1fd3d163da`  
		Last Modified: Tue, 27 Jul 2021 01:19:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83f5e8e2ce60a31e2b6723160edad367d80a1dd8677d7e650af6cd43d84cb6a`  
		Last Modified: Tue, 27 Jul 2021 01:19:35 GMT  
		Size: 78.4 MB (78409624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901678866177d90b4b62b1fe5d39bc27b9c4485b64c290167252b5f8d99f76f9`  
		Last Modified: Tue, 27 Jul 2021 01:19:24 GMT  
		Size: 16.4 MB (16362675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730b1b98982ff37b0d26a053f62a31f785d695504cc4b5e359ba3018868504af`  
		Last Modified: Tue, 27 Jul 2021 01:19:20 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:51365982d4827a84e316c48646392484d939ba70a820d43f462637024811fa89
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.0 MB (314981062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a4c5f72c39097736aa83ab7876f189de9b60787583f0f7f6184a73ab71b0855`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:10:43 GMT
ENV ROS_DISTRO=galactic
# Mon, 26 Jul 2021 23:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:11:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:11:26 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:11:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:12:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:12:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:12:27 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:12:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:12:28 GMT
ENV ROS1_DISTRO=noetic
# Mon, 26 Jul 2021 23:12:28 GMT
ENV ROS2_DISTRO=galactic
# Mon, 26 Jul 2021 23:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:13:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:13:07 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c0afa8948e130f316bf6e937a5009c86752b46a86110f2b0bc050963acae9a`  
		Last Modified: Mon, 26 Jul 2021 23:25:46 GMT  
		Size: 100.0 MB (100035926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacb211dd1e150cea7c549393186087c461f9055c1497d2fe1171b9b691a56e`  
		Last Modified: Mon, 26 Jul 2021 23:25:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791686871dcac1c755586850b4b34680c90d1a22eb2fb8e973797fa74ca00c`  
		Last Modified: Mon, 26 Jul 2021 23:26:11 GMT  
		Size: 65.1 MB (65138081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d6d89ff94a2c5bbf11ff673f6a8858ec987cf4c3a45ea8fadd495dbe19ebd4`  
		Last Modified: Mon, 26 Jul 2021 23:26:00 GMT  
		Size: 241.2 KB (241224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c0ee3348df19f1250bbf9b003b99c2eb1cdf51ca057364dae79d5e43ab5826`  
		Last Modified: Mon, 26 Jul 2021 23:25:59 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16deeb0c1f27f0ac61db069ece93545b39dd8ef8228c0d6e410445dfc02730f3`  
		Last Modified: Mon, 26 Jul 2021 23:26:04 GMT  
		Size: 21.4 MB (21430859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643322c5f06c1340568abc2f1700666a578e957621e104149c96726a12cef177`  
		Last Modified: Mon, 26 Jul 2021 23:26:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525060df38ebfe98320cd79ad7875e0870654a65c1bd2f2d7dd0a31ffba8516`  
		Last Modified: Mon, 26 Jul 2021 23:26:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a966924f783e389c9a5deb0b9584893f2989886735bc6f0c80d88eb3f3fb1519`  
		Last Modified: Mon, 26 Jul 2021 23:26:49 GMT  
		Size: 78.4 MB (78373807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f67a3aaa308e5228c9ab33d9f84a21f1ef9709987347cf151b3ae2e1a2a8aeb`  
		Last Modified: Mon, 26 Jul 2021 23:26:32 GMT  
		Size: 15.9 MB (15889714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bef8200d812a7c6b3f060af102eacb7431c14237f67c8852b4150be72255b4`  
		Last Modified: Mon, 26 Jul 2021 23:26:28 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:0c839a314cd5819355c488d30401827225f533f128c790365cfd0e0939cb2f3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:3cfba0166cb37b1a2e2b252102343ed7bd265bae34092826d2b39e0664275208
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.8 MB (326842374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb19318f478c5ad3deebb1767360a541c56af0014dd542003565bd5e3e24bf1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:05:32 GMT
ENV ROS_DISTRO=galactic
# Tue, 27 Jul 2021 01:06:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:17 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:06:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:06:17 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:06:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:06:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:06:48 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:07:14 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:07:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:07:15 GMT
ENV ROS1_DISTRO=noetic
# Tue, 27 Jul 2021 01:07:16 GMT
ENV ROS2_DISTRO=galactic
# Tue, 27 Jul 2021 01:07:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:07:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:07:49 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698085f1b967a89a6f46a3ab27fbf0926f76b483b0843140c750e906cdbce36e`  
		Last Modified: Tue, 27 Jul 2021 01:18:43 GMT  
		Size: 103.6 MB (103633085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66de36d29cf49a4bbc2b20c3f5795f7d9c972b6c03fbfef58203d93014aab22`  
		Last Modified: Tue, 27 Jul 2021 01:18:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71385bc5f93112c08888184a0254508d98eb9c547e40f70af98924d3c7f7b735`  
		Last Modified: Tue, 27 Jul 2021 01:19:05 GMT  
		Size: 70.8 MB (70797407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6f08ba387a09b78071f694d7eb0fb4774c732d8bbeba44462bd43acc75d78f`  
		Last Modified: Tue, 27 Jul 2021 01:18:55 GMT  
		Size: 241.2 KB (241230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7990cf09456775859f728e71494b2adcec01b46fdbcda5a418970af90f5e5056`  
		Last Modified: Tue, 27 Jul 2021 01:18:55 GMT  
		Size: 2.0 KB (2026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23344c0439abccd2d4aff93d7e57f3697c56daad83902005a615a0e70e52a77c`  
		Last Modified: Tue, 27 Jul 2021 01:18:59 GMT  
		Size: 22.1 MB (22095808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14520e7f4d5e7abaa150d713df486bd446780cf35343d659c964a116fb83314d`  
		Last Modified: Tue, 27 Jul 2021 01:19:20 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89be30453f2f44b3a020e5ec2bfe5b2c6da662ed820f295c10522d1fd3d163da`  
		Last Modified: Tue, 27 Jul 2021 01:19:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83f5e8e2ce60a31e2b6723160edad367d80a1dd8677d7e650af6cd43d84cb6a`  
		Last Modified: Tue, 27 Jul 2021 01:19:35 GMT  
		Size: 78.4 MB (78409624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901678866177d90b4b62b1fe5d39bc27b9c4485b64c290167252b5f8d99f76f9`  
		Last Modified: Tue, 27 Jul 2021 01:19:24 GMT  
		Size: 16.4 MB (16362675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730b1b98982ff37b0d26a053f62a31f785d695504cc4b5e359ba3018868504af`  
		Last Modified: Tue, 27 Jul 2021 01:19:20 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:51365982d4827a84e316c48646392484d939ba70a820d43f462637024811fa89
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.0 MB (314981062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a4c5f72c39097736aa83ab7876f189de9b60787583f0f7f6184a73ab71b0855`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:10:43 GMT
ENV ROS_DISTRO=galactic
# Mon, 26 Jul 2021 23:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:11:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:11:26 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:11:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:11:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:12:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:12:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:12:27 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:12:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:12:28 GMT
ENV ROS1_DISTRO=noetic
# Mon, 26 Jul 2021 23:12:28 GMT
ENV ROS2_DISTRO=galactic
# Mon, 26 Jul 2021 23:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:13:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:13:07 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c0afa8948e130f316bf6e937a5009c86752b46a86110f2b0bc050963acae9a`  
		Last Modified: Mon, 26 Jul 2021 23:25:46 GMT  
		Size: 100.0 MB (100035926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacb211dd1e150cea7c549393186087c461f9055c1497d2fe1171b9b691a56e`  
		Last Modified: Mon, 26 Jul 2021 23:25:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791686871dcac1c755586850b4b34680c90d1a22eb2fb8e973797fa74ca00c`  
		Last Modified: Mon, 26 Jul 2021 23:26:11 GMT  
		Size: 65.1 MB (65138081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d6d89ff94a2c5bbf11ff673f6a8858ec987cf4c3a45ea8fadd495dbe19ebd4`  
		Last Modified: Mon, 26 Jul 2021 23:26:00 GMT  
		Size: 241.2 KB (241224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c0ee3348df19f1250bbf9b003b99c2eb1cdf51ca057364dae79d5e43ab5826`  
		Last Modified: Mon, 26 Jul 2021 23:25:59 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16deeb0c1f27f0ac61db069ece93545b39dd8ef8228c0d6e410445dfc02730f3`  
		Last Modified: Mon, 26 Jul 2021 23:26:04 GMT  
		Size: 21.4 MB (21430859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643322c5f06c1340568abc2f1700666a578e957621e104149c96726a12cef177`  
		Last Modified: Mon, 26 Jul 2021 23:26:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525060df38ebfe98320cd79ad7875e0870654a65c1bd2f2d7dd0a31ffba8516`  
		Last Modified: Mon, 26 Jul 2021 23:26:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a966924f783e389c9a5deb0b9584893f2989886735bc6f0c80d88eb3f3fb1519`  
		Last Modified: Mon, 26 Jul 2021 23:26:49 GMT  
		Size: 78.4 MB (78373807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f67a3aaa308e5228c9ab33d9f84a21f1ef9709987347cf151b3ae2e1a2a8aeb`  
		Last Modified: Mon, 26 Jul 2021 23:26:32 GMT  
		Size: 15.9 MB (15889714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bef8200d812a7c6b3f060af102eacb7431c14237f67c8852b4150be72255b4`  
		Last Modified: Mon, 26 Jul 2021 23:26:28 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:0c0e69ff71d21bff3a263c54143a60ea28ecebe24e3c01fdcfc642f883088914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:c6c4dcdcdba4646d8a6bebd6448625ed80cb18d8f1cae85e21a55a7e3d7ffec2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236641898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df65e6ff4c8f4ed1107f086582df71878afcbeb8d71e39214959ca5517adda77`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV ROS_DISTRO=foxy
# Tue, 27 Jul 2021 01:03:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:03:15 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:03:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:03:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:04:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:04:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:04:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e1e6579146c6323e3e1408e11008ac77c4d5c5ed8e5943332bc7254a56a5`  
		Last Modified: Tue, 27 Jul 2021 01:17:18 GMT  
		Size: 120.0 MB (119974774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88662ced653f598458e0c89695b0fb9e3e8bce9259f6efed11574a8f7ae220f5`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588ff9fb226bda0f04608743623449eccc27c7cc333932238b83bb7ec32398ea`  
		Last Modified: Tue, 27 Jul 2021 01:17:40 GMT  
		Size: 70.8 MB (70843719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a912ea800775dd8e48e78dac7555405832fcd4ad530eeae4cc976ba08ed32dbf`  
		Last Modified: Tue, 27 Jul 2021 01:17:30 GMT  
		Size: 238.5 KB (238478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b8c908ab26db0ef9598ff88bf38a1008a48fa6cc4f426e318321c589e254b4`  
		Last Modified: Tue, 27 Jul 2021 01:17:29 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ba81eeaf2f769cfb5f06e3b9de2651d04e9927d713613e7e5e7f86afbdba4`  
		Last Modified: Tue, 27 Jul 2021 01:17:32 GMT  
		Size: 10.3 MB (10282984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cdcae8270776ec90508842a8c4507bb33cdc7d4214929a81086e14995baaca01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212758009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55fb2a38e2f521cb18fcad29f129d0d60d00ccfff4b77004a8f8f5c0e8dc4d75`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV ROS_DISTRO=foxy
# Mon, 26 Jul 2021 23:08:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:09:00 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:09:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:09:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:09:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:09:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99638d27524b744be6c72b148745cecbd30fce62732e56202509249a739f015`  
		Last Modified: Mon, 26 Jul 2021 23:24:01 GMT  
		Size: 104.2 MB (104166106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0795de1605d5236fe906b0103be795fd0d5906337ac8e1219ab8680fc286d6cc`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9212adaf308df7200d272b55747b777ee4c3f69fd8c33ed43a8cff46b456bcc`  
		Last Modified: Mon, 26 Jul 2021 23:24:25 GMT  
		Size: 65.2 MB (65183893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31858964d3495f929c4fbd43404976dce2b87c812a4a25b1a0c2c83dd29fddd`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 238.5 KB (238481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c120cd143733715303fadf97c47bb4fc1cb0590feeb076c32ccfe7258ac90b`  
		Last Modified: Mon, 26 Jul 2021 23:24:14 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28758a874a9f9821a0fabd399ffae95818ddd755930e5b479087a3bd9b77b272`  
		Last Modified: Mon, 26 Jul 2021 23:24:16 GMT  
		Size: 9.3 MB (9298707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:c2629dc0135caf62e003870fff2727ebaa3dfd5f2ff23189345f0c9dd131111e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:f9ab26ad9caf7c6025ff2669c4a4413746b68ea9ed05b3641829ccb515771e8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437364658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d07711f635f57ed1907b716dba3ea6e751395f9e0e6d27350c4bb37860fac936`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:38:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:35:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 00:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:38:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:38:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:38:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:39:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:39:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186553e47569a52e52d0ff6702d24c183760ccfa8f0865f5cd805b6a834f02a`  
		Last Modified: Tue, 27 Jul 2021 00:00:30 GMT  
		Size: 840.6 KB (840558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd42adfa4f4468cc09d87fcaba98a160059fdee872c36809a69e43ab054efb`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 4.9 MB (4872150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e44ba6559363a0c0463b83b1977a52b1063833026aa6e9dddf178d444e003d`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccab66b30a6739dd0e587dc7eb7a3a05990bf99d4f6089491838f3bac0cfbdd`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f8627bbf4a2b81469316a6529e5a8c8bdd100a4ad64e0d474e973ec43f302`  
		Last Modified: Tue, 27 Jul 2021 01:11:51 GMT  
		Size: 259.4 MB (259445689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3fba9583601e046746fa9e5fb95242575e869b6747a7f9d937b202d9081bc`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75838d174816c0a4cd1517ea28102b2d7fdff541aa8d4229b56f30f29817ca86`  
		Last Modified: Tue, 27 Jul 2021 01:12:14 GMT  
		Size: 70.2 MB (70229942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dde022f386e96e5a68cbc925d59be0ae93c493ce8f4915b24e88d8f8300035`  
		Last Modified: Tue, 27 Jul 2021 01:12:03 GMT  
		Size: 270.4 KB (270435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640152ffa6b1628c31822b6fed053f5978e7d41168ccdc646fca24e4869f1870`  
		Last Modified: Tue, 27 Jul 2021 01:12:18 GMT  
		Size: 75.0 MB (74994434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:6339006da8aa9f01c5f140ff102a1281d7211f285c2079dd99bf3f9b115548f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385879574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9813875c3478474e0d8357aaaf54b39d326da4491c5e3329cc4ea7ef5bf40e5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:55:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:55:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:55:50 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 01:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:59:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 01:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:59:04 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:59:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:00:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:01:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c6b394219d75466dd6176f09c02e5fe7400b0255c6d82480e7d35a0d34a8ee`  
		Last Modified: Tue, 27 Jul 2021 02:18:18 GMT  
		Size: 841.4 KB (841388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879567137a59e93bade6d5accbcd0176b192ccc85080022acea9edea54f9f6c1`  
		Last Modified: Tue, 27 Jul 2021 02:18:17 GMT  
		Size: 4.1 MB (4085785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7141a26daf78fc9f5e9d8cda14c17fb9be91fe6714168a8b33e5a379eeed3f8`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7addca390d668268cbed3008b2cb7707f27958f9f9bbb47a35a03159a18ea5ea`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95f8679d120ee66925b7105bdb869ae6de6c3cd59823868c707a5e768eeeb6b`  
		Last Modified: Tue, 27 Jul 2021 02:20:46 GMT  
		Size: 238.9 MB (238931369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49793c91e8a015ee752db63891347c7ba6811b6aa0837cf3d0715caadd94a942`  
		Last Modified: Tue, 27 Jul 2021 02:18:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488e4f135bc94ed38c27e20719c75a5e0a7159c305d1169046923b45458d5240`  
		Last Modified: Tue, 27 Jul 2021 02:21:29 GMT  
		Size: 54.7 MB (54695577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0296cffbb764eaba4174d14eb10d04dfaf32b3a2ee78b34e89246accb24e714`  
		Last Modified: Tue, 27 Jul 2021 02:21:00 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f4c0cb893c1e65e83d2d1e4b4a23b5987c6936c3effd137151aa55f3bdb5a6`  
		Last Modified: Tue, 27 Jul 2021 02:21:49 GMT  
		Size: 64.7 MB (64745753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:13a0303bb0f2769556ab356ebe7bfe219b853c231dd99630a6683fecf8fa804b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411949654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7c5f138f899b76a5d1a336165a47ed55398b821cbd84a95197f7995603c6e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:49 GMT
ADD file:e87e065765ef99e8db25307f469c7481ab480ac5fe6353ae4caf402766f14045 in / 
# Mon, 26 Jul 2021 21:48:50 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:58:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 22:58:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV ROS_DISTRO=melodic
# Mon, 26 Jul 2021 22:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:59:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 22:59:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 22:59:55 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:00:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:00:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fda1cca7a3cc2b66c161597f27e151a9b1cab79d73c7c0c2706606813a3e58cf`  
		Last Modified: Mon, 26 Jul 2021 21:50:37 GMT  
		Size: 23.7 MB (23731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec48fab32c57250a0a316617993b1f19f17f7e3eb1f5b4b632c9e249bb8be37`  
		Last Modified: Mon, 26 Jul 2021 23:17:30 GMT  
		Size: 841.3 KB (841297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cda3a4d02e2669921c5de51d652aabfb73f4df2b82620e22cee0613358f560c`  
		Last Modified: Mon, 26 Jul 2021 23:17:28 GMT  
		Size: 4.5 MB (4453714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc312c19bce6f60c0e01ada675f9b439a2c4e6e65fdc361f6d9dfa88a88968`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f078b2e134b3bbc567abf387a039e07d7e9b62a44937b65e4486b11a93d0fa`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bb5e0dcebd403b1631077c2bf6f918a579e8261929dd592e97c3599825d707`  
		Last Modified: Mon, 26 Jul 2021 23:18:13 GMT  
		Size: 252.4 MB (252370080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262db146cf4cceac59a83a88e61705c701c9d85f669bade5fb3551c8f1cee8e3`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab725edf1b9f4a135356a05ee3965e94a8d870362463cfa1fdd8b121ae62082`  
		Last Modified: Mon, 26 Jul 2021 23:18:36 GMT  
		Size: 63.1 MB (63058039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7c0963f89fcec01a24152c167c502a6ea1d71b33c04b6c7446ca5c665813a4`  
		Last Modified: Mon, 26 Jul 2021 23:18:25 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44737e66a0fd9299314b82210b7ef1b09c9ec7087b11e374538c570a10ef4e62`  
		Last Modified: Mon, 26 Jul 2021 23:18:39 GMT  
		Size: 67.2 MB (67222081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:e90e53077fd74cec26b0e76c9e4b6595a9958ce859eb4e02a204212e28788541
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:516907559ba16c6625cad9746a8347c807ccb17ae3418a84894b240066f629eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742484508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49c556e58f4297dda608e3de45be487be949cba84e99b0b7c6a2a5a74f9a153`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:38:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:35:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 00:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:38:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:38:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:38:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:39:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:39:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186553e47569a52e52d0ff6702d24c183760ccfa8f0865f5cd805b6a834f02a`  
		Last Modified: Tue, 27 Jul 2021 00:00:30 GMT  
		Size: 840.6 KB (840558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd42adfa4f4468cc09d87fcaba98a160059fdee872c36809a69e43ab054efb`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 4.9 MB (4872150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e44ba6559363a0c0463b83b1977a52b1063833026aa6e9dddf178d444e003d`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccab66b30a6739dd0e587dc7eb7a3a05990bf99d4f6089491838f3bac0cfbdd`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f8627bbf4a2b81469316a6529e5a8c8bdd100a4ad64e0d474e973ec43f302`  
		Last Modified: Tue, 27 Jul 2021 01:11:51 GMT  
		Size: 259.4 MB (259445689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3fba9583601e046746fa9e5fb95242575e869b6747a7f9d937b202d9081bc`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75838d174816c0a4cd1517ea28102b2d7fdff541aa8d4229b56f30f29817ca86`  
		Last Modified: Tue, 27 Jul 2021 01:12:14 GMT  
		Size: 70.2 MB (70229942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dde022f386e96e5a68cbc925d59be0ae93c493ce8f4915b24e88d8f8300035`  
		Last Modified: Tue, 27 Jul 2021 01:12:03 GMT  
		Size: 270.4 KB (270435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640152ffa6b1628c31822b6fed053f5978e7d41168ccdc646fca24e4869f1870`  
		Last Modified: Tue, 27 Jul 2021 01:12:18 GMT  
		Size: 75.0 MB (74994434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6babfc3c4e4d20e1f53e5fb0c1116097706546750ec7abc06b6f4fb8705b9c85`  
		Last Modified: Tue, 27 Jul 2021 01:13:38 GMT  
		Size: 305.1 MB (305119850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:10fd0dbc09abe923ce8d42ae5042cd13bff0e1d72eb835681c884f54d599e98c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.8 MB (645757906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf68020a039da037c8aeb6cd545bb4eb7c8e33dfc3677d94db76c7f2fdb58ae7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:55:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:55:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:55:50 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 01:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:59:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 01:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:59:04 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:59:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:00:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:01:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:05:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c6b394219d75466dd6176f09c02e5fe7400b0255c6d82480e7d35a0d34a8ee`  
		Last Modified: Tue, 27 Jul 2021 02:18:18 GMT  
		Size: 841.4 KB (841388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879567137a59e93bade6d5accbcd0176b192ccc85080022acea9edea54f9f6c1`  
		Last Modified: Tue, 27 Jul 2021 02:18:17 GMT  
		Size: 4.1 MB (4085785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7141a26daf78fc9f5e9d8cda14c17fb9be91fe6714168a8b33e5a379eeed3f8`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7addca390d668268cbed3008b2cb7707f27958f9f9bbb47a35a03159a18ea5ea`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95f8679d120ee66925b7105bdb869ae6de6c3cd59823868c707a5e768eeeb6b`  
		Last Modified: Tue, 27 Jul 2021 02:20:46 GMT  
		Size: 238.9 MB (238931369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49793c91e8a015ee752db63891347c7ba6811b6aa0837cf3d0715caadd94a942`  
		Last Modified: Tue, 27 Jul 2021 02:18:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488e4f135bc94ed38c27e20719c75a5e0a7159c305d1169046923b45458d5240`  
		Last Modified: Tue, 27 Jul 2021 02:21:29 GMT  
		Size: 54.7 MB (54695577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0296cffbb764eaba4174d14eb10d04dfaf32b3a2ee78b34e89246accb24e714`  
		Last Modified: Tue, 27 Jul 2021 02:21:00 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f4c0cb893c1e65e83d2d1e4b4a23b5987c6936c3effd137151aa55f3bdb5a6`  
		Last Modified: Tue, 27 Jul 2021 02:21:49 GMT  
		Size: 64.7 MB (64745753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e0922fb4aff190d3e807b024491145e6553e86cd576b6c12027240d8460c3c`  
		Last Modified: Tue, 27 Jul 2021 02:25:12 GMT  
		Size: 259.9 MB (259878332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:06a8877d06ee3d43cae4db4115f77c90941979182204247a10666a157dd51dfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.4 MB (703408937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa83fb8faa0ed8cf731122e6195d0bbc27cf22642b27c7c9bb5d2d32bdeea1f2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:49 GMT
ADD file:e87e065765ef99e8db25307f469c7481ab480ac5fe6353ae4caf402766f14045 in / 
# Mon, 26 Jul 2021 21:48:50 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:58:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 22:58:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV ROS_DISTRO=melodic
# Mon, 26 Jul 2021 22:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:59:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 22:59:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 22:59:55 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:00:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:00:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fda1cca7a3cc2b66c161597f27e151a9b1cab79d73c7c0c2706606813a3e58cf`  
		Last Modified: Mon, 26 Jul 2021 21:50:37 GMT  
		Size: 23.7 MB (23731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec48fab32c57250a0a316617993b1f19f17f7e3eb1f5b4b632c9e249bb8be37`  
		Last Modified: Mon, 26 Jul 2021 23:17:30 GMT  
		Size: 841.3 KB (841297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cda3a4d02e2669921c5de51d652aabfb73f4df2b82620e22cee0613358f560c`  
		Last Modified: Mon, 26 Jul 2021 23:17:28 GMT  
		Size: 4.5 MB (4453714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc312c19bce6f60c0e01ada675f9b439a2c4e6e65fdc361f6d9dfa88a88968`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f078b2e134b3bbc567abf387a039e07d7e9b62a44937b65e4486b11a93d0fa`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bb5e0dcebd403b1631077c2bf6f918a579e8261929dd592e97c3599825d707`  
		Last Modified: Mon, 26 Jul 2021 23:18:13 GMT  
		Size: 252.4 MB (252370080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262db146cf4cceac59a83a88e61705c701c9d85f669bade5fb3551c8f1cee8e3`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab725edf1b9f4a135356a05ee3965e94a8d870362463cfa1fdd8b121ae62082`  
		Last Modified: Mon, 26 Jul 2021 23:18:36 GMT  
		Size: 63.1 MB (63058039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7c0963f89fcec01a24152c167c502a6ea1d71b33c04b6c7446ca5c665813a4`  
		Last Modified: Mon, 26 Jul 2021 23:18:25 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44737e66a0fd9299314b82210b7ef1b09c9ec7087b11e374538c570a10ef4e62`  
		Last Modified: Mon, 26 Jul 2021 23:18:39 GMT  
		Size: 67.2 MB (67222081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11602763d81471ccb881ff943ad79df93f3f835646e285b1b1c71a97c4cceb8`  
		Last Modified: Mon, 26 Jul 2021 23:20:05 GMT  
		Size: 291.5 MB (291459283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:e90e53077fd74cec26b0e76c9e4b6595a9958ce859eb4e02a204212e28788541
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:516907559ba16c6625cad9746a8347c807ccb17ae3418a84894b240066f629eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742484508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49c556e58f4297dda608e3de45be487be949cba84e99b0b7c6a2a5a74f9a153`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:38:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:35:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 00:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:38:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:38:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:38:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:39:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:39:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186553e47569a52e52d0ff6702d24c183760ccfa8f0865f5cd805b6a834f02a`  
		Last Modified: Tue, 27 Jul 2021 00:00:30 GMT  
		Size: 840.6 KB (840558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd42adfa4f4468cc09d87fcaba98a160059fdee872c36809a69e43ab054efb`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 4.9 MB (4872150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e44ba6559363a0c0463b83b1977a52b1063833026aa6e9dddf178d444e003d`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccab66b30a6739dd0e587dc7eb7a3a05990bf99d4f6089491838f3bac0cfbdd`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f8627bbf4a2b81469316a6529e5a8c8bdd100a4ad64e0d474e973ec43f302`  
		Last Modified: Tue, 27 Jul 2021 01:11:51 GMT  
		Size: 259.4 MB (259445689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3fba9583601e046746fa9e5fb95242575e869b6747a7f9d937b202d9081bc`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75838d174816c0a4cd1517ea28102b2d7fdff541aa8d4229b56f30f29817ca86`  
		Last Modified: Tue, 27 Jul 2021 01:12:14 GMT  
		Size: 70.2 MB (70229942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dde022f386e96e5a68cbc925d59be0ae93c493ce8f4915b24e88d8f8300035`  
		Last Modified: Tue, 27 Jul 2021 01:12:03 GMT  
		Size: 270.4 KB (270435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640152ffa6b1628c31822b6fed053f5978e7d41168ccdc646fca24e4869f1870`  
		Last Modified: Tue, 27 Jul 2021 01:12:18 GMT  
		Size: 75.0 MB (74994434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6babfc3c4e4d20e1f53e5fb0c1116097706546750ec7abc06b6f4fb8705b9c85`  
		Last Modified: Tue, 27 Jul 2021 01:13:38 GMT  
		Size: 305.1 MB (305119850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:10fd0dbc09abe923ce8d42ae5042cd13bff0e1d72eb835681c884f54d599e98c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.8 MB (645757906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf68020a039da037c8aeb6cd545bb4eb7c8e33dfc3677d94db76c7f2fdb58ae7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:55:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:55:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:55:50 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 01:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:59:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 01:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:59:04 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:59:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:00:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:01:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:05:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c6b394219d75466dd6176f09c02e5fe7400b0255c6d82480e7d35a0d34a8ee`  
		Last Modified: Tue, 27 Jul 2021 02:18:18 GMT  
		Size: 841.4 KB (841388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879567137a59e93bade6d5accbcd0176b192ccc85080022acea9edea54f9f6c1`  
		Last Modified: Tue, 27 Jul 2021 02:18:17 GMT  
		Size: 4.1 MB (4085785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7141a26daf78fc9f5e9d8cda14c17fb9be91fe6714168a8b33e5a379eeed3f8`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7addca390d668268cbed3008b2cb7707f27958f9f9bbb47a35a03159a18ea5ea`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95f8679d120ee66925b7105bdb869ae6de6c3cd59823868c707a5e768eeeb6b`  
		Last Modified: Tue, 27 Jul 2021 02:20:46 GMT  
		Size: 238.9 MB (238931369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49793c91e8a015ee752db63891347c7ba6811b6aa0837cf3d0715caadd94a942`  
		Last Modified: Tue, 27 Jul 2021 02:18:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488e4f135bc94ed38c27e20719c75a5e0a7159c305d1169046923b45458d5240`  
		Last Modified: Tue, 27 Jul 2021 02:21:29 GMT  
		Size: 54.7 MB (54695577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0296cffbb764eaba4174d14eb10d04dfaf32b3a2ee78b34e89246accb24e714`  
		Last Modified: Tue, 27 Jul 2021 02:21:00 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f4c0cb893c1e65e83d2d1e4b4a23b5987c6936c3effd137151aa55f3bdb5a6`  
		Last Modified: Tue, 27 Jul 2021 02:21:49 GMT  
		Size: 64.7 MB (64745753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e0922fb4aff190d3e807b024491145e6553e86cd576b6c12027240d8460c3c`  
		Last Modified: Tue, 27 Jul 2021 02:25:12 GMT  
		Size: 259.9 MB (259878332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:06a8877d06ee3d43cae4db4115f77c90941979182204247a10666a157dd51dfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.4 MB (703408937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa83fb8faa0ed8cf731122e6195d0bbc27cf22642b27c7c9bb5d2d32bdeea1f2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:49 GMT
ADD file:e87e065765ef99e8db25307f469c7481ab480ac5fe6353ae4caf402766f14045 in / 
# Mon, 26 Jul 2021 21:48:50 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:58:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 22:58:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV ROS_DISTRO=melodic
# Mon, 26 Jul 2021 22:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:59:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 22:59:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 22:59:55 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:00:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:00:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fda1cca7a3cc2b66c161597f27e151a9b1cab79d73c7c0c2706606813a3e58cf`  
		Last Modified: Mon, 26 Jul 2021 21:50:37 GMT  
		Size: 23.7 MB (23731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec48fab32c57250a0a316617993b1f19f17f7e3eb1f5b4b632c9e249bb8be37`  
		Last Modified: Mon, 26 Jul 2021 23:17:30 GMT  
		Size: 841.3 KB (841297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cda3a4d02e2669921c5de51d652aabfb73f4df2b82620e22cee0613358f560c`  
		Last Modified: Mon, 26 Jul 2021 23:17:28 GMT  
		Size: 4.5 MB (4453714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc312c19bce6f60c0e01ada675f9b439a2c4e6e65fdc361f6d9dfa88a88968`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f078b2e134b3bbc567abf387a039e07d7e9b62a44937b65e4486b11a93d0fa`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bb5e0dcebd403b1631077c2bf6f918a579e8261929dd592e97c3599825d707`  
		Last Modified: Mon, 26 Jul 2021 23:18:13 GMT  
		Size: 252.4 MB (252370080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262db146cf4cceac59a83a88e61705c701c9d85f669bade5fb3551c8f1cee8e3`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab725edf1b9f4a135356a05ee3965e94a8d870362463cfa1fdd8b121ae62082`  
		Last Modified: Mon, 26 Jul 2021 23:18:36 GMT  
		Size: 63.1 MB (63058039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7c0963f89fcec01a24152c167c502a6ea1d71b33c04b6c7446ca5c665813a4`  
		Last Modified: Mon, 26 Jul 2021 23:18:25 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44737e66a0fd9299314b82210b7ef1b09c9ec7087b11e374538c570a10ef4e62`  
		Last Modified: Mon, 26 Jul 2021 23:18:39 GMT  
		Size: 67.2 MB (67222081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11602763d81471ccb881ff943ad79df93f3f835646e285b1b1c71a97c4cceb8`  
		Last Modified: Mon, 26 Jul 2021 23:20:05 GMT  
		Size: 291.5 MB (291459283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:c06ff4994f879fee6bb87b2d35638ac468746c37460219372ec6b7ed747b0824
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:c006321b47e47cf84b4c8bdf2c7eaddf2125080769e0038e1ce867507433273a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448441915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac37ed9cee6d46118984bf85d40fb6e2569cfe8f6e2e0c8d7dda02d35f91dd4b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:38:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:35:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 00:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:38:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:38:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:38:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:39:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:39:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:41:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186553e47569a52e52d0ff6702d24c183760ccfa8f0865f5cd805b6a834f02a`  
		Last Modified: Tue, 27 Jul 2021 00:00:30 GMT  
		Size: 840.6 KB (840558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd42adfa4f4468cc09d87fcaba98a160059fdee872c36809a69e43ab054efb`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 4.9 MB (4872150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e44ba6559363a0c0463b83b1977a52b1063833026aa6e9dddf178d444e003d`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccab66b30a6739dd0e587dc7eb7a3a05990bf99d4f6089491838f3bac0cfbdd`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f8627bbf4a2b81469316a6529e5a8c8bdd100a4ad64e0d474e973ec43f302`  
		Last Modified: Tue, 27 Jul 2021 01:11:51 GMT  
		Size: 259.4 MB (259445689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3fba9583601e046746fa9e5fb95242575e869b6747a7f9d937b202d9081bc`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75838d174816c0a4cd1517ea28102b2d7fdff541aa8d4229b56f30f29817ca86`  
		Last Modified: Tue, 27 Jul 2021 01:12:14 GMT  
		Size: 70.2 MB (70229942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dde022f386e96e5a68cbc925d59be0ae93c493ce8f4915b24e88d8f8300035`  
		Last Modified: Tue, 27 Jul 2021 01:12:03 GMT  
		Size: 270.4 KB (270435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640152ffa6b1628c31822b6fed053f5978e7d41168ccdc646fca24e4869f1870`  
		Last Modified: Tue, 27 Jul 2021 01:12:18 GMT  
		Size: 75.0 MB (74994434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eed9add0cfd575614a9c9c18845491df98558313d952c8c14fbe6419939423`  
		Last Modified: Tue, 27 Jul 2021 01:12:35 GMT  
		Size: 11.1 MB (11077257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:039b40aa8f2b991d341921a46f3d029c5ec3f746cdbd54dcf890c49ef4cef301
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396000038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23834d4bdbcb9fad85a5824bd8664267bdbd7ae601c602d0e8742d5c38fab3d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:55:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:55:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:55:50 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 01:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:59:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 01:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:59:04 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:59:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:00:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:01:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:02:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c6b394219d75466dd6176f09c02e5fe7400b0255c6d82480e7d35a0d34a8ee`  
		Last Modified: Tue, 27 Jul 2021 02:18:18 GMT  
		Size: 841.4 KB (841388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879567137a59e93bade6d5accbcd0176b192ccc85080022acea9edea54f9f6c1`  
		Last Modified: Tue, 27 Jul 2021 02:18:17 GMT  
		Size: 4.1 MB (4085785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7141a26daf78fc9f5e9d8cda14c17fb9be91fe6714168a8b33e5a379eeed3f8`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7addca390d668268cbed3008b2cb7707f27958f9f9bbb47a35a03159a18ea5ea`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95f8679d120ee66925b7105bdb869ae6de6c3cd59823868c707a5e768eeeb6b`  
		Last Modified: Tue, 27 Jul 2021 02:20:46 GMT  
		Size: 238.9 MB (238931369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49793c91e8a015ee752db63891347c7ba6811b6aa0837cf3d0715caadd94a942`  
		Last Modified: Tue, 27 Jul 2021 02:18:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488e4f135bc94ed38c27e20719c75a5e0a7159c305d1169046923b45458d5240`  
		Last Modified: Tue, 27 Jul 2021 02:21:29 GMT  
		Size: 54.7 MB (54695577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0296cffbb764eaba4174d14eb10d04dfaf32b3a2ee78b34e89246accb24e714`  
		Last Modified: Tue, 27 Jul 2021 02:21:00 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f4c0cb893c1e65e83d2d1e4b4a23b5987c6936c3effd137151aa55f3bdb5a6`  
		Last Modified: Tue, 27 Jul 2021 02:21:49 GMT  
		Size: 64.7 MB (64745753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dba6abf33f0661b634dc6452efbb426f401b8a7552592a3d87c980195ced29`  
		Last Modified: Tue, 27 Jul 2021 02:22:15 GMT  
		Size: 10.1 MB (10120464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:05c5827fbbb132334e84975ba1fc84d2eef0138682bf7a362717dfdd051b341c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422681441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc9bd321da8fe5fb4616604d544852bf1f687a6b6e022b2dec02a8e875bd2443`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:49 GMT
ADD file:e87e065765ef99e8db25307f469c7481ab480ac5fe6353ae4caf402766f14045 in / 
# Mon, 26 Jul 2021 21:48:50 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:58:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 22:58:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV ROS_DISTRO=melodic
# Mon, 26 Jul 2021 22:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:59:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 22:59:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 22:59:55 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:00:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:00:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:01:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fda1cca7a3cc2b66c161597f27e151a9b1cab79d73c7c0c2706606813a3e58cf`  
		Last Modified: Mon, 26 Jul 2021 21:50:37 GMT  
		Size: 23.7 MB (23731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec48fab32c57250a0a316617993b1f19f17f7e3eb1f5b4b632c9e249bb8be37`  
		Last Modified: Mon, 26 Jul 2021 23:17:30 GMT  
		Size: 841.3 KB (841297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cda3a4d02e2669921c5de51d652aabfb73f4df2b82620e22cee0613358f560c`  
		Last Modified: Mon, 26 Jul 2021 23:17:28 GMT  
		Size: 4.5 MB (4453714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc312c19bce6f60c0e01ada675f9b439a2c4e6e65fdc361f6d9dfa88a88968`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f078b2e134b3bbc567abf387a039e07d7e9b62a44937b65e4486b11a93d0fa`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bb5e0dcebd403b1631077c2bf6f918a579e8261929dd592e97c3599825d707`  
		Last Modified: Mon, 26 Jul 2021 23:18:13 GMT  
		Size: 252.4 MB (252370080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262db146cf4cceac59a83a88e61705c701c9d85f669bade5fb3551c8f1cee8e3`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab725edf1b9f4a135356a05ee3965e94a8d870362463cfa1fdd8b121ae62082`  
		Last Modified: Mon, 26 Jul 2021 23:18:36 GMT  
		Size: 63.1 MB (63058039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7c0963f89fcec01a24152c167c502a6ea1d71b33c04b6c7446ca5c665813a4`  
		Last Modified: Mon, 26 Jul 2021 23:18:25 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44737e66a0fd9299314b82210b7ef1b09c9ec7087b11e374538c570a10ef4e62`  
		Last Modified: Mon, 26 Jul 2021 23:18:39 GMT  
		Size: 67.2 MB (67222081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defb1f07598253f1598dffc61b99ea5ee236e4ac0e00c98184eda28dc455e63e`  
		Last Modified: Mon, 26 Jul 2021 23:18:58 GMT  
		Size: 10.7 MB (10731787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:c06ff4994f879fee6bb87b2d35638ac468746c37460219372ec6b7ed747b0824
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:c006321b47e47cf84b4c8bdf2c7eaddf2125080769e0038e1ce867507433273a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448441915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac37ed9cee6d46118984bf85d40fb6e2569cfe8f6e2e0c8d7dda02d35f91dd4b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:38:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:35:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 00:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:38:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:38:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:38:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:39:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:39:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:41:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186553e47569a52e52d0ff6702d24c183760ccfa8f0865f5cd805b6a834f02a`  
		Last Modified: Tue, 27 Jul 2021 00:00:30 GMT  
		Size: 840.6 KB (840558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd42adfa4f4468cc09d87fcaba98a160059fdee872c36809a69e43ab054efb`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 4.9 MB (4872150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e44ba6559363a0c0463b83b1977a52b1063833026aa6e9dddf178d444e003d`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccab66b30a6739dd0e587dc7eb7a3a05990bf99d4f6089491838f3bac0cfbdd`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f8627bbf4a2b81469316a6529e5a8c8bdd100a4ad64e0d474e973ec43f302`  
		Last Modified: Tue, 27 Jul 2021 01:11:51 GMT  
		Size: 259.4 MB (259445689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3fba9583601e046746fa9e5fb95242575e869b6747a7f9d937b202d9081bc`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75838d174816c0a4cd1517ea28102b2d7fdff541aa8d4229b56f30f29817ca86`  
		Last Modified: Tue, 27 Jul 2021 01:12:14 GMT  
		Size: 70.2 MB (70229942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dde022f386e96e5a68cbc925d59be0ae93c493ce8f4915b24e88d8f8300035`  
		Last Modified: Tue, 27 Jul 2021 01:12:03 GMT  
		Size: 270.4 KB (270435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640152ffa6b1628c31822b6fed053f5978e7d41168ccdc646fca24e4869f1870`  
		Last Modified: Tue, 27 Jul 2021 01:12:18 GMT  
		Size: 75.0 MB (74994434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eed9add0cfd575614a9c9c18845491df98558313d952c8c14fbe6419939423`  
		Last Modified: Tue, 27 Jul 2021 01:12:35 GMT  
		Size: 11.1 MB (11077257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:039b40aa8f2b991d341921a46f3d029c5ec3f746cdbd54dcf890c49ef4cef301
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396000038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23834d4bdbcb9fad85a5824bd8664267bdbd7ae601c602d0e8742d5c38fab3d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:55:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:55:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:55:50 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 01:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:59:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 01:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:59:04 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:59:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:00:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:01:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:02:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c6b394219d75466dd6176f09c02e5fe7400b0255c6d82480e7d35a0d34a8ee`  
		Last Modified: Tue, 27 Jul 2021 02:18:18 GMT  
		Size: 841.4 KB (841388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879567137a59e93bade6d5accbcd0176b192ccc85080022acea9edea54f9f6c1`  
		Last Modified: Tue, 27 Jul 2021 02:18:17 GMT  
		Size: 4.1 MB (4085785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7141a26daf78fc9f5e9d8cda14c17fb9be91fe6714168a8b33e5a379eeed3f8`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7addca390d668268cbed3008b2cb7707f27958f9f9bbb47a35a03159a18ea5ea`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95f8679d120ee66925b7105bdb869ae6de6c3cd59823868c707a5e768eeeb6b`  
		Last Modified: Tue, 27 Jul 2021 02:20:46 GMT  
		Size: 238.9 MB (238931369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49793c91e8a015ee752db63891347c7ba6811b6aa0837cf3d0715caadd94a942`  
		Last Modified: Tue, 27 Jul 2021 02:18:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488e4f135bc94ed38c27e20719c75a5e0a7159c305d1169046923b45458d5240`  
		Last Modified: Tue, 27 Jul 2021 02:21:29 GMT  
		Size: 54.7 MB (54695577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0296cffbb764eaba4174d14eb10d04dfaf32b3a2ee78b34e89246accb24e714`  
		Last Modified: Tue, 27 Jul 2021 02:21:00 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f4c0cb893c1e65e83d2d1e4b4a23b5987c6936c3effd137151aa55f3bdb5a6`  
		Last Modified: Tue, 27 Jul 2021 02:21:49 GMT  
		Size: 64.7 MB (64745753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dba6abf33f0661b634dc6452efbb426f401b8a7552592a3d87c980195ced29`  
		Last Modified: Tue, 27 Jul 2021 02:22:15 GMT  
		Size: 10.1 MB (10120464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:05c5827fbbb132334e84975ba1fc84d2eef0138682bf7a362717dfdd051b341c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422681441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc9bd321da8fe5fb4616604d544852bf1f687a6b6e022b2dec02a8e875bd2443`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:49 GMT
ADD file:e87e065765ef99e8db25307f469c7481ab480ac5fe6353ae4caf402766f14045 in / 
# Mon, 26 Jul 2021 21:48:50 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:58:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 22:58:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV ROS_DISTRO=melodic
# Mon, 26 Jul 2021 22:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:59:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 22:59:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 22:59:55 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:00:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:00:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:01:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fda1cca7a3cc2b66c161597f27e151a9b1cab79d73c7c0c2706606813a3e58cf`  
		Last Modified: Mon, 26 Jul 2021 21:50:37 GMT  
		Size: 23.7 MB (23731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec48fab32c57250a0a316617993b1f19f17f7e3eb1f5b4b632c9e249bb8be37`  
		Last Modified: Mon, 26 Jul 2021 23:17:30 GMT  
		Size: 841.3 KB (841297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cda3a4d02e2669921c5de51d652aabfb73f4df2b82620e22cee0613358f560c`  
		Last Modified: Mon, 26 Jul 2021 23:17:28 GMT  
		Size: 4.5 MB (4453714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc312c19bce6f60c0e01ada675f9b439a2c4e6e65fdc361f6d9dfa88a88968`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f078b2e134b3bbc567abf387a039e07d7e9b62a44937b65e4486b11a93d0fa`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bb5e0dcebd403b1631077c2bf6f918a579e8261929dd592e97c3599825d707`  
		Last Modified: Mon, 26 Jul 2021 23:18:13 GMT  
		Size: 252.4 MB (252370080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262db146cf4cceac59a83a88e61705c701c9d85f669bade5fb3551c8f1cee8e3`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab725edf1b9f4a135356a05ee3965e94a8d870362463cfa1fdd8b121ae62082`  
		Last Modified: Mon, 26 Jul 2021 23:18:36 GMT  
		Size: 63.1 MB (63058039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7c0963f89fcec01a24152c167c502a6ea1d71b33c04b6c7446ca5c665813a4`  
		Last Modified: Mon, 26 Jul 2021 23:18:25 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44737e66a0fd9299314b82210b7ef1b09c9ec7087b11e374538c570a10ef4e62`  
		Last Modified: Mon, 26 Jul 2021 23:18:39 GMT  
		Size: 67.2 MB (67222081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defb1f07598253f1598dffc61b99ea5ee236e4ac0e00c98184eda28dc455e63e`  
		Last Modified: Mon, 26 Jul 2021 23:18:58 GMT  
		Size: 10.7 MB (10731787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:c2629dc0135caf62e003870fff2727ebaa3dfd5f2ff23189345f0c9dd131111e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:f9ab26ad9caf7c6025ff2669c4a4413746b68ea9ed05b3641829ccb515771e8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437364658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d07711f635f57ed1907b716dba3ea6e751395f9e0e6d27350c4bb37860fac936`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:38:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:35:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 00:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:38:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:38:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:38:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:39:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:39:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186553e47569a52e52d0ff6702d24c183760ccfa8f0865f5cd805b6a834f02a`  
		Last Modified: Tue, 27 Jul 2021 00:00:30 GMT  
		Size: 840.6 KB (840558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd42adfa4f4468cc09d87fcaba98a160059fdee872c36809a69e43ab054efb`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 4.9 MB (4872150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e44ba6559363a0c0463b83b1977a52b1063833026aa6e9dddf178d444e003d`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccab66b30a6739dd0e587dc7eb7a3a05990bf99d4f6089491838f3bac0cfbdd`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f8627bbf4a2b81469316a6529e5a8c8bdd100a4ad64e0d474e973ec43f302`  
		Last Modified: Tue, 27 Jul 2021 01:11:51 GMT  
		Size: 259.4 MB (259445689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3fba9583601e046746fa9e5fb95242575e869b6747a7f9d937b202d9081bc`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75838d174816c0a4cd1517ea28102b2d7fdff541aa8d4229b56f30f29817ca86`  
		Last Modified: Tue, 27 Jul 2021 01:12:14 GMT  
		Size: 70.2 MB (70229942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dde022f386e96e5a68cbc925d59be0ae93c493ce8f4915b24e88d8f8300035`  
		Last Modified: Tue, 27 Jul 2021 01:12:03 GMT  
		Size: 270.4 KB (270435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640152ffa6b1628c31822b6fed053f5978e7d41168ccdc646fca24e4869f1870`  
		Last Modified: Tue, 27 Jul 2021 01:12:18 GMT  
		Size: 75.0 MB (74994434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:6339006da8aa9f01c5f140ff102a1281d7211f285c2079dd99bf3f9b115548f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385879574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9813875c3478474e0d8357aaaf54b39d326da4491c5e3329cc4ea7ef5bf40e5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:55:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:55:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:55:50 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 01:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:59:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 01:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:59:04 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:59:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:00:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:01:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c6b394219d75466dd6176f09c02e5fe7400b0255c6d82480e7d35a0d34a8ee`  
		Last Modified: Tue, 27 Jul 2021 02:18:18 GMT  
		Size: 841.4 KB (841388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879567137a59e93bade6d5accbcd0176b192ccc85080022acea9edea54f9f6c1`  
		Last Modified: Tue, 27 Jul 2021 02:18:17 GMT  
		Size: 4.1 MB (4085785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7141a26daf78fc9f5e9d8cda14c17fb9be91fe6714168a8b33e5a379eeed3f8`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7addca390d668268cbed3008b2cb7707f27958f9f9bbb47a35a03159a18ea5ea`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95f8679d120ee66925b7105bdb869ae6de6c3cd59823868c707a5e768eeeb6b`  
		Last Modified: Tue, 27 Jul 2021 02:20:46 GMT  
		Size: 238.9 MB (238931369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49793c91e8a015ee752db63891347c7ba6811b6aa0837cf3d0715caadd94a942`  
		Last Modified: Tue, 27 Jul 2021 02:18:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488e4f135bc94ed38c27e20719c75a5e0a7159c305d1169046923b45458d5240`  
		Last Modified: Tue, 27 Jul 2021 02:21:29 GMT  
		Size: 54.7 MB (54695577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0296cffbb764eaba4174d14eb10d04dfaf32b3a2ee78b34e89246accb24e714`  
		Last Modified: Tue, 27 Jul 2021 02:21:00 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f4c0cb893c1e65e83d2d1e4b4a23b5987c6936c3effd137151aa55f3bdb5a6`  
		Last Modified: Tue, 27 Jul 2021 02:21:49 GMT  
		Size: 64.7 MB (64745753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:13a0303bb0f2769556ab356ebe7bfe219b853c231dd99630a6683fecf8fa804b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411949654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7c5f138f899b76a5d1a336165a47ed55398b821cbd84a95197f7995603c6e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:49 GMT
ADD file:e87e065765ef99e8db25307f469c7481ab480ac5fe6353ae4caf402766f14045 in / 
# Mon, 26 Jul 2021 21:48:50 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:58:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 22:58:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV ROS_DISTRO=melodic
# Mon, 26 Jul 2021 22:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:59:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 22:59:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 22:59:55 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:00:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:00:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fda1cca7a3cc2b66c161597f27e151a9b1cab79d73c7c0c2706606813a3e58cf`  
		Last Modified: Mon, 26 Jul 2021 21:50:37 GMT  
		Size: 23.7 MB (23731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec48fab32c57250a0a316617993b1f19f17f7e3eb1f5b4b632c9e249bb8be37`  
		Last Modified: Mon, 26 Jul 2021 23:17:30 GMT  
		Size: 841.3 KB (841297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cda3a4d02e2669921c5de51d652aabfb73f4df2b82620e22cee0613358f560c`  
		Last Modified: Mon, 26 Jul 2021 23:17:28 GMT  
		Size: 4.5 MB (4453714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc312c19bce6f60c0e01ada675f9b439a2c4e6e65fdc361f6d9dfa88a88968`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f078b2e134b3bbc567abf387a039e07d7e9b62a44937b65e4486b11a93d0fa`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bb5e0dcebd403b1631077c2bf6f918a579e8261929dd592e97c3599825d707`  
		Last Modified: Mon, 26 Jul 2021 23:18:13 GMT  
		Size: 252.4 MB (252370080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262db146cf4cceac59a83a88e61705c701c9d85f669bade5fb3551c8f1cee8e3`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab725edf1b9f4a135356a05ee3965e94a8d870362463cfa1fdd8b121ae62082`  
		Last Modified: Mon, 26 Jul 2021 23:18:36 GMT  
		Size: 63.1 MB (63058039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7c0963f89fcec01a24152c167c502a6ea1d71b33c04b6c7446ca5c665813a4`  
		Last Modified: Mon, 26 Jul 2021 23:18:25 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44737e66a0fd9299314b82210b7ef1b09c9ec7087b11e374538c570a10ef4e62`  
		Last Modified: Mon, 26 Jul 2021 23:18:39 GMT  
		Size: 67.2 MB (67222081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:c2629dc0135caf62e003870fff2727ebaa3dfd5f2ff23189345f0c9dd131111e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:f9ab26ad9caf7c6025ff2669c4a4413746b68ea9ed05b3641829ccb515771e8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437364658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d07711f635f57ed1907b716dba3ea6e751395f9e0e6d27350c4bb37860fac936`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:38:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:35:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 00:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:38:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:38:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:38:15 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:39:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:39:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186553e47569a52e52d0ff6702d24c183760ccfa8f0865f5cd805b6a834f02a`  
		Last Modified: Tue, 27 Jul 2021 00:00:30 GMT  
		Size: 840.6 KB (840558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd42adfa4f4468cc09d87fcaba98a160059fdee872c36809a69e43ab054efb`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 4.9 MB (4872150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e44ba6559363a0c0463b83b1977a52b1063833026aa6e9dddf178d444e003d`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccab66b30a6739dd0e587dc7eb7a3a05990bf99d4f6089491838f3bac0cfbdd`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f8627bbf4a2b81469316a6529e5a8c8bdd100a4ad64e0d474e973ec43f302`  
		Last Modified: Tue, 27 Jul 2021 01:11:51 GMT  
		Size: 259.4 MB (259445689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3fba9583601e046746fa9e5fb95242575e869b6747a7f9d937b202d9081bc`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75838d174816c0a4cd1517ea28102b2d7fdff541aa8d4229b56f30f29817ca86`  
		Last Modified: Tue, 27 Jul 2021 01:12:14 GMT  
		Size: 70.2 MB (70229942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dde022f386e96e5a68cbc925d59be0ae93c493ce8f4915b24e88d8f8300035`  
		Last Modified: Tue, 27 Jul 2021 01:12:03 GMT  
		Size: 270.4 KB (270435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640152ffa6b1628c31822b6fed053f5978e7d41168ccdc646fca24e4869f1870`  
		Last Modified: Tue, 27 Jul 2021 01:12:18 GMT  
		Size: 75.0 MB (74994434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:6339006da8aa9f01c5f140ff102a1281d7211f285c2079dd99bf3f9b115548f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385879574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9813875c3478474e0d8357aaaf54b39d326da4491c5e3329cc4ea7ef5bf40e5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:55:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:55:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:55:50 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 01:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:59:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 01:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:59:04 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:59:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:00:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:01:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c6b394219d75466dd6176f09c02e5fe7400b0255c6d82480e7d35a0d34a8ee`  
		Last Modified: Tue, 27 Jul 2021 02:18:18 GMT  
		Size: 841.4 KB (841388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879567137a59e93bade6d5accbcd0176b192ccc85080022acea9edea54f9f6c1`  
		Last Modified: Tue, 27 Jul 2021 02:18:17 GMT  
		Size: 4.1 MB (4085785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7141a26daf78fc9f5e9d8cda14c17fb9be91fe6714168a8b33e5a379eeed3f8`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7addca390d668268cbed3008b2cb7707f27958f9f9bbb47a35a03159a18ea5ea`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95f8679d120ee66925b7105bdb869ae6de6c3cd59823868c707a5e768eeeb6b`  
		Last Modified: Tue, 27 Jul 2021 02:20:46 GMT  
		Size: 238.9 MB (238931369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49793c91e8a015ee752db63891347c7ba6811b6aa0837cf3d0715caadd94a942`  
		Last Modified: Tue, 27 Jul 2021 02:18:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488e4f135bc94ed38c27e20719c75a5e0a7159c305d1169046923b45458d5240`  
		Last Modified: Tue, 27 Jul 2021 02:21:29 GMT  
		Size: 54.7 MB (54695577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0296cffbb764eaba4174d14eb10d04dfaf32b3a2ee78b34e89246accb24e714`  
		Last Modified: Tue, 27 Jul 2021 02:21:00 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f4c0cb893c1e65e83d2d1e4b4a23b5987c6936c3effd137151aa55f3bdb5a6`  
		Last Modified: Tue, 27 Jul 2021 02:21:49 GMT  
		Size: 64.7 MB (64745753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:13a0303bb0f2769556ab356ebe7bfe219b853c231dd99630a6683fecf8fa804b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411949654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7c5f138f899b76a5d1a336165a47ed55398b821cbd84a95197f7995603c6e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:49 GMT
ADD file:e87e065765ef99e8db25307f469c7481ab480ac5fe6353ae4caf402766f14045 in / 
# Mon, 26 Jul 2021 21:48:50 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:58:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 22:58:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV ROS_DISTRO=melodic
# Mon, 26 Jul 2021 22:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:59:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 22:59:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 22:59:55 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:00:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:00:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fda1cca7a3cc2b66c161597f27e151a9b1cab79d73c7c0c2706606813a3e58cf`  
		Last Modified: Mon, 26 Jul 2021 21:50:37 GMT  
		Size: 23.7 MB (23731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec48fab32c57250a0a316617993b1f19f17f7e3eb1f5b4b632c9e249bb8be37`  
		Last Modified: Mon, 26 Jul 2021 23:17:30 GMT  
		Size: 841.3 KB (841297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cda3a4d02e2669921c5de51d652aabfb73f4df2b82620e22cee0613358f560c`  
		Last Modified: Mon, 26 Jul 2021 23:17:28 GMT  
		Size: 4.5 MB (4453714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc312c19bce6f60c0e01ada675f9b439a2c4e6e65fdc361f6d9dfa88a88968`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f078b2e134b3bbc567abf387a039e07d7e9b62a44937b65e4486b11a93d0fa`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bb5e0dcebd403b1631077c2bf6f918a579e8261929dd592e97c3599825d707`  
		Last Modified: Mon, 26 Jul 2021 23:18:13 GMT  
		Size: 252.4 MB (252370080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262db146cf4cceac59a83a88e61705c701c9d85f669bade5fb3551c8f1cee8e3`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab725edf1b9f4a135356a05ee3965e94a8d870362463cfa1fdd8b121ae62082`  
		Last Modified: Mon, 26 Jul 2021 23:18:36 GMT  
		Size: 63.1 MB (63058039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7c0963f89fcec01a24152c167c502a6ea1d71b33c04b6c7446ca5c665813a4`  
		Last Modified: Mon, 26 Jul 2021 23:18:25 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44737e66a0fd9299314b82210b7ef1b09c9ec7087b11e374538c570a10ef4e62`  
		Last Modified: Mon, 26 Jul 2021 23:18:39 GMT  
		Size: 67.2 MB (67222081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:9b03709d6c54ab97d50a1b99d3d00878071189aa2e7bf7faf3daac1c055bedc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:75a3bb07c9b6265827bf559fcc633d660776bb8f408b6dc4c3901f8d48a7fc3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291869847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:947363507d39ea6611167fc1c338d12ef5b49ba0a2a5cc6274d9860949f1d3a8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:38:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:35:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 00:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:38:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:38:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:38:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186553e47569a52e52d0ff6702d24c183760ccfa8f0865f5cd805b6a834f02a`  
		Last Modified: Tue, 27 Jul 2021 00:00:30 GMT  
		Size: 840.6 KB (840558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd42adfa4f4468cc09d87fcaba98a160059fdee872c36809a69e43ab054efb`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 4.9 MB (4872150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e44ba6559363a0c0463b83b1977a52b1063833026aa6e9dddf178d444e003d`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccab66b30a6739dd0e587dc7eb7a3a05990bf99d4f6089491838f3bac0cfbdd`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f8627bbf4a2b81469316a6529e5a8c8bdd100a4ad64e0d474e973ec43f302`  
		Last Modified: Tue, 27 Jul 2021 01:11:51 GMT  
		Size: 259.4 MB (259445689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3fba9583601e046746fa9e5fb95242575e869b6747a7f9d937b202d9081bc`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:bbd128c88179834dd78f67e2f697f122e407e77a4a2f0e86dc2873ff0deca7f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266167808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f71b21d55415e370ea0f2efce7f099343d10317d448c608d9927230700632df0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:55:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:55:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:55:50 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 01:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:59:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 01:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:59:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c6b394219d75466dd6176f09c02e5fe7400b0255c6d82480e7d35a0d34a8ee`  
		Last Modified: Tue, 27 Jul 2021 02:18:18 GMT  
		Size: 841.4 KB (841388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879567137a59e93bade6d5accbcd0176b192ccc85080022acea9edea54f9f6c1`  
		Last Modified: Tue, 27 Jul 2021 02:18:17 GMT  
		Size: 4.1 MB (4085785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7141a26daf78fc9f5e9d8cda14c17fb9be91fe6714168a8b33e5a379eeed3f8`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7addca390d668268cbed3008b2cb7707f27958f9f9bbb47a35a03159a18ea5ea`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95f8679d120ee66925b7105bdb869ae6de6c3cd59823868c707a5e768eeeb6b`  
		Last Modified: Tue, 27 Jul 2021 02:20:46 GMT  
		Size: 238.9 MB (238931369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49793c91e8a015ee752db63891347c7ba6811b6aa0837cf3d0715caadd94a942`  
		Last Modified: Tue, 27 Jul 2021 02:18:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bd615357015446c6a4266c213417b07280476af2f6870933de92121f921a3f37
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281399098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8a9970b020adee0ec5936a93a2db6069dc9e5f2db3a889e6ecda9ac45dd189`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:49 GMT
ADD file:e87e065765ef99e8db25307f469c7481ab480ac5fe6353ae4caf402766f14045 in / 
# Mon, 26 Jul 2021 21:48:50 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:58:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 22:58:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV ROS_DISTRO=melodic
# Mon, 26 Jul 2021 22:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:59:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 22:59:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 22:59:55 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fda1cca7a3cc2b66c161597f27e151a9b1cab79d73c7c0c2706606813a3e58cf`  
		Last Modified: Mon, 26 Jul 2021 21:50:37 GMT  
		Size: 23.7 MB (23731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec48fab32c57250a0a316617993b1f19f17f7e3eb1f5b4b632c9e249bb8be37`  
		Last Modified: Mon, 26 Jul 2021 23:17:30 GMT  
		Size: 841.3 KB (841297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cda3a4d02e2669921c5de51d652aabfb73f4df2b82620e22cee0613358f560c`  
		Last Modified: Mon, 26 Jul 2021 23:17:28 GMT  
		Size: 4.5 MB (4453714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc312c19bce6f60c0e01ada675f9b439a2c4e6e65fdc361f6d9dfa88a88968`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f078b2e134b3bbc567abf387a039e07d7e9b62a44937b65e4486b11a93d0fa`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bb5e0dcebd403b1631077c2bf6f918a579e8261929dd592e97c3599825d707`  
		Last Modified: Mon, 26 Jul 2021 23:18:13 GMT  
		Size: 252.4 MB (252370080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262db146cf4cceac59a83a88e61705c701c9d85f669bade5fb3551c8f1cee8e3`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:9b03709d6c54ab97d50a1b99d3d00878071189aa2e7bf7faf3daac1c055bedc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:75a3bb07c9b6265827bf559fcc633d660776bb8f408b6dc4c3901f8d48a7fc3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291869847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:947363507d39ea6611167fc1c338d12ef5b49ba0a2a5cc6274d9860949f1d3a8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:38:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:35:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:35:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 00:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:38:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:38:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:38:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186553e47569a52e52d0ff6702d24c183760ccfa8f0865f5cd805b6a834f02a`  
		Last Modified: Tue, 27 Jul 2021 00:00:30 GMT  
		Size: 840.6 KB (840558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbd42adfa4f4468cc09d87fcaba98a160059fdee872c36809a69e43ab054efb`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 4.9 MB (4872150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e44ba6559363a0c0463b83b1977a52b1063833026aa6e9dddf178d444e003d`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccab66b30a6739dd0e587dc7eb7a3a05990bf99d4f6089491838f3bac0cfbdd`  
		Last Modified: Tue, 27 Jul 2021 01:11:08 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f8627bbf4a2b81469316a6529e5a8c8bdd100a4ad64e0d474e973ec43f302`  
		Last Modified: Tue, 27 Jul 2021 01:11:51 GMT  
		Size: 259.4 MB (259445689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3fba9583601e046746fa9e5fb95242575e869b6747a7f9d937b202d9081bc`  
		Last Modified: Tue, 27 Jul 2021 01:11:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:bbd128c88179834dd78f67e2f697f122e407e77a4a2f0e86dc2873ff0deca7f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266167808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f71b21d55415e370ea0f2efce7f099343d10317d448c608d9927230700632df0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:55:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:55:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:55:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:55:50 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:55:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 27 Jul 2021 01:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:59:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 01:59:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:59:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c6b394219d75466dd6176f09c02e5fe7400b0255c6d82480e7d35a0d34a8ee`  
		Last Modified: Tue, 27 Jul 2021 02:18:18 GMT  
		Size: 841.4 KB (841388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879567137a59e93bade6d5accbcd0176b192ccc85080022acea9edea54f9f6c1`  
		Last Modified: Tue, 27 Jul 2021 02:18:17 GMT  
		Size: 4.1 MB (4085785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7141a26daf78fc9f5e9d8cda14c17fb9be91fe6714168a8b33e5a379eeed3f8`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7addca390d668268cbed3008b2cb7707f27958f9f9bbb47a35a03159a18ea5ea`  
		Last Modified: Tue, 27 Jul 2021 02:18:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95f8679d120ee66925b7105bdb869ae6de6c3cd59823868c707a5e768eeeb6b`  
		Last Modified: Tue, 27 Jul 2021 02:20:46 GMT  
		Size: 238.9 MB (238931369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49793c91e8a015ee752db63891347c7ba6811b6aa0837cf3d0715caadd94a942`  
		Last Modified: Tue, 27 Jul 2021 02:18:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bd615357015446c6a4266c213417b07280476af2f6870933de92121f921a3f37
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281399098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8a9970b020adee0ec5936a93a2db6069dc9e5f2db3a889e6ecda9ac45dd189`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:49 GMT
ADD file:e87e065765ef99e8db25307f469c7481ab480ac5fe6353ae4caf402766f14045 in / 
# Mon, 26 Jul 2021 21:48:50 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:58:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 22:58:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV ROS_DISTRO=melodic
# Mon, 26 Jul 2021 22:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:59:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 22:59:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 22:59:55 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fda1cca7a3cc2b66c161597f27e151a9b1cab79d73c7c0c2706606813a3e58cf`  
		Last Modified: Mon, 26 Jul 2021 21:50:37 GMT  
		Size: 23.7 MB (23731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec48fab32c57250a0a316617993b1f19f17f7e3eb1f5b4b632c9e249bb8be37`  
		Last Modified: Mon, 26 Jul 2021 23:17:30 GMT  
		Size: 841.3 KB (841297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cda3a4d02e2669921c5de51d652aabfb73f4df2b82620e22cee0613358f560c`  
		Last Modified: Mon, 26 Jul 2021 23:17:28 GMT  
		Size: 4.5 MB (4453714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc312c19bce6f60c0e01ada675f9b439a2c4e6e65fdc361f6d9dfa88a88968`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f078b2e134b3bbc567abf387a039e07d7e9b62a44937b65e4486b11a93d0fa`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bb5e0dcebd403b1631077c2bf6f918a579e8261929dd592e97c3599825d707`  
		Last Modified: Mon, 26 Jul 2021 23:18:13 GMT  
		Size: 252.4 MB (252370080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262db146cf4cceac59a83a88e61705c701c9d85f669bade5fb3551c8f1cee8e3`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:66ba20ba51d44779dff11f490b0f30ab04f8ca15935f32ea5f058f1ac011d84d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:42187c1172c16383c3115f69296874cf789b49f8139799c02b4e541da27c5244
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339178352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:426daddb2147136e833c0d5562c86f62a3be0b266a24c08482c3c12b919aae8b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:48:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 00:50:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:50:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:50:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:50:51 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:51:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:51:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997acb5dc01c0a5dcc159471aea13a7b87074a11df83667b1f8b108602e7dda`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853e486374821ccfc40d07b68affecdc12e88f4ff7e8be0d58d904d3f525d5a`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e9cabb7a6a3ae445854e8bda4e4762b3d7ab26b3191ab8a006360c8dd0689f`  
		Last Modified: Tue, 27 Jul 2021 01:14:29 GMT  
		Size: 176.7 MB (176702826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c5a6e61679ad83770b86fc37c72db8d318a69a8d5dcac2d00db8bf86b0e9fc`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b972074e1773fd5c4e1a932d55b75a2a2850d2e1ffced2c52e961b49f75d22`  
		Last Modified: Tue, 27 Jul 2021 01:14:49 GMT  
		Size: 47.3 MB (47259266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccfe2edcc7482e1d5dc3b436b2197ed3020befcbc53e9f4f4e18c3a46497772`  
		Last Modified: Tue, 27 Jul 2021 01:14:40 GMT  
		Size: 313.4 KB (313417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c855981c165d5abfeb9c7d6a5bbfd8616a913a3674a8e23f9f4f9e6efd7fe627`  
		Last Modified: Tue, 27 Jul 2021 01:14:54 GMT  
		Size: 79.6 MB (79602950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:611a526bca19877d1fbfdd8dd84b9b1c3991b9157f4910b1951704df716fa316
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284623996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7d588f8655d95e5f10227e22b94f2c5d45b6fa733577a24393b2cc9c5acfb1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:06:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 02:06:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 02:06:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 02:08:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 02:08:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 02:08:54 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:09:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:09:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:10:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3707933348ed35dee73fe666615c4468caff6e2006136da4acd92e3cc985216d`  
		Last Modified: Tue, 27 Jul 2021 02:25:29 GMT  
		Size: 1.2 MB (1183472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf3da2af0d31416b9fa8b8d6cdca9940f2b02f0114144b0dd45896609465550`  
		Last Modified: Tue, 27 Jul 2021 02:25:28 GMT  
		Size: 4.7 MB (4676474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894df612b4be55234c3870d52402c8e0f8d862a70d921469dabd90fce65dd19b`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b69804f2417b467f0d90f227007b6ad0784998510b3059db7781646c4d9d7b0`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5140583e1bb4ff168122d517efa0932ee6c515d4c64167423b2c65c7f945120`  
		Last Modified: Tue, 27 Jul 2021 02:27:32 GMT  
		Size: 157.2 MB (157210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b14c8f11163b8fb56261a038b46a4424d6e04e8de12d91373885b3374fedd6`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c215fdc8101cc4022455bc40043758167955d643398391a07fb8f274a8b4b2`  
		Last Modified: Tue, 27 Jul 2021 02:28:05 GMT  
		Size: 36.7 MB (36691203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a81c5b7e4065976c7abc3018689ba1a166dbebe6f84d05c97525d8b823e4d38`  
		Last Modified: Tue, 27 Jul 2021 02:27:45 GMT  
		Size: 313.4 KB (313420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095184adef319323695c597ab15710f2f39440c2e9d62ffbd0a61ac2a230cc0c`  
		Last Modified: Tue, 27 Jul 2021 02:28:28 GMT  
		Size: 60.5 MB (60481937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:973f36a399a16652f412766fbaf74a552ca509548d44887e81de74ff5eb6a66b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.8 MB (318815797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0429fc233de20f5700ecb1ef0aeea0cba7b91c780a0d7c8f07f30ba1db3b12`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:03:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:03:31 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV ROS_DISTRO=noetic
# Mon, 26 Jul 2021 23:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 23:04:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:04:25 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:04:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d28ea46fe795b56172879ee97757cb6ea98226a43662f62f5bd8e1490c4fb`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1b73a67b1165693bd1ae07bace3301ab4fb82cfe1b5e61e2b536d3e2f75e47`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2161207e597e1e7621916bed37a91d2ed819071ecf81902fa5f9a199d8581048`  
		Last Modified: Mon, 26 Jul 2021 23:20:58 GMT  
		Size: 171.1 MB (171140053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab310c95b66fdb5ac105888d128d19608c8cd336dad6a23a85eee7e7b3a3e8`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a92eab614e3b9eeb6dafa9c74d6549e3f0dae57bdac2230eb29df020a27579b`  
		Last Modified: Mon, 26 Jul 2021 23:21:20 GMT  
		Size: 41.5 MB (41520773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab38b7bb1545dc49ffeead82d684f27e43bd0881738800aa0c8bb84590cde`  
		Last Modified: Mon, 26 Jul 2021 23:21:12 GMT  
		Size: 313.4 KB (313419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0468d318c5f7ccddaa45f1306287d14921ecd8e72c5a532713085cbfde2131`  
		Last Modified: Mon, 26 Jul 2021 23:21:24 GMT  
		Size: 72.0 MB (71972776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:e21d3803b92e591dadb0a808a8f29e6f015c8e1d111d096564fd0cd4e2c3ac03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:26f10371a9feb831aaab0f337e007879cf2001ab060c1de3291a28cb06ce2b3a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **838.2 MB (838191492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5835c71f748dc1ca333528fbad856c0d030269b829e193d158db34fd104ff52e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:48:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 00:50:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:50:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:50:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:50:51 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:51:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:51:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:01:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997acb5dc01c0a5dcc159471aea13a7b87074a11df83667b1f8b108602e7dda`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853e486374821ccfc40d07b68affecdc12e88f4ff7e8be0d58d904d3f525d5a`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e9cabb7a6a3ae445854e8bda4e4762b3d7ab26b3191ab8a006360c8dd0689f`  
		Last Modified: Tue, 27 Jul 2021 01:14:29 GMT  
		Size: 176.7 MB (176702826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c5a6e61679ad83770b86fc37c72db8d318a69a8d5dcac2d00db8bf86b0e9fc`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b972074e1773fd5c4e1a932d55b75a2a2850d2e1ffced2c52e961b49f75d22`  
		Last Modified: Tue, 27 Jul 2021 01:14:49 GMT  
		Size: 47.3 MB (47259266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccfe2edcc7482e1d5dc3b436b2197ed3020befcbc53e9f4f4e18c3a46497772`  
		Last Modified: Tue, 27 Jul 2021 01:14:40 GMT  
		Size: 313.4 KB (313417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c855981c165d5abfeb9c7d6a5bbfd8616a913a3674a8e23f9f4f9e6efd7fe627`  
		Last Modified: Tue, 27 Jul 2021 01:14:54 GMT  
		Size: 79.6 MB (79602950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ae84aba4fac5673ddc385e0d102d1420378f500119d4cdb9e8c2d45d1da053`  
		Last Modified: Tue, 27 Jul 2021 01:16:43 GMT  
		Size: 499.0 MB (499013140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:8c8eaf9b8c1a8021a91e252e878cc9e4dc0e827adbdc334b59859afd385789f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **727.9 MB (727868158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de3d22869639ec3542d9a7c46d53c44fc952f1b9872a3e0d11d711b1a68e57a7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:06:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 02:06:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 02:06:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 02:08:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 02:08:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 02:08:54 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:09:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:09:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:10:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:16:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3707933348ed35dee73fe666615c4468caff6e2006136da4acd92e3cc985216d`  
		Last Modified: Tue, 27 Jul 2021 02:25:29 GMT  
		Size: 1.2 MB (1183472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf3da2af0d31416b9fa8b8d6cdca9940f2b02f0114144b0dd45896609465550`  
		Last Modified: Tue, 27 Jul 2021 02:25:28 GMT  
		Size: 4.7 MB (4676474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894df612b4be55234c3870d52402c8e0f8d862a70d921469dabd90fce65dd19b`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b69804f2417b467f0d90f227007b6ad0784998510b3059db7781646c4d9d7b0`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5140583e1bb4ff168122d517efa0932ee6c515d4c64167423b2c65c7f945120`  
		Last Modified: Tue, 27 Jul 2021 02:27:32 GMT  
		Size: 157.2 MB (157210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b14c8f11163b8fb56261a038b46a4424d6e04e8de12d91373885b3374fedd6`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c215fdc8101cc4022455bc40043758167955d643398391a07fb8f274a8b4b2`  
		Last Modified: Tue, 27 Jul 2021 02:28:05 GMT  
		Size: 36.7 MB (36691203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a81c5b7e4065976c7abc3018689ba1a166dbebe6f84d05c97525d8b823e4d38`  
		Last Modified: Tue, 27 Jul 2021 02:27:45 GMT  
		Size: 313.4 KB (313420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095184adef319323695c597ab15710f2f39440c2e9d62ffbd0a61ac2a230cc0c`  
		Last Modified: Tue, 27 Jul 2021 02:28:28 GMT  
		Size: 60.5 MB (60481937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853f747b06bd9dbd06fef00ef1ffeba03276c0e8b456e243008dd30e0fdc5887`  
		Last Modified: Tue, 27 Jul 2021 02:33:41 GMT  
		Size: 443.2 MB (443244162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ad94be46c31dcb53792ad5e6e4c5517b2f03b90630482f1c7894e7529efc5f1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.1 MB (787108935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:391759d03bfd5a3574f799429451c1d817a6f1bad67a3af3d5fab5761635fa3c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:03:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:03:31 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV ROS_DISTRO=noetic
# Mon, 26 Jul 2021 23:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 23:04:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:04:25 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:04:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:07:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d28ea46fe795b56172879ee97757cb6ea98226a43662f62f5bd8e1490c4fb`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1b73a67b1165693bd1ae07bace3301ab4fb82cfe1b5e61e2b536d3e2f75e47`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2161207e597e1e7621916bed37a91d2ed819071ecf81902fa5f9a199d8581048`  
		Last Modified: Mon, 26 Jul 2021 23:20:58 GMT  
		Size: 171.1 MB (171140053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab310c95b66fdb5ac105888d128d19608c8cd336dad6a23a85eee7e7b3a3e8`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a92eab614e3b9eeb6dafa9c74d6549e3f0dae57bdac2230eb29df020a27579b`  
		Last Modified: Mon, 26 Jul 2021 23:21:20 GMT  
		Size: 41.5 MB (41520773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab38b7bb1545dc49ffeead82d684f27e43bd0881738800aa0c8bb84590cde`  
		Last Modified: Mon, 26 Jul 2021 23:21:12 GMT  
		Size: 313.4 KB (313419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0468d318c5f7ccddaa45f1306287d14921ecd8e72c5a532713085cbfde2131`  
		Last Modified: Mon, 26 Jul 2021 23:21:24 GMT  
		Size: 72.0 MB (71972776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4266ed692a1f6a99e16d5be04951b2e80a22524a21fc5035e36f66abb2300b`  
		Last Modified: Mon, 26 Jul 2021 23:23:19 GMT  
		Size: 468.3 MB (468293138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:52f9e9bf4654bd70cab5fa729e4736db7ab299687f885f07cf06b979b7976e3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:08388a8f291a61bafc049a98bafc9c2ef2a7a58f3909cc90d67b98a1f7bb45b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **968.0 MB (968013134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a3b0467f6eb0d92bf3c16db06cb5a90993e6b1ef764947e6d64b4b3079627a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:54:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:54:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 17 Aug 2021 14:54:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV ROS_DISTRO=noetic
# Tue, 17 Aug 2021 14:55:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:55:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 17 Aug 2021 14:55:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Aug 2021 14:55:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:56:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 17 Aug 2021 14:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6a25b8c075beb4891f7c9088956d2a452f32036d8126e37217b5b62fd7024c`  
		Last Modified: Tue, 17 Aug 2021 15:02:09 GMT  
		Size: 10.9 MB (10891952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e00b43ac20734a706cb03369661415e15f6856a48275dcd4fe7744b0bde5d23`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b19825ce46253a4664a6e606382250ba22ec8d0e1d13516be7d225efcca57f`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034eef40d3fabaea23b5d4473263a3a6ab8cd3545504c1ba16818b3b90152d1f`  
		Last Modified: Tue, 17 Aug 2021 15:02:50 GMT  
		Size: 239.1 MB (239050839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ae7d371ba1fee4f46bf91b9a18289de1dd3472eb2c3b8458f8ff2df5825c78`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b4384fc4992e164b0946674e8bf7905f6037fbe56d20552b0a9f981e0b23df`  
		Last Modified: Tue, 17 Aug 2021 15:03:21 GMT  
		Size: 86.6 MB (86566411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6466d96361536da7163da2fbe6e4e5267a768c30f1f04480d818c767e0ef32`  
		Last Modified: Tue, 17 Aug 2021 15:02:59 GMT  
		Size: 310.1 KB (310086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43da0dad1381eb1948df8e9a05518d305a6b3a7df20eb1f0b82edb2a00bee76b`  
		Last Modified: Tue, 17 Aug 2021 15:03:19 GMT  
		Size: 76.0 MB (75975146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b682f5f1680f2c4ec265e9f6da30a3f02e3e8782fbb3f6ced55263d693845a`  
		Last Modified: Tue, 17 Aug 2021 15:05:05 GMT  
		Size: 504.8 MB (504780085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:80c222e67d0165628296171890545c1ce5142b993e96c8d56d5d13c08a75dc29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **884.8 MB (884788088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9313f1dfa329f985bc41257c8c9628e684c8a7357e520918d3373f8c9232e83`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:48:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:48:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 17 Aug 2021 11:48:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 17 Aug 2021 11:48:59 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 11:48:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Aug 2021 11:49:00 GMT
ENV ROS_DISTRO=noetic
# Tue, 17 Aug 2021 11:49:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:49:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 17 Aug 2021 11:49:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Aug 2021 11:49:54 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:50:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:50:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 17 Aug 2021 11:50:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:53:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21602f601a18ce34c8a479ae1d7bac4442282478925664d6f67ad1d2b34e020`  
		Last Modified: Tue, 17 Aug 2021 11:56:11 GMT  
		Size: 10.9 MB (10883354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d4e557cfdbdf3a855acc0ae4cb3c204ac63ae1dd071cd42e608dcb0645c2d`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f24119c6422825783e8ee727d9b12a12c7cb5605e9b6e883b5101a388b450a`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd82c4517707ac42892fd33d02b10b53c8eb41cf05683d381df617056c035fd`  
		Last Modified: Tue, 17 Aug 2021 11:56:42 GMT  
		Size: 184.2 MB (184236324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5bbd42e097110d8576baa6d6d16c7a91e608fad20f3b7978c7e0e99f4ee7df`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf124f136abb277ab2e63f14af6802ccc288e34cc0c43a7d62f7c42717f23e3`  
		Last Modified: Tue, 17 Aug 2021 11:57:03 GMT  
		Size: 84.4 MB (84358116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6515efab5054193f9a8defd851ec9536c17950ae722b38778b4bd6aef481e9`  
		Last Modified: Tue, 17 Aug 2021 11:56:51 GMT  
		Size: 310.1 KB (310090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa915bc3d0bc2ea62806da8704257a5df824c41fa8997831b5de9ac482cca14`  
		Last Modified: Tue, 17 Aug 2021 11:57:03 GMT  
		Size: 74.1 MB (74087852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8ca443554ff1e63ad39ca3a88974d297e3128e3fa0f11c10d900b45a58daac`  
		Last Modified: Tue, 17 Aug 2021 11:58:36 GMT  
		Size: 481.7 MB (481687577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:e21d3803b92e591dadb0a808a8f29e6f015c8e1d111d096564fd0cd4e2c3ac03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:26f10371a9feb831aaab0f337e007879cf2001ab060c1de3291a28cb06ce2b3a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **838.2 MB (838191492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5835c71f748dc1ca333528fbad856c0d030269b829e193d158db34fd104ff52e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:48:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 00:50:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:50:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:50:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:50:51 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:51:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:51:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:01:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997acb5dc01c0a5dcc159471aea13a7b87074a11df83667b1f8b108602e7dda`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853e486374821ccfc40d07b68affecdc12e88f4ff7e8be0d58d904d3f525d5a`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e9cabb7a6a3ae445854e8bda4e4762b3d7ab26b3191ab8a006360c8dd0689f`  
		Last Modified: Tue, 27 Jul 2021 01:14:29 GMT  
		Size: 176.7 MB (176702826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c5a6e61679ad83770b86fc37c72db8d318a69a8d5dcac2d00db8bf86b0e9fc`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b972074e1773fd5c4e1a932d55b75a2a2850d2e1ffced2c52e961b49f75d22`  
		Last Modified: Tue, 27 Jul 2021 01:14:49 GMT  
		Size: 47.3 MB (47259266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccfe2edcc7482e1d5dc3b436b2197ed3020befcbc53e9f4f4e18c3a46497772`  
		Last Modified: Tue, 27 Jul 2021 01:14:40 GMT  
		Size: 313.4 KB (313417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c855981c165d5abfeb9c7d6a5bbfd8616a913a3674a8e23f9f4f9e6efd7fe627`  
		Last Modified: Tue, 27 Jul 2021 01:14:54 GMT  
		Size: 79.6 MB (79602950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ae84aba4fac5673ddc385e0d102d1420378f500119d4cdb9e8c2d45d1da053`  
		Last Modified: Tue, 27 Jul 2021 01:16:43 GMT  
		Size: 499.0 MB (499013140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:8c8eaf9b8c1a8021a91e252e878cc9e4dc0e827adbdc334b59859afd385789f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **727.9 MB (727868158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de3d22869639ec3542d9a7c46d53c44fc952f1b9872a3e0d11d711b1a68e57a7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:06:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 02:06:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 02:06:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 02:08:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 02:08:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 02:08:54 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:09:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:09:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:10:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:16:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3707933348ed35dee73fe666615c4468caff6e2006136da4acd92e3cc985216d`  
		Last Modified: Tue, 27 Jul 2021 02:25:29 GMT  
		Size: 1.2 MB (1183472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf3da2af0d31416b9fa8b8d6cdca9940f2b02f0114144b0dd45896609465550`  
		Last Modified: Tue, 27 Jul 2021 02:25:28 GMT  
		Size: 4.7 MB (4676474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894df612b4be55234c3870d52402c8e0f8d862a70d921469dabd90fce65dd19b`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b69804f2417b467f0d90f227007b6ad0784998510b3059db7781646c4d9d7b0`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5140583e1bb4ff168122d517efa0932ee6c515d4c64167423b2c65c7f945120`  
		Last Modified: Tue, 27 Jul 2021 02:27:32 GMT  
		Size: 157.2 MB (157210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b14c8f11163b8fb56261a038b46a4424d6e04e8de12d91373885b3374fedd6`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c215fdc8101cc4022455bc40043758167955d643398391a07fb8f274a8b4b2`  
		Last Modified: Tue, 27 Jul 2021 02:28:05 GMT  
		Size: 36.7 MB (36691203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a81c5b7e4065976c7abc3018689ba1a166dbebe6f84d05c97525d8b823e4d38`  
		Last Modified: Tue, 27 Jul 2021 02:27:45 GMT  
		Size: 313.4 KB (313420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095184adef319323695c597ab15710f2f39440c2e9d62ffbd0a61ac2a230cc0c`  
		Last Modified: Tue, 27 Jul 2021 02:28:28 GMT  
		Size: 60.5 MB (60481937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853f747b06bd9dbd06fef00ef1ffeba03276c0e8b456e243008dd30e0fdc5887`  
		Last Modified: Tue, 27 Jul 2021 02:33:41 GMT  
		Size: 443.2 MB (443244162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ad94be46c31dcb53792ad5e6e4c5517b2f03b90630482f1c7894e7529efc5f1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.1 MB (787108935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:391759d03bfd5a3574f799429451c1d817a6f1bad67a3af3d5fab5761635fa3c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:03:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:03:31 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV ROS_DISTRO=noetic
# Mon, 26 Jul 2021 23:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 23:04:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:04:25 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:04:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:07:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d28ea46fe795b56172879ee97757cb6ea98226a43662f62f5bd8e1490c4fb`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1b73a67b1165693bd1ae07bace3301ab4fb82cfe1b5e61e2b536d3e2f75e47`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2161207e597e1e7621916bed37a91d2ed819071ecf81902fa5f9a199d8581048`  
		Last Modified: Mon, 26 Jul 2021 23:20:58 GMT  
		Size: 171.1 MB (171140053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab310c95b66fdb5ac105888d128d19608c8cd336dad6a23a85eee7e7b3a3e8`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a92eab614e3b9eeb6dafa9c74d6549e3f0dae57bdac2230eb29df020a27579b`  
		Last Modified: Mon, 26 Jul 2021 23:21:20 GMT  
		Size: 41.5 MB (41520773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab38b7bb1545dc49ffeead82d684f27e43bd0881738800aa0c8bb84590cde`  
		Last Modified: Mon, 26 Jul 2021 23:21:12 GMT  
		Size: 313.4 KB (313419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0468d318c5f7ccddaa45f1306287d14921ecd8e72c5a532713085cbfde2131`  
		Last Modified: Mon, 26 Jul 2021 23:21:24 GMT  
		Size: 72.0 MB (71972776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4266ed692a1f6a99e16d5be04951b2e80a22524a21fc5035e36f66abb2300b`  
		Last Modified: Mon, 26 Jul 2021 23:23:19 GMT  
		Size: 468.3 MB (468293138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:1e062fc3fbc5af598bfae630a869f036b538482d5e9c1cf5994bfadfa521a604
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:c8af0dded98fb671ba69c484aeca30af7fbbd5f9b6d22336982e2c32822e1341
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.9 MB (354915755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd21d28f34bd9d2dfe85aacd05d13ddf63490765d2557a24c8fd0ce03a8a384a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:48:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 00:50:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:50:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:50:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:50:51 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:51:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:51:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:53:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997acb5dc01c0a5dcc159471aea13a7b87074a11df83667b1f8b108602e7dda`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853e486374821ccfc40d07b68affecdc12e88f4ff7e8be0d58d904d3f525d5a`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e9cabb7a6a3ae445854e8bda4e4762b3d7ab26b3191ab8a006360c8dd0689f`  
		Last Modified: Tue, 27 Jul 2021 01:14:29 GMT  
		Size: 176.7 MB (176702826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c5a6e61679ad83770b86fc37c72db8d318a69a8d5dcac2d00db8bf86b0e9fc`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b972074e1773fd5c4e1a932d55b75a2a2850d2e1ffced2c52e961b49f75d22`  
		Last Modified: Tue, 27 Jul 2021 01:14:49 GMT  
		Size: 47.3 MB (47259266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccfe2edcc7482e1d5dc3b436b2197ed3020befcbc53e9f4f4e18c3a46497772`  
		Last Modified: Tue, 27 Jul 2021 01:14:40 GMT  
		Size: 313.4 KB (313417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c855981c165d5abfeb9c7d6a5bbfd8616a913a3674a8e23f9f4f9e6efd7fe627`  
		Last Modified: Tue, 27 Jul 2021 01:14:54 GMT  
		Size: 79.6 MB (79602950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caed4353fbe38855f36fb5376060099dca87d8674318e8a911b9943f6e574423`  
		Last Modified: Tue, 27 Jul 2021 01:15:12 GMT  
		Size: 15.7 MB (15737403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:9433435e54c4ccf5d734dd4be8e5492fecafb890743ad963d5ba5151c2beb583
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298584275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51362dde9245e1d744f33b498603a195f3e0cf834395a7eb3acaf9d4c003980b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:06:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 02:06:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 02:06:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 02:08:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 02:08:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 02:08:54 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:09:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:09:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:10:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:11:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3707933348ed35dee73fe666615c4468caff6e2006136da4acd92e3cc985216d`  
		Last Modified: Tue, 27 Jul 2021 02:25:29 GMT  
		Size: 1.2 MB (1183472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf3da2af0d31416b9fa8b8d6cdca9940f2b02f0114144b0dd45896609465550`  
		Last Modified: Tue, 27 Jul 2021 02:25:28 GMT  
		Size: 4.7 MB (4676474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894df612b4be55234c3870d52402c8e0f8d862a70d921469dabd90fce65dd19b`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b69804f2417b467f0d90f227007b6ad0784998510b3059db7781646c4d9d7b0`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5140583e1bb4ff168122d517efa0932ee6c515d4c64167423b2c65c7f945120`  
		Last Modified: Tue, 27 Jul 2021 02:27:32 GMT  
		Size: 157.2 MB (157210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b14c8f11163b8fb56261a038b46a4424d6e04e8de12d91373885b3374fedd6`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c215fdc8101cc4022455bc40043758167955d643398391a07fb8f274a8b4b2`  
		Last Modified: Tue, 27 Jul 2021 02:28:05 GMT  
		Size: 36.7 MB (36691203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a81c5b7e4065976c7abc3018689ba1a166dbebe6f84d05c97525d8b823e4d38`  
		Last Modified: Tue, 27 Jul 2021 02:27:45 GMT  
		Size: 313.4 KB (313420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095184adef319323695c597ab15710f2f39440c2e9d62ffbd0a61ac2a230cc0c`  
		Last Modified: Tue, 27 Jul 2021 02:28:28 GMT  
		Size: 60.5 MB (60481937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597531626f0d53d0a21f11d7ee2c6247efdaec8f4b239b813e51d780e664e40a`  
		Last Modified: Tue, 27 Jul 2021 02:28:54 GMT  
		Size: 14.0 MB (13960279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cd9e4dc5a97b8683c3165e7d8794162a65533b496812c94d5d84f4c2626047f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334167154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a4f1f852293947f134b97038a717079ef453df5e42114df4ee741ebc96891fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:03:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:03:31 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV ROS_DISTRO=noetic
# Mon, 26 Jul 2021 23:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 23:04:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:04:25 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:04:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:05:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d28ea46fe795b56172879ee97757cb6ea98226a43662f62f5bd8e1490c4fb`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1b73a67b1165693bd1ae07bace3301ab4fb82cfe1b5e61e2b536d3e2f75e47`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2161207e597e1e7621916bed37a91d2ed819071ecf81902fa5f9a199d8581048`  
		Last Modified: Mon, 26 Jul 2021 23:20:58 GMT  
		Size: 171.1 MB (171140053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab310c95b66fdb5ac105888d128d19608c8cd336dad6a23a85eee7e7b3a3e8`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a92eab614e3b9eeb6dafa9c74d6549e3f0dae57bdac2230eb29df020a27579b`  
		Last Modified: Mon, 26 Jul 2021 23:21:20 GMT  
		Size: 41.5 MB (41520773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab38b7bb1545dc49ffeead82d684f27e43bd0881738800aa0c8bb84590cde`  
		Last Modified: Mon, 26 Jul 2021 23:21:12 GMT  
		Size: 313.4 KB (313419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0468d318c5f7ccddaa45f1306287d14921ecd8e72c5a532713085cbfde2131`  
		Last Modified: Mon, 26 Jul 2021 23:21:24 GMT  
		Size: 72.0 MB (71972776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c66dec020980c4a0606add91e864f375b616437dd803afd9fe6259f3a6e3ef`  
		Last Modified: Mon, 26 Jul 2021 23:21:44 GMT  
		Size: 15.4 MB (15351357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:fd9e03a878cadcb365ccb236cd47c36dc1a19ce4105becedd4e9418dc8d1ca1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:8fc740c4c663c10544f1c6fcbe0d9ed232d15725bc41d4b4ee256a5cc193f534
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.5 MB (484451700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca0c9f7c246ad81ee27739eb65046725966c9334246e9e1571884a8cf33cdf6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:54:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:54:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 17 Aug 2021 14:54:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV ROS_DISTRO=noetic
# Tue, 17 Aug 2021 14:55:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:55:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 17 Aug 2021 14:55:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Aug 2021 14:55:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:56:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 17 Aug 2021 14:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:57:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6a25b8c075beb4891f7c9088956d2a452f32036d8126e37217b5b62fd7024c`  
		Last Modified: Tue, 17 Aug 2021 15:02:09 GMT  
		Size: 10.9 MB (10891952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e00b43ac20734a706cb03369661415e15f6856a48275dcd4fe7744b0bde5d23`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b19825ce46253a4664a6e606382250ba22ec8d0e1d13516be7d225efcca57f`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034eef40d3fabaea23b5d4473263a3a6ab8cd3545504c1ba16818b3b90152d1f`  
		Last Modified: Tue, 17 Aug 2021 15:02:50 GMT  
		Size: 239.1 MB (239050839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ae7d371ba1fee4f46bf91b9a18289de1dd3472eb2c3b8458f8ff2df5825c78`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b4384fc4992e164b0946674e8bf7905f6037fbe56d20552b0a9f981e0b23df`  
		Last Modified: Tue, 17 Aug 2021 15:03:21 GMT  
		Size: 86.6 MB (86566411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6466d96361536da7163da2fbe6e4e5267a768c30f1f04480d818c767e0ef32`  
		Last Modified: Tue, 17 Aug 2021 15:02:59 GMT  
		Size: 310.1 KB (310086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43da0dad1381eb1948df8e9a05518d305a6b3a7df20eb1f0b82edb2a00bee76b`  
		Last Modified: Tue, 17 Aug 2021 15:03:19 GMT  
		Size: 76.0 MB (75975146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb420023d0d4981e7e1c712cf7670854d7160f6cd251076d6fa94d822b18cef2`  
		Last Modified: Tue, 17 Aug 2021 15:03:35 GMT  
		Size: 21.2 MB (21218651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a71321e849437464740dadf3a7d92ba33aa9cd325313096b2092348fc5582503
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.0 MB (423996486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1339d6e7c2ba9eca967117d5d0a6a8b425002eb4c8f7803111013392eb2e9f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:48:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:48:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 17 Aug 2021 11:48:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 17 Aug 2021 11:48:59 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 11:48:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Aug 2021 11:49:00 GMT
ENV ROS_DISTRO=noetic
# Tue, 17 Aug 2021 11:49:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:49:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 17 Aug 2021 11:49:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Aug 2021 11:49:54 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:50:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:50:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 17 Aug 2021 11:50:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21602f601a18ce34c8a479ae1d7bac4442282478925664d6f67ad1d2b34e020`  
		Last Modified: Tue, 17 Aug 2021 11:56:11 GMT  
		Size: 10.9 MB (10883354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d4e557cfdbdf3a855acc0ae4cb3c204ac63ae1dd071cd42e608dcb0645c2d`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f24119c6422825783e8ee727d9b12a12c7cb5605e9b6e883b5101a388b450a`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd82c4517707ac42892fd33d02b10b53c8eb41cf05683d381df617056c035fd`  
		Last Modified: Tue, 17 Aug 2021 11:56:42 GMT  
		Size: 184.2 MB (184236324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5bbd42e097110d8576baa6d6d16c7a91e608fad20f3b7978c7e0e99f4ee7df`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf124f136abb277ab2e63f14af6802ccc288e34cc0c43a7d62f7c42717f23e3`  
		Last Modified: Tue, 17 Aug 2021 11:57:03 GMT  
		Size: 84.4 MB (84358116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6515efab5054193f9a8defd851ec9536c17950ae722b38778b4bd6aef481e9`  
		Last Modified: Tue, 17 Aug 2021 11:56:51 GMT  
		Size: 310.1 KB (310090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa915bc3d0bc2ea62806da8704257a5df824c41fa8997831b5de9ac482cca14`  
		Last Modified: Tue, 17 Aug 2021 11:57:03 GMT  
		Size: 74.1 MB (74087852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f1b5f110e2990823b69a716c68ef7506a92319e4d3c59c1991db59244653d1`  
		Last Modified: Tue, 17 Aug 2021 11:57:14 GMT  
		Size: 20.9 MB (20895975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:1e062fc3fbc5af598bfae630a869f036b538482d5e9c1cf5994bfadfa521a604
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:c8af0dded98fb671ba69c484aeca30af7fbbd5f9b6d22336982e2c32822e1341
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.9 MB (354915755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd21d28f34bd9d2dfe85aacd05d13ddf63490765d2557a24c8fd0ce03a8a384a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:48:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 00:50:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:50:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:50:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:50:51 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:51:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:51:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:53:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997acb5dc01c0a5dcc159471aea13a7b87074a11df83667b1f8b108602e7dda`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853e486374821ccfc40d07b68affecdc12e88f4ff7e8be0d58d904d3f525d5a`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e9cabb7a6a3ae445854e8bda4e4762b3d7ab26b3191ab8a006360c8dd0689f`  
		Last Modified: Tue, 27 Jul 2021 01:14:29 GMT  
		Size: 176.7 MB (176702826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c5a6e61679ad83770b86fc37c72db8d318a69a8d5dcac2d00db8bf86b0e9fc`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b972074e1773fd5c4e1a932d55b75a2a2850d2e1ffced2c52e961b49f75d22`  
		Last Modified: Tue, 27 Jul 2021 01:14:49 GMT  
		Size: 47.3 MB (47259266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccfe2edcc7482e1d5dc3b436b2197ed3020befcbc53e9f4f4e18c3a46497772`  
		Last Modified: Tue, 27 Jul 2021 01:14:40 GMT  
		Size: 313.4 KB (313417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c855981c165d5abfeb9c7d6a5bbfd8616a913a3674a8e23f9f4f9e6efd7fe627`  
		Last Modified: Tue, 27 Jul 2021 01:14:54 GMT  
		Size: 79.6 MB (79602950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caed4353fbe38855f36fb5376060099dca87d8674318e8a911b9943f6e574423`  
		Last Modified: Tue, 27 Jul 2021 01:15:12 GMT  
		Size: 15.7 MB (15737403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:9433435e54c4ccf5d734dd4be8e5492fecafb890743ad963d5ba5151c2beb583
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298584275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51362dde9245e1d744f33b498603a195f3e0cf834395a7eb3acaf9d4c003980b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:06:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 02:06:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 02:06:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 02:08:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 02:08:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 02:08:54 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:09:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:09:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:10:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:11:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3707933348ed35dee73fe666615c4468caff6e2006136da4acd92e3cc985216d`  
		Last Modified: Tue, 27 Jul 2021 02:25:29 GMT  
		Size: 1.2 MB (1183472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf3da2af0d31416b9fa8b8d6cdca9940f2b02f0114144b0dd45896609465550`  
		Last Modified: Tue, 27 Jul 2021 02:25:28 GMT  
		Size: 4.7 MB (4676474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894df612b4be55234c3870d52402c8e0f8d862a70d921469dabd90fce65dd19b`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b69804f2417b467f0d90f227007b6ad0784998510b3059db7781646c4d9d7b0`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5140583e1bb4ff168122d517efa0932ee6c515d4c64167423b2c65c7f945120`  
		Last Modified: Tue, 27 Jul 2021 02:27:32 GMT  
		Size: 157.2 MB (157210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b14c8f11163b8fb56261a038b46a4424d6e04e8de12d91373885b3374fedd6`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c215fdc8101cc4022455bc40043758167955d643398391a07fb8f274a8b4b2`  
		Last Modified: Tue, 27 Jul 2021 02:28:05 GMT  
		Size: 36.7 MB (36691203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a81c5b7e4065976c7abc3018689ba1a166dbebe6f84d05c97525d8b823e4d38`  
		Last Modified: Tue, 27 Jul 2021 02:27:45 GMT  
		Size: 313.4 KB (313420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095184adef319323695c597ab15710f2f39440c2e9d62ffbd0a61ac2a230cc0c`  
		Last Modified: Tue, 27 Jul 2021 02:28:28 GMT  
		Size: 60.5 MB (60481937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597531626f0d53d0a21f11d7ee2c6247efdaec8f4b239b813e51d780e664e40a`  
		Last Modified: Tue, 27 Jul 2021 02:28:54 GMT  
		Size: 14.0 MB (13960279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cd9e4dc5a97b8683c3165e7d8794162a65533b496812c94d5d84f4c2626047f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334167154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a4f1f852293947f134b97038a717079ef453df5e42114df4ee741ebc96891fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:03:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:03:31 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV ROS_DISTRO=noetic
# Mon, 26 Jul 2021 23:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 23:04:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:04:25 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:04:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:05:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d28ea46fe795b56172879ee97757cb6ea98226a43662f62f5bd8e1490c4fb`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1b73a67b1165693bd1ae07bace3301ab4fb82cfe1b5e61e2b536d3e2f75e47`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2161207e597e1e7621916bed37a91d2ed819071ecf81902fa5f9a199d8581048`  
		Last Modified: Mon, 26 Jul 2021 23:20:58 GMT  
		Size: 171.1 MB (171140053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab310c95b66fdb5ac105888d128d19608c8cd336dad6a23a85eee7e7b3a3e8`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a92eab614e3b9eeb6dafa9c74d6549e3f0dae57bdac2230eb29df020a27579b`  
		Last Modified: Mon, 26 Jul 2021 23:21:20 GMT  
		Size: 41.5 MB (41520773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab38b7bb1545dc49ffeead82d684f27e43bd0881738800aa0c8bb84590cde`  
		Last Modified: Mon, 26 Jul 2021 23:21:12 GMT  
		Size: 313.4 KB (313419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0468d318c5f7ccddaa45f1306287d14921ecd8e72c5a532713085cbfde2131`  
		Last Modified: Mon, 26 Jul 2021 23:21:24 GMT  
		Size: 72.0 MB (71972776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c66dec020980c4a0606add91e864f375b616437dd803afd9fe6259f3a6e3ef`  
		Last Modified: Mon, 26 Jul 2021 23:21:44 GMT  
		Size: 15.4 MB (15351357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:66ba20ba51d44779dff11f490b0f30ab04f8ca15935f32ea5f058f1ac011d84d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:42187c1172c16383c3115f69296874cf789b49f8139799c02b4e541da27c5244
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339178352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:426daddb2147136e833c0d5562c86f62a3be0b266a24c08482c3c12b919aae8b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:48:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 00:50:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:50:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:50:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:50:51 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:51:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:51:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997acb5dc01c0a5dcc159471aea13a7b87074a11df83667b1f8b108602e7dda`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853e486374821ccfc40d07b68affecdc12e88f4ff7e8be0d58d904d3f525d5a`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e9cabb7a6a3ae445854e8bda4e4762b3d7ab26b3191ab8a006360c8dd0689f`  
		Last Modified: Tue, 27 Jul 2021 01:14:29 GMT  
		Size: 176.7 MB (176702826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c5a6e61679ad83770b86fc37c72db8d318a69a8d5dcac2d00db8bf86b0e9fc`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b972074e1773fd5c4e1a932d55b75a2a2850d2e1ffced2c52e961b49f75d22`  
		Last Modified: Tue, 27 Jul 2021 01:14:49 GMT  
		Size: 47.3 MB (47259266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccfe2edcc7482e1d5dc3b436b2197ed3020befcbc53e9f4f4e18c3a46497772`  
		Last Modified: Tue, 27 Jul 2021 01:14:40 GMT  
		Size: 313.4 KB (313417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c855981c165d5abfeb9c7d6a5bbfd8616a913a3674a8e23f9f4f9e6efd7fe627`  
		Last Modified: Tue, 27 Jul 2021 01:14:54 GMT  
		Size: 79.6 MB (79602950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:611a526bca19877d1fbfdd8dd84b9b1c3991b9157f4910b1951704df716fa316
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284623996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7d588f8655d95e5f10227e22b94f2c5d45b6fa733577a24393b2cc9c5acfb1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:06:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 02:06:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 02:06:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 02:08:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 02:08:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 02:08:54 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:09:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:09:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:10:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3707933348ed35dee73fe666615c4468caff6e2006136da4acd92e3cc985216d`  
		Last Modified: Tue, 27 Jul 2021 02:25:29 GMT  
		Size: 1.2 MB (1183472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf3da2af0d31416b9fa8b8d6cdca9940f2b02f0114144b0dd45896609465550`  
		Last Modified: Tue, 27 Jul 2021 02:25:28 GMT  
		Size: 4.7 MB (4676474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894df612b4be55234c3870d52402c8e0f8d862a70d921469dabd90fce65dd19b`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b69804f2417b467f0d90f227007b6ad0784998510b3059db7781646c4d9d7b0`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5140583e1bb4ff168122d517efa0932ee6c515d4c64167423b2c65c7f945120`  
		Last Modified: Tue, 27 Jul 2021 02:27:32 GMT  
		Size: 157.2 MB (157210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b14c8f11163b8fb56261a038b46a4424d6e04e8de12d91373885b3374fedd6`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c215fdc8101cc4022455bc40043758167955d643398391a07fb8f274a8b4b2`  
		Last Modified: Tue, 27 Jul 2021 02:28:05 GMT  
		Size: 36.7 MB (36691203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a81c5b7e4065976c7abc3018689ba1a166dbebe6f84d05c97525d8b823e4d38`  
		Last Modified: Tue, 27 Jul 2021 02:27:45 GMT  
		Size: 313.4 KB (313420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095184adef319323695c597ab15710f2f39440c2e9d62ffbd0a61ac2a230cc0c`  
		Last Modified: Tue, 27 Jul 2021 02:28:28 GMT  
		Size: 60.5 MB (60481937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:973f36a399a16652f412766fbaf74a552ca509548d44887e81de74ff5eb6a66b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.8 MB (318815797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0429fc233de20f5700ecb1ef0aeea0cba7b91c780a0d7c8f07f30ba1db3b12`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:03:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:03:31 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV ROS_DISTRO=noetic
# Mon, 26 Jul 2021 23:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 23:04:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:04:25 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:04:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d28ea46fe795b56172879ee97757cb6ea98226a43662f62f5bd8e1490c4fb`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1b73a67b1165693bd1ae07bace3301ab4fb82cfe1b5e61e2b536d3e2f75e47`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2161207e597e1e7621916bed37a91d2ed819071ecf81902fa5f9a199d8581048`  
		Last Modified: Mon, 26 Jul 2021 23:20:58 GMT  
		Size: 171.1 MB (171140053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab310c95b66fdb5ac105888d128d19608c8cd336dad6a23a85eee7e7b3a3e8`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a92eab614e3b9eeb6dafa9c74d6549e3f0dae57bdac2230eb29df020a27579b`  
		Last Modified: Mon, 26 Jul 2021 23:21:20 GMT  
		Size: 41.5 MB (41520773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab38b7bb1545dc49ffeead82d684f27e43bd0881738800aa0c8bb84590cde`  
		Last Modified: Mon, 26 Jul 2021 23:21:12 GMT  
		Size: 313.4 KB (313419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0468d318c5f7ccddaa45f1306287d14921ecd8e72c5a532713085cbfde2131`  
		Last Modified: Mon, 26 Jul 2021 23:21:24 GMT  
		Size: 72.0 MB (71972776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:1ede5a1c4cc2e4f58e1584d4ddc67b3f557ab9a7e1c26e80416e50ba9e055910
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:90d57bbd4866380ad8d03a8d9442a8c476aafaf933950a491d513e90c41442f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.2 MB (463233049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d80fa568e8b606cab686e55d3a879a85c0de337ff0c5f9abc9987416b5c6ec4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:54:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:54:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 17 Aug 2021 14:54:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV ROS_DISTRO=noetic
# Tue, 17 Aug 2021 14:55:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:55:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 17 Aug 2021 14:55:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Aug 2021 14:55:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:56:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 17 Aug 2021 14:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6a25b8c075beb4891f7c9088956d2a452f32036d8126e37217b5b62fd7024c`  
		Last Modified: Tue, 17 Aug 2021 15:02:09 GMT  
		Size: 10.9 MB (10891952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e00b43ac20734a706cb03369661415e15f6856a48275dcd4fe7744b0bde5d23`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b19825ce46253a4664a6e606382250ba22ec8d0e1d13516be7d225efcca57f`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034eef40d3fabaea23b5d4473263a3a6ab8cd3545504c1ba16818b3b90152d1f`  
		Last Modified: Tue, 17 Aug 2021 15:02:50 GMT  
		Size: 239.1 MB (239050839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ae7d371ba1fee4f46bf91b9a18289de1dd3472eb2c3b8458f8ff2df5825c78`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b4384fc4992e164b0946674e8bf7905f6037fbe56d20552b0a9f981e0b23df`  
		Last Modified: Tue, 17 Aug 2021 15:03:21 GMT  
		Size: 86.6 MB (86566411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6466d96361536da7163da2fbe6e4e5267a768c30f1f04480d818c767e0ef32`  
		Last Modified: Tue, 17 Aug 2021 15:02:59 GMT  
		Size: 310.1 KB (310086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43da0dad1381eb1948df8e9a05518d305a6b3a7df20eb1f0b82edb2a00bee76b`  
		Last Modified: Tue, 17 Aug 2021 15:03:19 GMT  
		Size: 76.0 MB (75975146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a082ab94d8f9a2d34787226bfb46ba3cfb97bb8f6ce73f6d7fe1b49f34da4f20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.1 MB (403100511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24888980eb73078603a8d2bf0a573fd83f79dcfa00bd30e7dc6acb44a44897c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:48:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:48:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 17 Aug 2021 11:48:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 17 Aug 2021 11:48:59 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 11:48:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Aug 2021 11:49:00 GMT
ENV ROS_DISTRO=noetic
# Tue, 17 Aug 2021 11:49:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:49:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 17 Aug 2021 11:49:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Aug 2021 11:49:54 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:50:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:50:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 17 Aug 2021 11:50:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21602f601a18ce34c8a479ae1d7bac4442282478925664d6f67ad1d2b34e020`  
		Last Modified: Tue, 17 Aug 2021 11:56:11 GMT  
		Size: 10.9 MB (10883354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d4e557cfdbdf3a855acc0ae4cb3c204ac63ae1dd071cd42e608dcb0645c2d`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f24119c6422825783e8ee727d9b12a12c7cb5605e9b6e883b5101a388b450a`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd82c4517707ac42892fd33d02b10b53c8eb41cf05683d381df617056c035fd`  
		Last Modified: Tue, 17 Aug 2021 11:56:42 GMT  
		Size: 184.2 MB (184236324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5bbd42e097110d8576baa6d6d16c7a91e608fad20f3b7978c7e0e99f4ee7df`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf124f136abb277ab2e63f14af6802ccc288e34cc0c43a7d62f7c42717f23e3`  
		Last Modified: Tue, 17 Aug 2021 11:57:03 GMT  
		Size: 84.4 MB (84358116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6515efab5054193f9a8defd851ec9536c17950ae722b38778b4bd6aef481e9`  
		Last Modified: Tue, 17 Aug 2021 11:56:51 GMT  
		Size: 310.1 KB (310090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa915bc3d0bc2ea62806da8704257a5df824c41fa8997831b5de9ac482cca14`  
		Last Modified: Tue, 17 Aug 2021 11:57:03 GMT  
		Size: 74.1 MB (74087852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:66ba20ba51d44779dff11f490b0f30ab04f8ca15935f32ea5f058f1ac011d84d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:42187c1172c16383c3115f69296874cf789b49f8139799c02b4e541da27c5244
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339178352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:426daddb2147136e833c0d5562c86f62a3be0b266a24c08482c3c12b919aae8b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:48:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 00:50:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:50:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:50:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:50:51 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:51:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:51:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 00:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997acb5dc01c0a5dcc159471aea13a7b87074a11df83667b1f8b108602e7dda`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853e486374821ccfc40d07b68affecdc12e88f4ff7e8be0d58d904d3f525d5a`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e9cabb7a6a3ae445854e8bda4e4762b3d7ab26b3191ab8a006360c8dd0689f`  
		Last Modified: Tue, 27 Jul 2021 01:14:29 GMT  
		Size: 176.7 MB (176702826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c5a6e61679ad83770b86fc37c72db8d318a69a8d5dcac2d00db8bf86b0e9fc`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b972074e1773fd5c4e1a932d55b75a2a2850d2e1ffced2c52e961b49f75d22`  
		Last Modified: Tue, 27 Jul 2021 01:14:49 GMT  
		Size: 47.3 MB (47259266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccfe2edcc7482e1d5dc3b436b2197ed3020befcbc53e9f4f4e18c3a46497772`  
		Last Modified: Tue, 27 Jul 2021 01:14:40 GMT  
		Size: 313.4 KB (313417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c855981c165d5abfeb9c7d6a5bbfd8616a913a3674a8e23f9f4f9e6efd7fe627`  
		Last Modified: Tue, 27 Jul 2021 01:14:54 GMT  
		Size: 79.6 MB (79602950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:611a526bca19877d1fbfdd8dd84b9b1c3991b9157f4910b1951704df716fa316
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284623996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7d588f8655d95e5f10227e22b94f2c5d45b6fa733577a24393b2cc9c5acfb1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:06:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 02:06:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 02:06:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 02:08:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 02:08:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 02:08:54 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:09:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:09:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 02:10:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3707933348ed35dee73fe666615c4468caff6e2006136da4acd92e3cc985216d`  
		Last Modified: Tue, 27 Jul 2021 02:25:29 GMT  
		Size: 1.2 MB (1183472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf3da2af0d31416b9fa8b8d6cdca9940f2b02f0114144b0dd45896609465550`  
		Last Modified: Tue, 27 Jul 2021 02:25:28 GMT  
		Size: 4.7 MB (4676474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894df612b4be55234c3870d52402c8e0f8d862a70d921469dabd90fce65dd19b`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b69804f2417b467f0d90f227007b6ad0784998510b3059db7781646c4d9d7b0`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5140583e1bb4ff168122d517efa0932ee6c515d4c64167423b2c65c7f945120`  
		Last Modified: Tue, 27 Jul 2021 02:27:32 GMT  
		Size: 157.2 MB (157210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b14c8f11163b8fb56261a038b46a4424d6e04e8de12d91373885b3374fedd6`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c215fdc8101cc4022455bc40043758167955d643398391a07fb8f274a8b4b2`  
		Last Modified: Tue, 27 Jul 2021 02:28:05 GMT  
		Size: 36.7 MB (36691203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a81c5b7e4065976c7abc3018689ba1a166dbebe6f84d05c97525d8b823e4d38`  
		Last Modified: Tue, 27 Jul 2021 02:27:45 GMT  
		Size: 313.4 KB (313420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095184adef319323695c597ab15710f2f39440c2e9d62ffbd0a61ac2a230cc0c`  
		Last Modified: Tue, 27 Jul 2021 02:28:28 GMT  
		Size: 60.5 MB (60481937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:973f36a399a16652f412766fbaf74a552ca509548d44887e81de74ff5eb6a66b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.8 MB (318815797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0429fc233de20f5700ecb1ef0aeea0cba7b91c780a0d7c8f07f30ba1db3b12`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:03:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:03:31 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV ROS_DISTRO=noetic
# Mon, 26 Jul 2021 23:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 23:04:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:04:25 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:04:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d28ea46fe795b56172879ee97757cb6ea98226a43662f62f5bd8e1490c4fb`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1b73a67b1165693bd1ae07bace3301ab4fb82cfe1b5e61e2b536d3e2f75e47`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2161207e597e1e7621916bed37a91d2ed819071ecf81902fa5f9a199d8581048`  
		Last Modified: Mon, 26 Jul 2021 23:20:58 GMT  
		Size: 171.1 MB (171140053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab310c95b66fdb5ac105888d128d19608c8cd336dad6a23a85eee7e7b3a3e8`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a92eab614e3b9eeb6dafa9c74d6549e3f0dae57bdac2230eb29df020a27579b`  
		Last Modified: Mon, 26 Jul 2021 23:21:20 GMT  
		Size: 41.5 MB (41520773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab38b7bb1545dc49ffeead82d684f27e43bd0881738800aa0c8bb84590cde`  
		Last Modified: Mon, 26 Jul 2021 23:21:12 GMT  
		Size: 313.4 KB (313419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0468d318c5f7ccddaa45f1306287d14921ecd8e72c5a532713085cbfde2131`  
		Last Modified: Mon, 26 Jul 2021 23:21:24 GMT  
		Size: 72.0 MB (71972776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:1b88921e614ddb5e72223547f89868583789ca5912472f6019cdf7e998248651
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:518d9f49f3956bf92607be0c47a8dbf00d0c567dbb919c607b611e3bcf8c8912
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (212002719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b1740831ef859270de7fd9091d58dda92142f7d3f71df422fb26d0376da185`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:48:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 00:50:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:50:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:50:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:50:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997acb5dc01c0a5dcc159471aea13a7b87074a11df83667b1f8b108602e7dda`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853e486374821ccfc40d07b68affecdc12e88f4ff7e8be0d58d904d3f525d5a`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e9cabb7a6a3ae445854e8bda4e4762b3d7ab26b3191ab8a006360c8dd0689f`  
		Last Modified: Tue, 27 Jul 2021 01:14:29 GMT  
		Size: 176.7 MB (176702826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c5a6e61679ad83770b86fc37c72db8d318a69a8d5dcac2d00db8bf86b0e9fc`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:45f08fb5b042970e1b561d9b3940fdabc46b34958678536c54a07e17c3a253cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187137436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a223e481044d9ab0a67a6bad021ae42bd8957c52c4a9357dd2632e569d1594c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:06:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 02:06:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 02:06:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 02:08:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 02:08:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 02:08:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3707933348ed35dee73fe666615c4468caff6e2006136da4acd92e3cc985216d`  
		Last Modified: Tue, 27 Jul 2021 02:25:29 GMT  
		Size: 1.2 MB (1183472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf3da2af0d31416b9fa8b8d6cdca9940f2b02f0114144b0dd45896609465550`  
		Last Modified: Tue, 27 Jul 2021 02:25:28 GMT  
		Size: 4.7 MB (4676474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894df612b4be55234c3870d52402c8e0f8d862a70d921469dabd90fce65dd19b`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b69804f2417b467f0d90f227007b6ad0784998510b3059db7781646c4d9d7b0`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5140583e1bb4ff168122d517efa0932ee6c515d4c64167423b2c65c7f945120`  
		Last Modified: Tue, 27 Jul 2021 02:27:32 GMT  
		Size: 157.2 MB (157210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b14c8f11163b8fb56261a038b46a4424d6e04e8de12d91373885b3374fedd6`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9b5b88250a972b3fc9a192cdd5c9678df78af943a929029f915130fef85cbe43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205008829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca665cbdb77afab287059cb642a874abc6ffefb94725ad83c3ddf747724e552a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:03:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:03:31 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV ROS_DISTRO=noetic
# Mon, 26 Jul 2021 23:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 23:04:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:04:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d28ea46fe795b56172879ee97757cb6ea98226a43662f62f5bd8e1490c4fb`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1b73a67b1165693bd1ae07bace3301ab4fb82cfe1b5e61e2b536d3e2f75e47`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2161207e597e1e7621916bed37a91d2ed819071ecf81902fa5f9a199d8581048`  
		Last Modified: Mon, 26 Jul 2021 23:20:58 GMT  
		Size: 171.1 MB (171140053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab310c95b66fdb5ac105888d128d19608c8cd336dad6a23a85eee7e7b3a3e8`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:6e3a5b219f3a4a0e75256ba574886e178d4a9b35b4247877e3732193f2cf56a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:01366ef13d56050834f595349bc90ab8ae4359b56eedba140cfcb80ef2a36263
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300381406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:303e70ddcefe851421ed225be4fec71d1d962061c0b5bb14d1228dd5544eca97`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:54:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:54:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 17 Aug 2021 14:54:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Aug 2021 14:54:12 GMT
ENV ROS_DISTRO=noetic
# Tue, 17 Aug 2021 14:55:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:55:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 17 Aug 2021 14:55:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Aug 2021 14:55:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6a25b8c075beb4891f7c9088956d2a452f32036d8126e37217b5b62fd7024c`  
		Last Modified: Tue, 17 Aug 2021 15:02:09 GMT  
		Size: 10.9 MB (10891952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e00b43ac20734a706cb03369661415e15f6856a48275dcd4fe7744b0bde5d23`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b19825ce46253a4664a6e606382250ba22ec8d0e1d13516be7d225efcca57f`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034eef40d3fabaea23b5d4473263a3a6ab8cd3545504c1ba16818b3b90152d1f`  
		Last Modified: Tue, 17 Aug 2021 15:02:50 GMT  
		Size: 239.1 MB (239050839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ae7d371ba1fee4f46bf91b9a18289de1dd3472eb2c3b8458f8ff2df5825c78`  
		Last Modified: Tue, 17 Aug 2021 15:02:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fea064eda565638082f2e8760091f3fda497b0dd13579bbf933c410c8cf59381
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244344453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d1c6cce066e55bcf52b0af531c51e0602c93303ea9c98a7c580faaca63978f3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:48:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:48:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 17 Aug 2021 11:48:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 17 Aug 2021 11:48:59 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 11:48:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 17 Aug 2021 11:49:00 GMT
ENV ROS_DISTRO=noetic
# Tue, 17 Aug 2021 11:49:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:49:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 17 Aug 2021 11:49:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 17 Aug 2021 11:49:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21602f601a18ce34c8a479ae1d7bac4442282478925664d6f67ad1d2b34e020`  
		Last Modified: Tue, 17 Aug 2021 11:56:11 GMT  
		Size: 10.9 MB (10883354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d4e557cfdbdf3a855acc0ae4cb3c204ac63ae1dd071cd42e608dcb0645c2d`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f24119c6422825783e8ee727d9b12a12c7cb5605e9b6e883b5101a388b450a`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd82c4517707ac42892fd33d02b10b53c8eb41cf05683d381df617056c035fd`  
		Last Modified: Tue, 17 Aug 2021 11:56:42 GMT  
		Size: 184.2 MB (184236324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5bbd42e097110d8576baa6d6d16c7a91e608fad20f3b7978c7e0e99f4ee7df`  
		Last Modified: Tue, 17 Aug 2021 11:56:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:1b88921e614ddb5e72223547f89868583789ca5912472f6019cdf7e998248651
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:518d9f49f3956bf92607be0c47a8dbf00d0c567dbb919c607b611e3bcf8c8912
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (212002719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b1740831ef859270de7fd9091d58dda92142f7d3f71df422fb26d0376da185`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 00:48:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 00:48:27 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 00:50:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:50:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 00:50:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 00:50:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997acb5dc01c0a5dcc159471aea13a7b87074a11df83667b1f8b108602e7dda`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5853e486374821ccfc40d07b68affecdc12e88f4ff7e8be0d58d904d3f525d5a`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e9cabb7a6a3ae445854e8bda4e4762b3d7ab26b3191ab8a006360c8dd0689f`  
		Last Modified: Tue, 27 Jul 2021 01:14:29 GMT  
		Size: 176.7 MB (176702826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c5a6e61679ad83770b86fc37c72db8d318a69a8d5dcac2d00db8bf86b0e9fc`  
		Last Modified: Tue, 27 Jul 2021 01:13:50 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:45f08fb5b042970e1b561d9b3940fdabc46b34958678536c54a07e17c3a253cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187137436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a223e481044d9ab0a67a6bad021ae42bd8957c52c4a9357dd2632e569d1594c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:51 GMT
ADD file:dec1b30555f66d79050762dc2b6c8e55dc130245f3bd1af94d77f1e1e6aa3ccb in / 
# Mon, 26 Jul 2021 22:51:52 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:06:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 02:06:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 02:06:30 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 02:06:31 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jul 2021 02:08:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:08:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 27 Jul 2021 02:08:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 02:08:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:84f015b4bc25868153a5ad10fafccf4b87d5e230c6346262a972324d9846c3cb`  
		Last Modified: Mon, 26 Jul 2021 22:56:13 GMT  
		Size: 24.1 MB (24064238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3707933348ed35dee73fe666615c4468caff6e2006136da4acd92e3cc985216d`  
		Last Modified: Tue, 27 Jul 2021 02:25:29 GMT  
		Size: 1.2 MB (1183472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf3da2af0d31416b9fa8b8d6cdca9940f2b02f0114144b0dd45896609465550`  
		Last Modified: Tue, 27 Jul 2021 02:25:28 GMT  
		Size: 4.7 MB (4676474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894df612b4be55234c3870d52402c8e0f8d862a70d921469dabd90fce65dd19b`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b69804f2417b467f0d90f227007b6ad0784998510b3059db7781646c4d9d7b0`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5140583e1bb4ff168122d517efa0932ee6c515d4c64167423b2c65c7f945120`  
		Last Modified: Tue, 27 Jul 2021 02:27:32 GMT  
		Size: 157.2 MB (157210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b14c8f11163b8fb56261a038b46a4424d6e04e8de12d91373885b3374fedd6`  
		Last Modified: Tue, 27 Jul 2021 02:25:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9b5b88250a972b3fc9a192cdd5c9678df78af943a929029f915130fef85cbe43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205008829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca665cbdb77afab287059cb642a874abc6ffefb94725ad83c3ddf747724e552a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:03:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:03:31 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV ROS_DISTRO=noetic
# Mon, 26 Jul 2021 23:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 23:04:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:04:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d28ea46fe795b56172879ee97757cb6ea98226a43662f62f5bd8e1490c4fb`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1b73a67b1165693bd1ae07bace3301ab4fb82cfe1b5e61e2b536d3e2f75e47`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2161207e597e1e7621916bed37a91d2ed819071ecf81902fa5f9a199d8581048`  
		Last Modified: Mon, 26 Jul 2021 23:20:58 GMT  
		Size: 171.1 MB (171140053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab310c95b66fdb5ac105888d128d19608c8cd336dad6a23a85eee7e7b3a3e8`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:7935fab849d955c39f18ff3e464e64212703dbbe03bd2984d1f0a08c338b5648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:343d66d45a2db6917dcf8f2e9e0ecbb0dff0ebe4a10500330d92bd0199c6a8bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.5 MB (232538721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31047f12e16b5886c3a18ae5a9c86ecb487730e1f4d402d208ec8ba461027409`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:07:55 GMT
ENV ROS_DISTRO=rolling
# Tue, 27 Jul 2021 01:08:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:08:39 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:08:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:08:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:09:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:09:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:09:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8928ebb6fc76f821cd15ef57553baa7177425b57b45dca1dc55d1fa7ac567a99`  
		Last Modified: Tue, 27 Jul 2021 01:20:05 GMT  
		Size: 104.0 MB (104037402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87230aa31aac601bd98ed495d1da57881931ef6ba2fd088208ff7edcc11a6645`  
		Last Modified: Tue, 27 Jul 2021 01:19:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecfae6e660eea869e3a4f0b50e02e1f4d59061ecd4f0183ae66f147a79b142`  
		Last Modified: Tue, 27 Jul 2021 01:20:31 GMT  
		Size: 70.8 MB (70796958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9dc0d5adb890f7b8a3773d5280d5a49fc76acb26a178acc8625286d67ffb48`  
		Last Modified: Tue, 27 Jul 2021 01:20:21 GMT  
		Size: 239.9 KB (239910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72269352c197138327479f8993a3f63c4d1e1f551153f8892c4b0e0655b7cda`  
		Last Modified: Tue, 27 Jul 2021 01:20:20 GMT  
		Size: 2.0 KB (2029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164c9e6f758bbce1c98b1b54d6df1e86f651ececc09089ad70ff299c3251599b`  
		Last Modified: Tue, 27 Jul 2021 01:20:24 GMT  
		Size: 22.2 MB (22162528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0cf0917792e1bcb23de7a358622816a44bcdcb55b33f990b0d7c29d4884f0146
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.2 MB (221172399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b31b7302a93a70928eb4e71e4a8d5a333db4a62563ddf1ae569fbfa871152b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:13:18 GMT
ENV ROS_DISTRO=rolling
# Mon, 26 Jul 2021 23:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:01 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:14:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:14:01 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:14:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:14:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e68c4d5b35f3de11859acddc393c58b62b2c31765e4d01cf93e37b40996b1`  
		Last Modified: Mon, 26 Jul 2021 23:27:23 GMT  
		Size: 100.4 MB (100422986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ecefa2ec6d33c2b6ff69008016c9a0a8caca3b3f4696d61c1a3864a132cd7`  
		Last Modified: Mon, 26 Jul 2021 23:27:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466268875e4dd8ad642170e2c1132182e9c266799d18eefce6c20354351aa816`  
		Last Modified: Mon, 26 Jul 2021 23:27:46 GMT  
		Size: 65.1 MB (65137818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60d1728b6b23474a432d8ffaec35473daa09949408fac1589d8a7182f815ac`  
		Last Modified: Mon, 26 Jul 2021 23:27:36 GMT  
		Size: 239.9 KB (239911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114dfbbc3fee7c944f77b2c41db5aca4329fc0bc2e4a994721160762d54ecedd`  
		Last Modified: Mon, 26 Jul 2021 23:27:35 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d260efcfbe512e4fb840d5ea90945601804ede2a216902a171de34573131b`  
		Last Modified: Mon, 26 Jul 2021 23:27:39 GMT  
		Size: 21.5 MB (21500860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:7935fab849d955c39f18ff3e464e64212703dbbe03bd2984d1f0a08c338b5648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:343d66d45a2db6917dcf8f2e9e0ecbb0dff0ebe4a10500330d92bd0199c6a8bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.5 MB (232538721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31047f12e16b5886c3a18ae5a9c86ecb487730e1f4d402d208ec8ba461027409`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:07:55 GMT
ENV ROS_DISTRO=rolling
# Tue, 27 Jul 2021 01:08:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:08:39 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:08:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:08:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:09:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:09:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:09:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8928ebb6fc76f821cd15ef57553baa7177425b57b45dca1dc55d1fa7ac567a99`  
		Last Modified: Tue, 27 Jul 2021 01:20:05 GMT  
		Size: 104.0 MB (104037402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87230aa31aac601bd98ed495d1da57881931ef6ba2fd088208ff7edcc11a6645`  
		Last Modified: Tue, 27 Jul 2021 01:19:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecfae6e660eea869e3a4f0b50e02e1f4d59061ecd4f0183ae66f147a79b142`  
		Last Modified: Tue, 27 Jul 2021 01:20:31 GMT  
		Size: 70.8 MB (70796958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9dc0d5adb890f7b8a3773d5280d5a49fc76acb26a178acc8625286d67ffb48`  
		Last Modified: Tue, 27 Jul 2021 01:20:21 GMT  
		Size: 239.9 KB (239910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72269352c197138327479f8993a3f63c4d1e1f551153f8892c4b0e0655b7cda`  
		Last Modified: Tue, 27 Jul 2021 01:20:20 GMT  
		Size: 2.0 KB (2029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164c9e6f758bbce1c98b1b54d6df1e86f651ececc09089ad70ff299c3251599b`  
		Last Modified: Tue, 27 Jul 2021 01:20:24 GMT  
		Size: 22.2 MB (22162528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0cf0917792e1bcb23de7a358622816a44bcdcb55b33f990b0d7c29d4884f0146
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.2 MB (221172399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b31b7302a93a70928eb4e71e4a8d5a333db4a62563ddf1ae569fbfa871152b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:13:18 GMT
ENV ROS_DISTRO=rolling
# Mon, 26 Jul 2021 23:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:01 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:14:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:14:01 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:14:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:14:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e68c4d5b35f3de11859acddc393c58b62b2c31765e4d01cf93e37b40996b1`  
		Last Modified: Mon, 26 Jul 2021 23:27:23 GMT  
		Size: 100.4 MB (100422986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ecefa2ec6d33c2b6ff69008016c9a0a8caca3b3f4696d61c1a3864a132cd7`  
		Last Modified: Mon, 26 Jul 2021 23:27:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466268875e4dd8ad642170e2c1132182e9c266799d18eefce6c20354351aa816`  
		Last Modified: Mon, 26 Jul 2021 23:27:46 GMT  
		Size: 65.1 MB (65137818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60d1728b6b23474a432d8ffaec35473daa09949408fac1589d8a7182f815ac`  
		Last Modified: Mon, 26 Jul 2021 23:27:36 GMT  
		Size: 239.9 KB (239911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114dfbbc3fee7c944f77b2c41db5aca4329fc0bc2e4a994721160762d54ecedd`  
		Last Modified: Mon, 26 Jul 2021 23:27:35 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d260efcfbe512e4fb840d5ea90945601804ede2a216902a171de34573131b`  
		Last Modified: Mon, 26 Jul 2021 23:27:39 GMT  
		Size: 21.5 MB (21500860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-focal`

```console
$ docker pull ros@sha256:7935fab849d955c39f18ff3e464e64212703dbbe03bd2984d1f0a08c338b5648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:343d66d45a2db6917dcf8f2e9e0ecbb0dff0ebe4a10500330d92bd0199c6a8bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.5 MB (232538721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31047f12e16b5886c3a18ae5a9c86ecb487730e1f4d402d208ec8ba461027409`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:07:55 GMT
ENV ROS_DISTRO=rolling
# Tue, 27 Jul 2021 01:08:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:08:39 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:08:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:08:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:09:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:09:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:09:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8928ebb6fc76f821cd15ef57553baa7177425b57b45dca1dc55d1fa7ac567a99`  
		Last Modified: Tue, 27 Jul 2021 01:20:05 GMT  
		Size: 104.0 MB (104037402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87230aa31aac601bd98ed495d1da57881931ef6ba2fd088208ff7edcc11a6645`  
		Last Modified: Tue, 27 Jul 2021 01:19:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecfae6e660eea869e3a4f0b50e02e1f4d59061ecd4f0183ae66f147a79b142`  
		Last Modified: Tue, 27 Jul 2021 01:20:31 GMT  
		Size: 70.8 MB (70796958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9dc0d5adb890f7b8a3773d5280d5a49fc76acb26a178acc8625286d67ffb48`  
		Last Modified: Tue, 27 Jul 2021 01:20:21 GMT  
		Size: 239.9 KB (239910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72269352c197138327479f8993a3f63c4d1e1f551153f8892c4b0e0655b7cda`  
		Last Modified: Tue, 27 Jul 2021 01:20:20 GMT  
		Size: 2.0 KB (2029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164c9e6f758bbce1c98b1b54d6df1e86f651ececc09089ad70ff299c3251599b`  
		Last Modified: Tue, 27 Jul 2021 01:20:24 GMT  
		Size: 22.2 MB (22162528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0cf0917792e1bcb23de7a358622816a44bcdcb55b33f990b0d7c29d4884f0146
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.2 MB (221172399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b31b7302a93a70928eb4e71e4a8d5a333db4a62563ddf1ae569fbfa871152b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:13:18 GMT
ENV ROS_DISTRO=rolling
# Mon, 26 Jul 2021 23:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:01 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:14:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:14:01 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:14:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:14:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e68c4d5b35f3de11859acddc393c58b62b2c31765e4d01cf93e37b40996b1`  
		Last Modified: Mon, 26 Jul 2021 23:27:23 GMT  
		Size: 100.4 MB (100422986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ecefa2ec6d33c2b6ff69008016c9a0a8caca3b3f4696d61c1a3864a132cd7`  
		Last Modified: Mon, 26 Jul 2021 23:27:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466268875e4dd8ad642170e2c1132182e9c266799d18eefce6c20354351aa816`  
		Last Modified: Mon, 26 Jul 2021 23:27:46 GMT  
		Size: 65.1 MB (65137818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60d1728b6b23474a432d8ffaec35473daa09949408fac1589d8a7182f815ac`  
		Last Modified: Mon, 26 Jul 2021 23:27:36 GMT  
		Size: 239.9 KB (239911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114dfbbc3fee7c944f77b2c41db5aca4329fc0bc2e4a994721160762d54ecedd`  
		Last Modified: Mon, 26 Jul 2021 23:27:35 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d260efcfbe512e4fb840d5ea90945601804ede2a216902a171de34573131b`  
		Last Modified: Mon, 26 Jul 2021 23:27:39 GMT  
		Size: 21.5 MB (21500860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:5c9fb07c581faf2f9cc8e3cec49fbe4eaa56b9e9b718e3a402afc6b99cb63327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:c2f8c1fbe1b3dc3d98c532d7797036db90c409e648e473cc21cfba41bb97c834
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139337296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddaef19d5f6bebf29770911fea7c2a2377a782d34649acf780095cc1ce3b1f9c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:07:55 GMT
ENV ROS_DISTRO=rolling
# Tue, 27 Jul 2021 01:08:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:08:39 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:08:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:08:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8928ebb6fc76f821cd15ef57553baa7177425b57b45dca1dc55d1fa7ac567a99`  
		Last Modified: Tue, 27 Jul 2021 01:20:05 GMT  
		Size: 104.0 MB (104037402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87230aa31aac601bd98ed495d1da57881931ef6ba2fd088208ff7edcc11a6645`  
		Last Modified: Tue, 27 Jul 2021 01:19:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:151a24b40fe37d9652a6bd52c35a9bc0422139e6c777676a96131e17e500abd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134291759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa58646678d36f39b5ffb71a2ee469599a65598d4f965b6d6fc8a2b44f675fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:13:18 GMT
ENV ROS_DISTRO=rolling
# Mon, 26 Jul 2021 23:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:01 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:14:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:14:01 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e68c4d5b35f3de11859acddc393c58b62b2c31765e4d01cf93e37b40996b1`  
		Last Modified: Mon, 26 Jul 2021 23:27:23 GMT  
		Size: 100.4 MB (100422986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ecefa2ec6d33c2b6ff69008016c9a0a8caca3b3f4696d61c1a3864a132cd7`  
		Last Modified: Mon, 26 Jul 2021 23:27:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-focal`

```console
$ docker pull ros@sha256:5c9fb07c581faf2f9cc8e3cec49fbe4eaa56b9e9b718e3a402afc6b99cb63327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:c2f8c1fbe1b3dc3d98c532d7797036db90c409e648e473cc21cfba41bb97c834
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139337296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddaef19d5f6bebf29770911fea7c2a2377a782d34649acf780095cc1ce3b1f9c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:07:55 GMT
ENV ROS_DISTRO=rolling
# Tue, 27 Jul 2021 01:08:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:08:39 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:08:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:08:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8928ebb6fc76f821cd15ef57553baa7177425b57b45dca1dc55d1fa7ac567a99`  
		Last Modified: Tue, 27 Jul 2021 01:20:05 GMT  
		Size: 104.0 MB (104037402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87230aa31aac601bd98ed495d1da57881931ef6ba2fd088208ff7edcc11a6645`  
		Last Modified: Tue, 27 Jul 2021 01:19:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:151a24b40fe37d9652a6bd52c35a9bc0422139e6c777676a96131e17e500abd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134291759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa58646678d36f39b5ffb71a2ee469599a65598d4f965b6d6fc8a2b44f675fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:13:18 GMT
ENV ROS_DISTRO=rolling
# Mon, 26 Jul 2021 23:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:01 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:14:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:14:01 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e68c4d5b35f3de11859acddc393c58b62b2c31765e4d01cf93e37b40996b1`  
		Last Modified: Mon, 26 Jul 2021 23:27:23 GMT  
		Size: 100.4 MB (100422986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ecefa2ec6d33c2b6ff69008016c9a0a8caca3b3f4696d61c1a3864a132cd7`  
		Last Modified: Mon, 26 Jul 2021 23:27:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge`

```console
$ docker pull ros@sha256:990cc51d99701897f01c29dfc020f6a00c81ec0ae3f7ab7191c9e925a401fbb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:0419b55655a8a9788ef62f230ba0c5c0995210c7324d7219d9cb4e74f318bb77
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.0 MB (326047946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b68d462b62bcab867a18dd90da22c7a31a8a05a81712003a2346f4272d9f4fb7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:07:55 GMT
ENV ROS_DISTRO=rolling
# Tue, 27 Jul 2021 01:08:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:08:39 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:08:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:08:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:09:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:09:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:09:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:09:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:09:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:09:39 GMT
ENV ROS1_DISTRO=noetic
# Tue, 27 Jul 2021 01:09:39 GMT
ENV ROS2_DISTRO=rolling
# Tue, 27 Jul 2021 01:10:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:10:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.15.0-1*     ros-rolling-demo-nodes-py=0.15.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:10:15 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8928ebb6fc76f821cd15ef57553baa7177425b57b45dca1dc55d1fa7ac567a99`  
		Last Modified: Tue, 27 Jul 2021 01:20:05 GMT  
		Size: 104.0 MB (104037402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87230aa31aac601bd98ed495d1da57881931ef6ba2fd088208ff7edcc11a6645`  
		Last Modified: Tue, 27 Jul 2021 01:19:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecfae6e660eea869e3a4f0b50e02e1f4d59061ecd4f0183ae66f147a79b142`  
		Last Modified: Tue, 27 Jul 2021 01:20:31 GMT  
		Size: 70.8 MB (70796958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9dc0d5adb890f7b8a3773d5280d5a49fc76acb26a178acc8625286d67ffb48`  
		Last Modified: Tue, 27 Jul 2021 01:20:21 GMT  
		Size: 239.9 KB (239910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72269352c197138327479f8993a3f63c4d1e1f551153f8892c4b0e0655b7cda`  
		Last Modified: Tue, 27 Jul 2021 01:20:20 GMT  
		Size: 2.0 KB (2029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164c9e6f758bbce1c98b1b54d6df1e86f651ececc09089ad70ff299c3251599b`  
		Last Modified: Tue, 27 Jul 2021 01:20:24 GMT  
		Size: 22.2 MB (22162528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b7e5b68d937de167626e1fbf8f8aa89e0b98f223f92214e751b6bc93ac02ae`  
		Last Modified: Tue, 27 Jul 2021 01:20:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae277910ca8875daebb4c39ac8f951db856449b3de053bc5fd2b5823c5ee57b6`  
		Last Modified: Tue, 27 Jul 2021 01:20:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f022dbe32fe832b14ad9e12583044b8108dcef7b9a90ffdbe21c579aa88700df`  
		Last Modified: Tue, 27 Jul 2021 01:21:00 GMT  
		Size: 78.4 MB (78413507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81921727929ab00ed80fb90e17e0e83df6fedf858d8a2addc82b2ae712ee73c1`  
		Last Modified: Tue, 27 Jul 2021 01:20:49 GMT  
		Size: 15.1 MB (15095090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1189306f1356224513996d689a685113a9dedeee1a681978f8fd363a6c0c44`  
		Last Modified: Tue, 27 Jul 2021 01:20:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f1250cc8adbb1af04bfa1609832656cee28a8356680f564729f5eb2a6fb7a299
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.2 MB (314248509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b02289d93836ace703f870dfbceb86842ef410a8cddbd8dbdfa258e700a13bf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:13:18 GMT
ENV ROS_DISTRO=rolling
# Mon, 26 Jul 2021 23:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:01 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:14:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:14:01 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:14:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:14:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:15:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:15:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:15:04 GMT
ENV ROS1_DISTRO=noetic
# Mon, 26 Jul 2021 23:15:04 GMT
ENV ROS2_DISTRO=rolling
# Mon, 26 Jul 2021 23:15:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 21 Aug 2021 00:47:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.16.0-1*     ros-rolling-demo-nodes-py=0.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 21 Aug 2021 00:47:18 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e68c4d5b35f3de11859acddc393c58b62b2c31765e4d01cf93e37b40996b1`  
		Last Modified: Mon, 26 Jul 2021 23:27:23 GMT  
		Size: 100.4 MB (100422986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ecefa2ec6d33c2b6ff69008016c9a0a8caca3b3f4696d61c1a3864a132cd7`  
		Last Modified: Mon, 26 Jul 2021 23:27:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466268875e4dd8ad642170e2c1132182e9c266799d18eefce6c20354351aa816`  
		Last Modified: Mon, 26 Jul 2021 23:27:46 GMT  
		Size: 65.1 MB (65137818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60d1728b6b23474a432d8ffaec35473daa09949408fac1589d8a7182f815ac`  
		Last Modified: Mon, 26 Jul 2021 23:27:36 GMT  
		Size: 239.9 KB (239911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114dfbbc3fee7c944f77b2c41db5aca4329fc0bc2e4a994721160762d54ecedd`  
		Last Modified: Mon, 26 Jul 2021 23:27:35 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d260efcfbe512e4fb840d5ea90945601804ede2a216902a171de34573131b`  
		Last Modified: Mon, 26 Jul 2021 23:27:39 GMT  
		Size: 21.5 MB (21500860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2268c306b1f6a009ee0c79d6c1944981ed7dcd117e4e2097ae6bb68699573a`  
		Last Modified: Mon, 26 Jul 2021 23:28:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff82791f9fea2e59a2957e9d5aab45bf09b288a72892251ab9de125d71194c9c`  
		Last Modified: Mon, 26 Jul 2021 23:28:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a209440aeee45f4c1770fcbdde5de1d5c53a624af51ca0ab250d77e8d20c2767`  
		Last Modified: Mon, 26 Jul 2021 23:28:21 GMT  
		Size: 78.4 MB (78370885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fb53b43a27675601a6fd0fdf8bc19718d53ef84cc49756dec43c8b73c6d330`  
		Last Modified: Sat, 21 Aug 2021 00:49:39 GMT  
		Size: 14.7 MB (14704601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ec5035f5b4e3519133a2ea30b97d2599a7493c1dd926d6eaa32c5f564f755c`  
		Last Modified: Sat, 21 Aug 2021 00:49:36 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:990cc51d99701897f01c29dfc020f6a00c81ec0ae3f7ab7191c9e925a401fbb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:0419b55655a8a9788ef62f230ba0c5c0995210c7324d7219d9cb4e74f318bb77
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.0 MB (326047946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b68d462b62bcab867a18dd90da22c7a31a8a05a81712003a2346f4272d9f4fb7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:48:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:02:06 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 27 Jul 2021 01:02:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jul 2021 01:02:08 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jul 2021 01:07:55 GMT
ENV ROS_DISTRO=rolling
# Tue, 27 Jul 2021 01:08:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:08:39 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 27 Jul 2021 01:08:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jul 2021 01:08:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:09:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 27 Jul 2021 01:09:12 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 27 Jul 2021 01:09:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:09:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 27 Jul 2021 01:09:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 27 Jul 2021 01:09:39 GMT
ENV ROS1_DISTRO=noetic
# Tue, 27 Jul 2021 01:09:39 GMT
ENV ROS2_DISTRO=rolling
# Tue, 27 Jul 2021 01:10:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:10:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.15.0-1*     ros-rolling-demo-nodes-py=0.15.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:10:15 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39deaaa7423e6ef1165a73155147eae3a10e676ec72379e083d81881a0aed170`  
		Last Modified: Tue, 27 Jul 2021 01:13:51 GMT  
		Size: 5.5 MB (5547062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa09dd913f1251e30dc9e89af3583ddb796558251c0aa59b8fccabd59fc11ed0`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d4b7162625d29326104f879225ff200e77afe83b35bca9f42e7e26f4894ce2`  
		Last Modified: Tue, 27 Jul 2021 01:16:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8928ebb6fc76f821cd15ef57553baa7177425b57b45dca1dc55d1fa7ac567a99`  
		Last Modified: Tue, 27 Jul 2021 01:20:05 GMT  
		Size: 104.0 MB (104037402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87230aa31aac601bd98ed495d1da57881931ef6ba2fd088208ff7edcc11a6645`  
		Last Modified: Tue, 27 Jul 2021 01:19:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecfae6e660eea869e3a4f0b50e02e1f4d59061ecd4f0183ae66f147a79b142`  
		Last Modified: Tue, 27 Jul 2021 01:20:31 GMT  
		Size: 70.8 MB (70796958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9dc0d5adb890f7b8a3773d5280d5a49fc76acb26a178acc8625286d67ffb48`  
		Last Modified: Tue, 27 Jul 2021 01:20:21 GMT  
		Size: 239.9 KB (239910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72269352c197138327479f8993a3f63c4d1e1f551153f8892c4b0e0655b7cda`  
		Last Modified: Tue, 27 Jul 2021 01:20:20 GMT  
		Size: 2.0 KB (2029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164c9e6f758bbce1c98b1b54d6df1e86f651ececc09089ad70ff299c3251599b`  
		Last Modified: Tue, 27 Jul 2021 01:20:24 GMT  
		Size: 22.2 MB (22162528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b7e5b68d937de167626e1fbf8f8aa89e0b98f223f92214e751b6bc93ac02ae`  
		Last Modified: Tue, 27 Jul 2021 01:20:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae277910ca8875daebb4c39ac8f951db856449b3de053bc5fd2b5823c5ee57b6`  
		Last Modified: Tue, 27 Jul 2021 01:20:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f022dbe32fe832b14ad9e12583044b8108dcef7b9a90ffdbe21c579aa88700df`  
		Last Modified: Tue, 27 Jul 2021 01:21:00 GMT  
		Size: 78.4 MB (78413507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81921727929ab00ed80fb90e17e0e83df6fedf858d8a2addc82b2ae712ee73c1`  
		Last Modified: Tue, 27 Jul 2021 01:20:49 GMT  
		Size: 15.1 MB (15095090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1189306f1356224513996d689a685113a9dedeee1a681978f8fd363a6c0c44`  
		Last Modified: Tue, 27 Jul 2021 01:20:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f1250cc8adbb1af04bfa1609832656cee28a8356680f564729f5eb2a6fb7a299
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.2 MB (314248509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b02289d93836ace703f870dfbceb86842ef410a8cddbd8dbdfa258e700a13bf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:08:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 26 Jul 2021 23:08:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:08:17 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:13:18 GMT
ENV ROS_DISTRO=rolling
# Mon, 26 Jul 2021 23:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:01 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 26 Jul 2021 23:14:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:14:01 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:14:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:14:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:14:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 26 Jul 2021 23:14:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:15:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:15:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:15:04 GMT
ENV ROS1_DISTRO=noetic
# Mon, 26 Jul 2021 23:15:04 GMT
ENV ROS2_DISTRO=rolling
# Mon, 26 Jul 2021 23:15:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 21 Aug 2021 00:47:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.16.0-1*     ros-rolling-demo-nodes-py=0.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 21 Aug 2021 00:47:18 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145ea28ffd9b0942ba98116cde1e498e4572f6c665186683366584a32a0a9c0`  
		Last Modified: Mon, 26 Jul 2021 23:23:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb0e59f8a1856416b541915263ab8419535ec407203cdedec71cee7983a4f28`  
		Last Modified: Mon, 26 Jul 2021 23:23:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e68c4d5b35f3de11859acddc393c58b62b2c31765e4d01cf93e37b40996b1`  
		Last Modified: Mon, 26 Jul 2021 23:27:23 GMT  
		Size: 100.4 MB (100422986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ecefa2ec6d33c2b6ff69008016c9a0a8caca3b3f4696d61c1a3864a132cd7`  
		Last Modified: Mon, 26 Jul 2021 23:27:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466268875e4dd8ad642170e2c1132182e9c266799d18eefce6c20354351aa816`  
		Last Modified: Mon, 26 Jul 2021 23:27:46 GMT  
		Size: 65.1 MB (65137818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60d1728b6b23474a432d8ffaec35473daa09949408fac1589d8a7182f815ac`  
		Last Modified: Mon, 26 Jul 2021 23:27:36 GMT  
		Size: 239.9 KB (239911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114dfbbc3fee7c944f77b2c41db5aca4329fc0bc2e4a994721160762d54ecedd`  
		Last Modified: Mon, 26 Jul 2021 23:27:35 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d260efcfbe512e4fb840d5ea90945601804ede2a216902a171de34573131b`  
		Last Modified: Mon, 26 Jul 2021 23:27:39 GMT  
		Size: 21.5 MB (21500860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2268c306b1f6a009ee0c79d6c1944981ed7dcd117e4e2097ae6bb68699573a`  
		Last Modified: Mon, 26 Jul 2021 23:28:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff82791f9fea2e59a2957e9d5aab45bf09b288a72892251ab9de125d71194c9c`  
		Last Modified: Mon, 26 Jul 2021 23:28:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a209440aeee45f4c1770fcbdde5de1d5c53a624af51ca0ab250d77e8d20c2767`  
		Last Modified: Mon, 26 Jul 2021 23:28:21 GMT  
		Size: 78.4 MB (78370885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fb53b43a27675601a6fd0fdf8bc19718d53ef84cc49756dec43c8b73c6d330`  
		Last Modified: Sat, 21 Aug 2021 00:49:39 GMT  
		Size: 14.7 MB (14704601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ec5035f5b4e3519133a2ea30b97d2599a7493c1dd926d6eaa32c5f564f755c`  
		Last Modified: Sat, 21 Aug 2021 00:49:36 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
