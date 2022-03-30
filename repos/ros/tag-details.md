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
-	[`ros:rolling-ros-base-jammy`](#rosrolling-ros-base-jammy)
-	[`ros:rolling-ros-core`](#rosrolling-ros-core)
-	[`ros:rolling-ros-core-jammy`](#rosrolling-ros-core-jammy)

## `ros:foxy`

```console
$ docker pull ros@sha256:953899ce6b949c54ee4f76b15544e7fe139ca18319918f52044500237a864111
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:6b54889f363f92aa82ba6d57fa2c9ba0282de112b34eb933312d21983bf4796b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.9 MB (251867339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f54dd2b563ff4744848ca4cdc779b8ba16e96de3347a5d1c4d87cee6331a759b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 09:45:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:45:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:45:25 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:46:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:46:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:46:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:48:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e204965e59bcbf7ac6d87e13bc92ef5e16b1febf5872f402cad9056a770eba`  
		Last Modified: Fri, 18 Mar 2022 10:08:19 GMT  
		Size: 120.1 MB (120106779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2245accfb94d1ebb93d93f6d4680ae8e6fdea2b5571488a29f4642a49dc78d`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53c3ddd926cb4541eb970996c216deb7494ef199dbf5544a4c38c7ca9ce16b`  
		Last Modified: Fri, 18 Mar 2022 10:08:42 GMT  
		Size: 74.5 MB (74540409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c02732d82eb8528fc555a48b7b1f45939a4ce4c459dc35ffdab76db7a83321`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 251.9 KB (251854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3497504cc85c709ec7a661dbbde807899724d862b2b3c081fccd043de7b0e`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 2.2 KB (2197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b7a10bbe20d65fb6e10bcf4e2ad26de3d74467d7f9cbf4db8627f9670c1e2`  
		Last Modified: Fri, 18 Mar 2022 10:08:34 GMT  
		Size: 21.7 MB (21668774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c0271da37734c7bee2bf52ddacbad34cd3e75cb75452e856920d29abcaf8abac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227246060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cfb281669b65d5d519f1be680712daf507fed215f1d8d13f1a58d8a0bb9b6fa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:07:24 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 01:08:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:08:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:08:16 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:08:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:08:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a14b2daae663639c39577d0c7d4593bd5574bd84d8cc4eab597182dda98e14`  
		Last Modified: Fri, 18 Mar 2022 01:27:06 GMT  
		Size: 104.3 MB (104279184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc8ed32f6736949944b94d4d4616553dd4b8a76e9a9660f4521a62ac4284d7`  
		Last Modified: Fri, 18 Mar 2022 01:26:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bb58734c528dbf439eb6fd5f41bad51b1219ef59cbbb4aa9249f1b7ee7b776`  
		Last Modified: Fri, 18 Mar 2022 01:27:30 GMT  
		Size: 68.7 MB (68660506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f928dc74080d0875487138c18b5be16c28fb8eebeaca7cd7ff43e5c053bcf30`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 251.8 KB (251796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2de71e5cdcb594ee0949c5bd975f379ad91d9be834a96504a4506e12cdc8e6`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 2.1 KB (2136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0525ce65e691fa28b8277972d7bacd7427660a270de514d249fd213d63d36a`  
		Last Modified: Fri, 18 Mar 2022 01:27:21 GMT  
		Size: 20.4 MB (20373802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:953899ce6b949c54ee4f76b15544e7fe139ca18319918f52044500237a864111
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:6b54889f363f92aa82ba6d57fa2c9ba0282de112b34eb933312d21983bf4796b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.9 MB (251867339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f54dd2b563ff4744848ca4cdc779b8ba16e96de3347a5d1c4d87cee6331a759b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 09:45:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:45:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:45:25 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:46:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:46:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:46:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:48:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e204965e59bcbf7ac6d87e13bc92ef5e16b1febf5872f402cad9056a770eba`  
		Last Modified: Fri, 18 Mar 2022 10:08:19 GMT  
		Size: 120.1 MB (120106779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2245accfb94d1ebb93d93f6d4680ae8e6fdea2b5571488a29f4642a49dc78d`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53c3ddd926cb4541eb970996c216deb7494ef199dbf5544a4c38c7ca9ce16b`  
		Last Modified: Fri, 18 Mar 2022 10:08:42 GMT  
		Size: 74.5 MB (74540409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c02732d82eb8528fc555a48b7b1f45939a4ce4c459dc35ffdab76db7a83321`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 251.9 KB (251854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3497504cc85c709ec7a661dbbde807899724d862b2b3c081fccd043de7b0e`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 2.2 KB (2197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b7a10bbe20d65fb6e10bcf4e2ad26de3d74467d7f9cbf4db8627f9670c1e2`  
		Last Modified: Fri, 18 Mar 2022 10:08:34 GMT  
		Size: 21.7 MB (21668774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c0271da37734c7bee2bf52ddacbad34cd3e75cb75452e856920d29abcaf8abac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227246060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cfb281669b65d5d519f1be680712daf507fed215f1d8d13f1a58d8a0bb9b6fa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:07:24 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 01:08:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:08:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:08:16 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:08:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:08:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a14b2daae663639c39577d0c7d4593bd5574bd84d8cc4eab597182dda98e14`  
		Last Modified: Fri, 18 Mar 2022 01:27:06 GMT  
		Size: 104.3 MB (104279184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc8ed32f6736949944b94d4d4616553dd4b8a76e9a9660f4521a62ac4284d7`  
		Last Modified: Fri, 18 Mar 2022 01:26:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bb58734c528dbf439eb6fd5f41bad51b1219ef59cbbb4aa9249f1b7ee7b776`  
		Last Modified: Fri, 18 Mar 2022 01:27:30 GMT  
		Size: 68.7 MB (68660506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f928dc74080d0875487138c18b5be16c28fb8eebeaca7cd7ff43e5c053bcf30`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 251.8 KB (251796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2de71e5cdcb594ee0949c5bd975f379ad91d9be834a96504a4506e12cdc8e6`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 2.1 KB (2136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0525ce65e691fa28b8277972d7bacd7427660a270de514d249fd213d63d36a`  
		Last Modified: Fri, 18 Mar 2022 01:27:21 GMT  
		Size: 20.4 MB (20373802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:953899ce6b949c54ee4f76b15544e7fe139ca18319918f52044500237a864111
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:6b54889f363f92aa82ba6d57fa2c9ba0282de112b34eb933312d21983bf4796b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.9 MB (251867339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f54dd2b563ff4744848ca4cdc779b8ba16e96de3347a5d1c4d87cee6331a759b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 09:45:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:45:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:45:25 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:46:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:46:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:46:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:48:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e204965e59bcbf7ac6d87e13bc92ef5e16b1febf5872f402cad9056a770eba`  
		Last Modified: Fri, 18 Mar 2022 10:08:19 GMT  
		Size: 120.1 MB (120106779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2245accfb94d1ebb93d93f6d4680ae8e6fdea2b5571488a29f4642a49dc78d`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53c3ddd926cb4541eb970996c216deb7494ef199dbf5544a4c38c7ca9ce16b`  
		Last Modified: Fri, 18 Mar 2022 10:08:42 GMT  
		Size: 74.5 MB (74540409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c02732d82eb8528fc555a48b7b1f45939a4ce4c459dc35ffdab76db7a83321`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 251.9 KB (251854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3497504cc85c709ec7a661dbbde807899724d862b2b3c081fccd043de7b0e`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 2.2 KB (2197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b7a10bbe20d65fb6e10bcf4e2ad26de3d74467d7f9cbf4db8627f9670c1e2`  
		Last Modified: Fri, 18 Mar 2022 10:08:34 GMT  
		Size: 21.7 MB (21668774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c0271da37734c7bee2bf52ddacbad34cd3e75cb75452e856920d29abcaf8abac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227246060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cfb281669b65d5d519f1be680712daf507fed215f1d8d13f1a58d8a0bb9b6fa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:07:24 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 01:08:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:08:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:08:16 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:08:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:08:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a14b2daae663639c39577d0c7d4593bd5574bd84d8cc4eab597182dda98e14`  
		Last Modified: Fri, 18 Mar 2022 01:27:06 GMT  
		Size: 104.3 MB (104279184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc8ed32f6736949944b94d4d4616553dd4b8a76e9a9660f4521a62ac4284d7`  
		Last Modified: Fri, 18 Mar 2022 01:26:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bb58734c528dbf439eb6fd5f41bad51b1219ef59cbbb4aa9249f1b7ee7b776`  
		Last Modified: Fri, 18 Mar 2022 01:27:30 GMT  
		Size: 68.7 MB (68660506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f928dc74080d0875487138c18b5be16c28fb8eebeaca7cd7ff43e5c053bcf30`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 251.8 KB (251796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2de71e5cdcb594ee0949c5bd975f379ad91d9be834a96504a4506e12cdc8e6`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 2.1 KB (2136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0525ce65e691fa28b8277972d7bacd7427660a270de514d249fd213d63d36a`  
		Last Modified: Fri, 18 Mar 2022 01:27:21 GMT  
		Size: 20.4 MB (20373802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:f8a692514ddeafb042cab1040b24408cc2848d275b07b1143443e478d90f9ea9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:a353bad30f8e54502cc96e16d462326b862847aa23630e7ddc7d121e821e4fca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155404105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9136fbb6b27e41689557a6626287d8f3f371ec167b6e1292bc2ba9563d63a476`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 09:45:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:45:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:45:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e204965e59bcbf7ac6d87e13bc92ef5e16b1febf5872f402cad9056a770eba`  
		Last Modified: Fri, 18 Mar 2022 10:08:19 GMT  
		Size: 120.1 MB (120106779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2245accfb94d1ebb93d93f6d4680ae8e6fdea2b5571488a29f4642a49dc78d`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b4dc5ec86bf2af3696454731bfc6c559bc343b735836d8efef7cb858a96c15a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137957820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff29475e76a48b7f1b893c8ff1e2b84e0e46b1807173ed062e1f6ae865bab39`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:07:24 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 01:08:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:08:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:08:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a14b2daae663639c39577d0c7d4593bd5574bd84d8cc4eab597182dda98e14`  
		Last Modified: Fri, 18 Mar 2022 01:27:06 GMT  
		Size: 104.3 MB (104279184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc8ed32f6736949944b94d4d4616553dd4b8a76e9a9660f4521a62ac4284d7`  
		Last Modified: Fri, 18 Mar 2022 01:26:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:f8a692514ddeafb042cab1040b24408cc2848d275b07b1143443e478d90f9ea9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:a353bad30f8e54502cc96e16d462326b862847aa23630e7ddc7d121e821e4fca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155404105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9136fbb6b27e41689557a6626287d8f3f371ec167b6e1292bc2ba9563d63a476`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 09:45:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:45:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:45:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e204965e59bcbf7ac6d87e13bc92ef5e16b1febf5872f402cad9056a770eba`  
		Last Modified: Fri, 18 Mar 2022 10:08:19 GMT  
		Size: 120.1 MB (120106779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2245accfb94d1ebb93d93f6d4680ae8e6fdea2b5571488a29f4642a49dc78d`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b4dc5ec86bf2af3696454731bfc6c559bc343b735836d8efef7cb858a96c15a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137957820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff29475e76a48b7f1b893c8ff1e2b84e0e46b1807173ed062e1f6ae865bab39`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:07:24 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 01:08:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:08:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:08:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a14b2daae663639c39577d0c7d4593bd5574bd84d8cc4eab597182dda98e14`  
		Last Modified: Fri, 18 Mar 2022 01:27:06 GMT  
		Size: 104.3 MB (104279184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc8ed32f6736949944b94d4d4616553dd4b8a76e9a9660f4521a62ac4284d7`  
		Last Modified: Fri, 18 Mar 2022 01:26:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:dc8d0052b78ff87bf1cfa606cf03a31f8323c84876e81147ceecb4f2f2eedf72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:c00dbaf51811aeaf33e7471577a329f2ad4c2b5c8bbc3c60471e3fd7678b8c86
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.7 MB (349736548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e4dc13f54f411e6a139b68cb24830a0240035e64ef36776ede46349591e350`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 09:45:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:45:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:45:25 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:46:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:46:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:46:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:48:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:48:17 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:48:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:48:56 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Mar 2022 09:48:56 GMT
ENV ROS2_DISTRO=foxy
# Fri, 18 Mar 2022 09:50:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:50:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:50:27 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e204965e59bcbf7ac6d87e13bc92ef5e16b1febf5872f402cad9056a770eba`  
		Last Modified: Fri, 18 Mar 2022 10:08:19 GMT  
		Size: 120.1 MB (120106779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2245accfb94d1ebb93d93f6d4680ae8e6fdea2b5571488a29f4642a49dc78d`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53c3ddd926cb4541eb970996c216deb7494ef199dbf5544a4c38c7ca9ce16b`  
		Last Modified: Fri, 18 Mar 2022 10:08:42 GMT  
		Size: 74.5 MB (74540409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c02732d82eb8528fc555a48b7b1f45939a4ce4c459dc35ffdab76db7a83321`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 251.9 KB (251854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3497504cc85c709ec7a661dbbde807899724d862b2b3c081fccd043de7b0e`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 2.2 KB (2197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b7a10bbe20d65fb6e10bcf4e2ad26de3d74467d7f9cbf4db8627f9670c1e2`  
		Last Modified: Fri, 18 Mar 2022 10:08:34 GMT  
		Size: 21.7 MB (21668774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a201d00bc5263b947d0fc44bb870fe573de77e6026e258a194b52461ad70a2`  
		Last Modified: Fri, 18 Mar 2022 10:08:58 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed58bb0f25378323611dafd662ef4f33a85e10f764c28c39780565c8e6b7dfcc`  
		Last Modified: Fri, 18 Mar 2022 10:08:58 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d459e7221888437c2f3cf6c11744fef7cacbcffcd8c9f5b7d3863f86fd10b5`  
		Last Modified: Fri, 18 Mar 2022 10:09:18 GMT  
		Size: 76.3 MB (76324415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c2444e4d9e592a8e420f188bb86eb9f4f88cda249f4a4ecaa6cc5f8e2985d3`  
		Last Modified: Fri, 18 Mar 2022 10:09:04 GMT  
		Size: 21.5 MB (21544171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177d6d418fd69b23f5ac6d83fd7ad2cb72bcd7423eb7dc7629d3d74816584912`  
		Last Modified: Fri, 18 Mar 2022 10:08:58 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a1efd9981157111a468345b39dbdaa22229735fc859c71de45555cf595dfab59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.4 MB (317366822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cfe8df067c0062bb8e8927bc18896ce0afa9e9970f95e9fec3235f97b55d902`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:07:24 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 01:08:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:08:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:08:16 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:08:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:08:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:09:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 01:09:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:09:27 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Mar 2022 01:09:28 GMT
ENV ROS2_DISTRO=foxy
# Fri, 18 Mar 2022 01:09:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:10:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:10:35 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a14b2daae663639c39577d0c7d4593bd5574bd84d8cc4eab597182dda98e14`  
		Last Modified: Fri, 18 Mar 2022 01:27:06 GMT  
		Size: 104.3 MB (104279184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc8ed32f6736949944b94d4d4616553dd4b8a76e9a9660f4521a62ac4284d7`  
		Last Modified: Fri, 18 Mar 2022 01:26:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bb58734c528dbf439eb6fd5f41bad51b1219ef59cbbb4aa9249f1b7ee7b776`  
		Last Modified: Fri, 18 Mar 2022 01:27:30 GMT  
		Size: 68.7 MB (68660506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f928dc74080d0875487138c18b5be16c28fb8eebeaca7cd7ff43e5c053bcf30`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 251.8 KB (251796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2de71e5cdcb594ee0949c5bd975f379ad91d9be834a96504a4506e12cdc8e6`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 2.1 KB (2136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0525ce65e691fa28b8277972d7bacd7427660a270de514d249fd213d63d36a`  
		Last Modified: Fri, 18 Mar 2022 01:27:21 GMT  
		Size: 20.4 MB (20373802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad24ecbe9c7efb4897ead8256b5de51aaa70a6975457b5308234934d3eccbe6`  
		Last Modified: Fri, 18 Mar 2022 01:27:59 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ac548bf3515cbca7c930a68cb952494ac153c33c757588e9870a42bbeb2e03`  
		Last Modified: Fri, 18 Mar 2022 01:28:14 GMT  
		Size: 76.2 MB (76155220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce527927efa348d31fb039bc094edfddc20602790341fc2b0697eba09ce3ea6`  
		Last Modified: Fri, 18 Mar 2022 01:28:01 GMT  
		Size: 14.0 MB (13965074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b59f779d25f18d3f09e480bc05f31d9588066a82bc187dc74545a38266c985d`  
		Last Modified: Fri, 18 Mar 2022 01:27:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:dc8d0052b78ff87bf1cfa606cf03a31f8323c84876e81147ceecb4f2f2eedf72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:c00dbaf51811aeaf33e7471577a329f2ad4c2b5c8bbc3c60471e3fd7678b8c86
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.7 MB (349736548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e4dc13f54f411e6a139b68cb24830a0240035e64ef36776ede46349591e350`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 09:45:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:45:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:45:25 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:46:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:46:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:46:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:48:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:48:17 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:48:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:48:56 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Mar 2022 09:48:56 GMT
ENV ROS2_DISTRO=foxy
# Fri, 18 Mar 2022 09:50:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:50:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:50:27 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e204965e59bcbf7ac6d87e13bc92ef5e16b1febf5872f402cad9056a770eba`  
		Last Modified: Fri, 18 Mar 2022 10:08:19 GMT  
		Size: 120.1 MB (120106779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2245accfb94d1ebb93d93f6d4680ae8e6fdea2b5571488a29f4642a49dc78d`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53c3ddd926cb4541eb970996c216deb7494ef199dbf5544a4c38c7ca9ce16b`  
		Last Modified: Fri, 18 Mar 2022 10:08:42 GMT  
		Size: 74.5 MB (74540409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c02732d82eb8528fc555a48b7b1f45939a4ce4c459dc35ffdab76db7a83321`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 251.9 KB (251854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3497504cc85c709ec7a661dbbde807899724d862b2b3c081fccd043de7b0e`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 2.2 KB (2197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b7a10bbe20d65fb6e10bcf4e2ad26de3d74467d7f9cbf4db8627f9670c1e2`  
		Last Modified: Fri, 18 Mar 2022 10:08:34 GMT  
		Size: 21.7 MB (21668774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a201d00bc5263b947d0fc44bb870fe573de77e6026e258a194b52461ad70a2`  
		Last Modified: Fri, 18 Mar 2022 10:08:58 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed58bb0f25378323611dafd662ef4f33a85e10f764c28c39780565c8e6b7dfcc`  
		Last Modified: Fri, 18 Mar 2022 10:08:58 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d459e7221888437c2f3cf6c11744fef7cacbcffcd8c9f5b7d3863f86fd10b5`  
		Last Modified: Fri, 18 Mar 2022 10:09:18 GMT  
		Size: 76.3 MB (76324415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c2444e4d9e592a8e420f188bb86eb9f4f88cda249f4a4ecaa6cc5f8e2985d3`  
		Last Modified: Fri, 18 Mar 2022 10:09:04 GMT  
		Size: 21.5 MB (21544171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177d6d418fd69b23f5ac6d83fd7ad2cb72bcd7423eb7dc7629d3d74816584912`  
		Last Modified: Fri, 18 Mar 2022 10:08:58 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a1efd9981157111a468345b39dbdaa22229735fc859c71de45555cf595dfab59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.4 MB (317366822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cfe8df067c0062bb8e8927bc18896ce0afa9e9970f95e9fec3235f97b55d902`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:07:24 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 01:08:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:08:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:08:16 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:08:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:08:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:09:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 01:09:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:09:27 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Mar 2022 01:09:28 GMT
ENV ROS2_DISTRO=foxy
# Fri, 18 Mar 2022 01:09:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:10:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:10:35 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a14b2daae663639c39577d0c7d4593bd5574bd84d8cc4eab597182dda98e14`  
		Last Modified: Fri, 18 Mar 2022 01:27:06 GMT  
		Size: 104.3 MB (104279184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc8ed32f6736949944b94d4d4616553dd4b8a76e9a9660f4521a62ac4284d7`  
		Last Modified: Fri, 18 Mar 2022 01:26:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bb58734c528dbf439eb6fd5f41bad51b1219ef59cbbb4aa9249f1b7ee7b776`  
		Last Modified: Fri, 18 Mar 2022 01:27:30 GMT  
		Size: 68.7 MB (68660506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f928dc74080d0875487138c18b5be16c28fb8eebeaca7cd7ff43e5c053bcf30`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 251.8 KB (251796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2de71e5cdcb594ee0949c5bd975f379ad91d9be834a96504a4506e12cdc8e6`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 2.1 KB (2136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0525ce65e691fa28b8277972d7bacd7427660a270de514d249fd213d63d36a`  
		Last Modified: Fri, 18 Mar 2022 01:27:21 GMT  
		Size: 20.4 MB (20373802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad24ecbe9c7efb4897ead8256b5de51aaa70a6975457b5308234934d3eccbe6`  
		Last Modified: Fri, 18 Mar 2022 01:27:59 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ac548bf3515cbca7c930a68cb952494ac153c33c757588e9870a42bbeb2e03`  
		Last Modified: Fri, 18 Mar 2022 01:28:14 GMT  
		Size: 76.2 MB (76155220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce527927efa348d31fb039bc094edfddc20602790341fc2b0697eba09ce3ea6`  
		Last Modified: Fri, 18 Mar 2022 01:28:01 GMT  
		Size: 14.0 MB (13965074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b59f779d25f18d3f09e480bc05f31d9588066a82bc187dc74545a38266c985d`  
		Last Modified: Fri, 18 Mar 2022 01:27:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:e9892151380249c504812b732784bc7880d22166417375169898ba7d34a26c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:5e94a4cb9fa079ba2d516530161f629ff0c59650cf869bf63a5c19a4f9f0dd49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235821859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f091b223bb3c9c5e0b21510c65c6e2787a10de3bf79168617975d619c89eea99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:50:39 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 09:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:51:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:51:22 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:51:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:51:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:52:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecbe48ec5aab0647ef171eb47e850c5d7ad5d83d03228e51bc1d7eda62698c2`  
		Last Modified: Fri, 18 Mar 2022 10:09:52 GMT  
		Size: 103.7 MB (103665400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eacefe680e43024794dfcc74ecdff7f992bcd4611fb7d958133d4d2e891ade3`  
		Last Modified: Fri, 18 Mar 2022 10:09:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aa24fa831e078da44b8292fc82c4f2b388a5f209abd174cd05d44031d2aa08`  
		Last Modified: Fri, 18 Mar 2022 10:10:18 GMT  
		Size: 74.5 MB (74484668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4b6b5b1240cf12f3cb5b465fc759055ab33013d7a9c48ad6c439d8852c7d21`  
		Last Modified: Fri, 18 Mar 2022 10:10:03 GMT  
		Size: 259.3 KB (259302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8511182887f9e184c8ee62ea72b2c0230006899d385fbf64ba0cef6b95c9767`  
		Last Modified: Fri, 18 Mar 2022 10:10:03 GMT  
		Size: 2.2 KB (2214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1914ca541b732b088c94e6c3c6f853e2791960d1d22a2150e6967558a162144f`  
		Last Modified: Fri, 18 Mar 2022 10:10:07 GMT  
		Size: 22.1 MB (22112950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:26b7dc89a881a01432f5c2b54a79bbd5dbe6c12af3b5791c30e29ca10746c81e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.0 MB (224028322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88116c1b62558c8ca5d06ad866bdb21eb073df2933cee8d2981bf421b16967b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:10:49 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 01:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:11:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:11:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:11:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:12:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:12:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:12:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a68621b6f774214651ac6abdc7182e182f65e198edc8112e53efc9635570653`  
		Last Modified: Fri, 18 Mar 2022 01:28:42 GMT  
		Size: 100.0 MB (100048344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0425700bba9d81e2e3aa2f9073de062a8ef59bf7528a3774052d585b6657f`  
		Last Modified: Fri, 18 Mar 2022 01:28:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0752ff0f201f8040234ada44296e76571e1a26b9f7eaef86030d8366a355e1`  
		Last Modified: Fri, 18 Mar 2022 01:29:03 GMT  
		Size: 68.6 MB (68604630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325fcc44623858b41937cef47681db267ee3f0a06febd8105fc224eda7ab414f`  
		Last Modified: Fri, 18 Mar 2022 01:28:54 GMT  
		Size: 259.3 KB (259255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8308851502a476e636c5fcf9098126499bb61b893eb4aa5887fe129e92522b16`  
		Last Modified: Fri, 18 Mar 2022 01:28:53 GMT  
		Size: 2.2 KB (2156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d752b24be7e98822df467b4323827b090b86601fd6af6957b34b316230e94ad5`  
		Last Modified: Fri, 18 Mar 2022 01:28:57 GMT  
		Size: 21.4 MB (21435302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:e9892151380249c504812b732784bc7880d22166417375169898ba7d34a26c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:5e94a4cb9fa079ba2d516530161f629ff0c59650cf869bf63a5c19a4f9f0dd49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235821859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f091b223bb3c9c5e0b21510c65c6e2787a10de3bf79168617975d619c89eea99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:50:39 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 09:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:51:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:51:22 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:51:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:51:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:52:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecbe48ec5aab0647ef171eb47e850c5d7ad5d83d03228e51bc1d7eda62698c2`  
		Last Modified: Fri, 18 Mar 2022 10:09:52 GMT  
		Size: 103.7 MB (103665400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eacefe680e43024794dfcc74ecdff7f992bcd4611fb7d958133d4d2e891ade3`  
		Last Modified: Fri, 18 Mar 2022 10:09:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aa24fa831e078da44b8292fc82c4f2b388a5f209abd174cd05d44031d2aa08`  
		Last Modified: Fri, 18 Mar 2022 10:10:18 GMT  
		Size: 74.5 MB (74484668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4b6b5b1240cf12f3cb5b465fc759055ab33013d7a9c48ad6c439d8852c7d21`  
		Last Modified: Fri, 18 Mar 2022 10:10:03 GMT  
		Size: 259.3 KB (259302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8511182887f9e184c8ee62ea72b2c0230006899d385fbf64ba0cef6b95c9767`  
		Last Modified: Fri, 18 Mar 2022 10:10:03 GMT  
		Size: 2.2 KB (2214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1914ca541b732b088c94e6c3c6f853e2791960d1d22a2150e6967558a162144f`  
		Last Modified: Fri, 18 Mar 2022 10:10:07 GMT  
		Size: 22.1 MB (22112950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:26b7dc89a881a01432f5c2b54a79bbd5dbe6c12af3b5791c30e29ca10746c81e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.0 MB (224028322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88116c1b62558c8ca5d06ad866bdb21eb073df2933cee8d2981bf421b16967b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:10:49 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 01:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:11:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:11:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:11:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:12:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:12:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:12:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a68621b6f774214651ac6abdc7182e182f65e198edc8112e53efc9635570653`  
		Last Modified: Fri, 18 Mar 2022 01:28:42 GMT  
		Size: 100.0 MB (100048344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0425700bba9d81e2e3aa2f9073de062a8ef59bf7528a3774052d585b6657f`  
		Last Modified: Fri, 18 Mar 2022 01:28:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0752ff0f201f8040234ada44296e76571e1a26b9f7eaef86030d8366a355e1`  
		Last Modified: Fri, 18 Mar 2022 01:29:03 GMT  
		Size: 68.6 MB (68604630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325fcc44623858b41937cef47681db267ee3f0a06febd8105fc224eda7ab414f`  
		Last Modified: Fri, 18 Mar 2022 01:28:54 GMT  
		Size: 259.3 KB (259255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8308851502a476e636c5fcf9098126499bb61b893eb4aa5887fe129e92522b16`  
		Last Modified: Fri, 18 Mar 2022 01:28:53 GMT  
		Size: 2.2 KB (2156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d752b24be7e98822df467b4323827b090b86601fd6af6957b34b316230e94ad5`  
		Last Modified: Fri, 18 Mar 2022 01:28:57 GMT  
		Size: 21.4 MB (21435302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:e9892151380249c504812b732784bc7880d22166417375169898ba7d34a26c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:5e94a4cb9fa079ba2d516530161f629ff0c59650cf869bf63a5c19a4f9f0dd49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235821859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f091b223bb3c9c5e0b21510c65c6e2787a10de3bf79168617975d619c89eea99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:50:39 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 09:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:51:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:51:22 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:51:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:51:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:52:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecbe48ec5aab0647ef171eb47e850c5d7ad5d83d03228e51bc1d7eda62698c2`  
		Last Modified: Fri, 18 Mar 2022 10:09:52 GMT  
		Size: 103.7 MB (103665400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eacefe680e43024794dfcc74ecdff7f992bcd4611fb7d958133d4d2e891ade3`  
		Last Modified: Fri, 18 Mar 2022 10:09:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aa24fa831e078da44b8292fc82c4f2b388a5f209abd174cd05d44031d2aa08`  
		Last Modified: Fri, 18 Mar 2022 10:10:18 GMT  
		Size: 74.5 MB (74484668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4b6b5b1240cf12f3cb5b465fc759055ab33013d7a9c48ad6c439d8852c7d21`  
		Last Modified: Fri, 18 Mar 2022 10:10:03 GMT  
		Size: 259.3 KB (259302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8511182887f9e184c8ee62ea72b2c0230006899d385fbf64ba0cef6b95c9767`  
		Last Modified: Fri, 18 Mar 2022 10:10:03 GMT  
		Size: 2.2 KB (2214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1914ca541b732b088c94e6c3c6f853e2791960d1d22a2150e6967558a162144f`  
		Last Modified: Fri, 18 Mar 2022 10:10:07 GMT  
		Size: 22.1 MB (22112950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:26b7dc89a881a01432f5c2b54a79bbd5dbe6c12af3b5791c30e29ca10746c81e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.0 MB (224028322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88116c1b62558c8ca5d06ad866bdb21eb073df2933cee8d2981bf421b16967b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:10:49 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 01:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:11:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:11:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:11:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:12:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:12:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:12:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a68621b6f774214651ac6abdc7182e182f65e198edc8112e53efc9635570653`  
		Last Modified: Fri, 18 Mar 2022 01:28:42 GMT  
		Size: 100.0 MB (100048344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0425700bba9d81e2e3aa2f9073de062a8ef59bf7528a3774052d585b6657f`  
		Last Modified: Fri, 18 Mar 2022 01:28:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0752ff0f201f8040234ada44296e76571e1a26b9f7eaef86030d8366a355e1`  
		Last Modified: Fri, 18 Mar 2022 01:29:03 GMT  
		Size: 68.6 MB (68604630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325fcc44623858b41937cef47681db267ee3f0a06febd8105fc224eda7ab414f`  
		Last Modified: Fri, 18 Mar 2022 01:28:54 GMT  
		Size: 259.3 KB (259255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8308851502a476e636c5fcf9098126499bb61b893eb4aa5887fe129e92522b16`  
		Last Modified: Fri, 18 Mar 2022 01:28:53 GMT  
		Size: 2.2 KB (2156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d752b24be7e98822df467b4323827b090b86601fd6af6957b34b316230e94ad5`  
		Last Modified: Fri, 18 Mar 2022 01:28:57 GMT  
		Size: 21.4 MB (21435302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:7a354728e3c2ba90e3e1ea9374425bc7b5232d9c17f0918355f09893211acff7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:6f7d07bbdbed46c40ecbc71594b1f66473d03435b7e2b41baa7757582f83a5bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138962725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdaa0cff38ec08bc82b1aa8951185a44e7c2bde70104a7aed80b06f40318df84`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:50:39 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 09:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:51:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:51:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecbe48ec5aab0647ef171eb47e850c5d7ad5d83d03228e51bc1d7eda62698c2`  
		Last Modified: Fri, 18 Mar 2022 10:09:52 GMT  
		Size: 103.7 MB (103665400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eacefe680e43024794dfcc74ecdff7f992bcd4611fb7d958133d4d2e891ade3`  
		Last Modified: Fri, 18 Mar 2022 10:09:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c044d8afe82f21dd1ca060e955d71590114c47949dcdcc6a41633b3fda16db96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133726979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68954dc393f45884454cf79b6220b941ca112af860811abee00886793d16aa9d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:10:49 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 01:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:11:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:11:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:11:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a68621b6f774214651ac6abdc7182e182f65e198edc8112e53efc9635570653`  
		Last Modified: Fri, 18 Mar 2022 01:28:42 GMT  
		Size: 100.0 MB (100048344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0425700bba9d81e2e3aa2f9073de062a8ef59bf7528a3774052d585b6657f`  
		Last Modified: Fri, 18 Mar 2022 01:28:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:7a354728e3c2ba90e3e1ea9374425bc7b5232d9c17f0918355f09893211acff7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:6f7d07bbdbed46c40ecbc71594b1f66473d03435b7e2b41baa7757582f83a5bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138962725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdaa0cff38ec08bc82b1aa8951185a44e7c2bde70104a7aed80b06f40318df84`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:50:39 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 09:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:51:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:51:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecbe48ec5aab0647ef171eb47e850c5d7ad5d83d03228e51bc1d7eda62698c2`  
		Last Modified: Fri, 18 Mar 2022 10:09:52 GMT  
		Size: 103.7 MB (103665400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eacefe680e43024794dfcc74ecdff7f992bcd4611fb7d958133d4d2e891ade3`  
		Last Modified: Fri, 18 Mar 2022 10:09:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c044d8afe82f21dd1ca060e955d71590114c47949dcdcc6a41633b3fda16db96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133726979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68954dc393f45884454cf79b6220b941ca112af860811abee00886793d16aa9d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:10:49 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 01:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:11:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:11:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:11:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a68621b6f774214651ac6abdc7182e182f65e198edc8112e53efc9635570653`  
		Last Modified: Fri, 18 Mar 2022 01:28:42 GMT  
		Size: 100.0 MB (100048344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0425700bba9d81e2e3aa2f9073de062a8ef59bf7528a3774052d585b6657f`  
		Last Modified: Fri, 18 Mar 2022 01:28:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:0b61982b49cfbef498199b0abfdba30abfcf30ed8fb3f5ff70b88e2f3942b0b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:c9843278f8a3e4412d36cfc8bbeb0107b970f1aa59d012e2741e7660f6381644
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330792045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9f4bf15a00c1aa4091fef43dc89b1fb2bd6dfa5bc76bbf3c77466046d79582`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:50:39 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 09:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:51:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:51:22 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:51:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:51:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:52:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:52:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:52:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:52:24 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Mar 2022 09:52:24 GMT
ENV ROS2_DISTRO=galactic
# Fri, 18 Mar 2022 09:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:07 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecbe48ec5aab0647ef171eb47e850c5d7ad5d83d03228e51bc1d7eda62698c2`  
		Last Modified: Fri, 18 Mar 2022 10:09:52 GMT  
		Size: 103.7 MB (103665400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eacefe680e43024794dfcc74ecdff7f992bcd4611fb7d958133d4d2e891ade3`  
		Last Modified: Fri, 18 Mar 2022 10:09:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aa24fa831e078da44b8292fc82c4f2b388a5f209abd174cd05d44031d2aa08`  
		Last Modified: Fri, 18 Mar 2022 10:10:18 GMT  
		Size: 74.5 MB (74484668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4b6b5b1240cf12f3cb5b465fc759055ab33013d7a9c48ad6c439d8852c7d21`  
		Last Modified: Fri, 18 Mar 2022 10:10:03 GMT  
		Size: 259.3 KB (259302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8511182887f9e184c8ee62ea72b2c0230006899d385fbf64ba0cef6b95c9767`  
		Last Modified: Fri, 18 Mar 2022 10:10:03 GMT  
		Size: 2.2 KB (2214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1914ca541b732b088c94e6c3c6f853e2791960d1d22a2150e6967558a162144f`  
		Last Modified: Fri, 18 Mar 2022 10:10:07 GMT  
		Size: 22.1 MB (22112950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6a521c5bde0435347a1a0a0f8c1b166610d368f5d6d2128558f59fe943a87e`  
		Last Modified: Fri, 18 Mar 2022 10:10:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55b62fe2a55b48c9b93d8c181753f55f451ab24337a5742ec71d664005b5926`  
		Last Modified: Fri, 18 Mar 2022 10:10:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83677ecc1d0201634d746cf7648632e2e6c43f472547ebc6ac1de26c35afc31c`  
		Last Modified: Fri, 18 Mar 2022 10:10:52 GMT  
		Size: 78.6 MB (78598979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cdbf52613e9c9705cea9723271654064ec9c847eb356a17c344859931bbff5`  
		Last Modified: Fri, 18 Mar 2022 10:10:36 GMT  
		Size: 16.4 MB (16370582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cc894c1512a47fd5f7e3d29755288695494982b960630ba41bcc5c2e8fb64d`  
		Last Modified: Fri, 18 Mar 2022 10:10:31 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2975ee427f211500194134808a400b84f3729a4d5e23b70413317879fe3ccabf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.0 MB (318024972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb9abaf9378cb60c7c9f950ebaeabbb68607449f36fb5b67df54621e011da34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:10:49 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 01:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:11:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:11:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:11:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:12:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:12:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:12:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:12:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 01:13:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:13:27 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Mar 2022 01:13:28 GMT
ENV ROS2_DISTRO=galactic
# Fri, 18 Mar 2022 01:14:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:15 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a68621b6f774214651ac6abdc7182e182f65e198edc8112e53efc9635570653`  
		Last Modified: Fri, 18 Mar 2022 01:28:42 GMT  
		Size: 100.0 MB (100048344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0425700bba9d81e2e3aa2f9073de062a8ef59bf7528a3774052d585b6657f`  
		Last Modified: Fri, 18 Mar 2022 01:28:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0752ff0f201f8040234ada44296e76571e1a26b9f7eaef86030d8366a355e1`  
		Last Modified: Fri, 18 Mar 2022 01:29:03 GMT  
		Size: 68.6 MB (68604630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325fcc44623858b41937cef47681db267ee3f0a06febd8105fc224eda7ab414f`  
		Last Modified: Fri, 18 Mar 2022 01:28:54 GMT  
		Size: 259.3 KB (259255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8308851502a476e636c5fcf9098126499bb61b893eb4aa5887fe129e92522b16`  
		Last Modified: Fri, 18 Mar 2022 01:28:53 GMT  
		Size: 2.2 KB (2156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d752b24be7e98822df467b4323827b090b86601fd6af6957b34b316230e94ad5`  
		Last Modified: Fri, 18 Mar 2022 01:28:57 GMT  
		Size: 21.4 MB (21435302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62aedff668a0e67910ba219d30007f5cfc2bb58036456acc9b98d1917fbe0dd7`  
		Last Modified: Fri, 18 Mar 2022 01:29:19 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515852b6609020768fee94e01799e6ac715c4225576beddf84e28a4e92255c4e`  
		Last Modified: Fri, 18 Mar 2022 01:29:34 GMT  
		Size: 78.3 MB (78325813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ce119cf3d8d0e55950121b3d3b8fcc0938bea1d68bfab6b9c0aeb6b48b5cf2`  
		Last Modified: Fri, 18 Mar 2022 01:29:22 GMT  
		Size: 15.7 MB (15670368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143c870a9d6abba353f36c7a56a33207a89e66494c4707ce111073204ec20922`  
		Last Modified: Fri, 18 Mar 2022 01:29:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:0b61982b49cfbef498199b0abfdba30abfcf30ed8fb3f5ff70b88e2f3942b0b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:c9843278f8a3e4412d36cfc8bbeb0107b970f1aa59d012e2741e7660f6381644
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330792045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9f4bf15a00c1aa4091fef43dc89b1fb2bd6dfa5bc76bbf3c77466046d79582`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:50:39 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 09:51:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:51:22 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:51:22 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:51:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:51:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:51:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:52:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:52:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:52:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:52:24 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Mar 2022 09:52:24 GMT
ENV ROS2_DISTRO=galactic
# Fri, 18 Mar 2022 09:52:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:07 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecbe48ec5aab0647ef171eb47e850c5d7ad5d83d03228e51bc1d7eda62698c2`  
		Last Modified: Fri, 18 Mar 2022 10:09:52 GMT  
		Size: 103.7 MB (103665400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eacefe680e43024794dfcc74ecdff7f992bcd4611fb7d958133d4d2e891ade3`  
		Last Modified: Fri, 18 Mar 2022 10:09:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15aa24fa831e078da44b8292fc82c4f2b388a5f209abd174cd05d44031d2aa08`  
		Last Modified: Fri, 18 Mar 2022 10:10:18 GMT  
		Size: 74.5 MB (74484668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4b6b5b1240cf12f3cb5b465fc759055ab33013d7a9c48ad6c439d8852c7d21`  
		Last Modified: Fri, 18 Mar 2022 10:10:03 GMT  
		Size: 259.3 KB (259302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8511182887f9e184c8ee62ea72b2c0230006899d385fbf64ba0cef6b95c9767`  
		Last Modified: Fri, 18 Mar 2022 10:10:03 GMT  
		Size: 2.2 KB (2214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1914ca541b732b088c94e6c3c6f853e2791960d1d22a2150e6967558a162144f`  
		Last Modified: Fri, 18 Mar 2022 10:10:07 GMT  
		Size: 22.1 MB (22112950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6a521c5bde0435347a1a0a0f8c1b166610d368f5d6d2128558f59fe943a87e`  
		Last Modified: Fri, 18 Mar 2022 10:10:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55b62fe2a55b48c9b93d8c181753f55f451ab24337a5742ec71d664005b5926`  
		Last Modified: Fri, 18 Mar 2022 10:10:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83677ecc1d0201634d746cf7648632e2e6c43f472547ebc6ac1de26c35afc31c`  
		Last Modified: Fri, 18 Mar 2022 10:10:52 GMT  
		Size: 78.6 MB (78598979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cdbf52613e9c9705cea9723271654064ec9c847eb356a17c344859931bbff5`  
		Last Modified: Fri, 18 Mar 2022 10:10:36 GMT  
		Size: 16.4 MB (16370582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cc894c1512a47fd5f7e3d29755288695494982b960630ba41bcc5c2e8fb64d`  
		Last Modified: Fri, 18 Mar 2022 10:10:31 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2975ee427f211500194134808a400b84f3729a4d5e23b70413317879fe3ccabf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.0 MB (318024972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb9abaf9378cb60c7c9f950ebaeabbb68607449f36fb5b67df54621e011da34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:10:49 GMT
ENV ROS_DISTRO=galactic
# Fri, 18 Mar 2022 01:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:11:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:11:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:11:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:12:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:12:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:12:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:12:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 01:13:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:13:27 GMT
ENV ROS1_DISTRO=noetic
# Fri, 18 Mar 2022 01:13:28 GMT
ENV ROS2_DISTRO=galactic
# Fri, 18 Mar 2022 01:14:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:15 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a68621b6f774214651ac6abdc7182e182f65e198edc8112e53efc9635570653`  
		Last Modified: Fri, 18 Mar 2022 01:28:42 GMT  
		Size: 100.0 MB (100048344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0425700bba9d81e2e3aa2f9073de062a8ef59bf7528a3774052d585b6657f`  
		Last Modified: Fri, 18 Mar 2022 01:28:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0752ff0f201f8040234ada44296e76571e1a26b9f7eaef86030d8366a355e1`  
		Last Modified: Fri, 18 Mar 2022 01:29:03 GMT  
		Size: 68.6 MB (68604630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325fcc44623858b41937cef47681db267ee3f0a06febd8105fc224eda7ab414f`  
		Last Modified: Fri, 18 Mar 2022 01:28:54 GMT  
		Size: 259.3 KB (259255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8308851502a476e636c5fcf9098126499bb61b893eb4aa5887fe129e92522b16`  
		Last Modified: Fri, 18 Mar 2022 01:28:53 GMT  
		Size: 2.2 KB (2156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d752b24be7e98822df467b4323827b090b86601fd6af6957b34b316230e94ad5`  
		Last Modified: Fri, 18 Mar 2022 01:28:57 GMT  
		Size: 21.4 MB (21435302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62aedff668a0e67910ba219d30007f5cfc2bb58036456acc9b98d1917fbe0dd7`  
		Last Modified: Fri, 18 Mar 2022 01:29:19 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515852b6609020768fee94e01799e6ac715c4225576beddf84e28a4e92255c4e`  
		Last Modified: Fri, 18 Mar 2022 01:29:34 GMT  
		Size: 78.3 MB (78325813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ce119cf3d8d0e55950121b3d3b8fcc0938bea1d68bfab6b9c0aeb6b48b5cf2`  
		Last Modified: Fri, 18 Mar 2022 01:29:22 GMT  
		Size: 15.7 MB (15670368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143c870a9d6abba353f36c7a56a33207a89e66494c4707ce111073204ec20922`  
		Last Modified: Fri, 18 Mar 2022 01:29:19 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:953899ce6b949c54ee4f76b15544e7fe139ca18319918f52044500237a864111
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:6b54889f363f92aa82ba6d57fa2c9ba0282de112b34eb933312d21983bf4796b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.9 MB (251867339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f54dd2b563ff4744848ca4cdc779b8ba16e96de3347a5d1c4d87cee6331a759b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:43:01 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:43:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:43:14 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 09:45:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:45:25 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:45:25 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:46:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:46:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:46:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:48:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22820834ebe0dcfa8d7bcb53cf29645a8a84723f49eee2bfcf3f1b56eaecf3`  
		Last Modified: Fri, 18 Mar 2022 10:07:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e726ad7b878a3341cd14f7b9f457c1aff4d4793b6753753697f71cecdfcf61`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e204965e59bcbf7ac6d87e13bc92ef5e16b1febf5872f402cad9056a770eba`  
		Last Modified: Fri, 18 Mar 2022 10:08:19 GMT  
		Size: 120.1 MB (120106779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2245accfb94d1ebb93d93f6d4680ae8e6fdea2b5571488a29f4642a49dc78d`  
		Last Modified: Fri, 18 Mar 2022 10:07:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53c3ddd926cb4541eb970996c216deb7494ef199dbf5544a4c38c7ca9ce16b`  
		Last Modified: Fri, 18 Mar 2022 10:08:42 GMT  
		Size: 74.5 MB (74540409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c02732d82eb8528fc555a48b7b1f45939a4ce4c459dc35ffdab76db7a83321`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 251.9 KB (251854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3497504cc85c709ec7a661dbbde807899724d862b2b3c081fccd043de7b0e`  
		Last Modified: Fri, 18 Mar 2022 10:08:30 GMT  
		Size: 2.2 KB (2197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b7a10bbe20d65fb6e10bcf4e2ad26de3d74467d7f9cbf4db8627f9670c1e2`  
		Last Modified: Fri, 18 Mar 2022 10:08:34 GMT  
		Size: 21.7 MB (21668774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c0271da37734c7bee2bf52ddacbad34cd3e75cb75452e856920d29abcaf8abac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227246060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cfb281669b65d5d519f1be680712daf507fed215f1d8d13f1a58d8a0bb9b6fa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:06:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:07:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:07:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:07:24 GMT
ENV ROS_DISTRO=foxy
# Fri, 18 Mar 2022 01:08:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:08:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:08:16 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:08:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:08:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:08:53 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226af793efce534c13da03becff4b9ca10c9a78e73068425350180b1f6dd357`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4830ffd26df3e3e23de6bb26197dded9d88809e2a88b370594102526587bb`  
		Last Modified: Fri, 18 Mar 2022 01:26:49 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a14b2daae663639c39577d0c7d4593bd5574bd84d8cc4eab597182dda98e14`  
		Last Modified: Fri, 18 Mar 2022 01:27:06 GMT  
		Size: 104.3 MB (104279184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc8ed32f6736949944b94d4d4616553dd4b8a76e9a9660f4521a62ac4284d7`  
		Last Modified: Fri, 18 Mar 2022 01:26:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bb58734c528dbf439eb6fd5f41bad51b1219ef59cbbb4aa9249f1b7ee7b776`  
		Last Modified: Fri, 18 Mar 2022 01:27:30 GMT  
		Size: 68.7 MB (68660506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f928dc74080d0875487138c18b5be16c28fb8eebeaca7cd7ff43e5c053bcf30`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 251.8 KB (251796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2de71e5cdcb594ee0949c5bd975f379ad91d9be834a96504a4506e12cdc8e6`  
		Last Modified: Fri, 18 Mar 2022 01:27:18 GMT  
		Size: 2.1 KB (2136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0525ce65e691fa28b8277972d7bacd7427660a270de514d249fd213d63d36a`  
		Last Modified: Fri, 18 Mar 2022 01:27:21 GMT  
		Size: 20.4 MB (20373802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:bdcbddad7768e528b58032f31c7b0fd5276d33a4f7ae3bfc795f3999e3b0c479
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:8fe315979e3a133af811a88a5e2e39d962f0e1fda1be856bd3e665978b09d777
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437402957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2fb8456313b58221416273a4088f109d60587247a0b579b70a3022e59ee275`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:07:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:08:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 09:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:13:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:13:02 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:13:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:15:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed186fe30ca85957e7e878753de089d2e8a5010dea43d74e99fb9771929b361`  
		Last Modified: Fri, 18 Mar 2022 09:59:31 GMT  
		Size: 839.0 KB (838975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac38668a25e5c8cb5f52e0ffdd479b065a5b768f641384a77a9dad0e5e3a452`  
		Last Modified: Fri, 18 Mar 2022 09:59:29 GMT  
		Size: 4.9 MB (4872095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3121bbb0fedc1e2db1e5b93f19539efa4d73a3d2e13dc6383e07e5f8307e18d4`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eff7c67bd61ade3c431ca761f80a2ca2e92c123b438fc182703230d41f6d8`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f141a0064ed4688cdba0e30eb81c5f5cc6461474bf113cf9d86b369552eb1247`  
		Last Modified: Fri, 18 Mar 2022 10:00:13 GMT  
		Size: 259.5 MB (259473309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5e41cd901de4d480b01b31605bb094d3495205a16373e06e5ecc7af3e7486`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6519125a60ec57cf2c9469503d427de715a2423e9e3a1e46fdafb8e72212153c`  
		Last Modified: Fri, 18 Mar 2022 10:00:34 GMT  
		Size: 70.2 MB (70235434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3f1f2c1cd9000c6cf11644d9abad67432915059410b93571d879aa424909d0`  
		Last Modified: Fri, 18 Mar 2022 10:00:23 GMT  
		Size: 277.6 KB (277642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02602ee04379bef53741958e500badd53cf9d1fcfb57a4c04a303f0e5ccc2bb1`  
		Last Modified: Fri, 18 Mar 2022 10:00:38 GMT  
		Size: 75.0 MB (74994455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:8a146a66ef4da88770c6101f28d11e0dab4d36dc1907940620f3c90f6be8eac8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385909624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca288673c9e8b1920f7c8d177abed0e86a63137b36e3b325d9fd63d531ef0041`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:49:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 06:49:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 06:49:38 GMT
ENV ROS_DISTRO=melodic
# Sun, 20 Mar 2022 06:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 06:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 06:52:54 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:53:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:54:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 06:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0309665cde8260b163c9e436387ea06be877b3c887a1365db723b937d1ac8fc`  
		Last Modified: Sun, 20 Mar 2022 07:13:01 GMT  
		Size: 840.0 KB (840016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0593d08dd549efcc955de18967872b207c683a278c5586dcb9a577891dc9c1d7`  
		Last Modified: Sun, 20 Mar 2022 07:13:00 GMT  
		Size: 4.1 MB (4085989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ed4b7d5f241ebe3379b98be689c55f2e918de69df9dc49c35e2e22acc881d`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b147465263ff3ff695ba9e407284cd9970d44fd30518ac19b0734e913f245a1`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877fa07064d973f881e0f26b3e7112a8203d28c75ceb36b4c3ce788525211152`  
		Last Modified: Sun, 20 Mar 2022 07:15:34 GMT  
		Size: 238.9 MB (238943937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc7436df57dde7519ce798a787f16a185dd05890111d2c5df42e48f19ad9750`  
		Last Modified: Sun, 20 Mar 2022 07:12:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a73c96c22488951b6e10271500c7ae9dae36006046d7c6858e7ad0a6acce36`  
		Last Modified: Sun, 20 Mar 2022 07:16:16 GMT  
		Size: 54.7 MB (54704857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a084159b6f1947316796ca94640e140f6d1da68cb6b505f8a02811b0798261aa`  
		Last Modified: Sun, 20 Mar 2022 07:15:46 GMT  
		Size: 277.7 KB (277670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b5b4a20eac99ac0d47d0e0b16f1125c06f84a312e6306484b7f29bb7cd812a`  
		Last Modified: Sun, 20 Mar 2022 07:16:32 GMT  
		Size: 64.7 MB (64746609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:216b21396f8e5e93070b79cea49c165848ddbe6cba3c08760cebd896f311668c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.5 MB (411549271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f25124f73cd679ceefc2017c58ae024de1f61c353a3114942428437b810e46d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:43:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:44:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:44:50 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:44:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:44:52 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 00:46:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:46:21 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:46:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:47:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3ab66e8231603adb03d0ab793fb0e59972981a99ffc720e57c383f793946d1`  
		Last Modified: Fri, 18 Mar 2022 01:19:05 GMT  
		Size: 839.7 KB (839706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205e19bfaf7b34cc3a9b24062d2decf853a9385f3fef4d92087fb5f722c192f`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 4.3 MB (4264013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecfed1d8156c3c766d1cf52767451b94c4bddebf47c6077a252748e8a8efe14`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944bedb1f36c611f0fb39e835b936986f1dff2992e5b1af78dd788f93c8935ec`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01676100b2c71e8cba083dac9fa5b52bcc5bb6ce3e9f6aa8e7df42107bee34ab`  
		Last Modified: Fri, 18 Mar 2022 01:19:38 GMT  
		Size: 252.4 MB (252367186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fbf59c647844e4d4b6adb832d7aa654d99f008356bfa2e20f9326b02133b43`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e032b61c129c218c14d1f7db94a569b57660cf8588cc7f05f693eda8c43209`  
		Last Modified: Fri, 18 Mar 2022 01:19:59 GMT  
		Size: 63.1 MB (63067569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab07924ab6769ed024d06805340c41da0fa74e475f78c54e27d5d9e9e0c7fa2`  
		Last Modified: Fri, 18 Mar 2022 01:19:50 GMT  
		Size: 277.6 KB (277589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6507226de0a55e0899df013993c3ba1708f3ba1f41e91ad8b92287104a4aad`  
		Last Modified: Fri, 18 Mar 2022 01:20:01 GMT  
		Size: 67.0 MB (67001735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:8b804884073debb1b09da49e5a7d8b37297aa464e63b9fc6221a6097b0be30f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:1fb161962e56cb2161ca13fc69f52c68c6e66410f67973667160e8da6e21454c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742728743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e1874b68bea6b76b5a9fd19576d22e6fe060eec05c41848fbe5827c34742f3e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:07:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:08:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 09:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:13:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:13:02 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:13:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:15:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:22:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed186fe30ca85957e7e878753de089d2e8a5010dea43d74e99fb9771929b361`  
		Last Modified: Fri, 18 Mar 2022 09:59:31 GMT  
		Size: 839.0 KB (838975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac38668a25e5c8cb5f52e0ffdd479b065a5b768f641384a77a9dad0e5e3a452`  
		Last Modified: Fri, 18 Mar 2022 09:59:29 GMT  
		Size: 4.9 MB (4872095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3121bbb0fedc1e2db1e5b93f19539efa4d73a3d2e13dc6383e07e5f8307e18d4`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eff7c67bd61ade3c431ca761f80a2ca2e92c123b438fc182703230d41f6d8`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f141a0064ed4688cdba0e30eb81c5f5cc6461474bf113cf9d86b369552eb1247`  
		Last Modified: Fri, 18 Mar 2022 10:00:13 GMT  
		Size: 259.5 MB (259473309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5e41cd901de4d480b01b31605bb094d3495205a16373e06e5ecc7af3e7486`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6519125a60ec57cf2c9469503d427de715a2423e9e3a1e46fdafb8e72212153c`  
		Last Modified: Fri, 18 Mar 2022 10:00:34 GMT  
		Size: 70.2 MB (70235434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3f1f2c1cd9000c6cf11644d9abad67432915059410b93571d879aa424909d0`  
		Last Modified: Fri, 18 Mar 2022 10:00:23 GMT  
		Size: 277.6 KB (277642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02602ee04379bef53741958e500badd53cf9d1fcfb57a4c04a303f0e5ccc2bb1`  
		Last Modified: Fri, 18 Mar 2022 10:00:38 GMT  
		Size: 75.0 MB (74994455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744d91d71b38a8c9ed678e8d60ba83cbb32ff512d5702b84976740798a657087`  
		Last Modified: Fri, 18 Mar 2022 10:01:56 GMT  
		Size: 305.3 MB (305325786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:46c5876cc732f326215dda5d8a5b28c758599bc288e4b2779b7fa28f899bc205
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.9 MB (645943235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680dbb8da687f0949c681cca860b37b1d4aeac424baeda9da131d60c115a804a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:49:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 06:49:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 06:49:38 GMT
ENV ROS_DISTRO=melodic
# Sun, 20 Mar 2022 06:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 06:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 06:52:54 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:53:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:54:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 06:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:59:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0309665cde8260b163c9e436387ea06be877b3c887a1365db723b937d1ac8fc`  
		Last Modified: Sun, 20 Mar 2022 07:13:01 GMT  
		Size: 840.0 KB (840016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0593d08dd549efcc955de18967872b207c683a278c5586dcb9a577891dc9c1d7`  
		Last Modified: Sun, 20 Mar 2022 07:13:00 GMT  
		Size: 4.1 MB (4085989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ed4b7d5f241ebe3379b98be689c55f2e918de69df9dc49c35e2e22acc881d`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b147465263ff3ff695ba9e407284cd9970d44fd30518ac19b0734e913f245a1`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877fa07064d973f881e0f26b3e7112a8203d28c75ceb36b4c3ce788525211152`  
		Last Modified: Sun, 20 Mar 2022 07:15:34 GMT  
		Size: 238.9 MB (238943937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc7436df57dde7519ce798a787f16a185dd05890111d2c5df42e48f19ad9750`  
		Last Modified: Sun, 20 Mar 2022 07:12:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a73c96c22488951b6e10271500c7ae9dae36006046d7c6858e7ad0a6acce36`  
		Last Modified: Sun, 20 Mar 2022 07:16:16 GMT  
		Size: 54.7 MB (54704857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a084159b6f1947316796ca94640e140f6d1da68cb6b505f8a02811b0798261aa`  
		Last Modified: Sun, 20 Mar 2022 07:15:46 GMT  
		Size: 277.7 KB (277670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b5b4a20eac99ac0d47d0e0b16f1125c06f84a312e6306484b7f29bb7cd812a`  
		Last Modified: Sun, 20 Mar 2022 07:16:32 GMT  
		Size: 64.7 MB (64746609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d07f56b382ef1ed12fa2cdcbc5744a1e4f6e55a60444301487fcf59edc7853`  
		Last Modified: Sun, 20 Mar 2022 07:19:54 GMT  
		Size: 260.0 MB (260033611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:edacfc7a87b90c24654282216023c773c523f48e64c97d5b852eec4ce7855ff5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **702.9 MB (702932603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b814ca31a82a239dbb0e7c34ae11450922fdc45b7933fb7ca9fb9b369aaeb28`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:43:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:44:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:44:50 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:44:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:44:52 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 00:46:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:46:21 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:46:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:47:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:49:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3ab66e8231603adb03d0ab793fb0e59972981a99ffc720e57c383f793946d1`  
		Last Modified: Fri, 18 Mar 2022 01:19:05 GMT  
		Size: 839.7 KB (839706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205e19bfaf7b34cc3a9b24062d2decf853a9385f3fef4d92087fb5f722c192f`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 4.3 MB (4264013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecfed1d8156c3c766d1cf52767451b94c4bddebf47c6077a252748e8a8efe14`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944bedb1f36c611f0fb39e835b936986f1dff2992e5b1af78dd788f93c8935ec`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01676100b2c71e8cba083dac9fa5b52bcc5bb6ce3e9f6aa8e7df42107bee34ab`  
		Last Modified: Fri, 18 Mar 2022 01:19:38 GMT  
		Size: 252.4 MB (252367186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fbf59c647844e4d4b6adb832d7aa654d99f008356bfa2e20f9326b02133b43`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e032b61c129c218c14d1f7db94a569b57660cf8588cc7f05f693eda8c43209`  
		Last Modified: Fri, 18 Mar 2022 01:19:59 GMT  
		Size: 63.1 MB (63067569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab07924ab6769ed024d06805340c41da0fa74e475f78c54e27d5d9e9e0c7fa2`  
		Last Modified: Fri, 18 Mar 2022 01:19:50 GMT  
		Size: 277.6 KB (277589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6507226de0a55e0899df013993c3ba1708f3ba1f41e91ad8b92287104a4aad`  
		Last Modified: Fri, 18 Mar 2022 01:20:01 GMT  
		Size: 67.0 MB (67001735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0825d2c20990804559f3d682273fea296981f238be61747781d6dfa41d0f41f`  
		Last Modified: Fri, 18 Mar 2022 01:21:16 GMT  
		Size: 291.4 MB (291383332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:8b804884073debb1b09da49e5a7d8b37297aa464e63b9fc6221a6097b0be30f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:1fb161962e56cb2161ca13fc69f52c68c6e66410f67973667160e8da6e21454c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742728743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e1874b68bea6b76b5a9fd19576d22e6fe060eec05c41848fbe5827c34742f3e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:07:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:08:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 09:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:13:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:13:02 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:13:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:15:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:22:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed186fe30ca85957e7e878753de089d2e8a5010dea43d74e99fb9771929b361`  
		Last Modified: Fri, 18 Mar 2022 09:59:31 GMT  
		Size: 839.0 KB (838975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac38668a25e5c8cb5f52e0ffdd479b065a5b768f641384a77a9dad0e5e3a452`  
		Last Modified: Fri, 18 Mar 2022 09:59:29 GMT  
		Size: 4.9 MB (4872095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3121bbb0fedc1e2db1e5b93f19539efa4d73a3d2e13dc6383e07e5f8307e18d4`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eff7c67bd61ade3c431ca761f80a2ca2e92c123b438fc182703230d41f6d8`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f141a0064ed4688cdba0e30eb81c5f5cc6461474bf113cf9d86b369552eb1247`  
		Last Modified: Fri, 18 Mar 2022 10:00:13 GMT  
		Size: 259.5 MB (259473309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5e41cd901de4d480b01b31605bb094d3495205a16373e06e5ecc7af3e7486`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6519125a60ec57cf2c9469503d427de715a2423e9e3a1e46fdafb8e72212153c`  
		Last Modified: Fri, 18 Mar 2022 10:00:34 GMT  
		Size: 70.2 MB (70235434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3f1f2c1cd9000c6cf11644d9abad67432915059410b93571d879aa424909d0`  
		Last Modified: Fri, 18 Mar 2022 10:00:23 GMT  
		Size: 277.6 KB (277642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02602ee04379bef53741958e500badd53cf9d1fcfb57a4c04a303f0e5ccc2bb1`  
		Last Modified: Fri, 18 Mar 2022 10:00:38 GMT  
		Size: 75.0 MB (74994455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744d91d71b38a8c9ed678e8d60ba83cbb32ff512d5702b84976740798a657087`  
		Last Modified: Fri, 18 Mar 2022 10:01:56 GMT  
		Size: 305.3 MB (305325786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:46c5876cc732f326215dda5d8a5b28c758599bc288e4b2779b7fa28f899bc205
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.9 MB (645943235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680dbb8da687f0949c681cca860b37b1d4aeac424baeda9da131d60c115a804a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:49:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 06:49:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 06:49:38 GMT
ENV ROS_DISTRO=melodic
# Sun, 20 Mar 2022 06:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 06:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 06:52:54 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:53:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:54:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 06:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:59:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0309665cde8260b163c9e436387ea06be877b3c887a1365db723b937d1ac8fc`  
		Last Modified: Sun, 20 Mar 2022 07:13:01 GMT  
		Size: 840.0 KB (840016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0593d08dd549efcc955de18967872b207c683a278c5586dcb9a577891dc9c1d7`  
		Last Modified: Sun, 20 Mar 2022 07:13:00 GMT  
		Size: 4.1 MB (4085989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ed4b7d5f241ebe3379b98be689c55f2e918de69df9dc49c35e2e22acc881d`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b147465263ff3ff695ba9e407284cd9970d44fd30518ac19b0734e913f245a1`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877fa07064d973f881e0f26b3e7112a8203d28c75ceb36b4c3ce788525211152`  
		Last Modified: Sun, 20 Mar 2022 07:15:34 GMT  
		Size: 238.9 MB (238943937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc7436df57dde7519ce798a787f16a185dd05890111d2c5df42e48f19ad9750`  
		Last Modified: Sun, 20 Mar 2022 07:12:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a73c96c22488951b6e10271500c7ae9dae36006046d7c6858e7ad0a6acce36`  
		Last Modified: Sun, 20 Mar 2022 07:16:16 GMT  
		Size: 54.7 MB (54704857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a084159b6f1947316796ca94640e140f6d1da68cb6b505f8a02811b0798261aa`  
		Last Modified: Sun, 20 Mar 2022 07:15:46 GMT  
		Size: 277.7 KB (277670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b5b4a20eac99ac0d47d0e0b16f1125c06f84a312e6306484b7f29bb7cd812a`  
		Last Modified: Sun, 20 Mar 2022 07:16:32 GMT  
		Size: 64.7 MB (64746609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d07f56b382ef1ed12fa2cdcbc5744a1e4f6e55a60444301487fcf59edc7853`  
		Last Modified: Sun, 20 Mar 2022 07:19:54 GMT  
		Size: 260.0 MB (260033611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:edacfc7a87b90c24654282216023c773c523f48e64c97d5b852eec4ce7855ff5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **702.9 MB (702932603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b814ca31a82a239dbb0e7c34ae11450922fdc45b7933fb7ca9fb9b369aaeb28`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:43:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:44:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:44:50 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:44:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:44:52 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 00:46:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:46:21 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:46:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:47:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:49:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3ab66e8231603adb03d0ab793fb0e59972981a99ffc720e57c383f793946d1`  
		Last Modified: Fri, 18 Mar 2022 01:19:05 GMT  
		Size: 839.7 KB (839706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205e19bfaf7b34cc3a9b24062d2decf853a9385f3fef4d92087fb5f722c192f`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 4.3 MB (4264013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecfed1d8156c3c766d1cf52767451b94c4bddebf47c6077a252748e8a8efe14`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944bedb1f36c611f0fb39e835b936986f1dff2992e5b1af78dd788f93c8935ec`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01676100b2c71e8cba083dac9fa5b52bcc5bb6ce3e9f6aa8e7df42107bee34ab`  
		Last Modified: Fri, 18 Mar 2022 01:19:38 GMT  
		Size: 252.4 MB (252367186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fbf59c647844e4d4b6adb832d7aa654d99f008356bfa2e20f9326b02133b43`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e032b61c129c218c14d1f7db94a569b57660cf8588cc7f05f693eda8c43209`  
		Last Modified: Fri, 18 Mar 2022 01:19:59 GMT  
		Size: 63.1 MB (63067569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab07924ab6769ed024d06805340c41da0fa74e475f78c54e27d5d9e9e0c7fa2`  
		Last Modified: Fri, 18 Mar 2022 01:19:50 GMT  
		Size: 277.6 KB (277589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6507226de0a55e0899df013993c3ba1708f3ba1f41e91ad8b92287104a4aad`  
		Last Modified: Fri, 18 Mar 2022 01:20:01 GMT  
		Size: 67.0 MB (67001735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0825d2c20990804559f3d682273fea296981f238be61747781d6dfa41d0f41f`  
		Last Modified: Fri, 18 Mar 2022 01:21:16 GMT  
		Size: 291.4 MB (291383332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:316e427b4b79b10d0a2d4f9dd1d22624a67d40868521423a6e95bcd224451fb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:a2bc51a561be508b4aafbb7883cc7eb3b76f6eeaf9e9116cc3fd5bcd037608f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448485023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5acad77a852c2660d9fdef8e20a0b627e66a2b5548d83c95f93835571741192`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:07:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:08:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 09:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:13:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:13:02 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:13:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:15:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:15:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed186fe30ca85957e7e878753de089d2e8a5010dea43d74e99fb9771929b361`  
		Last Modified: Fri, 18 Mar 2022 09:59:31 GMT  
		Size: 839.0 KB (838975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac38668a25e5c8cb5f52e0ffdd479b065a5b768f641384a77a9dad0e5e3a452`  
		Last Modified: Fri, 18 Mar 2022 09:59:29 GMT  
		Size: 4.9 MB (4872095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3121bbb0fedc1e2db1e5b93f19539efa4d73a3d2e13dc6383e07e5f8307e18d4`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eff7c67bd61ade3c431ca761f80a2ca2e92c123b438fc182703230d41f6d8`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f141a0064ed4688cdba0e30eb81c5f5cc6461474bf113cf9d86b369552eb1247`  
		Last Modified: Fri, 18 Mar 2022 10:00:13 GMT  
		Size: 259.5 MB (259473309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5e41cd901de4d480b01b31605bb094d3495205a16373e06e5ecc7af3e7486`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6519125a60ec57cf2c9469503d427de715a2423e9e3a1e46fdafb8e72212153c`  
		Last Modified: Fri, 18 Mar 2022 10:00:34 GMT  
		Size: 70.2 MB (70235434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3f1f2c1cd9000c6cf11644d9abad67432915059410b93571d879aa424909d0`  
		Last Modified: Fri, 18 Mar 2022 10:00:23 GMT  
		Size: 277.6 KB (277642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02602ee04379bef53741958e500badd53cf9d1fcfb57a4c04a303f0e5ccc2bb1`  
		Last Modified: Fri, 18 Mar 2022 10:00:38 GMT  
		Size: 75.0 MB (74994455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e23a7d621003e6b0583915577ad995e9c1b718da0883c2064ba3063dcb9790`  
		Last Modified: Fri, 18 Mar 2022 10:00:54 GMT  
		Size: 11.1 MB (11082066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:293bc4324cd5df5a966ecb42adbe46b1e916fa9c99995ecad5ecb39e0520768c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396032709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2811cc67a0714882a4cf5500fdbc9d2768e49f9d119293438673429da634a5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:49:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 06:49:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 06:49:38 GMT
ENV ROS_DISTRO=melodic
# Sun, 20 Mar 2022 06:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 06:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 06:52:54 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:53:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:54:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 06:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:56:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0309665cde8260b163c9e436387ea06be877b3c887a1365db723b937d1ac8fc`  
		Last Modified: Sun, 20 Mar 2022 07:13:01 GMT  
		Size: 840.0 KB (840016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0593d08dd549efcc955de18967872b207c683a278c5586dcb9a577891dc9c1d7`  
		Last Modified: Sun, 20 Mar 2022 07:13:00 GMT  
		Size: 4.1 MB (4085989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ed4b7d5f241ebe3379b98be689c55f2e918de69df9dc49c35e2e22acc881d`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b147465263ff3ff695ba9e407284cd9970d44fd30518ac19b0734e913f245a1`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877fa07064d973f881e0f26b3e7112a8203d28c75ceb36b4c3ce788525211152`  
		Last Modified: Sun, 20 Mar 2022 07:15:34 GMT  
		Size: 238.9 MB (238943937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc7436df57dde7519ce798a787f16a185dd05890111d2c5df42e48f19ad9750`  
		Last Modified: Sun, 20 Mar 2022 07:12:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a73c96c22488951b6e10271500c7ae9dae36006046d7c6858e7ad0a6acce36`  
		Last Modified: Sun, 20 Mar 2022 07:16:16 GMT  
		Size: 54.7 MB (54704857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a084159b6f1947316796ca94640e140f6d1da68cb6b505f8a02811b0798261aa`  
		Last Modified: Sun, 20 Mar 2022 07:15:46 GMT  
		Size: 277.7 KB (277670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b5b4a20eac99ac0d47d0e0b16f1125c06f84a312e6306484b7f29bb7cd812a`  
		Last Modified: Sun, 20 Mar 2022 07:16:32 GMT  
		Size: 64.7 MB (64746609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45054fdb660a1107cc4ca00cff6bf0904c3375f35685dc184875656e0ff075`  
		Last Modified: Sun, 20 Mar 2022 07:16:56 GMT  
		Size: 10.1 MB (10123085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3508fd391cd3a04d17bdef5ae81fee5629fa92e8067647e5abf8bd237f54851b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.3 MB (422282594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf04c775307b1bdd38a83226853edefc2c77ae0db0a202b700ec4d94d64accf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:43:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:44:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:44:50 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:44:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:44:52 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 00:46:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:46:21 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:46:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:47:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:48:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3ab66e8231603adb03d0ab793fb0e59972981a99ffc720e57c383f793946d1`  
		Last Modified: Fri, 18 Mar 2022 01:19:05 GMT  
		Size: 839.7 KB (839706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205e19bfaf7b34cc3a9b24062d2decf853a9385f3fef4d92087fb5f722c192f`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 4.3 MB (4264013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecfed1d8156c3c766d1cf52767451b94c4bddebf47c6077a252748e8a8efe14`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944bedb1f36c611f0fb39e835b936986f1dff2992e5b1af78dd788f93c8935ec`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01676100b2c71e8cba083dac9fa5b52bcc5bb6ce3e9f6aa8e7df42107bee34ab`  
		Last Modified: Fri, 18 Mar 2022 01:19:38 GMT  
		Size: 252.4 MB (252367186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fbf59c647844e4d4b6adb832d7aa654d99f008356bfa2e20f9326b02133b43`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e032b61c129c218c14d1f7db94a569b57660cf8588cc7f05f693eda8c43209`  
		Last Modified: Fri, 18 Mar 2022 01:19:59 GMT  
		Size: 63.1 MB (63067569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab07924ab6769ed024d06805340c41da0fa74e475f78c54e27d5d9e9e0c7fa2`  
		Last Modified: Fri, 18 Mar 2022 01:19:50 GMT  
		Size: 277.6 KB (277589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6507226de0a55e0899df013993c3ba1708f3ba1f41e91ad8b92287104a4aad`  
		Last Modified: Fri, 18 Mar 2022 01:20:01 GMT  
		Size: 67.0 MB (67001735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d23de27f3ef927299f426cd06ca235e8103309202affb70a850483ad55864d0`  
		Last Modified: Fri, 18 Mar 2022 01:20:19 GMT  
		Size: 10.7 MB (10733323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:316e427b4b79b10d0a2d4f9dd1d22624a67d40868521423a6e95bcd224451fb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:a2bc51a561be508b4aafbb7883cc7eb3b76f6eeaf9e9116cc3fd5bcd037608f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448485023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5acad77a852c2660d9fdef8e20a0b627e66a2b5548d83c95f93835571741192`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:07:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:08:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 09:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:13:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:13:02 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:13:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:15:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:15:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed186fe30ca85957e7e878753de089d2e8a5010dea43d74e99fb9771929b361`  
		Last Modified: Fri, 18 Mar 2022 09:59:31 GMT  
		Size: 839.0 KB (838975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac38668a25e5c8cb5f52e0ffdd479b065a5b768f641384a77a9dad0e5e3a452`  
		Last Modified: Fri, 18 Mar 2022 09:59:29 GMT  
		Size: 4.9 MB (4872095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3121bbb0fedc1e2db1e5b93f19539efa4d73a3d2e13dc6383e07e5f8307e18d4`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eff7c67bd61ade3c431ca761f80a2ca2e92c123b438fc182703230d41f6d8`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f141a0064ed4688cdba0e30eb81c5f5cc6461474bf113cf9d86b369552eb1247`  
		Last Modified: Fri, 18 Mar 2022 10:00:13 GMT  
		Size: 259.5 MB (259473309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5e41cd901de4d480b01b31605bb094d3495205a16373e06e5ecc7af3e7486`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6519125a60ec57cf2c9469503d427de715a2423e9e3a1e46fdafb8e72212153c`  
		Last Modified: Fri, 18 Mar 2022 10:00:34 GMT  
		Size: 70.2 MB (70235434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3f1f2c1cd9000c6cf11644d9abad67432915059410b93571d879aa424909d0`  
		Last Modified: Fri, 18 Mar 2022 10:00:23 GMT  
		Size: 277.6 KB (277642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02602ee04379bef53741958e500badd53cf9d1fcfb57a4c04a303f0e5ccc2bb1`  
		Last Modified: Fri, 18 Mar 2022 10:00:38 GMT  
		Size: 75.0 MB (74994455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e23a7d621003e6b0583915577ad995e9c1b718da0883c2064ba3063dcb9790`  
		Last Modified: Fri, 18 Mar 2022 10:00:54 GMT  
		Size: 11.1 MB (11082066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:293bc4324cd5df5a966ecb42adbe46b1e916fa9c99995ecad5ecb39e0520768c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396032709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2811cc67a0714882a4cf5500fdbc9d2768e49f9d119293438673429da634a5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:49:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 06:49:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 06:49:38 GMT
ENV ROS_DISTRO=melodic
# Sun, 20 Mar 2022 06:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 06:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 06:52:54 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:53:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:54:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 06:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:56:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0309665cde8260b163c9e436387ea06be877b3c887a1365db723b937d1ac8fc`  
		Last Modified: Sun, 20 Mar 2022 07:13:01 GMT  
		Size: 840.0 KB (840016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0593d08dd549efcc955de18967872b207c683a278c5586dcb9a577891dc9c1d7`  
		Last Modified: Sun, 20 Mar 2022 07:13:00 GMT  
		Size: 4.1 MB (4085989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ed4b7d5f241ebe3379b98be689c55f2e918de69df9dc49c35e2e22acc881d`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b147465263ff3ff695ba9e407284cd9970d44fd30518ac19b0734e913f245a1`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877fa07064d973f881e0f26b3e7112a8203d28c75ceb36b4c3ce788525211152`  
		Last Modified: Sun, 20 Mar 2022 07:15:34 GMT  
		Size: 238.9 MB (238943937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc7436df57dde7519ce798a787f16a185dd05890111d2c5df42e48f19ad9750`  
		Last Modified: Sun, 20 Mar 2022 07:12:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a73c96c22488951b6e10271500c7ae9dae36006046d7c6858e7ad0a6acce36`  
		Last Modified: Sun, 20 Mar 2022 07:16:16 GMT  
		Size: 54.7 MB (54704857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a084159b6f1947316796ca94640e140f6d1da68cb6b505f8a02811b0798261aa`  
		Last Modified: Sun, 20 Mar 2022 07:15:46 GMT  
		Size: 277.7 KB (277670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b5b4a20eac99ac0d47d0e0b16f1125c06f84a312e6306484b7f29bb7cd812a`  
		Last Modified: Sun, 20 Mar 2022 07:16:32 GMT  
		Size: 64.7 MB (64746609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45054fdb660a1107cc4ca00cff6bf0904c3375f35685dc184875656e0ff075`  
		Last Modified: Sun, 20 Mar 2022 07:16:56 GMT  
		Size: 10.1 MB (10123085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3508fd391cd3a04d17bdef5ae81fee5629fa92e8067647e5abf8bd237f54851b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.3 MB (422282594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf04c775307b1bdd38a83226853edefc2c77ae0db0a202b700ec4d94d64accf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:43:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:44:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:44:50 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:44:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:44:52 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 00:46:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:46:21 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:46:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:47:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:48:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3ab66e8231603adb03d0ab793fb0e59972981a99ffc720e57c383f793946d1`  
		Last Modified: Fri, 18 Mar 2022 01:19:05 GMT  
		Size: 839.7 KB (839706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205e19bfaf7b34cc3a9b24062d2decf853a9385f3fef4d92087fb5f722c192f`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 4.3 MB (4264013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecfed1d8156c3c766d1cf52767451b94c4bddebf47c6077a252748e8a8efe14`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944bedb1f36c611f0fb39e835b936986f1dff2992e5b1af78dd788f93c8935ec`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01676100b2c71e8cba083dac9fa5b52bcc5bb6ce3e9f6aa8e7df42107bee34ab`  
		Last Modified: Fri, 18 Mar 2022 01:19:38 GMT  
		Size: 252.4 MB (252367186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fbf59c647844e4d4b6adb832d7aa654d99f008356bfa2e20f9326b02133b43`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e032b61c129c218c14d1f7db94a569b57660cf8588cc7f05f693eda8c43209`  
		Last Modified: Fri, 18 Mar 2022 01:19:59 GMT  
		Size: 63.1 MB (63067569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab07924ab6769ed024d06805340c41da0fa74e475f78c54e27d5d9e9e0c7fa2`  
		Last Modified: Fri, 18 Mar 2022 01:19:50 GMT  
		Size: 277.6 KB (277589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6507226de0a55e0899df013993c3ba1708f3ba1f41e91ad8b92287104a4aad`  
		Last Modified: Fri, 18 Mar 2022 01:20:01 GMT  
		Size: 67.0 MB (67001735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d23de27f3ef927299f426cd06ca235e8103309202affb70a850483ad55864d0`  
		Last Modified: Fri, 18 Mar 2022 01:20:19 GMT  
		Size: 10.7 MB (10733323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:bdcbddad7768e528b58032f31c7b0fd5276d33a4f7ae3bfc795f3999e3b0c479
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:8fe315979e3a133af811a88a5e2e39d962f0e1fda1be856bd3e665978b09d777
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437402957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2fb8456313b58221416273a4088f109d60587247a0b579b70a3022e59ee275`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:07:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:08:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 09:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:13:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:13:02 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:13:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:15:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed186fe30ca85957e7e878753de089d2e8a5010dea43d74e99fb9771929b361`  
		Last Modified: Fri, 18 Mar 2022 09:59:31 GMT  
		Size: 839.0 KB (838975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac38668a25e5c8cb5f52e0ffdd479b065a5b768f641384a77a9dad0e5e3a452`  
		Last Modified: Fri, 18 Mar 2022 09:59:29 GMT  
		Size: 4.9 MB (4872095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3121bbb0fedc1e2db1e5b93f19539efa4d73a3d2e13dc6383e07e5f8307e18d4`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eff7c67bd61ade3c431ca761f80a2ca2e92c123b438fc182703230d41f6d8`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f141a0064ed4688cdba0e30eb81c5f5cc6461474bf113cf9d86b369552eb1247`  
		Last Modified: Fri, 18 Mar 2022 10:00:13 GMT  
		Size: 259.5 MB (259473309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5e41cd901de4d480b01b31605bb094d3495205a16373e06e5ecc7af3e7486`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6519125a60ec57cf2c9469503d427de715a2423e9e3a1e46fdafb8e72212153c`  
		Last Modified: Fri, 18 Mar 2022 10:00:34 GMT  
		Size: 70.2 MB (70235434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3f1f2c1cd9000c6cf11644d9abad67432915059410b93571d879aa424909d0`  
		Last Modified: Fri, 18 Mar 2022 10:00:23 GMT  
		Size: 277.6 KB (277642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02602ee04379bef53741958e500badd53cf9d1fcfb57a4c04a303f0e5ccc2bb1`  
		Last Modified: Fri, 18 Mar 2022 10:00:38 GMT  
		Size: 75.0 MB (74994455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:8a146a66ef4da88770c6101f28d11e0dab4d36dc1907940620f3c90f6be8eac8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385909624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca288673c9e8b1920f7c8d177abed0e86a63137b36e3b325d9fd63d531ef0041`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:49:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 06:49:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 06:49:38 GMT
ENV ROS_DISTRO=melodic
# Sun, 20 Mar 2022 06:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 06:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 06:52:54 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:53:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:54:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 06:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0309665cde8260b163c9e436387ea06be877b3c887a1365db723b937d1ac8fc`  
		Last Modified: Sun, 20 Mar 2022 07:13:01 GMT  
		Size: 840.0 KB (840016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0593d08dd549efcc955de18967872b207c683a278c5586dcb9a577891dc9c1d7`  
		Last Modified: Sun, 20 Mar 2022 07:13:00 GMT  
		Size: 4.1 MB (4085989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ed4b7d5f241ebe3379b98be689c55f2e918de69df9dc49c35e2e22acc881d`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b147465263ff3ff695ba9e407284cd9970d44fd30518ac19b0734e913f245a1`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877fa07064d973f881e0f26b3e7112a8203d28c75ceb36b4c3ce788525211152`  
		Last Modified: Sun, 20 Mar 2022 07:15:34 GMT  
		Size: 238.9 MB (238943937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc7436df57dde7519ce798a787f16a185dd05890111d2c5df42e48f19ad9750`  
		Last Modified: Sun, 20 Mar 2022 07:12:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a73c96c22488951b6e10271500c7ae9dae36006046d7c6858e7ad0a6acce36`  
		Last Modified: Sun, 20 Mar 2022 07:16:16 GMT  
		Size: 54.7 MB (54704857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a084159b6f1947316796ca94640e140f6d1da68cb6b505f8a02811b0798261aa`  
		Last Modified: Sun, 20 Mar 2022 07:15:46 GMT  
		Size: 277.7 KB (277670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b5b4a20eac99ac0d47d0e0b16f1125c06f84a312e6306484b7f29bb7cd812a`  
		Last Modified: Sun, 20 Mar 2022 07:16:32 GMT  
		Size: 64.7 MB (64746609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:216b21396f8e5e93070b79cea49c165848ddbe6cba3c08760cebd896f311668c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.5 MB (411549271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f25124f73cd679ceefc2017c58ae024de1f61c353a3114942428437b810e46d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:43:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:44:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:44:50 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:44:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:44:52 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 00:46:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:46:21 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:46:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:47:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3ab66e8231603adb03d0ab793fb0e59972981a99ffc720e57c383f793946d1`  
		Last Modified: Fri, 18 Mar 2022 01:19:05 GMT  
		Size: 839.7 KB (839706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205e19bfaf7b34cc3a9b24062d2decf853a9385f3fef4d92087fb5f722c192f`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 4.3 MB (4264013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecfed1d8156c3c766d1cf52767451b94c4bddebf47c6077a252748e8a8efe14`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944bedb1f36c611f0fb39e835b936986f1dff2992e5b1af78dd788f93c8935ec`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01676100b2c71e8cba083dac9fa5b52bcc5bb6ce3e9f6aa8e7df42107bee34ab`  
		Last Modified: Fri, 18 Mar 2022 01:19:38 GMT  
		Size: 252.4 MB (252367186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fbf59c647844e4d4b6adb832d7aa654d99f008356bfa2e20f9326b02133b43`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e032b61c129c218c14d1f7db94a569b57660cf8588cc7f05f693eda8c43209`  
		Last Modified: Fri, 18 Mar 2022 01:19:59 GMT  
		Size: 63.1 MB (63067569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab07924ab6769ed024d06805340c41da0fa74e475f78c54e27d5d9e9e0c7fa2`  
		Last Modified: Fri, 18 Mar 2022 01:19:50 GMT  
		Size: 277.6 KB (277589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6507226de0a55e0899df013993c3ba1708f3ba1f41e91ad8b92287104a4aad`  
		Last Modified: Fri, 18 Mar 2022 01:20:01 GMT  
		Size: 67.0 MB (67001735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:bdcbddad7768e528b58032f31c7b0fd5276d33a4f7ae3bfc795f3999e3b0c479
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:8fe315979e3a133af811a88a5e2e39d962f0e1fda1be856bd3e665978b09d777
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437402957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2fb8456313b58221416273a4088f109d60587247a0b579b70a3022e59ee275`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:07:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:08:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 09:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:13:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:13:02 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:13:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:15:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed186fe30ca85957e7e878753de089d2e8a5010dea43d74e99fb9771929b361`  
		Last Modified: Fri, 18 Mar 2022 09:59:31 GMT  
		Size: 839.0 KB (838975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac38668a25e5c8cb5f52e0ffdd479b065a5b768f641384a77a9dad0e5e3a452`  
		Last Modified: Fri, 18 Mar 2022 09:59:29 GMT  
		Size: 4.9 MB (4872095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3121bbb0fedc1e2db1e5b93f19539efa4d73a3d2e13dc6383e07e5f8307e18d4`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eff7c67bd61ade3c431ca761f80a2ca2e92c123b438fc182703230d41f6d8`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f141a0064ed4688cdba0e30eb81c5f5cc6461474bf113cf9d86b369552eb1247`  
		Last Modified: Fri, 18 Mar 2022 10:00:13 GMT  
		Size: 259.5 MB (259473309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5e41cd901de4d480b01b31605bb094d3495205a16373e06e5ecc7af3e7486`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6519125a60ec57cf2c9469503d427de715a2423e9e3a1e46fdafb8e72212153c`  
		Last Modified: Fri, 18 Mar 2022 10:00:34 GMT  
		Size: 70.2 MB (70235434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3f1f2c1cd9000c6cf11644d9abad67432915059410b93571d879aa424909d0`  
		Last Modified: Fri, 18 Mar 2022 10:00:23 GMT  
		Size: 277.6 KB (277642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02602ee04379bef53741958e500badd53cf9d1fcfb57a4c04a303f0e5ccc2bb1`  
		Last Modified: Fri, 18 Mar 2022 10:00:38 GMT  
		Size: 75.0 MB (74994455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:8a146a66ef4da88770c6101f28d11e0dab4d36dc1907940620f3c90f6be8eac8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385909624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca288673c9e8b1920f7c8d177abed0e86a63137b36e3b325d9fd63d531ef0041`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:49:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 06:49:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 06:49:38 GMT
ENV ROS_DISTRO=melodic
# Sun, 20 Mar 2022 06:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 06:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 06:52:54 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:53:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:54:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 06:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0309665cde8260b163c9e436387ea06be877b3c887a1365db723b937d1ac8fc`  
		Last Modified: Sun, 20 Mar 2022 07:13:01 GMT  
		Size: 840.0 KB (840016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0593d08dd549efcc955de18967872b207c683a278c5586dcb9a577891dc9c1d7`  
		Last Modified: Sun, 20 Mar 2022 07:13:00 GMT  
		Size: 4.1 MB (4085989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ed4b7d5f241ebe3379b98be689c55f2e918de69df9dc49c35e2e22acc881d`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b147465263ff3ff695ba9e407284cd9970d44fd30518ac19b0734e913f245a1`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877fa07064d973f881e0f26b3e7112a8203d28c75ceb36b4c3ce788525211152`  
		Last Modified: Sun, 20 Mar 2022 07:15:34 GMT  
		Size: 238.9 MB (238943937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc7436df57dde7519ce798a787f16a185dd05890111d2c5df42e48f19ad9750`  
		Last Modified: Sun, 20 Mar 2022 07:12:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a73c96c22488951b6e10271500c7ae9dae36006046d7c6858e7ad0a6acce36`  
		Last Modified: Sun, 20 Mar 2022 07:16:16 GMT  
		Size: 54.7 MB (54704857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a084159b6f1947316796ca94640e140f6d1da68cb6b505f8a02811b0798261aa`  
		Last Modified: Sun, 20 Mar 2022 07:15:46 GMT  
		Size: 277.7 KB (277670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b5b4a20eac99ac0d47d0e0b16f1125c06f84a312e6306484b7f29bb7cd812a`  
		Last Modified: Sun, 20 Mar 2022 07:16:32 GMT  
		Size: 64.7 MB (64746609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:216b21396f8e5e93070b79cea49c165848ddbe6cba3c08760cebd896f311668c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.5 MB (411549271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f25124f73cd679ceefc2017c58ae024de1f61c353a3114942428437b810e46d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:43:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:44:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:44:50 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:44:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:44:52 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 00:46:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:46:21 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:46:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:47:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3ab66e8231603adb03d0ab793fb0e59972981a99ffc720e57c383f793946d1`  
		Last Modified: Fri, 18 Mar 2022 01:19:05 GMT  
		Size: 839.7 KB (839706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205e19bfaf7b34cc3a9b24062d2decf853a9385f3fef4d92087fb5f722c192f`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 4.3 MB (4264013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecfed1d8156c3c766d1cf52767451b94c4bddebf47c6077a252748e8a8efe14`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944bedb1f36c611f0fb39e835b936986f1dff2992e5b1af78dd788f93c8935ec`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01676100b2c71e8cba083dac9fa5b52bcc5bb6ce3e9f6aa8e7df42107bee34ab`  
		Last Modified: Fri, 18 Mar 2022 01:19:38 GMT  
		Size: 252.4 MB (252367186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fbf59c647844e4d4b6adb832d7aa654d99f008356bfa2e20f9326b02133b43`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e032b61c129c218c14d1f7db94a569b57660cf8588cc7f05f693eda8c43209`  
		Last Modified: Fri, 18 Mar 2022 01:19:59 GMT  
		Size: 63.1 MB (63067569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab07924ab6769ed024d06805340c41da0fa74e475f78c54e27d5d9e9e0c7fa2`  
		Last Modified: Fri, 18 Mar 2022 01:19:50 GMT  
		Size: 277.6 KB (277589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6507226de0a55e0899df013993c3ba1708f3ba1f41e91ad8b92287104a4aad`  
		Last Modified: Fri, 18 Mar 2022 01:20:01 GMT  
		Size: 67.0 MB (67001735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:16384805bb6a985e6af821e696f9661c55cb2f79ab3f37001d4013045de89da4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:7993411bf869c56bcae9dfe1f3e7250822ec1312e7c6d22f0e16e41de11974e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291895426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e79425a7677bf6ffcffe61661c336ad245d7181195bb16cbd6d7683d7e9ebe1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:07:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:08:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 09:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:13:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:13:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed186fe30ca85957e7e878753de089d2e8a5010dea43d74e99fb9771929b361`  
		Last Modified: Fri, 18 Mar 2022 09:59:31 GMT  
		Size: 839.0 KB (838975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac38668a25e5c8cb5f52e0ffdd479b065a5b768f641384a77a9dad0e5e3a452`  
		Last Modified: Fri, 18 Mar 2022 09:59:29 GMT  
		Size: 4.9 MB (4872095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3121bbb0fedc1e2db1e5b93f19539efa4d73a3d2e13dc6383e07e5f8307e18d4`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eff7c67bd61ade3c431ca761f80a2ca2e92c123b438fc182703230d41f6d8`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f141a0064ed4688cdba0e30eb81c5f5cc6461474bf113cf9d86b369552eb1247`  
		Last Modified: Fri, 18 Mar 2022 10:00:13 GMT  
		Size: 259.5 MB (259473309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5e41cd901de4d480b01b31605bb094d3495205a16373e06e5ecc7af3e7486`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:89a7740d73bfb9f34a943f770d2b2392e5381bcc607c2733031088253afd66df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266180488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d371ee251ec4166d9475e5957cbd74ddfb69fffa55dc10c60f40a6d581e608b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:49:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 06:49:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 06:49:38 GMT
ENV ROS_DISTRO=melodic
# Sun, 20 Mar 2022 06:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 06:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 06:52:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0309665cde8260b163c9e436387ea06be877b3c887a1365db723b937d1ac8fc`  
		Last Modified: Sun, 20 Mar 2022 07:13:01 GMT  
		Size: 840.0 KB (840016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0593d08dd549efcc955de18967872b207c683a278c5586dcb9a577891dc9c1d7`  
		Last Modified: Sun, 20 Mar 2022 07:13:00 GMT  
		Size: 4.1 MB (4085989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ed4b7d5f241ebe3379b98be689c55f2e918de69df9dc49c35e2e22acc881d`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b147465263ff3ff695ba9e407284cd9970d44fd30518ac19b0734e913f245a1`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877fa07064d973f881e0f26b3e7112a8203d28c75ceb36b4c3ce788525211152`  
		Last Modified: Sun, 20 Mar 2022 07:15:34 GMT  
		Size: 238.9 MB (238943937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc7436df57dde7519ce798a787f16a185dd05890111d2c5df42e48f19ad9750`  
		Last Modified: Sun, 20 Mar 2022 07:12:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:87be3317cb2a6134c2086e2edbd7a5e25d0a7b2bec4dfceaec14089a1805a6fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281202378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c2d2946360479912556ac17a20d97a2e632ce0514f992d7857a16f9b13e61d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:43:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:44:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:44:50 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:44:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:44:52 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 00:46:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:46:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3ab66e8231603adb03d0ab793fb0e59972981a99ffc720e57c383f793946d1`  
		Last Modified: Fri, 18 Mar 2022 01:19:05 GMT  
		Size: 839.7 KB (839706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205e19bfaf7b34cc3a9b24062d2decf853a9385f3fef4d92087fb5f722c192f`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 4.3 MB (4264013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecfed1d8156c3c766d1cf52767451b94c4bddebf47c6077a252748e8a8efe14`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944bedb1f36c611f0fb39e835b936986f1dff2992e5b1af78dd788f93c8935ec`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01676100b2c71e8cba083dac9fa5b52bcc5bb6ce3e9f6aa8e7df42107bee34ab`  
		Last Modified: Fri, 18 Mar 2022 01:19:38 GMT  
		Size: 252.4 MB (252367186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fbf59c647844e4d4b6adb832d7aa654d99f008356bfa2e20f9326b02133b43`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:16384805bb6a985e6af821e696f9661c55cb2f79ab3f37001d4013045de89da4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:7993411bf869c56bcae9dfe1f3e7250822ec1312e7c6d22f0e16e41de11974e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291895426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e79425a7677bf6ffcffe61661c336ad245d7181195bb16cbd6d7683d7e9ebe1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:07:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:08:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 09:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:13:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:13:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed186fe30ca85957e7e878753de089d2e8a5010dea43d74e99fb9771929b361`  
		Last Modified: Fri, 18 Mar 2022 09:59:31 GMT  
		Size: 839.0 KB (838975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac38668a25e5c8cb5f52e0ffdd479b065a5b768f641384a77a9dad0e5e3a452`  
		Last Modified: Fri, 18 Mar 2022 09:59:29 GMT  
		Size: 4.9 MB (4872095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3121bbb0fedc1e2db1e5b93f19539efa4d73a3d2e13dc6383e07e5f8307e18d4`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eff7c67bd61ade3c431ca761f80a2ca2e92c123b438fc182703230d41f6d8`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f141a0064ed4688cdba0e30eb81c5f5cc6461474bf113cf9d86b369552eb1247`  
		Last Modified: Fri, 18 Mar 2022 10:00:13 GMT  
		Size: 259.5 MB (259473309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5e41cd901de4d480b01b31605bb094d3495205a16373e06e5ecc7af3e7486`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:89a7740d73bfb9f34a943f770d2b2392e5381bcc607c2733031088253afd66df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266180488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d371ee251ec4166d9475e5957cbd74ddfb69fffa55dc10c60f40a6d581e608b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:49:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 06:49:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 06:49:38 GMT
ENV ROS_DISTRO=melodic
# Sun, 20 Mar 2022 06:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 06:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 06:52:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0309665cde8260b163c9e436387ea06be877b3c887a1365db723b937d1ac8fc`  
		Last Modified: Sun, 20 Mar 2022 07:13:01 GMT  
		Size: 840.0 KB (840016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0593d08dd549efcc955de18967872b207c683a278c5586dcb9a577891dc9c1d7`  
		Last Modified: Sun, 20 Mar 2022 07:13:00 GMT  
		Size: 4.1 MB (4085989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ed4b7d5f241ebe3379b98be689c55f2e918de69df9dc49c35e2e22acc881d`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b147465263ff3ff695ba9e407284cd9970d44fd30518ac19b0734e913f245a1`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877fa07064d973f881e0f26b3e7112a8203d28c75ceb36b4c3ce788525211152`  
		Last Modified: Sun, 20 Mar 2022 07:15:34 GMT  
		Size: 238.9 MB (238943937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc7436df57dde7519ce798a787f16a185dd05890111d2c5df42e48f19ad9750`  
		Last Modified: Sun, 20 Mar 2022 07:12:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:87be3317cb2a6134c2086e2edbd7a5e25d0a7b2bec4dfceaec14089a1805a6fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281202378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c2d2946360479912556ac17a20d97a2e632ce0514f992d7857a16f9b13e61d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:43:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:44:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:44:50 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:44:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:44:52 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 00:46:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:46:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3ab66e8231603adb03d0ab793fb0e59972981a99ffc720e57c383f793946d1`  
		Last Modified: Fri, 18 Mar 2022 01:19:05 GMT  
		Size: 839.7 KB (839706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205e19bfaf7b34cc3a9b24062d2decf853a9385f3fef4d92087fb5f722c192f`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 4.3 MB (4264013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecfed1d8156c3c766d1cf52767451b94c4bddebf47c6077a252748e8a8efe14`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944bedb1f36c611f0fb39e835b936986f1dff2992e5b1af78dd788f93c8935ec`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01676100b2c71e8cba083dac9fa5b52bcc5bb6ce3e9f6aa8e7df42107bee34ab`  
		Last Modified: Fri, 18 Mar 2022 01:19:38 GMT  
		Size: 252.4 MB (252367186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fbf59c647844e4d4b6adb832d7aa654d99f008356bfa2e20f9326b02133b43`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:0e66e6bf7e956c4c50577880987ba9861db235de3511c8a319069e747f8983a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:9b75661da80faf3b5d0deb5ebaed43a5487c684aca287985f092b688cc9e4b6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.0 MB (343017861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3cd9bd6c0db0a3ebf755c2ab307a9a610b643a1e2b77006476a829774218726`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:24:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:24:05 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 09:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:27:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:27:05 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:27:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:29:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6f46945c7e61459cc807bd264e92ae6f254bce14667e13e57e3a38adff31bb`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a145b9a78a3099e4946daa290200e13b29f54334fa496bfaf2ac60f282b24369`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459b4d84d6a32186346a67cc2a06468ca8e0cccd0f1b8f19d01816b2ad50a047`  
		Last Modified: Fri, 18 Mar 2022 10:02:44 GMT  
		Size: 176.9 MB (176874638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256c9b9a453b2348c4bec2aefd58b6dd0a962e1bfff4daf19f3d5ac9381a1358`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52beffc3a5993c04fcdda712650f03b20b68f55cf83f081cbac79c3688e20500`  
		Last Modified: Fri, 18 Mar 2022 10:03:03 GMT  
		Size: 50.9 MB (50933646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35144418cfd2788822674be46a32f0fbadfaaabe27d6baf1c2b95d054aa55c5`  
		Last Modified: Fri, 18 Mar 2022 10:02:54 GMT  
		Size: 309.7 KB (309749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8ae79b3fa72b513e2e3c4bd575cba9787a21d87c061b574741dea6159cd44`  
		Last Modified: Fri, 18 Mar 2022 10:03:08 GMT  
		Size: 79.6 MB (79602501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:84fd50ea4bad4b3f727169749118c82c6f529210555305d2b3b7e51b70f7ad4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288637269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed3586c8a5141470016cf1e5f108e16791ed756172d4d1ce63d7fdd7b372d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:00:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 07:00:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV ROS_DISTRO=noetic
# Sun, 20 Mar 2022 07:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:03:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 07:03:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 07:03:03 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:03:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:04:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 07:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f048f5c68a54f99a35bee4d4b0a13e82ac0ee029d722eb1b3cd577d3172f4`  
		Last Modified: Sun, 20 Mar 2022 07:20:11 GMT  
		Size: 1.2 MB (1183144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aec4be27211291e0b1e16aefaeabf6d3343d12411346d61bac48b83232271c`  
		Last Modified: Sun, 20 Mar 2022 07:20:09 GMT  
		Size: 4.7 MB (4676253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046c0e20ca9cc401b15ff5ca7165ecfdd57b6f3259a78ed7e4fe43cf4299a2c`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c962c958fdc0b93aae4d0682545be02b454679f359b6c43a05504b8f5db339`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19955f8d16a75dbaa5e58e7c97d9bec68d5d14f87661bd6f158d3b2af4a40256`  
		Last Modified: Sun, 20 Mar 2022 07:22:14 GMT  
		Size: 157.4 MB (157410454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c45523235b7c7dbe24a37e12bee6d584d1de4581201be98dd3c45450bd12939`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb81b4baba259580967dab9f6acc59fa2e9a9122a42517dfe0351cf2147e342`  
		Last Modified: Sun, 20 Mar 2022 07:22:49 GMT  
		Size: 40.5 MB (40499961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a463cc1e0fec2292ca47c9797f6c38634cc34aeabc5c27a05dc43cb32c46968`  
		Last Modified: Sun, 20 Mar 2022 07:22:27 GMT  
		Size: 310.1 KB (310053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d283a5a995bad0eac878167993f10c7d4492ee33ae1c3e5789ed21c53ef739a`  
		Last Modified: Sun, 20 Mar 2022 07:23:07 GMT  
		Size: 60.5 MB (60481505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:98cd70c10ff4df1be1ca4ffe4773599732cc6ad9d0df5317b36cd5747f3404c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (322043425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b07985eac887457a17f7ee96639bbe836b4f70b0c71081e0d1c634c8269fe778`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:50:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:50:44 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:50:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:50:46 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 00:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:54:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:54:12 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:54:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:55:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b5aa37b1e8b16ca5b233578bd893ae2b152504bacf5e3b1d6635bcb7c6a9b`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fde79bbfd73df6e787bcd777ee24ee614779f1f71387d905fdfbfbc57c6fa`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7755b1ea906b03f6abea33ec915fc50b397e81d51623b2fb53c5eca32a07f1cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:57 GMT  
		Size: 171.3 MB (171312849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24432d16f00c088adad0694c3e1947c1d04571b5017b0efccf0e474a309a4cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1123465819e97a16d02df62c3d29857756ddf43e8145b1662bf8f7b58236b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:16 GMT  
		Size: 45.0 MB (44988367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8467940c68893247cb81c8b805a4bf657b258a8fc0d7eb85019e2d9d87857bc`  
		Last Modified: Fri, 18 Mar 2022 01:22:09 GMT  
		Size: 309.7 KB (309691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b228bc817a9cd426eae4c08966800f5873dd05be2477d50e67b1c6d677df93b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:19 GMT  
		Size: 71.8 MB (71753882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:307fd54d3224d1749e3e80ed762233b7153b435da11547980c1a276960cd09a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:0b752a91552be168e4bbd2df5bd3b8138e4ec56ca8094a7a52b8dcd1a01d00c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.0 MB (834967052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1014acac283ddd7673cc9694e41bcf08dcb29d1a27bc68724b28a3b04137ed3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:24:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:24:05 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 09:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:27:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:27:05 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:27:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:29:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:37:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6f46945c7e61459cc807bd264e92ae6f254bce14667e13e57e3a38adff31bb`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a145b9a78a3099e4946daa290200e13b29f54334fa496bfaf2ac60f282b24369`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459b4d84d6a32186346a67cc2a06468ca8e0cccd0f1b8f19d01816b2ad50a047`  
		Last Modified: Fri, 18 Mar 2022 10:02:44 GMT  
		Size: 176.9 MB (176874638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256c9b9a453b2348c4bec2aefd58b6dd0a962e1bfff4daf19f3d5ac9381a1358`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52beffc3a5993c04fcdda712650f03b20b68f55cf83f081cbac79c3688e20500`  
		Last Modified: Fri, 18 Mar 2022 10:03:03 GMT  
		Size: 50.9 MB (50933646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35144418cfd2788822674be46a32f0fbadfaaabe27d6baf1c2b95d054aa55c5`  
		Last Modified: Fri, 18 Mar 2022 10:02:54 GMT  
		Size: 309.7 KB (309749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8ae79b3fa72b513e2e3c4bd575cba9787a21d87c061b574741dea6159cd44`  
		Last Modified: Fri, 18 Mar 2022 10:03:08 GMT  
		Size: 79.6 MB (79602501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49666ae87dd1924963710d43abad08d521ef59e1a383e492d7c86b4edb7d2c68`  
		Last Modified: Fri, 18 Mar 2022 10:04:52 GMT  
		Size: 491.9 MB (491949191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:b721144a4318cb8903d926430e184dcebdfbb07c7aedadf11be27789cd9493f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.6 MB (725553674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b2c26d8f423d3ec23cb3d9f5d1b44eaa01788a61d0d4e0e7f48f58ea796369`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:00:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 07:00:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV ROS_DISTRO=noetic
# Sun, 20 Mar 2022 07:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:03:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 07:03:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 07:03:03 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:03:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:04:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 07:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:11:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f048f5c68a54f99a35bee4d4b0a13e82ac0ee029d722eb1b3cd577d3172f4`  
		Last Modified: Sun, 20 Mar 2022 07:20:11 GMT  
		Size: 1.2 MB (1183144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aec4be27211291e0b1e16aefaeabf6d3343d12411346d61bac48b83232271c`  
		Last Modified: Sun, 20 Mar 2022 07:20:09 GMT  
		Size: 4.7 MB (4676253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046c0e20ca9cc401b15ff5ca7165ecfdd57b6f3259a78ed7e4fe43cf4299a2c`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c962c958fdc0b93aae4d0682545be02b454679f359b6c43a05504b8f5db339`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19955f8d16a75dbaa5e58e7c97d9bec68d5d14f87661bd6f158d3b2af4a40256`  
		Last Modified: Sun, 20 Mar 2022 07:22:14 GMT  
		Size: 157.4 MB (157410454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c45523235b7c7dbe24a37e12bee6d584d1de4581201be98dd3c45450bd12939`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb81b4baba259580967dab9f6acc59fa2e9a9122a42517dfe0351cf2147e342`  
		Last Modified: Sun, 20 Mar 2022 07:22:49 GMT  
		Size: 40.5 MB (40499961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a463cc1e0fec2292ca47c9797f6c38634cc34aeabc5c27a05dc43cb32c46968`  
		Last Modified: Sun, 20 Mar 2022 07:22:27 GMT  
		Size: 310.1 KB (310053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d283a5a995bad0eac878167993f10c7d4492ee33ae1c3e5789ed21c53ef739a`  
		Last Modified: Sun, 20 Mar 2022 07:23:07 GMT  
		Size: 60.5 MB (60481505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8300f6e89bf75a396f978150a11d35286feacba186c103f2a03641ca5f5aca6`  
		Last Modified: Sun, 20 Mar 2022 07:28:15 GMT  
		Size: 436.9 MB (436916405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7ddc5cad946a4a960a50676b0b5117d276f20641bd186aebbea063ebfbe835d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.5 MB (784522779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7eb0b30269a839e4e7de0470bb40011cede686d0a639ba337abbd33d60fb62`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:50:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:50:44 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:50:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:50:46 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 00:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:54:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:54:12 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:54:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:55:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:57:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b5aa37b1e8b16ca5b233578bd893ae2b152504bacf5e3b1d6635bcb7c6a9b`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fde79bbfd73df6e787bcd777ee24ee614779f1f71387d905fdfbfbc57c6fa`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7755b1ea906b03f6abea33ec915fc50b397e81d51623b2fb53c5eca32a07f1cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:57 GMT  
		Size: 171.3 MB (171312849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24432d16f00c088adad0694c3e1947c1d04571b5017b0efccf0e474a309a4cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1123465819e97a16d02df62c3d29857756ddf43e8145b1662bf8f7b58236b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:16 GMT  
		Size: 45.0 MB (44988367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8467940c68893247cb81c8b805a4bf657b258a8fc0d7eb85019e2d9d87857bc`  
		Last Modified: Fri, 18 Mar 2022 01:22:09 GMT  
		Size: 309.7 KB (309691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b228bc817a9cd426eae4c08966800f5873dd05be2477d50e67b1c6d677df93b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:19 GMT  
		Size: 71.8 MB (71753882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4e0cd6f211de70f6e121561d5b0a2a96abe02ac50266b07b75e6e85ed8998a`  
		Last Modified: Fri, 18 Mar 2022 01:24:08 GMT  
		Size: 462.5 MB (462479354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:bdc8875699ff2903b22e44d3ef10cb5a205452cc9f033f76782cde172897087e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:db82d60f869a0518b5ad542546f7cf2fdf5d2e8c0d06b384c1929920b250340d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.4 MB (951352321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afb7732aea903f86c83c53b1808bc21ff3387ccf8b43fb2d8dea1433ef57f5d8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:28 GMT
ADD file:8c5e9f12fd3b6e830ec0ee1800d8e9dcebf217896148f2dc72c010c8a88d9b8f in / 
# Tue, 29 Mar 2022 00:22:28 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:38:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:38:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 29 Mar 2022 18:38:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 29 Mar 2022 18:38:10 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 18:38:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Mar 2022 18:38:10 GMT
ENV ROS_DISTRO=noetic
# Tue, 29 Mar 2022 18:39:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:39:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Mar 2022 18:39:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Mar 2022 18:39:14 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:39:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:39:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Mar 2022 18:40:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b281ebec60d2630a225601bd58a4681375a31b7316263b64d3b149f49694c3fe`  
		Last Modified: Tue, 29 Mar 2022 00:27:37 GMT  
		Size: 50.4 MB (50437915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd41fb40810985980555ad4f3e5c98a2d1fb6aba5406dfb13c3a5751591bb3e4`  
		Last Modified: Tue, 29 Mar 2022 18:43:53 GMT  
		Size: 10.9 MB (10892020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd07b963a0a4666adbf672efe29068ca41a393dbe4e8857520f10bbf6567fbe`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15a903c4ecdd8129ebf93bbb6558cae4631b7c8cbdb52f7b8aabed4da3ec9d8`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff0aa132a5f18476525f41162559ac29a36d8d7fae933dc20478fd1e1cdce0e`  
		Last Modified: Tue, 29 Mar 2022 18:44:24 GMT  
		Size: 239.2 MB (239165595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04437849c9723fd4c815474f1c9148d9917c601f413fd74c7f39a9de06b02e7b`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4312d90907c6e468e1d0d5dca383651b811b150e9b6e169af56a5650d492fe38`  
		Last Modified: Tue, 29 Mar 2022 18:44:45 GMT  
		Size: 86.6 MB (86566668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b306a49cda07cd17bf29d90b1b872d94dfefcec3a9a19e13770ae6b052165d7`  
		Last Modified: Tue, 29 Mar 2022 18:44:32 GMT  
		Size: 305.0 KB (304968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e60e6f9eb483ac56169058a0ad6cd0a9f4d5438c948eeb61f5d931c47b346fd`  
		Last Modified: Tue, 29 Mar 2022 18:44:43 GMT  
		Size: 76.0 MB (75976127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1434dbdc8739ffa12a6e4465d18b21043bb55843aa83afd30c12fe0c34f8f22d`  
		Last Modified: Tue, 29 Mar 2022 18:46:14 GMT  
		Size: 488.0 MB (488006617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:445b84241de395fd5f6874b448723a922a8f672eba931cf9564480eab05aeab6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **867.6 MB (867626599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f97d09e132b5201c9aaf0638163bcdf9b1a4c12f680aef38ef0aad71f9f4eb74`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:27 GMT
ADD file:7686930f8c48390948992fbe39ce798cc57ee1d8785b3da70f4a3220f6e7b024 in / 
# Tue, 29 Mar 2022 00:43:28 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 04:34:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:34:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Mar 2022 04:34:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Mar 2022 04:34:25 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 04:34:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Mar 2022 04:34:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Mar 2022 04:35:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:35:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Mar 2022 04:35:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Mar 2022 04:35:58 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 04:36:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:36:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Mar 2022 04:37:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:41:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c732c99090fe64466c6911ecfdd8d4d3f6dfb183aab95d7746163bc49ebe35c9`  
		Last Modified: Tue, 29 Mar 2022 00:50:29 GMT  
		Size: 49.2 MB (49225896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0436424bca719f680c1fa31bd209153e27bae4df6f8ab0c88f6f556fd86307`  
		Last Modified: Wed, 30 Mar 2022 04:44:00 GMT  
		Size: 10.7 MB (10688200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d686950d8b86d430859218f26abce26283e732385e6e4628c7429eba7832a100`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4bd18027e243a00e84b9735b7938cde61199963e2bbc17ae05e85f67f80407`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86b5d2ea1e4b4e0797a8e0a2938389a64eb82319bb6529d624a6ec2a3fa569a`  
		Last Modified: Wed, 30 Mar 2022 04:44:29 GMT  
		Size: 184.4 MB (184374338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a27d959bf736646019bdf8cf51e4942ddecd224101884479f6ccca6070ee452`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5db582a1aecd5ca67e5b89c286be79777101278f9914867e9e19070a0c52db4`  
		Last Modified: Wed, 30 Mar 2022 04:44:48 GMT  
		Size: 84.4 MB (84351038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfa363f4fd3acddae5e480d68c74edd2ad900349f498c9d74774e1fbd98ce84`  
		Last Modified: Wed, 30 Mar 2022 04:44:38 GMT  
		Size: 304.9 KB (304925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e3c3857cda4e11d22479d728cf8b9caad08735e08d037d5512627830dcc03f`  
		Last Modified: Wed, 30 Mar 2022 04:44:47 GMT  
		Size: 73.9 MB (73865231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c31f2416c11907b5589d69d428938dce4c0e51c703fecb3da9390666c3fae1`  
		Last Modified: Wed, 30 Mar 2022 04:46:13 GMT  
		Size: 464.8 MB (464814602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:307fd54d3224d1749e3e80ed762233b7153b435da11547980c1a276960cd09a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:0b752a91552be168e4bbd2df5bd3b8138e4ec56ca8094a7a52b8dcd1a01d00c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.0 MB (834967052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1014acac283ddd7673cc9694e41bcf08dcb29d1a27bc68724b28a3b04137ed3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:24:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:24:05 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 09:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:27:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:27:05 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:27:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:29:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:37:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6f46945c7e61459cc807bd264e92ae6f254bce14667e13e57e3a38adff31bb`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a145b9a78a3099e4946daa290200e13b29f54334fa496bfaf2ac60f282b24369`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459b4d84d6a32186346a67cc2a06468ca8e0cccd0f1b8f19d01816b2ad50a047`  
		Last Modified: Fri, 18 Mar 2022 10:02:44 GMT  
		Size: 176.9 MB (176874638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256c9b9a453b2348c4bec2aefd58b6dd0a962e1bfff4daf19f3d5ac9381a1358`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52beffc3a5993c04fcdda712650f03b20b68f55cf83f081cbac79c3688e20500`  
		Last Modified: Fri, 18 Mar 2022 10:03:03 GMT  
		Size: 50.9 MB (50933646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35144418cfd2788822674be46a32f0fbadfaaabe27d6baf1c2b95d054aa55c5`  
		Last Modified: Fri, 18 Mar 2022 10:02:54 GMT  
		Size: 309.7 KB (309749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8ae79b3fa72b513e2e3c4bd575cba9787a21d87c061b574741dea6159cd44`  
		Last Modified: Fri, 18 Mar 2022 10:03:08 GMT  
		Size: 79.6 MB (79602501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49666ae87dd1924963710d43abad08d521ef59e1a383e492d7c86b4edb7d2c68`  
		Last Modified: Fri, 18 Mar 2022 10:04:52 GMT  
		Size: 491.9 MB (491949191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:b721144a4318cb8903d926430e184dcebdfbb07c7aedadf11be27789cd9493f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.6 MB (725553674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b2c26d8f423d3ec23cb3d9f5d1b44eaa01788a61d0d4e0e7f48f58ea796369`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:00:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 07:00:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV ROS_DISTRO=noetic
# Sun, 20 Mar 2022 07:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:03:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 07:03:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 07:03:03 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:03:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:04:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 07:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:11:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f048f5c68a54f99a35bee4d4b0a13e82ac0ee029d722eb1b3cd577d3172f4`  
		Last Modified: Sun, 20 Mar 2022 07:20:11 GMT  
		Size: 1.2 MB (1183144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aec4be27211291e0b1e16aefaeabf6d3343d12411346d61bac48b83232271c`  
		Last Modified: Sun, 20 Mar 2022 07:20:09 GMT  
		Size: 4.7 MB (4676253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046c0e20ca9cc401b15ff5ca7165ecfdd57b6f3259a78ed7e4fe43cf4299a2c`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c962c958fdc0b93aae4d0682545be02b454679f359b6c43a05504b8f5db339`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19955f8d16a75dbaa5e58e7c97d9bec68d5d14f87661bd6f158d3b2af4a40256`  
		Last Modified: Sun, 20 Mar 2022 07:22:14 GMT  
		Size: 157.4 MB (157410454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c45523235b7c7dbe24a37e12bee6d584d1de4581201be98dd3c45450bd12939`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb81b4baba259580967dab9f6acc59fa2e9a9122a42517dfe0351cf2147e342`  
		Last Modified: Sun, 20 Mar 2022 07:22:49 GMT  
		Size: 40.5 MB (40499961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a463cc1e0fec2292ca47c9797f6c38634cc34aeabc5c27a05dc43cb32c46968`  
		Last Modified: Sun, 20 Mar 2022 07:22:27 GMT  
		Size: 310.1 KB (310053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d283a5a995bad0eac878167993f10c7d4492ee33ae1c3e5789ed21c53ef739a`  
		Last Modified: Sun, 20 Mar 2022 07:23:07 GMT  
		Size: 60.5 MB (60481505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8300f6e89bf75a396f978150a11d35286feacba186c103f2a03641ca5f5aca6`  
		Last Modified: Sun, 20 Mar 2022 07:28:15 GMT  
		Size: 436.9 MB (436916405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7ddc5cad946a4a960a50676b0b5117d276f20641bd186aebbea063ebfbe835d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.5 MB (784522779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7eb0b30269a839e4e7de0470bb40011cede686d0a639ba337abbd33d60fb62`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:50:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:50:44 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:50:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:50:46 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 00:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:54:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:54:12 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:54:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:55:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:57:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b5aa37b1e8b16ca5b233578bd893ae2b152504bacf5e3b1d6635bcb7c6a9b`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fde79bbfd73df6e787bcd777ee24ee614779f1f71387d905fdfbfbc57c6fa`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7755b1ea906b03f6abea33ec915fc50b397e81d51623b2fb53c5eca32a07f1cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:57 GMT  
		Size: 171.3 MB (171312849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24432d16f00c088adad0694c3e1947c1d04571b5017b0efccf0e474a309a4cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1123465819e97a16d02df62c3d29857756ddf43e8145b1662bf8f7b58236b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:16 GMT  
		Size: 45.0 MB (44988367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8467940c68893247cb81c8b805a4bf657b258a8fc0d7eb85019e2d9d87857bc`  
		Last Modified: Fri, 18 Mar 2022 01:22:09 GMT  
		Size: 309.7 KB (309691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b228bc817a9cd426eae4c08966800f5873dd05be2477d50e67b1c6d677df93b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:19 GMT  
		Size: 71.8 MB (71753882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4e0cd6f211de70f6e121561d5b0a2a96abe02ac50266b07b75e6e85ed8998a`  
		Last Modified: Fri, 18 Mar 2022 01:24:08 GMT  
		Size: 462.5 MB (462479354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:e4ca720faaff237039849a82bd4a1ee9ca4c2da83c2d05b7c78d152300141c49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:6d77a6f2215d20a4f7a43e37fc9c38cd20eedd1d9ee0c87c980ee99930116ecb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.9 MB (358876553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e89738f4b762f6bde05ebc574ea3b1de6951a75d7930fbd1bdb56844ff3a87a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:24:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:24:05 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 09:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:27:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:27:05 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:27:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:29:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6f46945c7e61459cc807bd264e92ae6f254bce14667e13e57e3a38adff31bb`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a145b9a78a3099e4946daa290200e13b29f54334fa496bfaf2ac60f282b24369`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459b4d84d6a32186346a67cc2a06468ca8e0cccd0f1b8f19d01816b2ad50a047`  
		Last Modified: Fri, 18 Mar 2022 10:02:44 GMT  
		Size: 176.9 MB (176874638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256c9b9a453b2348c4bec2aefd58b6dd0a962e1bfff4daf19f3d5ac9381a1358`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52beffc3a5993c04fcdda712650f03b20b68f55cf83f081cbac79c3688e20500`  
		Last Modified: Fri, 18 Mar 2022 10:03:03 GMT  
		Size: 50.9 MB (50933646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35144418cfd2788822674be46a32f0fbadfaaabe27d6baf1c2b95d054aa55c5`  
		Last Modified: Fri, 18 Mar 2022 10:02:54 GMT  
		Size: 309.7 KB (309749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8ae79b3fa72b513e2e3c4bd575cba9787a21d87c061b574741dea6159cd44`  
		Last Modified: Fri, 18 Mar 2022 10:03:08 GMT  
		Size: 79.6 MB (79602501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14b3d178340a142f77be930235205eba0cbb20d38f959c60b80bafcca9a2396`  
		Last Modified: Fri, 18 Mar 2022 10:03:23 GMT  
		Size: 15.9 MB (15858692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:dcc26aed86d745e75f74b0f20f00593688e2b3f5ea7a6366a1aa1a172ab802cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302700588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3478fe0ec1f8032569256444f4a62e516a6da81bdbcd269497c59fae5068c70`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:00:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 07:00:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV ROS_DISTRO=noetic
# Sun, 20 Mar 2022 07:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:03:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 07:03:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 07:03:03 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:03:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:04:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 07:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:05:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f048f5c68a54f99a35bee4d4b0a13e82ac0ee029d722eb1b3cd577d3172f4`  
		Last Modified: Sun, 20 Mar 2022 07:20:11 GMT  
		Size: 1.2 MB (1183144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aec4be27211291e0b1e16aefaeabf6d3343d12411346d61bac48b83232271c`  
		Last Modified: Sun, 20 Mar 2022 07:20:09 GMT  
		Size: 4.7 MB (4676253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046c0e20ca9cc401b15ff5ca7165ecfdd57b6f3259a78ed7e4fe43cf4299a2c`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c962c958fdc0b93aae4d0682545be02b454679f359b6c43a05504b8f5db339`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19955f8d16a75dbaa5e58e7c97d9bec68d5d14f87661bd6f158d3b2af4a40256`  
		Last Modified: Sun, 20 Mar 2022 07:22:14 GMT  
		Size: 157.4 MB (157410454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c45523235b7c7dbe24a37e12bee6d584d1de4581201be98dd3c45450bd12939`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb81b4baba259580967dab9f6acc59fa2e9a9122a42517dfe0351cf2147e342`  
		Last Modified: Sun, 20 Mar 2022 07:22:49 GMT  
		Size: 40.5 MB (40499961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a463cc1e0fec2292ca47c9797f6c38634cc34aeabc5c27a05dc43cb32c46968`  
		Last Modified: Sun, 20 Mar 2022 07:22:27 GMT  
		Size: 310.1 KB (310053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d283a5a995bad0eac878167993f10c7d4492ee33ae1c3e5789ed21c53ef739a`  
		Last Modified: Sun, 20 Mar 2022 07:23:07 GMT  
		Size: 60.5 MB (60481505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0431b613bbb09218e76bd77919289ac304de70f5a8298da508929c92d87c0b`  
		Last Modified: Sun, 20 Mar 2022 07:23:32 GMT  
		Size: 14.1 MB (14063319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8c32e120858113e11f1b32171bb6023f7d53557b3ba50070e26fc9190f8657ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.5 MB (337490786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9799d75786b5d247442b54801332512161a3038e4d816e494c96582dde6a228`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:50:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:50:44 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:50:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:50:46 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 00:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:54:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:54:12 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:54:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:55:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:55:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b5aa37b1e8b16ca5b233578bd893ae2b152504bacf5e3b1d6635bcb7c6a9b`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fde79bbfd73df6e787bcd777ee24ee614779f1f71387d905fdfbfbc57c6fa`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7755b1ea906b03f6abea33ec915fc50b397e81d51623b2fb53c5eca32a07f1cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:57 GMT  
		Size: 171.3 MB (171312849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24432d16f00c088adad0694c3e1947c1d04571b5017b0efccf0e474a309a4cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1123465819e97a16d02df62c3d29857756ddf43e8145b1662bf8f7b58236b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:16 GMT  
		Size: 45.0 MB (44988367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8467940c68893247cb81c8b805a4bf657b258a8fc0d7eb85019e2d9d87857bc`  
		Last Modified: Fri, 18 Mar 2022 01:22:09 GMT  
		Size: 309.7 KB (309691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b228bc817a9cd426eae4c08966800f5873dd05be2477d50e67b1c6d677df93b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:19 GMT  
		Size: 71.8 MB (71753882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bc39db48f396854215b5422c9a3ebf01e6ee06216501b6f8496b9b9f356e9`  
		Last Modified: Fri, 18 Mar 2022 01:22:38 GMT  
		Size: 15.4 MB (15447361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:06b8bf6d9ecbd13e088828647dddb74b0740c40f5b3fd8d74de094c08819910e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:f308e27224fefbe58eadac92ea2742d2a35d5647049afb81e0d09ba596d6c53d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.8 MB (484792758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83d918e598098c117dd93a6e2bc000973143239018b8e4dc79b8a8d54e767592`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:28 GMT
ADD file:8c5e9f12fd3b6e830ec0ee1800d8e9dcebf217896148f2dc72c010c8a88d9b8f in / 
# Tue, 29 Mar 2022 00:22:28 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:38:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:38:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 29 Mar 2022 18:38:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 29 Mar 2022 18:38:10 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 18:38:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Mar 2022 18:38:10 GMT
ENV ROS_DISTRO=noetic
# Tue, 29 Mar 2022 18:39:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:39:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Mar 2022 18:39:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Mar 2022 18:39:14 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:39:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:39:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Mar 2022 18:40:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b281ebec60d2630a225601bd58a4681375a31b7316263b64d3b149f49694c3fe`  
		Last Modified: Tue, 29 Mar 2022 00:27:37 GMT  
		Size: 50.4 MB (50437915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd41fb40810985980555ad4f3e5c98a2d1fb6aba5406dfb13c3a5751591bb3e4`  
		Last Modified: Tue, 29 Mar 2022 18:43:53 GMT  
		Size: 10.9 MB (10892020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd07b963a0a4666adbf672efe29068ca41a393dbe4e8857520f10bbf6567fbe`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15a903c4ecdd8129ebf93bbb6558cae4631b7c8cbdb52f7b8aabed4da3ec9d8`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff0aa132a5f18476525f41162559ac29a36d8d7fae933dc20478fd1e1cdce0e`  
		Last Modified: Tue, 29 Mar 2022 18:44:24 GMT  
		Size: 239.2 MB (239165595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04437849c9723fd4c815474f1c9148d9917c601f413fd74c7f39a9de06b02e7b`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4312d90907c6e468e1d0d5dca383651b811b150e9b6e169af56a5650d492fe38`  
		Last Modified: Tue, 29 Mar 2022 18:44:45 GMT  
		Size: 86.6 MB (86566668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b306a49cda07cd17bf29d90b1b872d94dfefcec3a9a19e13770ae6b052165d7`  
		Last Modified: Tue, 29 Mar 2022 18:44:32 GMT  
		Size: 305.0 KB (304968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e60e6f9eb483ac56169058a0ad6cd0a9f4d5438c948eeb61f5d931c47b346fd`  
		Last Modified: Tue, 29 Mar 2022 18:44:43 GMT  
		Size: 76.0 MB (75976127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cc3325edd54d472e0b8be75b92e47569cd1357d66c46639a3737edd2d8243c`  
		Last Modified: Tue, 29 Mar 2022 18:44:55 GMT  
		Size: 21.4 MB (21447054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7b35ff9bf29bbf3524f42cecf9bef91dc46c6d1685d4173ede6cea307ce7e907
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.9 MB (423918075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2206328d81f1e0738c216f689e97b7e11041def821f9d1affd9a46f76368c7cc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:27 GMT
ADD file:7686930f8c48390948992fbe39ce798cc57ee1d8785b3da70f4a3220f6e7b024 in / 
# Tue, 29 Mar 2022 00:43:28 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 04:34:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:34:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Mar 2022 04:34:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Mar 2022 04:34:25 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 04:34:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Mar 2022 04:34:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Mar 2022 04:35:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:35:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Mar 2022 04:35:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Mar 2022 04:35:58 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 04:36:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:36:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Mar 2022 04:37:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:38:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c732c99090fe64466c6911ecfdd8d4d3f6dfb183aab95d7746163bc49ebe35c9`  
		Last Modified: Tue, 29 Mar 2022 00:50:29 GMT  
		Size: 49.2 MB (49225896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0436424bca719f680c1fa31bd209153e27bae4df6f8ab0c88f6f556fd86307`  
		Last Modified: Wed, 30 Mar 2022 04:44:00 GMT  
		Size: 10.7 MB (10688200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d686950d8b86d430859218f26abce26283e732385e6e4628c7429eba7832a100`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4bd18027e243a00e84b9735b7938cde61199963e2bbc17ae05e85f67f80407`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86b5d2ea1e4b4e0797a8e0a2938389a64eb82319bb6529d624a6ec2a3fa569a`  
		Last Modified: Wed, 30 Mar 2022 04:44:29 GMT  
		Size: 184.4 MB (184374338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a27d959bf736646019bdf8cf51e4942ddecd224101884479f6ccca6070ee452`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5db582a1aecd5ca67e5b89c286be79777101278f9914867e9e19070a0c52db4`  
		Last Modified: Wed, 30 Mar 2022 04:44:48 GMT  
		Size: 84.4 MB (84351038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfa363f4fd3acddae5e480d68c74edd2ad900349f498c9d74774e1fbd98ce84`  
		Last Modified: Wed, 30 Mar 2022 04:44:38 GMT  
		Size: 304.9 KB (304925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e3c3857cda4e11d22479d728cf8b9caad08735e08d037d5512627830dcc03f`  
		Last Modified: Wed, 30 Mar 2022 04:44:47 GMT  
		Size: 73.9 MB (73865231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb174647804aafeba2c0dea35ef2027bc1400697775198f3f3495581db821f62`  
		Last Modified: Wed, 30 Mar 2022 04:44:59 GMT  
		Size: 21.1 MB (21106078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:e4ca720faaff237039849a82bd4a1ee9ca4c2da83c2d05b7c78d152300141c49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:6d77a6f2215d20a4f7a43e37fc9c38cd20eedd1d9ee0c87c980ee99930116ecb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.9 MB (358876553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e89738f4b762f6bde05ebc574ea3b1de6951a75d7930fbd1bdb56844ff3a87a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:24:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:24:05 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 09:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:27:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:27:05 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:27:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:29:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:30:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6f46945c7e61459cc807bd264e92ae6f254bce14667e13e57e3a38adff31bb`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a145b9a78a3099e4946daa290200e13b29f54334fa496bfaf2ac60f282b24369`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459b4d84d6a32186346a67cc2a06468ca8e0cccd0f1b8f19d01816b2ad50a047`  
		Last Modified: Fri, 18 Mar 2022 10:02:44 GMT  
		Size: 176.9 MB (176874638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256c9b9a453b2348c4bec2aefd58b6dd0a962e1bfff4daf19f3d5ac9381a1358`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52beffc3a5993c04fcdda712650f03b20b68f55cf83f081cbac79c3688e20500`  
		Last Modified: Fri, 18 Mar 2022 10:03:03 GMT  
		Size: 50.9 MB (50933646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35144418cfd2788822674be46a32f0fbadfaaabe27d6baf1c2b95d054aa55c5`  
		Last Modified: Fri, 18 Mar 2022 10:02:54 GMT  
		Size: 309.7 KB (309749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8ae79b3fa72b513e2e3c4bd575cba9787a21d87c061b574741dea6159cd44`  
		Last Modified: Fri, 18 Mar 2022 10:03:08 GMT  
		Size: 79.6 MB (79602501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14b3d178340a142f77be930235205eba0cbb20d38f959c60b80bafcca9a2396`  
		Last Modified: Fri, 18 Mar 2022 10:03:23 GMT  
		Size: 15.9 MB (15858692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:dcc26aed86d745e75f74b0f20f00593688e2b3f5ea7a6366a1aa1a172ab802cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302700588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3478fe0ec1f8032569256444f4a62e516a6da81bdbcd269497c59fae5068c70`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:00:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 07:00:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV ROS_DISTRO=noetic
# Sun, 20 Mar 2022 07:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:03:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 07:03:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 07:03:03 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:03:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:04:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 07:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:05:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f048f5c68a54f99a35bee4d4b0a13e82ac0ee029d722eb1b3cd577d3172f4`  
		Last Modified: Sun, 20 Mar 2022 07:20:11 GMT  
		Size: 1.2 MB (1183144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aec4be27211291e0b1e16aefaeabf6d3343d12411346d61bac48b83232271c`  
		Last Modified: Sun, 20 Mar 2022 07:20:09 GMT  
		Size: 4.7 MB (4676253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046c0e20ca9cc401b15ff5ca7165ecfdd57b6f3259a78ed7e4fe43cf4299a2c`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c962c958fdc0b93aae4d0682545be02b454679f359b6c43a05504b8f5db339`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19955f8d16a75dbaa5e58e7c97d9bec68d5d14f87661bd6f158d3b2af4a40256`  
		Last Modified: Sun, 20 Mar 2022 07:22:14 GMT  
		Size: 157.4 MB (157410454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c45523235b7c7dbe24a37e12bee6d584d1de4581201be98dd3c45450bd12939`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb81b4baba259580967dab9f6acc59fa2e9a9122a42517dfe0351cf2147e342`  
		Last Modified: Sun, 20 Mar 2022 07:22:49 GMT  
		Size: 40.5 MB (40499961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a463cc1e0fec2292ca47c9797f6c38634cc34aeabc5c27a05dc43cb32c46968`  
		Last Modified: Sun, 20 Mar 2022 07:22:27 GMT  
		Size: 310.1 KB (310053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d283a5a995bad0eac878167993f10c7d4492ee33ae1c3e5789ed21c53ef739a`  
		Last Modified: Sun, 20 Mar 2022 07:23:07 GMT  
		Size: 60.5 MB (60481505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0431b613bbb09218e76bd77919289ac304de70f5a8298da508929c92d87c0b`  
		Last Modified: Sun, 20 Mar 2022 07:23:32 GMT  
		Size: 14.1 MB (14063319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8c32e120858113e11f1b32171bb6023f7d53557b3ba50070e26fc9190f8657ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.5 MB (337490786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9799d75786b5d247442b54801332512161a3038e4d816e494c96582dde6a228`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:50:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:50:44 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:50:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:50:46 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 00:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:54:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:54:12 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:54:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:55:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:55:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b5aa37b1e8b16ca5b233578bd893ae2b152504bacf5e3b1d6635bcb7c6a9b`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fde79bbfd73df6e787bcd777ee24ee614779f1f71387d905fdfbfbc57c6fa`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7755b1ea906b03f6abea33ec915fc50b397e81d51623b2fb53c5eca32a07f1cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:57 GMT  
		Size: 171.3 MB (171312849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24432d16f00c088adad0694c3e1947c1d04571b5017b0efccf0e474a309a4cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1123465819e97a16d02df62c3d29857756ddf43e8145b1662bf8f7b58236b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:16 GMT  
		Size: 45.0 MB (44988367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8467940c68893247cb81c8b805a4bf657b258a8fc0d7eb85019e2d9d87857bc`  
		Last Modified: Fri, 18 Mar 2022 01:22:09 GMT  
		Size: 309.7 KB (309691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b228bc817a9cd426eae4c08966800f5873dd05be2477d50e67b1c6d677df93b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:19 GMT  
		Size: 71.8 MB (71753882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bc39db48f396854215b5422c9a3ebf01e6ee06216501b6f8496b9b9f356e9`  
		Last Modified: Fri, 18 Mar 2022 01:22:38 GMT  
		Size: 15.4 MB (15447361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:0e66e6bf7e956c4c50577880987ba9861db235de3511c8a319069e747f8983a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:9b75661da80faf3b5d0deb5ebaed43a5487c684aca287985f092b688cc9e4b6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.0 MB (343017861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3cd9bd6c0db0a3ebf755c2ab307a9a610b643a1e2b77006476a829774218726`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:24:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:24:05 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 09:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:27:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:27:05 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:27:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:29:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6f46945c7e61459cc807bd264e92ae6f254bce14667e13e57e3a38adff31bb`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a145b9a78a3099e4946daa290200e13b29f54334fa496bfaf2ac60f282b24369`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459b4d84d6a32186346a67cc2a06468ca8e0cccd0f1b8f19d01816b2ad50a047`  
		Last Modified: Fri, 18 Mar 2022 10:02:44 GMT  
		Size: 176.9 MB (176874638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256c9b9a453b2348c4bec2aefd58b6dd0a962e1bfff4daf19f3d5ac9381a1358`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52beffc3a5993c04fcdda712650f03b20b68f55cf83f081cbac79c3688e20500`  
		Last Modified: Fri, 18 Mar 2022 10:03:03 GMT  
		Size: 50.9 MB (50933646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35144418cfd2788822674be46a32f0fbadfaaabe27d6baf1c2b95d054aa55c5`  
		Last Modified: Fri, 18 Mar 2022 10:02:54 GMT  
		Size: 309.7 KB (309749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8ae79b3fa72b513e2e3c4bd575cba9787a21d87c061b574741dea6159cd44`  
		Last Modified: Fri, 18 Mar 2022 10:03:08 GMT  
		Size: 79.6 MB (79602501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:84fd50ea4bad4b3f727169749118c82c6f529210555305d2b3b7e51b70f7ad4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288637269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed3586c8a5141470016cf1e5f108e16791ed756172d4d1ce63d7fdd7b372d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:00:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 07:00:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV ROS_DISTRO=noetic
# Sun, 20 Mar 2022 07:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:03:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 07:03:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 07:03:03 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:03:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:04:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 07:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f048f5c68a54f99a35bee4d4b0a13e82ac0ee029d722eb1b3cd577d3172f4`  
		Last Modified: Sun, 20 Mar 2022 07:20:11 GMT  
		Size: 1.2 MB (1183144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aec4be27211291e0b1e16aefaeabf6d3343d12411346d61bac48b83232271c`  
		Last Modified: Sun, 20 Mar 2022 07:20:09 GMT  
		Size: 4.7 MB (4676253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046c0e20ca9cc401b15ff5ca7165ecfdd57b6f3259a78ed7e4fe43cf4299a2c`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c962c958fdc0b93aae4d0682545be02b454679f359b6c43a05504b8f5db339`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19955f8d16a75dbaa5e58e7c97d9bec68d5d14f87661bd6f158d3b2af4a40256`  
		Last Modified: Sun, 20 Mar 2022 07:22:14 GMT  
		Size: 157.4 MB (157410454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c45523235b7c7dbe24a37e12bee6d584d1de4581201be98dd3c45450bd12939`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb81b4baba259580967dab9f6acc59fa2e9a9122a42517dfe0351cf2147e342`  
		Last Modified: Sun, 20 Mar 2022 07:22:49 GMT  
		Size: 40.5 MB (40499961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a463cc1e0fec2292ca47c9797f6c38634cc34aeabc5c27a05dc43cb32c46968`  
		Last Modified: Sun, 20 Mar 2022 07:22:27 GMT  
		Size: 310.1 KB (310053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d283a5a995bad0eac878167993f10c7d4492ee33ae1c3e5789ed21c53ef739a`  
		Last Modified: Sun, 20 Mar 2022 07:23:07 GMT  
		Size: 60.5 MB (60481505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:98cd70c10ff4df1be1ca4ffe4773599732cc6ad9d0df5317b36cd5747f3404c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (322043425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b07985eac887457a17f7ee96639bbe836b4f70b0c71081e0d1c634c8269fe778`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:50:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:50:44 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:50:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:50:46 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 00:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:54:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:54:12 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:54:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:55:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b5aa37b1e8b16ca5b233578bd893ae2b152504bacf5e3b1d6635bcb7c6a9b`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fde79bbfd73df6e787bcd777ee24ee614779f1f71387d905fdfbfbc57c6fa`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7755b1ea906b03f6abea33ec915fc50b397e81d51623b2fb53c5eca32a07f1cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:57 GMT  
		Size: 171.3 MB (171312849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24432d16f00c088adad0694c3e1947c1d04571b5017b0efccf0e474a309a4cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1123465819e97a16d02df62c3d29857756ddf43e8145b1662bf8f7b58236b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:16 GMT  
		Size: 45.0 MB (44988367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8467940c68893247cb81c8b805a4bf657b258a8fc0d7eb85019e2d9d87857bc`  
		Last Modified: Fri, 18 Mar 2022 01:22:09 GMT  
		Size: 309.7 KB (309691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b228bc817a9cd426eae4c08966800f5873dd05be2477d50e67b1c6d677df93b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:19 GMT  
		Size: 71.8 MB (71753882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:68292f6442d9a335f0c095dd3a79684a37f4bfb5571fac950473af2b4b355c16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:e96e34d4dbcd475ca6cf853d057fb8570bf32fc53bcd4435d06411b728d0c121
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.3 MB (463345704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00ae4dfb48508ccf4b9cc436b97de0230175db74153eb3b6a7c0b94e10f1afe1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:28 GMT
ADD file:8c5e9f12fd3b6e830ec0ee1800d8e9dcebf217896148f2dc72c010c8a88d9b8f in / 
# Tue, 29 Mar 2022 00:22:28 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:38:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:38:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 29 Mar 2022 18:38:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 29 Mar 2022 18:38:10 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 18:38:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Mar 2022 18:38:10 GMT
ENV ROS_DISTRO=noetic
# Tue, 29 Mar 2022 18:39:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:39:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Mar 2022 18:39:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Mar 2022 18:39:14 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:39:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:39:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Mar 2022 18:40:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b281ebec60d2630a225601bd58a4681375a31b7316263b64d3b149f49694c3fe`  
		Last Modified: Tue, 29 Mar 2022 00:27:37 GMT  
		Size: 50.4 MB (50437915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd41fb40810985980555ad4f3e5c98a2d1fb6aba5406dfb13c3a5751591bb3e4`  
		Last Modified: Tue, 29 Mar 2022 18:43:53 GMT  
		Size: 10.9 MB (10892020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd07b963a0a4666adbf672efe29068ca41a393dbe4e8857520f10bbf6567fbe`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15a903c4ecdd8129ebf93bbb6558cae4631b7c8cbdb52f7b8aabed4da3ec9d8`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff0aa132a5f18476525f41162559ac29a36d8d7fae933dc20478fd1e1cdce0e`  
		Last Modified: Tue, 29 Mar 2022 18:44:24 GMT  
		Size: 239.2 MB (239165595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04437849c9723fd4c815474f1c9148d9917c601f413fd74c7f39a9de06b02e7b`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4312d90907c6e468e1d0d5dca383651b811b150e9b6e169af56a5650d492fe38`  
		Last Modified: Tue, 29 Mar 2022 18:44:45 GMT  
		Size: 86.6 MB (86566668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b306a49cda07cd17bf29d90b1b872d94dfefcec3a9a19e13770ae6b052165d7`  
		Last Modified: Tue, 29 Mar 2022 18:44:32 GMT  
		Size: 305.0 KB (304968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e60e6f9eb483ac56169058a0ad6cd0a9f4d5438c948eeb61f5d931c47b346fd`  
		Last Modified: Tue, 29 Mar 2022 18:44:43 GMT  
		Size: 76.0 MB (75976127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5cc576a7d1f81464d643eebcb8fc69b455081e737eb974d9c3fc8968850bc3fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.8 MB (402811997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dfd5679fb23e1214d8b101e73d52266aaf7f053a7122cfaf9f23214a97fa5cd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:27 GMT
ADD file:7686930f8c48390948992fbe39ce798cc57ee1d8785b3da70f4a3220f6e7b024 in / 
# Tue, 29 Mar 2022 00:43:28 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 04:34:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:34:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Mar 2022 04:34:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Mar 2022 04:34:25 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 04:34:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Mar 2022 04:34:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Mar 2022 04:35:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:35:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Mar 2022 04:35:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Mar 2022 04:35:58 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 04:36:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:36:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Mar 2022 04:37:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c732c99090fe64466c6911ecfdd8d4d3f6dfb183aab95d7746163bc49ebe35c9`  
		Last Modified: Tue, 29 Mar 2022 00:50:29 GMT  
		Size: 49.2 MB (49225896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0436424bca719f680c1fa31bd209153e27bae4df6f8ab0c88f6f556fd86307`  
		Last Modified: Wed, 30 Mar 2022 04:44:00 GMT  
		Size: 10.7 MB (10688200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d686950d8b86d430859218f26abce26283e732385e6e4628c7429eba7832a100`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4bd18027e243a00e84b9735b7938cde61199963e2bbc17ae05e85f67f80407`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86b5d2ea1e4b4e0797a8e0a2938389a64eb82319bb6529d624a6ec2a3fa569a`  
		Last Modified: Wed, 30 Mar 2022 04:44:29 GMT  
		Size: 184.4 MB (184374338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a27d959bf736646019bdf8cf51e4942ddecd224101884479f6ccca6070ee452`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5db582a1aecd5ca67e5b89c286be79777101278f9914867e9e19070a0c52db4`  
		Last Modified: Wed, 30 Mar 2022 04:44:48 GMT  
		Size: 84.4 MB (84351038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfa363f4fd3acddae5e480d68c74edd2ad900349f498c9d74774e1fbd98ce84`  
		Last Modified: Wed, 30 Mar 2022 04:44:38 GMT  
		Size: 304.9 KB (304925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e3c3857cda4e11d22479d728cf8b9caad08735e08d037d5512627830dcc03f`  
		Last Modified: Wed, 30 Mar 2022 04:44:47 GMT  
		Size: 73.9 MB (73865231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:0e66e6bf7e956c4c50577880987ba9861db235de3511c8a319069e747f8983a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:9b75661da80faf3b5d0deb5ebaed43a5487c684aca287985f092b688cc9e4b6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.0 MB (343017861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3cd9bd6c0db0a3ebf755c2ab307a9a610b643a1e2b77006476a829774218726`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:24:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:24:05 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 09:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:27:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:27:05 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:27:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:29:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6f46945c7e61459cc807bd264e92ae6f254bce14667e13e57e3a38adff31bb`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a145b9a78a3099e4946daa290200e13b29f54334fa496bfaf2ac60f282b24369`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459b4d84d6a32186346a67cc2a06468ca8e0cccd0f1b8f19d01816b2ad50a047`  
		Last Modified: Fri, 18 Mar 2022 10:02:44 GMT  
		Size: 176.9 MB (176874638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256c9b9a453b2348c4bec2aefd58b6dd0a962e1bfff4daf19f3d5ac9381a1358`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52beffc3a5993c04fcdda712650f03b20b68f55cf83f081cbac79c3688e20500`  
		Last Modified: Fri, 18 Mar 2022 10:03:03 GMT  
		Size: 50.9 MB (50933646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35144418cfd2788822674be46a32f0fbadfaaabe27d6baf1c2b95d054aa55c5`  
		Last Modified: Fri, 18 Mar 2022 10:02:54 GMT  
		Size: 309.7 KB (309749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee8ae79b3fa72b513e2e3c4bd575cba9787a21d87c061b574741dea6159cd44`  
		Last Modified: Fri, 18 Mar 2022 10:03:08 GMT  
		Size: 79.6 MB (79602501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:84fd50ea4bad4b3f727169749118c82c6f529210555305d2b3b7e51b70f7ad4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288637269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed3586c8a5141470016cf1e5f108e16791ed756172d4d1ce63d7fdd7b372d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:00:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 07:00:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV ROS_DISTRO=noetic
# Sun, 20 Mar 2022 07:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:03:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 07:03:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 07:03:03 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:03:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:04:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sun, 20 Mar 2022 07:04:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f048f5c68a54f99a35bee4d4b0a13e82ac0ee029d722eb1b3cd577d3172f4`  
		Last Modified: Sun, 20 Mar 2022 07:20:11 GMT  
		Size: 1.2 MB (1183144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aec4be27211291e0b1e16aefaeabf6d3343d12411346d61bac48b83232271c`  
		Last Modified: Sun, 20 Mar 2022 07:20:09 GMT  
		Size: 4.7 MB (4676253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046c0e20ca9cc401b15ff5ca7165ecfdd57b6f3259a78ed7e4fe43cf4299a2c`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c962c958fdc0b93aae4d0682545be02b454679f359b6c43a05504b8f5db339`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19955f8d16a75dbaa5e58e7c97d9bec68d5d14f87661bd6f158d3b2af4a40256`  
		Last Modified: Sun, 20 Mar 2022 07:22:14 GMT  
		Size: 157.4 MB (157410454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c45523235b7c7dbe24a37e12bee6d584d1de4581201be98dd3c45450bd12939`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb81b4baba259580967dab9f6acc59fa2e9a9122a42517dfe0351cf2147e342`  
		Last Modified: Sun, 20 Mar 2022 07:22:49 GMT  
		Size: 40.5 MB (40499961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a463cc1e0fec2292ca47c9797f6c38634cc34aeabc5c27a05dc43cb32c46968`  
		Last Modified: Sun, 20 Mar 2022 07:22:27 GMT  
		Size: 310.1 KB (310053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d283a5a995bad0eac878167993f10c7d4492ee33ae1c3e5789ed21c53ef739a`  
		Last Modified: Sun, 20 Mar 2022 07:23:07 GMT  
		Size: 60.5 MB (60481505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:98cd70c10ff4df1be1ca4ffe4773599732cc6ad9d0df5317b36cd5747f3404c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (322043425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b07985eac887457a17f7ee96639bbe836b4f70b0c71081e0d1c634c8269fe778`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:50:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:50:44 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:50:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:50:46 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 00:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:54:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:54:12 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:54:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 00:55:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b5aa37b1e8b16ca5b233578bd893ae2b152504bacf5e3b1d6635bcb7c6a9b`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fde79bbfd73df6e787bcd777ee24ee614779f1f71387d905fdfbfbc57c6fa`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7755b1ea906b03f6abea33ec915fc50b397e81d51623b2fb53c5eca32a07f1cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:57 GMT  
		Size: 171.3 MB (171312849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24432d16f00c088adad0694c3e1947c1d04571b5017b0efccf0e474a309a4cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1123465819e97a16d02df62c3d29857756ddf43e8145b1662bf8f7b58236b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:16 GMT  
		Size: 45.0 MB (44988367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8467940c68893247cb81c8b805a4bf657b258a8fc0d7eb85019e2d9d87857bc`  
		Last Modified: Fri, 18 Mar 2022 01:22:09 GMT  
		Size: 309.7 KB (309691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b228bc817a9cd426eae4c08966800f5873dd05be2477d50e67b1c6d677df93b4`  
		Last Modified: Fri, 18 Mar 2022 01:22:19 GMT  
		Size: 71.8 MB (71753882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:a54358764648a2db66f0f81a908adcba5dba649ef2cd705edf487dcaf93aa518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:e66315d6472a885d35e209d8b7023015acc393f0c0b0a995a0f0405b838aacff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212171965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb5250b0b5be511cc624421c7fc7501c16e351e5deb15cb422e28cfcb2944d2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:24:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:24:05 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 09:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:27:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:27:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6f46945c7e61459cc807bd264e92ae6f254bce14667e13e57e3a38adff31bb`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a145b9a78a3099e4946daa290200e13b29f54334fa496bfaf2ac60f282b24369`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459b4d84d6a32186346a67cc2a06468ca8e0cccd0f1b8f19d01816b2ad50a047`  
		Last Modified: Fri, 18 Mar 2022 10:02:44 GMT  
		Size: 176.9 MB (176874638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256c9b9a453b2348c4bec2aefd58b6dd0a962e1bfff4daf19f3d5ac9381a1358`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:c97085126978c1a8a3b6df4b58f6fe5fc6f79bcca5b4c02b1957ff2f143f4952
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.3 MB (187345750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91bd2f973b092013bcbf5e380922f8ba1ece641f245d653cddebb43bdb7b3cf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:00:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 07:00:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV ROS_DISTRO=noetic
# Sun, 20 Mar 2022 07:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:03:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 07:03:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 07:03:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f048f5c68a54f99a35bee4d4b0a13e82ac0ee029d722eb1b3cd577d3172f4`  
		Last Modified: Sun, 20 Mar 2022 07:20:11 GMT  
		Size: 1.2 MB (1183144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aec4be27211291e0b1e16aefaeabf6d3343d12411346d61bac48b83232271c`  
		Last Modified: Sun, 20 Mar 2022 07:20:09 GMT  
		Size: 4.7 MB (4676253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046c0e20ca9cc401b15ff5ca7165ecfdd57b6f3259a78ed7e4fe43cf4299a2c`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c962c958fdc0b93aae4d0682545be02b454679f359b6c43a05504b8f5db339`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19955f8d16a75dbaa5e58e7c97d9bec68d5d14f87661bd6f158d3b2af4a40256`  
		Last Modified: Sun, 20 Mar 2022 07:22:14 GMT  
		Size: 157.4 MB (157410454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c45523235b7c7dbe24a37e12bee6d584d1de4581201be98dd3c45450bd12939`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:57e2eb6cb1a93699329efea25f0a8b55981572cc9b85a300248889e76715b509
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (204991485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1923e44a0b1aea950d94e881520c3dcb56fd51938170dc107aabc210269f61d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:50:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:50:44 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:50:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:50:46 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 00:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:54:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:54:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b5aa37b1e8b16ca5b233578bd893ae2b152504bacf5e3b1d6635bcb7c6a9b`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fde79bbfd73df6e787bcd777ee24ee614779f1f71387d905fdfbfbc57c6fa`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7755b1ea906b03f6abea33ec915fc50b397e81d51623b2fb53c5eca32a07f1cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:57 GMT  
		Size: 171.3 MB (171312849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24432d16f00c088adad0694c3e1947c1d04571b5017b0efccf0e474a309a4cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:c89e65d950775ced6555254d601f74987af0da690d16370e0b5a1881ad7ecdc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:be3bd0e9ad9b1bfa201092046aa111ed15e429892cada8ede01eea7097c65306
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300497941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2552ba432ab152d2c72b30990be71d54482da668cc845aa226d1cf84abfc12`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:28 GMT
ADD file:8c5e9f12fd3b6e830ec0ee1800d8e9dcebf217896148f2dc72c010c8a88d9b8f in / 
# Tue, 29 Mar 2022 00:22:28 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:38:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:38:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 29 Mar 2022 18:38:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 29 Mar 2022 18:38:10 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 18:38:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Mar 2022 18:38:10 GMT
ENV ROS_DISTRO=noetic
# Tue, 29 Mar 2022 18:39:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:39:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Mar 2022 18:39:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Mar 2022 18:39:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b281ebec60d2630a225601bd58a4681375a31b7316263b64d3b149f49694c3fe`  
		Last Modified: Tue, 29 Mar 2022 00:27:37 GMT  
		Size: 50.4 MB (50437915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd41fb40810985980555ad4f3e5c98a2d1fb6aba5406dfb13c3a5751591bb3e4`  
		Last Modified: Tue, 29 Mar 2022 18:43:53 GMT  
		Size: 10.9 MB (10892020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd07b963a0a4666adbf672efe29068ca41a393dbe4e8857520f10bbf6567fbe`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15a903c4ecdd8129ebf93bbb6558cae4631b7c8cbdb52f7b8aabed4da3ec9d8`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff0aa132a5f18476525f41162559ac29a36d8d7fae933dc20478fd1e1cdce0e`  
		Last Modified: Tue, 29 Mar 2022 18:44:24 GMT  
		Size: 239.2 MB (239165595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04437849c9723fd4c815474f1c9148d9917c601f413fd74c7f39a9de06b02e7b`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:99c39bef50cdd00d850c3c9ab1e91f8a2505ec2f1f89fe200f5c5f0796b39d0d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244290803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbd8471853ee4964dcb30625bb7ca89e30a3d288be782a0962b7764bcbceb30`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:27 GMT
ADD file:7686930f8c48390948992fbe39ce798cc57ee1d8785b3da70f4a3220f6e7b024 in / 
# Tue, 29 Mar 2022 00:43:28 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 04:34:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:34:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Mar 2022 04:34:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Mar 2022 04:34:25 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 04:34:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Mar 2022 04:34:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Mar 2022 04:35:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:35:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Mar 2022 04:35:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Mar 2022 04:35:58 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c732c99090fe64466c6911ecfdd8d4d3f6dfb183aab95d7746163bc49ebe35c9`  
		Last Modified: Tue, 29 Mar 2022 00:50:29 GMT  
		Size: 49.2 MB (49225896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0436424bca719f680c1fa31bd209153e27bae4df6f8ab0c88f6f556fd86307`  
		Last Modified: Wed, 30 Mar 2022 04:44:00 GMT  
		Size: 10.7 MB (10688200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d686950d8b86d430859218f26abce26283e732385e6e4628c7429eba7832a100`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4bd18027e243a00e84b9735b7938cde61199963e2bbc17ae05e85f67f80407`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86b5d2ea1e4b4e0797a8e0a2938389a64eb82319bb6529d624a6ec2a3fa569a`  
		Last Modified: Wed, 30 Mar 2022 04:44:29 GMT  
		Size: 184.4 MB (184374338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a27d959bf736646019bdf8cf51e4942ddecd224101884479f6ccca6070ee452`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:a54358764648a2db66f0f81a908adcba5dba649ef2cd705edf487dcaf93aa518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:e66315d6472a885d35e209d8b7023015acc393f0c0b0a995a0f0405b838aacff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212171965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb5250b0b5be511cc624421c7fc7501c16e351e5deb15cb422e28cfcb2944d2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:22:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:23:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:24:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:24:05 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:24:06 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 09:27:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:27:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:27:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:27:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c4c8a04a75d0deca101bddfd337da1b55149d41339593d865efd91492247f`  
		Last Modified: Fri, 18 Mar 2022 10:02:09 GMT  
		Size: 1.2 MB (1182329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0793f098b90ab990601158b31502e031a89684270e659f5778c52daf85b8e3`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 5.5 MB (5546677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6f46945c7e61459cc807bd264e92ae6f254bce14667e13e57e3a38adff31bb`  
		Last Modified: Fri, 18 Mar 2022 10:02:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a145b9a78a3099e4946daa290200e13b29f54334fa496bfaf2ac60f282b24369`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459b4d84d6a32186346a67cc2a06468ca8e0cccd0f1b8f19d01816b2ad50a047`  
		Last Modified: Fri, 18 Mar 2022 10:02:44 GMT  
		Size: 176.9 MB (176874638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256c9b9a453b2348c4bec2aefd58b6dd0a962e1bfff4daf19f3d5ac9381a1358`  
		Last Modified: Fri, 18 Mar 2022 10:02:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:c97085126978c1a8a3b6df4b58f6fe5fc6f79bcca5b4c02b1957ff2f143f4952
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.3 MB (187345750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91bd2f973b092013bcbf5e380922f8ba1ece641f245d653cddebb43bdb7b3cf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 07:00:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 07:00:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 07:00:35 GMT
ENV ROS_DISTRO=noetic
# Sun, 20 Mar 2022 07:03:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 07:03:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 07:03:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 07:03:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8f048f5c68a54f99a35bee4d4b0a13e82ac0ee029d722eb1b3cd577d3172f4`  
		Last Modified: Sun, 20 Mar 2022 07:20:11 GMT  
		Size: 1.2 MB (1183144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aec4be27211291e0b1e16aefaeabf6d3343d12411346d61bac48b83232271c`  
		Last Modified: Sun, 20 Mar 2022 07:20:09 GMT  
		Size: 4.7 MB (4676253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046c0e20ca9cc401b15ff5ca7165ecfdd57b6f3259a78ed7e4fe43cf4299a2c`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c962c958fdc0b93aae4d0682545be02b454679f359b6c43a05504b8f5db339`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19955f8d16a75dbaa5e58e7c97d9bec68d5d14f87661bd6f158d3b2af4a40256`  
		Last Modified: Sun, 20 Mar 2022 07:22:14 GMT  
		Size: 157.4 MB (157410454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c45523235b7c7dbe24a37e12bee6d584d1de4581201be98dd3c45450bd12939`  
		Last Modified: Sun, 20 Mar 2022 07:20:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:57e2eb6cb1a93699329efea25f0a8b55981572cc9b85a300248889e76715b509
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (204991485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1923e44a0b1aea950d94e881520c3dcb56fd51938170dc107aabc210269f61d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:50:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:50:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:50:44 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:50:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:50:46 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Mar 2022 00:54:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:54:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:54:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:54:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d953991afcd7221257c049654fd6b9a0badc205ef512295d0a14e5b32d79048a`  
		Last Modified: Fri, 18 Mar 2022 01:21:31 GMT  
		Size: 1.2 MB (1184246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7450625577b445654ef80809da992a35c912b1abbf9bbc4ae7cbdd5b1acba574`  
		Last Modified: Fri, 18 Mar 2022 01:21:29 GMT  
		Size: 5.3 MB (5322403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b5aa37b1e8b16ca5b233578bd893ae2b152504bacf5e3b1d6635bcb7c6a9b`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646fde79bbfd73df6e787bcd777ee24ee614779f1f71387d905fdfbfbc57c6fa`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7755b1ea906b03f6abea33ec915fc50b397e81d51623b2fb53c5eca32a07f1cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:57 GMT  
		Size: 171.3 MB (171312849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24432d16f00c088adad0694c3e1947c1d04571b5017b0efccf0e474a309a4cc`  
		Last Modified: Fri, 18 Mar 2022 01:21:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:6557686b61e7b1527565ca93aaed7a49da2baed88399b376b3d729f9909f4ee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:c9eacc240a89ee8a9db884f127a9efb911ee14c000cde1715a6d05595dd8a1db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273638184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca153e6f0bc50c5076de93a82246c399778da1e2d803577d78134cc783bd1b3f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:31:09 GMT
ADD file:ce9bee138da151fa0b9e441f7ef06865e0171006e686f0dc5e1ca6a06e0a3d0c in / 
# Fri, 18 Mar 2022 05:31:09 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:53:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:54:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 09:56:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:56:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:56:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:56:20 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:57:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:57:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:57:46 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:58:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11581404396c9d08d16b97c64bb2fd043ef3216bd3e3ff3d1c6e03398dc8e336`  
		Last Modified: Wed, 16 Mar 2022 11:30:57 GMT  
		Size: 30.5 MB (30485551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d449d4c1f6f849759c38658c4e2053c7b2950c7f69d42c0fcdbd7fd490b7d`  
		Last Modified: Fri, 18 Mar 2022 10:11:05 GMT  
		Size: 1.2 MB (1192034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855467c60b27cd7745629db97415c3b46e1b14929c08528fe5e29366df56502c`  
		Last Modified: Fri, 18 Mar 2022 10:11:03 GMT  
		Size: 3.8 MB (3826992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6ac5bb5e9af926be15f77146a24734345444a1a6adaff26e3e6294242a743`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4282676e74b396a8e1c48a6889a965866ac0fb68c719a00711200bd53e3e198`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3605b0dd24d9612e9bf001c434a312571f6c91a4e4195d8fb584835cbdd08c`  
		Last Modified: Fri, 18 Mar 2022 10:11:27 GMT  
		Size: 116.3 MB (116342876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47eb45f708718a35b2c6e268082dd402aa16bdd526b8281bbb3516dd9ea94dd`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a218eaa26cbe5756270488eb0d4581c2492bf26490978b5865689c4382e79a`  
		Last Modified: Fri, 18 Mar 2022 10:11:53 GMT  
		Size: 98.8 MB (98783196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb12bc5efca8d903bbcad7b07c2b6364116e17f95ba526498f9ec44b221bf7`  
		Last Modified: Fri, 18 Mar 2022 10:11:38 GMT  
		Size: 265.4 KB (265375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0592ca52bbeae58f9cb49bc8f6ffd5c7d0dc03b32866c15a0c71f72e67065bb`  
		Last Modified: Fri, 18 Mar 2022 10:11:37 GMT  
		Size: 2.2 KB (2211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2892c1ea6814cafa696c1dcecaa8e33cc43af83781038cd03b98a9ccefed59a`  
		Last Modified: Fri, 18 Mar 2022 10:11:43 GMT  
		Size: 22.7 MB (22737534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fcd2be142f079e58f2e96193cb417b4b27d3dc3d4dfa8c43c73ea7a6e428de1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.8 MB (267793838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a34026bc9d979398ca8a8f7a494b3e3cf61d68286e37065a5dd24790a4c71bf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:41:10 GMT
ADD file:c81be95ae491788086dc606dd86ac47b679f2ce48c96016d4ba321e995541bca in / 
# Fri, 18 Mar 2022 00:41:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:14:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:51 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:15:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:15:25 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:15:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:15:27 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 01:16:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:16:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:16:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:16:22 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:16:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:16:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:17:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:17:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8037d5c930bd3f2cc0b5ef6849e32124c3c5efaf4389d0974934bba554464390`  
		Last Modified: Fri, 18 Mar 2022 00:43:17 GMT  
		Size: 28.4 MB (28425528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a2d6d51d5672d6a89bcd061ceb0abb70543ab14cf758b52dae0ea10a9ed89`  
		Last Modified: Fri, 18 Mar 2022 01:29:49 GMT  
		Size: 1.2 MB (1193964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a484c953b5a8ac5a49bdfa6ef2654513ce04b2c545724ed23887ed4e26ecf1e0`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 3.6 MB (3594382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c71cdbe64ce9e2a57214b4db9fcdfb68ece3c8c4d618cd6e7ca840103a663f3`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff9291a332798080bfb5b2e8ffa0d988a72c8939ca254eb21592d43f1716372`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b90c99c3d8313d7660084c587776cc644ff55ca2453c2b9abd86d7d6236df1`  
		Last Modified: Fri, 18 Mar 2022 01:30:05 GMT  
		Size: 116.0 MB (116006679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e2c942e9e5613f749e090c5d6e24e6309980924397b270887cdec8ef21a9a`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1ad18863e690660ff2da1cf5734414de53b7815bf58fcd1c7dbac36a107152`  
		Last Modified: Fri, 18 Mar 2022 01:30:31 GMT  
		Size: 96.2 MB (96155191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3c6b05283aa818a9d773afa7b1d3f5f76f2e8842f5ef23f90cc496c3d4dfca`  
		Last Modified: Fri, 18 Mar 2022 01:30:17 GMT  
		Size: 265.3 KB (265325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80fd2612b798c76dea877085bf4e5f263d60d4f6332625917549ce24ac497c1`  
		Last Modified: Fri, 18 Mar 2022 01:30:16 GMT  
		Size: 2.1 KB (2133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd394d49e57956f6844b2e0b95fb1dd971c02f60f1c5e3456cda64c0f5dd2f6`  
		Last Modified: Fri, 18 Mar 2022 01:30:20 GMT  
		Size: 22.1 MB (22148265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:6557686b61e7b1527565ca93aaed7a49da2baed88399b376b3d729f9909f4ee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:c9eacc240a89ee8a9db884f127a9efb911ee14c000cde1715a6d05595dd8a1db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273638184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca153e6f0bc50c5076de93a82246c399778da1e2d803577d78134cc783bd1b3f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:31:09 GMT
ADD file:ce9bee138da151fa0b9e441f7ef06865e0171006e686f0dc5e1ca6a06e0a3d0c in / 
# Fri, 18 Mar 2022 05:31:09 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:53:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:54:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 09:56:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:56:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:56:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:56:20 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:57:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:57:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:57:46 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:58:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11581404396c9d08d16b97c64bb2fd043ef3216bd3e3ff3d1c6e03398dc8e336`  
		Last Modified: Wed, 16 Mar 2022 11:30:57 GMT  
		Size: 30.5 MB (30485551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d449d4c1f6f849759c38658c4e2053c7b2950c7f69d42c0fcdbd7fd490b7d`  
		Last Modified: Fri, 18 Mar 2022 10:11:05 GMT  
		Size: 1.2 MB (1192034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855467c60b27cd7745629db97415c3b46e1b14929c08528fe5e29366df56502c`  
		Last Modified: Fri, 18 Mar 2022 10:11:03 GMT  
		Size: 3.8 MB (3826992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6ac5bb5e9af926be15f77146a24734345444a1a6adaff26e3e6294242a743`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4282676e74b396a8e1c48a6889a965866ac0fb68c719a00711200bd53e3e198`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3605b0dd24d9612e9bf001c434a312571f6c91a4e4195d8fb584835cbdd08c`  
		Last Modified: Fri, 18 Mar 2022 10:11:27 GMT  
		Size: 116.3 MB (116342876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47eb45f708718a35b2c6e268082dd402aa16bdd526b8281bbb3516dd9ea94dd`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a218eaa26cbe5756270488eb0d4581c2492bf26490978b5865689c4382e79a`  
		Last Modified: Fri, 18 Mar 2022 10:11:53 GMT  
		Size: 98.8 MB (98783196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb12bc5efca8d903bbcad7b07c2b6364116e17f95ba526498f9ec44b221bf7`  
		Last Modified: Fri, 18 Mar 2022 10:11:38 GMT  
		Size: 265.4 KB (265375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0592ca52bbeae58f9cb49bc8f6ffd5c7d0dc03b32866c15a0c71f72e67065bb`  
		Last Modified: Fri, 18 Mar 2022 10:11:37 GMT  
		Size: 2.2 KB (2211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2892c1ea6814cafa696c1dcecaa8e33cc43af83781038cd03b98a9ccefed59a`  
		Last Modified: Fri, 18 Mar 2022 10:11:43 GMT  
		Size: 22.7 MB (22737534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fcd2be142f079e58f2e96193cb417b4b27d3dc3d4dfa8c43c73ea7a6e428de1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.8 MB (267793838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a34026bc9d979398ca8a8f7a494b3e3cf61d68286e37065a5dd24790a4c71bf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:41:10 GMT
ADD file:c81be95ae491788086dc606dd86ac47b679f2ce48c96016d4ba321e995541bca in / 
# Fri, 18 Mar 2022 00:41:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:14:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:51 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:15:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:15:25 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:15:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:15:27 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 01:16:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:16:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:16:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:16:22 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:16:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:16:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:17:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:17:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8037d5c930bd3f2cc0b5ef6849e32124c3c5efaf4389d0974934bba554464390`  
		Last Modified: Fri, 18 Mar 2022 00:43:17 GMT  
		Size: 28.4 MB (28425528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a2d6d51d5672d6a89bcd061ceb0abb70543ab14cf758b52dae0ea10a9ed89`  
		Last Modified: Fri, 18 Mar 2022 01:29:49 GMT  
		Size: 1.2 MB (1193964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a484c953b5a8ac5a49bdfa6ef2654513ce04b2c545724ed23887ed4e26ecf1e0`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 3.6 MB (3594382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c71cdbe64ce9e2a57214b4db9fcdfb68ece3c8c4d618cd6e7ca840103a663f3`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff9291a332798080bfb5b2e8ffa0d988a72c8939ca254eb21592d43f1716372`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b90c99c3d8313d7660084c587776cc644ff55ca2453c2b9abd86d7d6236df1`  
		Last Modified: Fri, 18 Mar 2022 01:30:05 GMT  
		Size: 116.0 MB (116006679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e2c942e9e5613f749e090c5d6e24e6309980924397b270887cdec8ef21a9a`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1ad18863e690660ff2da1cf5734414de53b7815bf58fcd1c7dbac36a107152`  
		Last Modified: Fri, 18 Mar 2022 01:30:31 GMT  
		Size: 96.2 MB (96155191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3c6b05283aa818a9d773afa7b1d3f5f76f2e8842f5ef23f90cc496c3d4dfca`  
		Last Modified: Fri, 18 Mar 2022 01:30:17 GMT  
		Size: 265.3 KB (265325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80fd2612b798c76dea877085bf4e5f263d60d4f6332625917549ce24ac497c1`  
		Last Modified: Fri, 18 Mar 2022 01:30:16 GMT  
		Size: 2.1 KB (2133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd394d49e57956f6844b2e0b95fb1dd971c02f60f1c5e3456cda64c0f5dd2f6`  
		Last Modified: Fri, 18 Mar 2022 01:30:20 GMT  
		Size: 22.1 MB (22148265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:6557686b61e7b1527565ca93aaed7a49da2baed88399b376b3d729f9909f4ee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:c9eacc240a89ee8a9db884f127a9efb911ee14c000cde1715a6d05595dd8a1db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273638184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca153e6f0bc50c5076de93a82246c399778da1e2d803577d78134cc783bd1b3f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:31:09 GMT
ADD file:ce9bee138da151fa0b9e441f7ef06865e0171006e686f0dc5e1ca6a06e0a3d0c in / 
# Fri, 18 Mar 2022 05:31:09 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:53:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:54:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 09:56:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:56:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:56:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:56:20 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:57:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:57:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 09:57:46 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 09:58:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11581404396c9d08d16b97c64bb2fd043ef3216bd3e3ff3d1c6e03398dc8e336`  
		Last Modified: Wed, 16 Mar 2022 11:30:57 GMT  
		Size: 30.5 MB (30485551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d449d4c1f6f849759c38658c4e2053c7b2950c7f69d42c0fcdbd7fd490b7d`  
		Last Modified: Fri, 18 Mar 2022 10:11:05 GMT  
		Size: 1.2 MB (1192034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855467c60b27cd7745629db97415c3b46e1b14929c08528fe5e29366df56502c`  
		Last Modified: Fri, 18 Mar 2022 10:11:03 GMT  
		Size: 3.8 MB (3826992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6ac5bb5e9af926be15f77146a24734345444a1a6adaff26e3e6294242a743`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4282676e74b396a8e1c48a6889a965866ac0fb68c719a00711200bd53e3e198`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3605b0dd24d9612e9bf001c434a312571f6c91a4e4195d8fb584835cbdd08c`  
		Last Modified: Fri, 18 Mar 2022 10:11:27 GMT  
		Size: 116.3 MB (116342876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47eb45f708718a35b2c6e268082dd402aa16bdd526b8281bbb3516dd9ea94dd`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a218eaa26cbe5756270488eb0d4581c2492bf26490978b5865689c4382e79a`  
		Last Modified: Fri, 18 Mar 2022 10:11:53 GMT  
		Size: 98.8 MB (98783196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bb12bc5efca8d903bbcad7b07c2b6364116e17f95ba526498f9ec44b221bf7`  
		Last Modified: Fri, 18 Mar 2022 10:11:38 GMT  
		Size: 265.4 KB (265375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0592ca52bbeae58f9cb49bc8f6ffd5c7d0dc03b32866c15a0c71f72e67065bb`  
		Last Modified: Fri, 18 Mar 2022 10:11:37 GMT  
		Size: 2.2 KB (2211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2892c1ea6814cafa696c1dcecaa8e33cc43af83781038cd03b98a9ccefed59a`  
		Last Modified: Fri, 18 Mar 2022 10:11:43 GMT  
		Size: 22.7 MB (22737534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fcd2be142f079e58f2e96193cb417b4b27d3dc3d4dfa8c43c73ea7a6e428de1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.8 MB (267793838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a34026bc9d979398ca8a8f7a494b3e3cf61d68286e37065a5dd24790a4c71bf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:41:10 GMT
ADD file:c81be95ae491788086dc606dd86ac47b679f2ce48c96016d4ba321e995541bca in / 
# Fri, 18 Mar 2022 00:41:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:14:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:51 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:15:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:15:25 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:15:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:15:27 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 01:16:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:16:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:16:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:16:22 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:16:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:16:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Mar 2022 01:17:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 18 Mar 2022 01:17:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8037d5c930bd3f2cc0b5ef6849e32124c3c5efaf4389d0974934bba554464390`  
		Last Modified: Fri, 18 Mar 2022 00:43:17 GMT  
		Size: 28.4 MB (28425528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a2d6d51d5672d6a89bcd061ceb0abb70543ab14cf758b52dae0ea10a9ed89`  
		Last Modified: Fri, 18 Mar 2022 01:29:49 GMT  
		Size: 1.2 MB (1193964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a484c953b5a8ac5a49bdfa6ef2654513ce04b2c545724ed23887ed4e26ecf1e0`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 3.6 MB (3594382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c71cdbe64ce9e2a57214b4db9fcdfb68ece3c8c4d618cd6e7ca840103a663f3`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff9291a332798080bfb5b2e8ffa0d988a72c8939ca254eb21592d43f1716372`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b90c99c3d8313d7660084c587776cc644ff55ca2453c2b9abd86d7d6236df1`  
		Last Modified: Fri, 18 Mar 2022 01:30:05 GMT  
		Size: 116.0 MB (116006679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e2c942e9e5613f749e090c5d6e24e6309980924397b270887cdec8ef21a9a`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1ad18863e690660ff2da1cf5734414de53b7815bf58fcd1c7dbac36a107152`  
		Last Modified: Fri, 18 Mar 2022 01:30:31 GMT  
		Size: 96.2 MB (96155191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3c6b05283aa818a9d773afa7b1d3f5f76f2e8842f5ef23f90cc496c3d4dfca`  
		Last Modified: Fri, 18 Mar 2022 01:30:17 GMT  
		Size: 265.3 KB (265325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80fd2612b798c76dea877085bf4e5f263d60d4f6332625917549ce24ac497c1`  
		Last Modified: Fri, 18 Mar 2022 01:30:16 GMT  
		Size: 2.1 KB (2133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd394d49e57956f6844b2e0b95fb1dd971c02f60f1c5e3456cda64c0f5dd2f6`  
		Last Modified: Fri, 18 Mar 2022 01:30:20 GMT  
		Size: 22.1 MB (22148265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:0e7875d1f332c025ea2471dda47bc26e6b92ac8745391ba55f34fb877040b470
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:cc56027496019e29cb7f8c3c52c13533ab161b783d9f21986968cbe449d5d0c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.8 MB (151849868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e81171fdda7aceab141fe9243b1e1b064fab7d1ebe5f238ef7fdb2fcdd16e9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:31:09 GMT
ADD file:ce9bee138da151fa0b9e441f7ef06865e0171006e686f0dc5e1ca6a06e0a3d0c in / 
# Fri, 18 Mar 2022 05:31:09 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:53:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:54:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 09:56:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:56:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:56:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:56:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11581404396c9d08d16b97c64bb2fd043ef3216bd3e3ff3d1c6e03398dc8e336`  
		Last Modified: Wed, 16 Mar 2022 11:30:57 GMT  
		Size: 30.5 MB (30485551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d449d4c1f6f849759c38658c4e2053c7b2950c7f69d42c0fcdbd7fd490b7d`  
		Last Modified: Fri, 18 Mar 2022 10:11:05 GMT  
		Size: 1.2 MB (1192034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855467c60b27cd7745629db97415c3b46e1b14929c08528fe5e29366df56502c`  
		Last Modified: Fri, 18 Mar 2022 10:11:03 GMT  
		Size: 3.8 MB (3826992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6ac5bb5e9af926be15f77146a24734345444a1a6adaff26e3e6294242a743`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4282676e74b396a8e1c48a6889a965866ac0fb68c719a00711200bd53e3e198`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3605b0dd24d9612e9bf001c434a312571f6c91a4e4195d8fb584835cbdd08c`  
		Last Modified: Fri, 18 Mar 2022 10:11:27 GMT  
		Size: 116.3 MB (116342876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47eb45f708718a35b2c6e268082dd402aa16bdd526b8281bbb3516dd9ea94dd`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:33fb547172debbc26b8b51c53c0093dd61aa633905cd5c25497ebd7e3c174669
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.2 MB (149222924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8825532c46ae89a067cb23a4e016b986c597c0733c3bf539051d86d723235d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:41:10 GMT
ADD file:c81be95ae491788086dc606dd86ac47b679f2ce48c96016d4ba321e995541bca in / 
# Fri, 18 Mar 2022 00:41:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:14:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:51 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:15:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:15:25 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:15:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:15:27 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 01:16:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:16:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:16:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:16:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8037d5c930bd3f2cc0b5ef6849e32124c3c5efaf4389d0974934bba554464390`  
		Last Modified: Fri, 18 Mar 2022 00:43:17 GMT  
		Size: 28.4 MB (28425528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a2d6d51d5672d6a89bcd061ceb0abb70543ab14cf758b52dae0ea10a9ed89`  
		Last Modified: Fri, 18 Mar 2022 01:29:49 GMT  
		Size: 1.2 MB (1193964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a484c953b5a8ac5a49bdfa6ef2654513ce04b2c545724ed23887ed4e26ecf1e0`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 3.6 MB (3594382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c71cdbe64ce9e2a57214b4db9fcdfb68ece3c8c4d618cd6e7ca840103a663f3`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff9291a332798080bfb5b2e8ffa0d988a72c8939ca254eb21592d43f1716372`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b90c99c3d8313d7660084c587776cc644ff55ca2453c2b9abd86d7d6236df1`  
		Last Modified: Fri, 18 Mar 2022 01:30:05 GMT  
		Size: 116.0 MB (116006679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e2c942e9e5613f749e090c5d6e24e6309980924397b270887cdec8ef21a9a`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:0e7875d1f332c025ea2471dda47bc26e6b92ac8745391ba55f34fb877040b470
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:cc56027496019e29cb7f8c3c52c13533ab161b783d9f21986968cbe449d5d0c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.8 MB (151849868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e81171fdda7aceab141fe9243b1e1b064fab7d1ebe5f238ef7fdb2fcdd16e9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:31:09 GMT
ADD file:ce9bee138da151fa0b9e441f7ef06865e0171006e686f0dc5e1ca6a06e0a3d0c in / 
# Fri, 18 Mar 2022 05:31:09 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:53:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:54:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 09:56:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:56:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:56:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:56:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11581404396c9d08d16b97c64bb2fd043ef3216bd3e3ff3d1c6e03398dc8e336`  
		Last Modified: Wed, 16 Mar 2022 11:30:57 GMT  
		Size: 30.5 MB (30485551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d449d4c1f6f849759c38658c4e2053c7b2950c7f69d42c0fcdbd7fd490b7d`  
		Last Modified: Fri, 18 Mar 2022 10:11:05 GMT  
		Size: 1.2 MB (1192034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855467c60b27cd7745629db97415c3b46e1b14929c08528fe5e29366df56502c`  
		Last Modified: Fri, 18 Mar 2022 10:11:03 GMT  
		Size: 3.8 MB (3826992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6ac5bb5e9af926be15f77146a24734345444a1a6adaff26e3e6294242a743`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4282676e74b396a8e1c48a6889a965866ac0fb68c719a00711200bd53e3e198`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3605b0dd24d9612e9bf001c434a312571f6c91a4e4195d8fb584835cbdd08c`  
		Last Modified: Fri, 18 Mar 2022 10:11:27 GMT  
		Size: 116.3 MB (116342876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47eb45f708718a35b2c6e268082dd402aa16bdd526b8281bbb3516dd9ea94dd`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:33fb547172debbc26b8b51c53c0093dd61aa633905cd5c25497ebd7e3c174669
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.2 MB (149222924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8825532c46ae89a067cb23a4e016b986c597c0733c3bf539051d86d723235d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:41:10 GMT
ADD file:c81be95ae491788086dc606dd86ac47b679f2ce48c96016d4ba321e995541bca in / 
# Fri, 18 Mar 2022 00:41:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:14:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:51 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:15:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:15:25 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:15:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:15:27 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 01:16:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:16:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:16:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:16:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8037d5c930bd3f2cc0b5ef6849e32124c3c5efaf4389d0974934bba554464390`  
		Last Modified: Fri, 18 Mar 2022 00:43:17 GMT  
		Size: 28.4 MB (28425528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a2d6d51d5672d6a89bcd061ceb0abb70543ab14cf758b52dae0ea10a9ed89`  
		Last Modified: Fri, 18 Mar 2022 01:29:49 GMT  
		Size: 1.2 MB (1193964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a484c953b5a8ac5a49bdfa6ef2654513ce04b2c545724ed23887ed4e26ecf1e0`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 3.6 MB (3594382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c71cdbe64ce9e2a57214b4db9fcdfb68ece3c8c4d618cd6e7ca840103a663f3`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff9291a332798080bfb5b2e8ffa0d988a72c8939ca254eb21592d43f1716372`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b90c99c3d8313d7660084c587776cc644ff55ca2453c2b9abd86d7d6236df1`  
		Last Modified: Fri, 18 Mar 2022 01:30:05 GMT  
		Size: 116.0 MB (116006679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e2c942e9e5613f749e090c5d6e24e6309980924397b270887cdec8ef21a9a`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
