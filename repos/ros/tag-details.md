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
$ docker pull ros@sha256:e40e3f528095ad129694b2c686527cd7c231a9a773e76932f5a1dd7bad113cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:de88ec5f83170c16d3241172c0519b89558d52f0e307556e04f623c840266683
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236778688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15ea8872063a9a23fe47d2a8f855bdb84c4f8614b2a8a3c2f2e1b7df0db33743`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 04:23:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:24:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:24:00 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:24:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:25:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e5fcbc56cc018564403b3e0d7a2ba1c551dbbfef70614bab532a6cec5e4b17`  
		Last Modified: Fri, 07 Jan 2022 04:38:06 GMT  
		Size: 120.1 MB (120084781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca376e51cfddbb5565d4cb5bcd27b84bd29b7814c3a10f1f27d006fd2fdb5f57`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce6db45f220ec4a768963fbf00033b6f7591d9485c3aba2b9b1a4cded3c6e14`  
		Last Modified: Fri, 07 Jan 2022 04:38:27 GMT  
		Size: 70.9 MB (70857002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f29fb66d2b2ac4fc5c4792af937f08192b56597651670a8e9c50033168736ea`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 248.0 KB (247988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c59003bb7bd2d1ecbcb0ce6a54795c7047db81b534f807837c0b56db2f43b`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d2c6e532f1e832e4514e246cdd3c73654b2e2d065e9170ef5b28dac48ba046`  
		Last Modified: Fri, 07 Jan 2022 04:38:19 GMT  
		Size: 10.3 MB (10288814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:031ec1bef47d9c2d25fd78ae182c1bdac1c1de258fcd3925162b0a98dd8792ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212273414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958ce2ddd377dc731b4732ae55d2f375b8ae2d965f3f9b32be19343692906066`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:21:33 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 03:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:22:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:22:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:22:29 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:23:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:23:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:23:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:23:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66a92a9fd6a8886d123d670db5303b8dd67ddd77a81725baeb2a0b505ced2a`  
		Last Modified: Fri, 07 Jan 2022 03:38:30 GMT  
		Size: 104.3 MB (104278769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff28861e6a517aa6142fc99de642cca95e1dd5a89fd9ed6a6b91f4fb027858c9`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e70d35be41ad697b7032634ba5ac686f40fb7d1f3a3831d3ab3bd181700f2`  
		Last Modified: Fri, 07 Jan 2022 03:38:52 GMT  
		Size: 65.0 MB (64978411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4de71e579016c7dd5135332644ab4822e7de561bf903b27f4b7abf4463d2e9a`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 247.9 KB (247929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c68e716a4fe65ae789bc8663115985441757e1dd471ceb660c034af46acb3`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff754c55fcced401707c7c7c28dee657d3c984b05bd0eb84f455b7a34e8838`  
		Last Modified: Fri, 07 Jan 2022 03:38:44 GMT  
		Size: 9.1 MB (9086053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:e40e3f528095ad129694b2c686527cd7c231a9a773e76932f5a1dd7bad113cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:de88ec5f83170c16d3241172c0519b89558d52f0e307556e04f623c840266683
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236778688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15ea8872063a9a23fe47d2a8f855bdb84c4f8614b2a8a3c2f2e1b7df0db33743`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 04:23:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:24:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:24:00 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:24:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:25:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e5fcbc56cc018564403b3e0d7a2ba1c551dbbfef70614bab532a6cec5e4b17`  
		Last Modified: Fri, 07 Jan 2022 04:38:06 GMT  
		Size: 120.1 MB (120084781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca376e51cfddbb5565d4cb5bcd27b84bd29b7814c3a10f1f27d006fd2fdb5f57`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce6db45f220ec4a768963fbf00033b6f7591d9485c3aba2b9b1a4cded3c6e14`  
		Last Modified: Fri, 07 Jan 2022 04:38:27 GMT  
		Size: 70.9 MB (70857002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f29fb66d2b2ac4fc5c4792af937f08192b56597651670a8e9c50033168736ea`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 248.0 KB (247988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c59003bb7bd2d1ecbcb0ce6a54795c7047db81b534f807837c0b56db2f43b`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d2c6e532f1e832e4514e246cdd3c73654b2e2d065e9170ef5b28dac48ba046`  
		Last Modified: Fri, 07 Jan 2022 04:38:19 GMT  
		Size: 10.3 MB (10288814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:031ec1bef47d9c2d25fd78ae182c1bdac1c1de258fcd3925162b0a98dd8792ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212273414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958ce2ddd377dc731b4732ae55d2f375b8ae2d965f3f9b32be19343692906066`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:21:33 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 03:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:22:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:22:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:22:29 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:23:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:23:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:23:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:23:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66a92a9fd6a8886d123d670db5303b8dd67ddd77a81725baeb2a0b505ced2a`  
		Last Modified: Fri, 07 Jan 2022 03:38:30 GMT  
		Size: 104.3 MB (104278769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff28861e6a517aa6142fc99de642cca95e1dd5a89fd9ed6a6b91f4fb027858c9`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e70d35be41ad697b7032634ba5ac686f40fb7d1f3a3831d3ab3bd181700f2`  
		Last Modified: Fri, 07 Jan 2022 03:38:52 GMT  
		Size: 65.0 MB (64978411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4de71e579016c7dd5135332644ab4822e7de561bf903b27f4b7abf4463d2e9a`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 247.9 KB (247929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c68e716a4fe65ae789bc8663115985441757e1dd471ceb660c034af46acb3`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff754c55fcced401707c7c7c28dee657d3c984b05bd0eb84f455b7a34e8838`  
		Last Modified: Fri, 07 Jan 2022 03:38:44 GMT  
		Size: 9.1 MB (9086053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:e40e3f528095ad129694b2c686527cd7c231a9a773e76932f5a1dd7bad113cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:de88ec5f83170c16d3241172c0519b89558d52f0e307556e04f623c840266683
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236778688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15ea8872063a9a23fe47d2a8f855bdb84c4f8614b2a8a3c2f2e1b7df0db33743`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 04:23:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:24:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:24:00 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:24:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:25:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e5fcbc56cc018564403b3e0d7a2ba1c551dbbfef70614bab532a6cec5e4b17`  
		Last Modified: Fri, 07 Jan 2022 04:38:06 GMT  
		Size: 120.1 MB (120084781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca376e51cfddbb5565d4cb5bcd27b84bd29b7814c3a10f1f27d006fd2fdb5f57`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce6db45f220ec4a768963fbf00033b6f7591d9485c3aba2b9b1a4cded3c6e14`  
		Last Modified: Fri, 07 Jan 2022 04:38:27 GMT  
		Size: 70.9 MB (70857002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f29fb66d2b2ac4fc5c4792af937f08192b56597651670a8e9c50033168736ea`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 248.0 KB (247988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c59003bb7bd2d1ecbcb0ce6a54795c7047db81b534f807837c0b56db2f43b`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d2c6e532f1e832e4514e246cdd3c73654b2e2d065e9170ef5b28dac48ba046`  
		Last Modified: Fri, 07 Jan 2022 04:38:19 GMT  
		Size: 10.3 MB (10288814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:031ec1bef47d9c2d25fd78ae182c1bdac1c1de258fcd3925162b0a98dd8792ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212273414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958ce2ddd377dc731b4732ae55d2f375b8ae2d965f3f9b32be19343692906066`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:21:33 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 03:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:22:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:22:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:22:29 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:23:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:23:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:23:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:23:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66a92a9fd6a8886d123d670db5303b8dd67ddd77a81725baeb2a0b505ced2a`  
		Last Modified: Fri, 07 Jan 2022 03:38:30 GMT  
		Size: 104.3 MB (104278769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff28861e6a517aa6142fc99de642cca95e1dd5a89fd9ed6a6b91f4fb027858c9`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e70d35be41ad697b7032634ba5ac686f40fb7d1f3a3831d3ab3bd181700f2`  
		Last Modified: Fri, 07 Jan 2022 03:38:52 GMT  
		Size: 65.0 MB (64978411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4de71e579016c7dd5135332644ab4822e7de561bf903b27f4b7abf4463d2e9a`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 247.9 KB (247929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c68e716a4fe65ae789bc8663115985441757e1dd471ceb660c034af46acb3`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff754c55fcced401707c7c7c28dee657d3c984b05bd0eb84f455b7a34e8838`  
		Last Modified: Fri, 07 Jan 2022 03:38:44 GMT  
		Size: 9.1 MB (9086053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:67ea1ec506b2b134928ddf3a7bc27f286c33192d30f36ac956768fe5d38acf83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:592aa96c4bed38273f9db0806f8d68680cdd69d516b6baa7630b2258015d9a38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155382797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45bc46b6422cd2f63f97602b1eebc864c6fa256f599b9ba1ef116a92ffc9d928`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 04:23:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:24:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:24:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e5fcbc56cc018564403b3e0d7a2ba1c551dbbfef70614bab532a6cec5e4b17`  
		Last Modified: Fri, 07 Jan 2022 04:38:06 GMT  
		Size: 120.1 MB (120084781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca376e51cfddbb5565d4cb5bcd27b84bd29b7814c3a10f1f27d006fd2fdb5f57`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7f880c87a1212402733ced060c175cd0f25f941b385342f95b2e18cdd80d9721
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137958981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f49ee6b978d8824f20fab73ce324f315c5754ffbd0c2cf5d844cb46c111b48a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:21:33 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 03:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:22:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:22:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:22:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66a92a9fd6a8886d123d670db5303b8dd67ddd77a81725baeb2a0b505ced2a`  
		Last Modified: Fri, 07 Jan 2022 03:38:30 GMT  
		Size: 104.3 MB (104278769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff28861e6a517aa6142fc99de642cca95e1dd5a89fd9ed6a6b91f4fb027858c9`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:67ea1ec506b2b134928ddf3a7bc27f286c33192d30f36ac956768fe5d38acf83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:592aa96c4bed38273f9db0806f8d68680cdd69d516b6baa7630b2258015d9a38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155382797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45bc46b6422cd2f63f97602b1eebc864c6fa256f599b9ba1ef116a92ffc9d928`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 04:23:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:24:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:24:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e5fcbc56cc018564403b3e0d7a2ba1c551dbbfef70614bab532a6cec5e4b17`  
		Last Modified: Fri, 07 Jan 2022 04:38:06 GMT  
		Size: 120.1 MB (120084781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca376e51cfddbb5565d4cb5bcd27b84bd29b7814c3a10f1f27d006fd2fdb5f57`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7f880c87a1212402733ced060c175cd0f25f941b385342f95b2e18cdd80d9721
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137958981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f49ee6b978d8824f20fab73ce324f315c5754ffbd0c2cf5d844cb46c111b48a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:21:33 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 03:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:22:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:22:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:22:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66a92a9fd6a8886d123d670db5303b8dd67ddd77a81725baeb2a0b505ced2a`  
		Last Modified: Fri, 07 Jan 2022 03:38:30 GMT  
		Size: 104.3 MB (104278769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff28861e6a517aa6142fc99de642cca95e1dd5a89fd9ed6a6b91f4fb027858c9`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:a3df82bdc0575212c2c93d8913ee05dbdab624054a83722827254444b7631f98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:7e4e7383fed8cee2b9d167e06cde05d491831e9e30d63a0821b98171f4c50030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.8 MB (345848796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bd2e2e4147eacb183e28e50658cb81c5fbd606a8553f8a7f55a1424cf1c627`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 04:23:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:24:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:24:00 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:24:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:25:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:25:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:25:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:25:16 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 04:25:16 GMT
ENV ROS2_DISTRO=foxy
# Mon, 24 Jan 2022 19:54:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:55:07 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e5fcbc56cc018564403b3e0d7a2ba1c551dbbfef70614bab532a6cec5e4b17`  
		Last Modified: Fri, 07 Jan 2022 04:38:06 GMT  
		Size: 120.1 MB (120084781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca376e51cfddbb5565d4cb5bcd27b84bd29b7814c3a10f1f27d006fd2fdb5f57`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce6db45f220ec4a768963fbf00033b6f7591d9485c3aba2b9b1a4cded3c6e14`  
		Last Modified: Fri, 07 Jan 2022 04:38:27 GMT  
		Size: 70.9 MB (70857002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f29fb66d2b2ac4fc5c4792af937f08192b56597651670a8e9c50033168736ea`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 248.0 KB (247988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c59003bb7bd2d1ecbcb0ce6a54795c7047db81b534f807837c0b56db2f43b`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d2c6e532f1e832e4514e246cdd3c73654b2e2d065e9170ef5b28dac48ba046`  
		Last Modified: Fri, 07 Jan 2022 04:38:19 GMT  
		Size: 10.3 MB (10288814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a848922735be67a54da86ca5c12bfe94a37cafbf38338666e4b357e52d33459d`  
		Last Modified: Fri, 07 Jan 2022 04:38:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0188b8603e20cb241ba9ee2a4f803df3998bc141216a82eb0d648cecd27192d8`  
		Last Modified: Fri, 07 Jan 2022 04:38:45 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad26c3ba95887e9d9a232ed2fb9039fbf21eb3abdad27a42ab509d96bcaf54d9`  
		Last Modified: Mon, 24 Jan 2022 19:58:28 GMT  
		Size: 76.3 MB (76299062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ce84cd827cee158a64f76e9d1b2f00cb8e4db650a0d0d72a08ae1d45de8b1e`  
		Last Modified: Mon, 24 Jan 2022 19:58:20 GMT  
		Size: 32.8 MB (32770419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b00db5d24916e607219b0d993ab2db6c4ffdf0226a9da7720ce3140afa3bce`  
		Last Modified: Mon, 24 Jan 2022 19:58:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a18804a2a518af9798d39fbe5f39b64383e9e023e1764caef793eb60c798f5a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.5 MB (313538491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6168480373001075297888d07b8d08b37750838020b328b0ce486a6796bc12`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:21:33 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 03:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:22:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:22:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:22:29 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:23:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:23:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:23:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:23:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:23:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:23:44 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 03:23:45 GMT
ENV ROS2_DISTRO=foxy
# Mon, 24 Jan 2022 19:42:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:43:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:43:07 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66a92a9fd6a8886d123d670db5303b8dd67ddd77a81725baeb2a0b505ced2a`  
		Last Modified: Fri, 07 Jan 2022 03:38:30 GMT  
		Size: 104.3 MB (104278769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff28861e6a517aa6142fc99de642cca95e1dd5a89fd9ed6a6b91f4fb027858c9`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e70d35be41ad697b7032634ba5ac686f40fb7d1f3a3831d3ab3bd181700f2`  
		Last Modified: Fri, 07 Jan 2022 03:38:52 GMT  
		Size: 65.0 MB (64978411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4de71e579016c7dd5135332644ab4822e7de561bf903b27f4b7abf4463d2e9a`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 247.9 KB (247929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c68e716a4fe65ae789bc8663115985441757e1dd471ceb660c034af46acb3`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff754c55fcced401707c7c7c28dee657d3c984b05bd0eb84f455b7a34e8838`  
		Last Modified: Fri, 07 Jan 2022 03:38:44 GMT  
		Size: 9.1 MB (9086053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be18a064e2514eca521a6cc4d9b7040766b8757c57d4eead497cd00bbb3bc5ad`  
		Last Modified: Fri, 07 Jan 2022 03:39:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daf43f23dfa0d1beee60a93e52efc0607fc08a36a3c62779e10e1317c36893c`  
		Last Modified: Mon, 24 Jan 2022 19:47:46 GMT  
		Size: 76.1 MB (76131997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212510fdafe6dea26fc145d19d916b9e58279f23b1a0dc98a8f1bd2e0f3cbf8d`  
		Last Modified: Mon, 24 Jan 2022 19:47:35 GMT  
		Size: 25.1 MB (25132608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0e4bdfc786c2b4b9ac562a138d2a215c5de2a3f0c2ac4f9b21b008695141e8`  
		Last Modified: Mon, 24 Jan 2022 19:47:31 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:a3df82bdc0575212c2c93d8913ee05dbdab624054a83722827254444b7631f98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:7e4e7383fed8cee2b9d167e06cde05d491831e9e30d63a0821b98171f4c50030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.8 MB (345848796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bd2e2e4147eacb183e28e50658cb81c5fbd606a8553f8a7f55a1424cf1c627`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 04:23:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:24:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:24:00 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:24:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:25:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:25:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:25:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:25:16 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 04:25:16 GMT
ENV ROS2_DISTRO=foxy
# Mon, 24 Jan 2022 19:54:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:55:07 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e5fcbc56cc018564403b3e0d7a2ba1c551dbbfef70614bab532a6cec5e4b17`  
		Last Modified: Fri, 07 Jan 2022 04:38:06 GMT  
		Size: 120.1 MB (120084781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca376e51cfddbb5565d4cb5bcd27b84bd29b7814c3a10f1f27d006fd2fdb5f57`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce6db45f220ec4a768963fbf00033b6f7591d9485c3aba2b9b1a4cded3c6e14`  
		Last Modified: Fri, 07 Jan 2022 04:38:27 GMT  
		Size: 70.9 MB (70857002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f29fb66d2b2ac4fc5c4792af937f08192b56597651670a8e9c50033168736ea`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 248.0 KB (247988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c59003bb7bd2d1ecbcb0ce6a54795c7047db81b534f807837c0b56db2f43b`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d2c6e532f1e832e4514e246cdd3c73654b2e2d065e9170ef5b28dac48ba046`  
		Last Modified: Fri, 07 Jan 2022 04:38:19 GMT  
		Size: 10.3 MB (10288814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a848922735be67a54da86ca5c12bfe94a37cafbf38338666e4b357e52d33459d`  
		Last Modified: Fri, 07 Jan 2022 04:38:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0188b8603e20cb241ba9ee2a4f803df3998bc141216a82eb0d648cecd27192d8`  
		Last Modified: Fri, 07 Jan 2022 04:38:45 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad26c3ba95887e9d9a232ed2fb9039fbf21eb3abdad27a42ab509d96bcaf54d9`  
		Last Modified: Mon, 24 Jan 2022 19:58:28 GMT  
		Size: 76.3 MB (76299062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ce84cd827cee158a64f76e9d1b2f00cb8e4db650a0d0d72a08ae1d45de8b1e`  
		Last Modified: Mon, 24 Jan 2022 19:58:20 GMT  
		Size: 32.8 MB (32770419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b00db5d24916e607219b0d993ab2db6c4ffdf0226a9da7720ce3140afa3bce`  
		Last Modified: Mon, 24 Jan 2022 19:58:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a18804a2a518af9798d39fbe5f39b64383e9e023e1764caef793eb60c798f5a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.5 MB (313538491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6168480373001075297888d07b8d08b37750838020b328b0ce486a6796bc12`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:21:33 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 03:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:22:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:22:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:22:29 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:23:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:23:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:23:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:23:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:23:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:23:44 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 03:23:45 GMT
ENV ROS2_DISTRO=foxy
# Mon, 24 Jan 2022 19:42:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:43:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:43:07 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66a92a9fd6a8886d123d670db5303b8dd67ddd77a81725baeb2a0b505ced2a`  
		Last Modified: Fri, 07 Jan 2022 03:38:30 GMT  
		Size: 104.3 MB (104278769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff28861e6a517aa6142fc99de642cca95e1dd5a89fd9ed6a6b91f4fb027858c9`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e70d35be41ad697b7032634ba5ac686f40fb7d1f3a3831d3ab3bd181700f2`  
		Last Modified: Fri, 07 Jan 2022 03:38:52 GMT  
		Size: 65.0 MB (64978411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4de71e579016c7dd5135332644ab4822e7de561bf903b27f4b7abf4463d2e9a`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 247.9 KB (247929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c68e716a4fe65ae789bc8663115985441757e1dd471ceb660c034af46acb3`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff754c55fcced401707c7c7c28dee657d3c984b05bd0eb84f455b7a34e8838`  
		Last Modified: Fri, 07 Jan 2022 03:38:44 GMT  
		Size: 9.1 MB (9086053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be18a064e2514eca521a6cc4d9b7040766b8757c57d4eead497cd00bbb3bc5ad`  
		Last Modified: Fri, 07 Jan 2022 03:39:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daf43f23dfa0d1beee60a93e52efc0607fc08a36a3c62779e10e1317c36893c`  
		Last Modified: Mon, 24 Jan 2022 19:47:46 GMT  
		Size: 76.1 MB (76131997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212510fdafe6dea26fc145d19d916b9e58279f23b1a0dc98a8f1bd2e0f3cbf8d`  
		Last Modified: Mon, 24 Jan 2022 19:47:35 GMT  
		Size: 25.1 MB (25132608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0e4bdfc786c2b4b9ac562a138d2a215c5de2a3f0c2ac4f9b21b008695141e8`  
		Last Modified: Mon, 24 Jan 2022 19:47:31 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:f08c9bf0d5b14a7de1d8e1c657d7a15b0b6e4068c0c6c493710609b2dd451706
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:d52ee1b0d65d7df83a4897c39568d6a450a10d76c330450c90ae0e79e4c0d2a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232134139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e1993371ff82346bdcf8ea1a5fab45a153980926422cb292e7ab6c883b2386b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:26:06 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 04:26:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:26:51 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:27:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:27:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:27:20 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:27:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063d0746de5719c9156895722399b01972416e0e80c658155982c00200f443a6`  
		Last Modified: Fri, 07 Jan 2022 04:39:27 GMT  
		Size: 103.7 MB (103658457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc154cdc673512ad761544d2fcd686eb54be2f05bb2979f99ce88721916b3292`  
		Last Modified: Fri, 07 Jan 2022 04:39:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1649390eb8dcd2fe6e5c6ad2852f46c75286c1f2aa6e823189e62a9bd8f5b48`  
		Last Modified: Fri, 07 Jan 2022 04:39:47 GMT  
		Size: 70.8 MB (70809018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e5b5f85fd50dc8f63a00fe68c4f8868cf1630d84d9376b50105e52b86be46`  
		Last Modified: Fri, 07 Jan 2022 04:39:37 GMT  
		Size: 256.5 KB (256531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359e6648253521fa3d50934dd6fbc1fea6cc84b875fe7767fe4c6c432a0269f9`  
		Last Modified: Fri, 07 Jan 2022 04:39:37 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad327712cfc9c7179f06c300cf31922d30a760439761d2e0f603970aca6cb12`  
		Last Modified: Fri, 07 Jan 2022 04:39:40 GMT  
		Size: 22.1 MB (22110051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:145e83c2b57018c4bc6a727dbf07a982bebec73787e781e8ee90f28ac5a0e9af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.3 MB (220334485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775c4b4329a07a55b93057468a54ea7b064239f59da3d544cf6e865a43e89aca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:25:03 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 03:25:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:25:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:25:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:25:57 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:26:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:26:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9bb206bac894b41230de1b372cdfd2492571d0b1c1ec86904932c7374bbc06`  
		Last Modified: Fri, 07 Jan 2022 03:39:54 GMT  
		Size: 100.0 MB (100036692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9173d5fa207ed202cce7d701cf4f3a127f3ae3d247c1b3573a2fb6f4e404c2f`  
		Last Modified: Fri, 07 Jan 2022 03:39:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03661c68c764e1b462e8b4d59a1451a2e740012fac57cf6aaafc9cb6fae6d43b`  
		Last Modified: Fri, 07 Jan 2022 03:40:16 GMT  
		Size: 64.9 MB (64932295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ac2e61c69997f1e16aabf40bace777ed589f95ec842fbe63614cb66260b653`  
		Last Modified: Fri, 07 Jan 2022 03:40:06 GMT  
		Size: 256.5 KB (256483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74e2289bc0665dd9b4e3a6bb89203e323516e31f58b9ead5b87e36bd3f8a15e`  
		Last Modified: Fri, 07 Jan 2022 03:40:06 GMT  
		Size: 2.0 KB (2015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb713b315270cfa8e2114ba6e2666e342cd902c9b34683b86073a68a21910d41`  
		Last Modified: Fri, 07 Jan 2022 03:40:09 GMT  
		Size: 21.4 MB (21426788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:f08c9bf0d5b14a7de1d8e1c657d7a15b0b6e4068c0c6c493710609b2dd451706
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:d52ee1b0d65d7df83a4897c39568d6a450a10d76c330450c90ae0e79e4c0d2a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232134139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e1993371ff82346bdcf8ea1a5fab45a153980926422cb292e7ab6c883b2386b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:26:06 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 04:26:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:26:51 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:27:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:27:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:27:20 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:27:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063d0746de5719c9156895722399b01972416e0e80c658155982c00200f443a6`  
		Last Modified: Fri, 07 Jan 2022 04:39:27 GMT  
		Size: 103.7 MB (103658457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc154cdc673512ad761544d2fcd686eb54be2f05bb2979f99ce88721916b3292`  
		Last Modified: Fri, 07 Jan 2022 04:39:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1649390eb8dcd2fe6e5c6ad2852f46c75286c1f2aa6e823189e62a9bd8f5b48`  
		Last Modified: Fri, 07 Jan 2022 04:39:47 GMT  
		Size: 70.8 MB (70809018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e5b5f85fd50dc8f63a00fe68c4f8868cf1630d84d9376b50105e52b86be46`  
		Last Modified: Fri, 07 Jan 2022 04:39:37 GMT  
		Size: 256.5 KB (256531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359e6648253521fa3d50934dd6fbc1fea6cc84b875fe7767fe4c6c432a0269f9`  
		Last Modified: Fri, 07 Jan 2022 04:39:37 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad327712cfc9c7179f06c300cf31922d30a760439761d2e0f603970aca6cb12`  
		Last Modified: Fri, 07 Jan 2022 04:39:40 GMT  
		Size: 22.1 MB (22110051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:145e83c2b57018c4bc6a727dbf07a982bebec73787e781e8ee90f28ac5a0e9af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.3 MB (220334485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775c4b4329a07a55b93057468a54ea7b064239f59da3d544cf6e865a43e89aca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:25:03 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 03:25:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:25:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:25:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:25:57 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:26:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:26:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9bb206bac894b41230de1b372cdfd2492571d0b1c1ec86904932c7374bbc06`  
		Last Modified: Fri, 07 Jan 2022 03:39:54 GMT  
		Size: 100.0 MB (100036692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9173d5fa207ed202cce7d701cf4f3a127f3ae3d247c1b3573a2fb6f4e404c2f`  
		Last Modified: Fri, 07 Jan 2022 03:39:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03661c68c764e1b462e8b4d59a1451a2e740012fac57cf6aaafc9cb6fae6d43b`  
		Last Modified: Fri, 07 Jan 2022 03:40:16 GMT  
		Size: 64.9 MB (64932295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ac2e61c69997f1e16aabf40bace777ed589f95ec842fbe63614cb66260b653`  
		Last Modified: Fri, 07 Jan 2022 03:40:06 GMT  
		Size: 256.5 KB (256483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74e2289bc0665dd9b4e3a6bb89203e323516e31f58b9ead5b87e36bd3f8a15e`  
		Last Modified: Fri, 07 Jan 2022 03:40:06 GMT  
		Size: 2.0 KB (2015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb713b315270cfa8e2114ba6e2666e342cd902c9b34683b86073a68a21910d41`  
		Last Modified: Fri, 07 Jan 2022 03:40:09 GMT  
		Size: 21.4 MB (21426788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:f08c9bf0d5b14a7de1d8e1c657d7a15b0b6e4068c0c6c493710609b2dd451706
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:d52ee1b0d65d7df83a4897c39568d6a450a10d76c330450c90ae0e79e4c0d2a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232134139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e1993371ff82346bdcf8ea1a5fab45a153980926422cb292e7ab6c883b2386b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:26:06 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 04:26:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:26:51 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:27:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:27:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:27:20 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:27:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063d0746de5719c9156895722399b01972416e0e80c658155982c00200f443a6`  
		Last Modified: Fri, 07 Jan 2022 04:39:27 GMT  
		Size: 103.7 MB (103658457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc154cdc673512ad761544d2fcd686eb54be2f05bb2979f99ce88721916b3292`  
		Last Modified: Fri, 07 Jan 2022 04:39:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1649390eb8dcd2fe6e5c6ad2852f46c75286c1f2aa6e823189e62a9bd8f5b48`  
		Last Modified: Fri, 07 Jan 2022 04:39:47 GMT  
		Size: 70.8 MB (70809018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e5b5f85fd50dc8f63a00fe68c4f8868cf1630d84d9376b50105e52b86be46`  
		Last Modified: Fri, 07 Jan 2022 04:39:37 GMT  
		Size: 256.5 KB (256531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359e6648253521fa3d50934dd6fbc1fea6cc84b875fe7767fe4c6c432a0269f9`  
		Last Modified: Fri, 07 Jan 2022 04:39:37 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad327712cfc9c7179f06c300cf31922d30a760439761d2e0f603970aca6cb12`  
		Last Modified: Fri, 07 Jan 2022 04:39:40 GMT  
		Size: 22.1 MB (22110051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:145e83c2b57018c4bc6a727dbf07a982bebec73787e781e8ee90f28ac5a0e9af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.3 MB (220334485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775c4b4329a07a55b93057468a54ea7b064239f59da3d544cf6e865a43e89aca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:25:03 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 03:25:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:25:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:25:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:25:57 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:26:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:26:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9bb206bac894b41230de1b372cdfd2492571d0b1c1ec86904932c7374bbc06`  
		Last Modified: Fri, 07 Jan 2022 03:39:54 GMT  
		Size: 100.0 MB (100036692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9173d5fa207ed202cce7d701cf4f3a127f3ae3d247c1b3573a2fb6f4e404c2f`  
		Last Modified: Fri, 07 Jan 2022 03:39:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03661c68c764e1b462e8b4d59a1451a2e740012fac57cf6aaafc9cb6fae6d43b`  
		Last Modified: Fri, 07 Jan 2022 03:40:16 GMT  
		Size: 64.9 MB (64932295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ac2e61c69997f1e16aabf40bace777ed589f95ec842fbe63614cb66260b653`  
		Last Modified: Fri, 07 Jan 2022 03:40:06 GMT  
		Size: 256.5 KB (256483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74e2289bc0665dd9b4e3a6bb89203e323516e31f58b9ead5b87e36bd3f8a15e`  
		Last Modified: Fri, 07 Jan 2022 03:40:06 GMT  
		Size: 2.0 KB (2015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb713b315270cfa8e2114ba6e2666e342cd902c9b34683b86073a68a21910d41`  
		Last Modified: Fri, 07 Jan 2022 03:40:09 GMT  
		Size: 21.4 MB (21426788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:98e57821876dae1a4cf9433dd1d033ce7f97483d9148085e1ebccf4b805cec93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:ed03b07f7560de940d550373f5e8ec036e46265ffa43e8629579c2d38c99d240
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138956473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49ad3d18244cb8aca811a5a190664f0ad5431a4f2be9c052d40d9f5d958bc706`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:26:06 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 04:26:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:26:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063d0746de5719c9156895722399b01972416e0e80c658155982c00200f443a6`  
		Last Modified: Fri, 07 Jan 2022 04:39:27 GMT  
		Size: 103.7 MB (103658457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc154cdc673512ad761544d2fcd686eb54be2f05bb2979f99ce88721916b3292`  
		Last Modified: Fri, 07 Jan 2022 04:39:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bf74caf34c33125b891d1c600725006b4fdb31d3ec0861601699d498f39bbcdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133716904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe1d857d72a744668a6b9cd01ce466357c741384d14ebbd333abd13ab83d183`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:25:03 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 03:25:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:25:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:25:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:25:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9bb206bac894b41230de1b372cdfd2492571d0b1c1ec86904932c7374bbc06`  
		Last Modified: Fri, 07 Jan 2022 03:39:54 GMT  
		Size: 100.0 MB (100036692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9173d5fa207ed202cce7d701cf4f3a127f3ae3d247c1b3573a2fb6f4e404c2f`  
		Last Modified: Fri, 07 Jan 2022 03:39:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:98e57821876dae1a4cf9433dd1d033ce7f97483d9148085e1ebccf4b805cec93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:ed03b07f7560de940d550373f5e8ec036e46265ffa43e8629579c2d38c99d240
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138956473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49ad3d18244cb8aca811a5a190664f0ad5431a4f2be9c052d40d9f5d958bc706`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:26:06 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 04:26:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:26:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063d0746de5719c9156895722399b01972416e0e80c658155982c00200f443a6`  
		Last Modified: Fri, 07 Jan 2022 04:39:27 GMT  
		Size: 103.7 MB (103658457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc154cdc673512ad761544d2fcd686eb54be2f05bb2979f99ce88721916b3292`  
		Last Modified: Fri, 07 Jan 2022 04:39:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bf74caf34c33125b891d1c600725006b4fdb31d3ec0861601699d498f39bbcdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133716904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe1d857d72a744668a6b9cd01ce466357c741384d14ebbd333abd13ab83d183`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:25:03 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 03:25:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:25:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:25:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:25:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9bb206bac894b41230de1b372cdfd2492571d0b1c1ec86904932c7374bbc06`  
		Last Modified: Fri, 07 Jan 2022 03:39:54 GMT  
		Size: 100.0 MB (100036692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9173d5fa207ed202cce7d701cf4f3a127f3ae3d247c1b3573a2fb6f4e404c2f`  
		Last Modified: Fri, 07 Jan 2022 03:39:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:c65a3b687a783519de8d8e3a911cd0f6872ff7125850e08409c36dd4e55ddf76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:f3f0e6317bbe74b9a8c4ac862b42090308aacd992466af0c8a6dbc6c4170b37b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.1 MB (327098631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e836c552d83df196ee1273a50296503f0a3f5d162a0f650c3672621f03cfb1f2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:26:06 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 04:26:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:26:51 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:27:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:27:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:27:20 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:27:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:27:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:27:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:27:52 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 04:27:52 GMT
ENV ROS2_DISTRO=galactic
# Mon, 24 Jan 2022 19:55:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:55:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:55:55 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063d0746de5719c9156895722399b01972416e0e80c658155982c00200f443a6`  
		Last Modified: Fri, 07 Jan 2022 04:39:27 GMT  
		Size: 103.7 MB (103658457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc154cdc673512ad761544d2fcd686eb54be2f05bb2979f99ce88721916b3292`  
		Last Modified: Fri, 07 Jan 2022 04:39:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1649390eb8dcd2fe6e5c6ad2852f46c75286c1f2aa6e823189e62a9bd8f5b48`  
		Last Modified: Fri, 07 Jan 2022 04:39:47 GMT  
		Size: 70.8 MB (70809018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e5b5f85fd50dc8f63a00fe68c4f8868cf1630d84d9376b50105e52b86be46`  
		Last Modified: Fri, 07 Jan 2022 04:39:37 GMT  
		Size: 256.5 KB (256531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359e6648253521fa3d50934dd6fbc1fea6cc84b875fe7767fe4c6c432a0269f9`  
		Last Modified: Fri, 07 Jan 2022 04:39:37 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad327712cfc9c7179f06c300cf31922d30a760439761d2e0f603970aca6cb12`  
		Last Modified: Fri, 07 Jan 2022 04:39:40 GMT  
		Size: 22.1 MB (22110051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85215c58e455a99da7ddf6c775a7e8063bbefa1294015bb699213b9b32e08fdc`  
		Last Modified: Fri, 07 Jan 2022 04:40:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fc1f54e736214a55d34a88c31251a566f91c74ef68e7e999efcd29e93047c5`  
		Last Modified: Fri, 07 Jan 2022 04:40:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e95fceab9e4912b17705a1f8a816a4e7bf235c343682349d1c1a7207237078`  
		Last Modified: Mon, 24 Jan 2022 19:59:32 GMT  
		Size: 78.6 MB (78593060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c55525cd5db9326521f64572a36e4aff757bb928f982c850716f841f2da7cc`  
		Last Modified: Mon, 24 Jan 2022 19:59:19 GMT  
		Size: 16.4 MB (16370804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ce02495efa50cab0b55008267b6caa56f5748eecf137740528f252c5549192`  
		Last Modified: Mon, 24 Jan 2022 19:59:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ae7e37d62db89fb08df1cf6c1896a7f93b44a2344144d377a7268cd25bbc7438
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.3 MB (314329011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d5dc4c139326e993d698dd5620269a9f553f75d20df50b38a20ae47f66d521`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:25:03 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 03:25:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:25:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:25:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:25:57 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:26:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:26:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:27:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:27:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:27:16 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 03:27:17 GMT
ENV ROS2_DISTRO=galactic
# Mon, 24 Jan 2022 19:44:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:44:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:44:28 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9bb206bac894b41230de1b372cdfd2492571d0b1c1ec86904932c7374bbc06`  
		Last Modified: Fri, 07 Jan 2022 03:39:54 GMT  
		Size: 100.0 MB (100036692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9173d5fa207ed202cce7d701cf4f3a127f3ae3d247c1b3573a2fb6f4e404c2f`  
		Last Modified: Fri, 07 Jan 2022 03:39:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03661c68c764e1b462e8b4d59a1451a2e740012fac57cf6aaafc9cb6fae6d43b`  
		Last Modified: Fri, 07 Jan 2022 03:40:16 GMT  
		Size: 64.9 MB (64932295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ac2e61c69997f1e16aabf40bace777ed589f95ec842fbe63614cb66260b653`  
		Last Modified: Fri, 07 Jan 2022 03:40:06 GMT  
		Size: 256.5 KB (256483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74e2289bc0665dd9b4e3a6bb89203e323516e31f58b9ead5b87e36bd3f8a15e`  
		Last Modified: Fri, 07 Jan 2022 03:40:06 GMT  
		Size: 2.0 KB (2015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb713b315270cfa8e2114ba6e2666e342cd902c9b34683b86073a68a21910d41`  
		Last Modified: Fri, 07 Jan 2022 03:40:09 GMT  
		Size: 21.4 MB (21426788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d837971b2f51e4c13fd2b39f61daf5732be9e74307a34ab7099eafb1510782`  
		Last Modified: Fri, 07 Jan 2022 03:40:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79301ebea25cc17f02053c62454849ccd835c801212e266b390635073094d85c`  
		Last Modified: Mon, 24 Jan 2022 19:48:20 GMT  
		Size: 78.3 MB (78323954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e962e8f42e697587df7382ee450914d9f7f399c1e0d6783c5f26233c6878e5`  
		Last Modified: Mon, 24 Jan 2022 19:48:05 GMT  
		Size: 15.7 MB (15670101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45bfe0f18c94f41ae86b61b706d648da98955a9c07e4ee4a2dfc9dfc88e7311`  
		Last Modified: Mon, 24 Jan 2022 19:48:02 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:c65a3b687a783519de8d8e3a911cd0f6872ff7125850e08409c36dd4e55ddf76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:f3f0e6317bbe74b9a8c4ac862b42090308aacd992466af0c8a6dbc6c4170b37b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.1 MB (327098631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e836c552d83df196ee1273a50296503f0a3f5d162a0f650c3672621f03cfb1f2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:26:06 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 04:26:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:26:51 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:27:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:27:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:27:20 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:27:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:27:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:27:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:27:52 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 04:27:52 GMT
ENV ROS2_DISTRO=galactic
# Mon, 24 Jan 2022 19:55:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:55:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:55:55 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063d0746de5719c9156895722399b01972416e0e80c658155982c00200f443a6`  
		Last Modified: Fri, 07 Jan 2022 04:39:27 GMT  
		Size: 103.7 MB (103658457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc154cdc673512ad761544d2fcd686eb54be2f05bb2979f99ce88721916b3292`  
		Last Modified: Fri, 07 Jan 2022 04:39:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1649390eb8dcd2fe6e5c6ad2852f46c75286c1f2aa6e823189e62a9bd8f5b48`  
		Last Modified: Fri, 07 Jan 2022 04:39:47 GMT  
		Size: 70.8 MB (70809018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e5b5f85fd50dc8f63a00fe68c4f8868cf1630d84d9376b50105e52b86be46`  
		Last Modified: Fri, 07 Jan 2022 04:39:37 GMT  
		Size: 256.5 KB (256531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359e6648253521fa3d50934dd6fbc1fea6cc84b875fe7767fe4c6c432a0269f9`  
		Last Modified: Fri, 07 Jan 2022 04:39:37 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad327712cfc9c7179f06c300cf31922d30a760439761d2e0f603970aca6cb12`  
		Last Modified: Fri, 07 Jan 2022 04:39:40 GMT  
		Size: 22.1 MB (22110051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85215c58e455a99da7ddf6c775a7e8063bbefa1294015bb699213b9b32e08fdc`  
		Last Modified: Fri, 07 Jan 2022 04:40:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fc1f54e736214a55d34a88c31251a566f91c74ef68e7e999efcd29e93047c5`  
		Last Modified: Fri, 07 Jan 2022 04:40:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e95fceab9e4912b17705a1f8a816a4e7bf235c343682349d1c1a7207237078`  
		Last Modified: Mon, 24 Jan 2022 19:59:32 GMT  
		Size: 78.6 MB (78593060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c55525cd5db9326521f64572a36e4aff757bb928f982c850716f841f2da7cc`  
		Last Modified: Mon, 24 Jan 2022 19:59:19 GMT  
		Size: 16.4 MB (16370804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ce02495efa50cab0b55008267b6caa56f5748eecf137740528f252c5549192`  
		Last Modified: Mon, 24 Jan 2022 19:59:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ae7e37d62db89fb08df1cf6c1896a7f93b44a2344144d377a7268cd25bbc7438
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.3 MB (314329011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d5dc4c139326e993d698dd5620269a9f553f75d20df50b38a20ae47f66d521`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:25:03 GMT
ENV ROS_DISTRO=galactic
# Fri, 07 Jan 2022 03:25:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:25:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:25:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:25:57 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:26:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:26:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:26:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:26:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:27:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:27:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:27:16 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 03:27:17 GMT
ENV ROS2_DISTRO=galactic
# Mon, 24 Jan 2022 19:44:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:44:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:44:28 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9bb206bac894b41230de1b372cdfd2492571d0b1c1ec86904932c7374bbc06`  
		Last Modified: Fri, 07 Jan 2022 03:39:54 GMT  
		Size: 100.0 MB (100036692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9173d5fa207ed202cce7d701cf4f3a127f3ae3d247c1b3573a2fb6f4e404c2f`  
		Last Modified: Fri, 07 Jan 2022 03:39:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03661c68c764e1b462e8b4d59a1451a2e740012fac57cf6aaafc9cb6fae6d43b`  
		Last Modified: Fri, 07 Jan 2022 03:40:16 GMT  
		Size: 64.9 MB (64932295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ac2e61c69997f1e16aabf40bace777ed589f95ec842fbe63614cb66260b653`  
		Last Modified: Fri, 07 Jan 2022 03:40:06 GMT  
		Size: 256.5 KB (256483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74e2289bc0665dd9b4e3a6bb89203e323516e31f58b9ead5b87e36bd3f8a15e`  
		Last Modified: Fri, 07 Jan 2022 03:40:06 GMT  
		Size: 2.0 KB (2015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb713b315270cfa8e2114ba6e2666e342cd902c9b34683b86073a68a21910d41`  
		Last Modified: Fri, 07 Jan 2022 03:40:09 GMT  
		Size: 21.4 MB (21426788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d837971b2f51e4c13fd2b39f61daf5732be9e74307a34ab7099eafb1510782`  
		Last Modified: Fri, 07 Jan 2022 03:40:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79301ebea25cc17f02053c62454849ccd835c801212e266b390635073094d85c`  
		Last Modified: Mon, 24 Jan 2022 19:48:20 GMT  
		Size: 78.3 MB (78323954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e962e8f42e697587df7382ee450914d9f7f399c1e0d6783c5f26233c6878e5`  
		Last Modified: Mon, 24 Jan 2022 19:48:05 GMT  
		Size: 15.7 MB (15670101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45bfe0f18c94f41ae86b61b706d648da98955a9c07e4ee4a2dfc9dfc88e7311`  
		Last Modified: Mon, 24 Jan 2022 19:48:02 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:e40e3f528095ad129694b2c686527cd7c231a9a773e76932f5a1dd7bad113cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:de88ec5f83170c16d3241172c0519b89558d52f0e307556e04f623c840266683
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236778688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15ea8872063a9a23fe47d2a8f855bdb84c4f8614b2a8a3c2f2e1b7df0db33743`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 04:23:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:24:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:24:00 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:24:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:24:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:24:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:25:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e5fcbc56cc018564403b3e0d7a2ba1c551dbbfef70614bab532a6cec5e4b17`  
		Last Modified: Fri, 07 Jan 2022 04:38:06 GMT  
		Size: 120.1 MB (120084781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca376e51cfddbb5565d4cb5bcd27b84bd29b7814c3a10f1f27d006fd2fdb5f57`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce6db45f220ec4a768963fbf00033b6f7591d9485c3aba2b9b1a4cded3c6e14`  
		Last Modified: Fri, 07 Jan 2022 04:38:27 GMT  
		Size: 70.9 MB (70857002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f29fb66d2b2ac4fc5c4792af937f08192b56597651670a8e9c50033168736ea`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 248.0 KB (247988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c59003bb7bd2d1ecbcb0ce6a54795c7047db81b534f807837c0b56db2f43b`  
		Last Modified: Fri, 07 Jan 2022 04:38:17 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d2c6e532f1e832e4514e246cdd3c73654b2e2d065e9170ef5b28dac48ba046`  
		Last Modified: Fri, 07 Jan 2022 04:38:19 GMT  
		Size: 10.3 MB (10288814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:031ec1bef47d9c2d25fd78ae182c1bdac1c1de258fcd3925162b0a98dd8792ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212273414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958ce2ddd377dc731b4732ae55d2f375b8ae2d965f3f9b32be19343692906066`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:21:33 GMT
ENV ROS_DISTRO=foxy
# Fri, 07 Jan 2022 03:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:22:27 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:22:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:22:29 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:23:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:23:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:23:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:23:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66a92a9fd6a8886d123d670db5303b8dd67ddd77a81725baeb2a0b505ced2a`  
		Last Modified: Fri, 07 Jan 2022 03:38:30 GMT  
		Size: 104.3 MB (104278769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff28861e6a517aa6142fc99de642cca95e1dd5a89fd9ed6a6b91f4fb027858c9`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e70d35be41ad697b7032634ba5ac686f40fb7d1f3a3831d3ab3bd181700f2`  
		Last Modified: Fri, 07 Jan 2022 03:38:52 GMT  
		Size: 65.0 MB (64978411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4de71e579016c7dd5135332644ab4822e7de561bf903b27f4b7abf4463d2e9a`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 247.9 KB (247929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c68e716a4fe65ae789bc8663115985441757e1dd471ceb660c034af46acb3`  
		Last Modified: Fri, 07 Jan 2022 03:38:42 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff754c55fcced401707c7c7c28dee657d3c984b05bd0eb84f455b7a34e8838`  
		Last Modified: Fri, 07 Jan 2022 03:38:44 GMT  
		Size: 9.1 MB (9086053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:05e82fd8df82863e670725c3a06ac5e8e3521db6be5321918202217757ca6eaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:7b541bee2dd035dbb89383d0d08329a3304eb647da512c54eadd40af230f37e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437375392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb5ca5b6529483f2629b6a3e8d38a75090c22d543c77562dacb5c5c6d656ef06`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:55:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:59:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:59:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:59:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:00:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:00:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbf856ad4adc3f793ce064ea3fda7e4706e6e0d4b80ca4fe027d96f13a87dab`  
		Last Modified: Fri, 07 Jan 2022 04:32:02 GMT  
		Size: 839.5 KB (839500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19d9c773a8e3aa88af3da94878762a541aab51a81f76bb243ce22986621397`  
		Last Modified: Fri, 07 Jan 2022 04:32:00 GMT  
		Size: 4.9 MB (4872675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56d181a6951ac02f2348017091a5ea75f9c9b179c5aca8afec0a206090b6e3`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089e5a8628e7bc56e73d03702ed0336e18cdf2376719b4c9bc41aaf9f4feb69e`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb0fe2a049369c3aa544eb6b4f7c1f9f7a40074b0d95e8c5d4c8aae1b3995e9`  
		Last Modified: Fri, 07 Jan 2022 04:32:47 GMT  
		Size: 259.4 MB (259449273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3ff65a6b590db242ed4d09391158922c6d1e24a633dd27d58482854501332`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654ab1c4144dbdbf70fdd206f268a6b0c73e0d75aa43c7ae81675a3f1a469003`  
		Last Modified: Fri, 07 Jan 2022 04:33:10 GMT  
		Size: 70.2 MB (70235637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef173f71564f9fa83bd3290bf69987840b7b26a538f67ae46de90934396ea83e`  
		Last Modified: Fri, 07 Jan 2022 04:32:59 GMT  
		Size: 275.9 KB (275867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fd5992e383f303d239a085959c8f07efbe0bdd1cf70c5d4aee0eeafc428dec`  
		Last Modified: Fri, 07 Jan 2022 04:33:15 GMT  
		Size: 75.0 MB (74994999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:1698701dbbb4fb1d2820c370b866ca1cfd736eb9ec8be5d83b67ff883c12da31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385879479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e840122aab862341d9c8ff4ffd9f725d70333aac4618b815a2eb95e45ea9d0b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:03 GMT
ADD file:04c050ae3b998115f9e3f0da295a93a62bdff5d2efc3c37e792665d263cbf804 in / 
# Fri, 07 Jan 2022 02:26:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:41:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:41:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:41:59 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:45:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:45:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:46:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:46:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db4feefed17933b9e08cd0d0fd6c63db5c115552848576f2bc2062c8c5f69628`  
		Last Modified: Fri, 07 Jan 2022 02:30:10 GMT  
		Size: 22.3 MB (22303634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b5a1a2a0cd898e6a263e2752a2a0c70e3b9f18aca5e6dd0d1fc3bd11e2fc05`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 840.2 KB (840158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc89e947a0da5dceeebc4b92b77167fc247cb9805bffda1d5b6dc231c4f780`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 4.1 MB (4086107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb0ea1bc505b6e24af6dfd211660f3460432820e6b8c1f760bb7ea6c17913d`  
		Last Modified: Fri, 07 Jan 2022 04:05:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09688fa34b6295d2f86dacfd315dcae2bebc5b999531d3c87f78eb9a9a20457d`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977285ff1ff017f6f62e983da18f935bc160be6b6198dbd8624027b4f059a7a`  
		Last Modified: Fri, 07 Jan 2022 04:08:27 GMT  
		Size: 238.9 MB (238920238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b3b7c7ee0ad28b5bf8f651f9dbb344529ec73f21eab872fb5bab652dbf08e`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea142cf00340822a541e62a3c5918346f6f80d2b9ee4b3730c2374cb23b5e8`  
		Last Modified: Fri, 07 Jan 2022 04:09:11 GMT  
		Size: 54.7 MB (54704807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505bd1f0567e09c1ba0faecf71656cbb1d54e9daef574fcca4238df773defe01`  
		Last Modified: Fri, 07 Jan 2022 04:08:42 GMT  
		Size: 275.8 KB (275818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad17b52c3afe2f4e17f6930b9001b9008b8864e9d71ea854774ebcbabaf9dbb`  
		Last Modified: Fri, 07 Jan 2022 04:09:25 GMT  
		Size: 64.7 MB (64746306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bbb1ffc350458f77e3acb322553eac1333fa186131f11164517efc40fe532a0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.5 MB (411535638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b79a6f7bc4df605028d8554e55d499fad95c222cfd69f5478d8e581fb74e3e93`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:10:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:10:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:10:35 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:10:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:10:37 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:12:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:12:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:12:07 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:12:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:13:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7cb05d07ef46feac0fe88a2a5076e86982a4783b2bd17c98cf09974e499fd`  
		Last Modified: Fri, 07 Jan 2022 03:33:03 GMT  
		Size: 839.7 KB (839701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26bd7d783afca747fac46c5c9e260d26c390e10997bb98aa9916c1d64e138`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 4.3 MB (4263976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1962a21cee4ae01758aa1e7590e18d5b4447a0367015777fee7c81f8b7eac5`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e8179c314f217515dcf0a6d2885f2052277608fa6a674eb34d27d962d73c40`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992366677b7dcdca6e06367d0f8144bd2730dd68ae4a3ada2877eb399f28bd86`  
		Last Modified: Fri, 07 Jan 2022 03:33:38 GMT  
		Size: 252.4 MB (252357211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c0fcb5d49558d6ca44a8e0671e4bf31db08a187b90278eddda3cd6b18a564`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26ee3aa7ab81e1ae02f90c68840af00275e514a1856ea2c341aa79a0f38e9e7`  
		Last Modified: Fri, 07 Jan 2022 03:34:00 GMT  
		Size: 63.1 MB (63067247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ed727ae92cb44ed96c637dde8e913fb1a0dfc87c6a50ad27fbbf7ad7ebda77`  
		Last Modified: Fri, 07 Jan 2022 03:33:52 GMT  
		Size: 275.8 KB (275812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9649eedfe287e53fba655551c5e75655c3096639775d06d0f681cf3e075642`  
		Last Modified: Fri, 07 Jan 2022 03:34:02 GMT  
		Size: 67.0 MB (67002406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:0cb0dbe06581dfa142211537c433f649a7da685201eff422f6eb676075d591a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:6a85697f6734ef66326a90a302018646cd3b4234990ace51c90eb96ce771cf80
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742701233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b49ae8b9b35c6c2430e8c0b4b0919f03038767d8117d919e894874056b34a1d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:55:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:59:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:59:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:59:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:00:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:00:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbf856ad4adc3f793ce064ea3fda7e4706e6e0d4b80ca4fe027d96f13a87dab`  
		Last Modified: Fri, 07 Jan 2022 04:32:02 GMT  
		Size: 839.5 KB (839500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19d9c773a8e3aa88af3da94878762a541aab51a81f76bb243ce22986621397`  
		Last Modified: Fri, 07 Jan 2022 04:32:00 GMT  
		Size: 4.9 MB (4872675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56d181a6951ac02f2348017091a5ea75f9c9b179c5aca8afec0a206090b6e3`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089e5a8628e7bc56e73d03702ed0336e18cdf2376719b4c9bc41aaf9f4feb69e`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb0fe2a049369c3aa544eb6b4f7c1f9f7a40074b0d95e8c5d4c8aae1b3995e9`  
		Last Modified: Fri, 07 Jan 2022 04:32:47 GMT  
		Size: 259.4 MB (259449273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3ff65a6b590db242ed4d09391158922c6d1e24a633dd27d58482854501332`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654ab1c4144dbdbf70fdd206f268a6b0c73e0d75aa43c7ae81675a3f1a469003`  
		Last Modified: Fri, 07 Jan 2022 04:33:10 GMT  
		Size: 70.2 MB (70235637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef173f71564f9fa83bd3290bf69987840b7b26a538f67ae46de90934396ea83e`  
		Last Modified: Fri, 07 Jan 2022 04:32:59 GMT  
		Size: 275.9 KB (275867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fd5992e383f303d239a085959c8f07efbe0bdd1cf70c5d4aee0eeafc428dec`  
		Last Modified: Fri, 07 Jan 2022 04:33:15 GMT  
		Size: 75.0 MB (74994999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5660e1c9fe436bfbd34680ad650c072c8451ec4dbc87fbd2c5870fa18627eb`  
		Last Modified: Fri, 07 Jan 2022 04:34:36 GMT  
		Size: 305.3 MB (305325841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:c6fc7be1b7becb57f8068b6c375101756c09df1fc3cb92b4b30baf97aee61b3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.9 MB (645914351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401c6bc42ba54a393d9d03d795b45b5f11695f17f359bf243099c1b9778be290`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:03 GMT
ADD file:04c050ae3b998115f9e3f0da295a93a62bdff5d2efc3c37e792665d263cbf804 in / 
# Fri, 07 Jan 2022 02:26:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:41:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:41:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:41:59 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:45:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:45:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:46:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:46:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db4feefed17933b9e08cd0d0fd6c63db5c115552848576f2bc2062c8c5f69628`  
		Last Modified: Fri, 07 Jan 2022 02:30:10 GMT  
		Size: 22.3 MB (22303634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b5a1a2a0cd898e6a263e2752a2a0c70e3b9f18aca5e6dd0d1fc3bd11e2fc05`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 840.2 KB (840158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc89e947a0da5dceeebc4b92b77167fc247cb9805bffda1d5b6dc231c4f780`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 4.1 MB (4086107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb0ea1bc505b6e24af6dfd211660f3460432820e6b8c1f760bb7ea6c17913d`  
		Last Modified: Fri, 07 Jan 2022 04:05:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09688fa34b6295d2f86dacfd315dcae2bebc5b999531d3c87f78eb9a9a20457d`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977285ff1ff017f6f62e983da18f935bc160be6b6198dbd8624027b4f059a7a`  
		Last Modified: Fri, 07 Jan 2022 04:08:27 GMT  
		Size: 238.9 MB (238920238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b3b7c7ee0ad28b5bf8f651f9dbb344529ec73f21eab872fb5bab652dbf08e`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea142cf00340822a541e62a3c5918346f6f80d2b9ee4b3730c2374cb23b5e8`  
		Last Modified: Fri, 07 Jan 2022 04:09:11 GMT  
		Size: 54.7 MB (54704807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505bd1f0567e09c1ba0faecf71656cbb1d54e9daef574fcca4238df773defe01`  
		Last Modified: Fri, 07 Jan 2022 04:08:42 GMT  
		Size: 275.8 KB (275818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad17b52c3afe2f4e17f6930b9001b9008b8864e9d71ea854774ebcbabaf9dbb`  
		Last Modified: Fri, 07 Jan 2022 04:09:25 GMT  
		Size: 64.7 MB (64746306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb6f19beb6ea8383c29b3d6c750ac3668263f33079b5f9e52e3f9efed7e49dd`  
		Last Modified: Fri, 07 Jan 2022 04:12:45 GMT  
		Size: 260.0 MB (260034872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c4c159951ecb344d4d938be74fdffa8b98eb9f3212b1bf3f32abc667bc3eb2c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **702.9 MB (702918472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6167b16b39d712390c6d76b4d9e74079934df43eca8cc36cb777c384ddb891a4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:10:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:10:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:10:35 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:10:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:10:37 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:12:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:12:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:12:07 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:12:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:13:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7cb05d07ef46feac0fe88a2a5076e86982a4783b2bd17c98cf09974e499fd`  
		Last Modified: Fri, 07 Jan 2022 03:33:03 GMT  
		Size: 839.7 KB (839701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26bd7d783afca747fac46c5c9e260d26c390e10997bb98aa9916c1d64e138`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 4.3 MB (4263976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1962a21cee4ae01758aa1e7590e18d5b4447a0367015777fee7c81f8b7eac5`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e8179c314f217515dcf0a6d2885f2052277608fa6a674eb34d27d962d73c40`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992366677b7dcdca6e06367d0f8144bd2730dd68ae4a3ada2877eb399f28bd86`  
		Last Modified: Fri, 07 Jan 2022 03:33:38 GMT  
		Size: 252.4 MB (252357211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c0fcb5d49558d6ca44a8e0671e4bf31db08a187b90278eddda3cd6b18a564`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26ee3aa7ab81e1ae02f90c68840af00275e514a1856ea2c341aa79a0f38e9e7`  
		Last Modified: Fri, 07 Jan 2022 03:34:00 GMT  
		Size: 63.1 MB (63067247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ed727ae92cb44ed96c637dde8e913fb1a0dfc87c6a50ad27fbbf7ad7ebda77`  
		Last Modified: Fri, 07 Jan 2022 03:33:52 GMT  
		Size: 275.8 KB (275812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9649eedfe287e53fba655551c5e75655c3096639775d06d0f681cf3e075642`  
		Last Modified: Fri, 07 Jan 2022 03:34:02 GMT  
		Size: 67.0 MB (67002406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1869584807e21cfd1b68597c82773705ae10af91d3e093729080b38f5138d4e2`  
		Last Modified: Fri, 07 Jan 2022 03:35:15 GMT  
		Size: 291.4 MB (291382834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:0cb0dbe06581dfa142211537c433f649a7da685201eff422f6eb676075d591a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:6a85697f6734ef66326a90a302018646cd3b4234990ace51c90eb96ce771cf80
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742701233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b49ae8b9b35c6c2430e8c0b4b0919f03038767d8117d919e894874056b34a1d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:55:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:59:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:59:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:59:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:00:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:00:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbf856ad4adc3f793ce064ea3fda7e4706e6e0d4b80ca4fe027d96f13a87dab`  
		Last Modified: Fri, 07 Jan 2022 04:32:02 GMT  
		Size: 839.5 KB (839500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19d9c773a8e3aa88af3da94878762a541aab51a81f76bb243ce22986621397`  
		Last Modified: Fri, 07 Jan 2022 04:32:00 GMT  
		Size: 4.9 MB (4872675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56d181a6951ac02f2348017091a5ea75f9c9b179c5aca8afec0a206090b6e3`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089e5a8628e7bc56e73d03702ed0336e18cdf2376719b4c9bc41aaf9f4feb69e`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb0fe2a049369c3aa544eb6b4f7c1f9f7a40074b0d95e8c5d4c8aae1b3995e9`  
		Last Modified: Fri, 07 Jan 2022 04:32:47 GMT  
		Size: 259.4 MB (259449273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3ff65a6b590db242ed4d09391158922c6d1e24a633dd27d58482854501332`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654ab1c4144dbdbf70fdd206f268a6b0c73e0d75aa43c7ae81675a3f1a469003`  
		Last Modified: Fri, 07 Jan 2022 04:33:10 GMT  
		Size: 70.2 MB (70235637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef173f71564f9fa83bd3290bf69987840b7b26a538f67ae46de90934396ea83e`  
		Last Modified: Fri, 07 Jan 2022 04:32:59 GMT  
		Size: 275.9 KB (275867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fd5992e383f303d239a085959c8f07efbe0bdd1cf70c5d4aee0eeafc428dec`  
		Last Modified: Fri, 07 Jan 2022 04:33:15 GMT  
		Size: 75.0 MB (74994999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5660e1c9fe436bfbd34680ad650c072c8451ec4dbc87fbd2c5870fa18627eb`  
		Last Modified: Fri, 07 Jan 2022 04:34:36 GMT  
		Size: 305.3 MB (305325841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:c6fc7be1b7becb57f8068b6c375101756c09df1fc3cb92b4b30baf97aee61b3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.9 MB (645914351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401c6bc42ba54a393d9d03d795b45b5f11695f17f359bf243099c1b9778be290`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:03 GMT
ADD file:04c050ae3b998115f9e3f0da295a93a62bdff5d2efc3c37e792665d263cbf804 in / 
# Fri, 07 Jan 2022 02:26:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:41:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:41:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:41:59 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:45:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:45:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:46:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:46:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db4feefed17933b9e08cd0d0fd6c63db5c115552848576f2bc2062c8c5f69628`  
		Last Modified: Fri, 07 Jan 2022 02:30:10 GMT  
		Size: 22.3 MB (22303634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b5a1a2a0cd898e6a263e2752a2a0c70e3b9f18aca5e6dd0d1fc3bd11e2fc05`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 840.2 KB (840158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc89e947a0da5dceeebc4b92b77167fc247cb9805bffda1d5b6dc231c4f780`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 4.1 MB (4086107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb0ea1bc505b6e24af6dfd211660f3460432820e6b8c1f760bb7ea6c17913d`  
		Last Modified: Fri, 07 Jan 2022 04:05:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09688fa34b6295d2f86dacfd315dcae2bebc5b999531d3c87f78eb9a9a20457d`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977285ff1ff017f6f62e983da18f935bc160be6b6198dbd8624027b4f059a7a`  
		Last Modified: Fri, 07 Jan 2022 04:08:27 GMT  
		Size: 238.9 MB (238920238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b3b7c7ee0ad28b5bf8f651f9dbb344529ec73f21eab872fb5bab652dbf08e`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea142cf00340822a541e62a3c5918346f6f80d2b9ee4b3730c2374cb23b5e8`  
		Last Modified: Fri, 07 Jan 2022 04:09:11 GMT  
		Size: 54.7 MB (54704807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505bd1f0567e09c1ba0faecf71656cbb1d54e9daef574fcca4238df773defe01`  
		Last Modified: Fri, 07 Jan 2022 04:08:42 GMT  
		Size: 275.8 KB (275818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad17b52c3afe2f4e17f6930b9001b9008b8864e9d71ea854774ebcbabaf9dbb`  
		Last Modified: Fri, 07 Jan 2022 04:09:25 GMT  
		Size: 64.7 MB (64746306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb6f19beb6ea8383c29b3d6c750ac3668263f33079b5f9e52e3f9efed7e49dd`  
		Last Modified: Fri, 07 Jan 2022 04:12:45 GMT  
		Size: 260.0 MB (260034872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c4c159951ecb344d4d938be74fdffa8b98eb9f3212b1bf3f32abc667bc3eb2c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **702.9 MB (702918472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6167b16b39d712390c6d76b4d9e74079934df43eca8cc36cb777c384ddb891a4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:10:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:10:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:10:35 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:10:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:10:37 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:12:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:12:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:12:07 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:12:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:13:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7cb05d07ef46feac0fe88a2a5076e86982a4783b2bd17c98cf09974e499fd`  
		Last Modified: Fri, 07 Jan 2022 03:33:03 GMT  
		Size: 839.7 KB (839701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26bd7d783afca747fac46c5c9e260d26c390e10997bb98aa9916c1d64e138`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 4.3 MB (4263976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1962a21cee4ae01758aa1e7590e18d5b4447a0367015777fee7c81f8b7eac5`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e8179c314f217515dcf0a6d2885f2052277608fa6a674eb34d27d962d73c40`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992366677b7dcdca6e06367d0f8144bd2730dd68ae4a3ada2877eb399f28bd86`  
		Last Modified: Fri, 07 Jan 2022 03:33:38 GMT  
		Size: 252.4 MB (252357211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c0fcb5d49558d6ca44a8e0671e4bf31db08a187b90278eddda3cd6b18a564`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26ee3aa7ab81e1ae02f90c68840af00275e514a1856ea2c341aa79a0f38e9e7`  
		Last Modified: Fri, 07 Jan 2022 03:34:00 GMT  
		Size: 63.1 MB (63067247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ed727ae92cb44ed96c637dde8e913fb1a0dfc87c6a50ad27fbbf7ad7ebda77`  
		Last Modified: Fri, 07 Jan 2022 03:33:52 GMT  
		Size: 275.8 KB (275812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9649eedfe287e53fba655551c5e75655c3096639775d06d0f681cf3e075642`  
		Last Modified: Fri, 07 Jan 2022 03:34:02 GMT  
		Size: 67.0 MB (67002406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1869584807e21cfd1b68597c82773705ae10af91d3e093729080b38f5138d4e2`  
		Last Modified: Fri, 07 Jan 2022 03:35:15 GMT  
		Size: 291.4 MB (291382834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:9270874f94d17b69d8aeda024b1af616d32cd1266de511c566dad07d7df49fe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:8109753fd1fdadc3d85a56e0ed993c1935ebfdadc207f76374642bc1997b91e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448458268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67bb694c09b4d919aa09a294c4a269aca790768242a1dc884e9129ed6a9333e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:55:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:59:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:59:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:59:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:00:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:00:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:02:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbf856ad4adc3f793ce064ea3fda7e4706e6e0d4b80ca4fe027d96f13a87dab`  
		Last Modified: Fri, 07 Jan 2022 04:32:02 GMT  
		Size: 839.5 KB (839500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19d9c773a8e3aa88af3da94878762a541aab51a81f76bb243ce22986621397`  
		Last Modified: Fri, 07 Jan 2022 04:32:00 GMT  
		Size: 4.9 MB (4872675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56d181a6951ac02f2348017091a5ea75f9c9b179c5aca8afec0a206090b6e3`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089e5a8628e7bc56e73d03702ed0336e18cdf2376719b4c9bc41aaf9f4feb69e`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb0fe2a049369c3aa544eb6b4f7c1f9f7a40074b0d95e8c5d4c8aae1b3995e9`  
		Last Modified: Fri, 07 Jan 2022 04:32:47 GMT  
		Size: 259.4 MB (259449273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3ff65a6b590db242ed4d09391158922c6d1e24a633dd27d58482854501332`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654ab1c4144dbdbf70fdd206f268a6b0c73e0d75aa43c7ae81675a3f1a469003`  
		Last Modified: Fri, 07 Jan 2022 04:33:10 GMT  
		Size: 70.2 MB (70235637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef173f71564f9fa83bd3290bf69987840b7b26a538f67ae46de90934396ea83e`  
		Last Modified: Fri, 07 Jan 2022 04:32:59 GMT  
		Size: 275.9 KB (275867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fd5992e383f303d239a085959c8f07efbe0bdd1cf70c5d4aee0eeafc428dec`  
		Last Modified: Fri, 07 Jan 2022 04:33:15 GMT  
		Size: 75.0 MB (74994999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4211cd1404d0df620af49b32d4ef72abf5e406df483e7e65927aa27f5adee03`  
		Last Modified: Fri, 07 Jan 2022 04:33:30 GMT  
		Size: 11.1 MB (11082876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:318a1fe70bcf6470e59df44c4860dee6b23af1fb3090ce25b3360fa15daf6bfb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396001804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1680f73911ea21499e95b328ab6e559159394a8d1c3816e046e0ab0a869595cc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:03 GMT
ADD file:04c050ae3b998115f9e3f0da295a93a62bdff5d2efc3c37e792665d263cbf804 in / 
# Fri, 07 Jan 2022 02:26:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:41:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:41:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:41:59 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:45:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:45:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:46:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:46:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:48:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db4feefed17933b9e08cd0d0fd6c63db5c115552848576f2bc2062c8c5f69628`  
		Last Modified: Fri, 07 Jan 2022 02:30:10 GMT  
		Size: 22.3 MB (22303634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b5a1a2a0cd898e6a263e2752a2a0c70e3b9f18aca5e6dd0d1fc3bd11e2fc05`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 840.2 KB (840158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc89e947a0da5dceeebc4b92b77167fc247cb9805bffda1d5b6dc231c4f780`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 4.1 MB (4086107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb0ea1bc505b6e24af6dfd211660f3460432820e6b8c1f760bb7ea6c17913d`  
		Last Modified: Fri, 07 Jan 2022 04:05:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09688fa34b6295d2f86dacfd315dcae2bebc5b999531d3c87f78eb9a9a20457d`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977285ff1ff017f6f62e983da18f935bc160be6b6198dbd8624027b4f059a7a`  
		Last Modified: Fri, 07 Jan 2022 04:08:27 GMT  
		Size: 238.9 MB (238920238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b3b7c7ee0ad28b5bf8f651f9dbb344529ec73f21eab872fb5bab652dbf08e`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea142cf00340822a541e62a3c5918346f6f80d2b9ee4b3730c2374cb23b5e8`  
		Last Modified: Fri, 07 Jan 2022 04:09:11 GMT  
		Size: 54.7 MB (54704807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505bd1f0567e09c1ba0faecf71656cbb1d54e9daef574fcca4238df773defe01`  
		Last Modified: Fri, 07 Jan 2022 04:08:42 GMT  
		Size: 275.8 KB (275818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad17b52c3afe2f4e17f6930b9001b9008b8864e9d71ea854774ebcbabaf9dbb`  
		Last Modified: Fri, 07 Jan 2022 04:09:25 GMT  
		Size: 64.7 MB (64746306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4834aeb1ab29cfa8e7ab30d3f3f5b67c6510beace70cdd7869cda04c1e7d5d39`  
		Last Modified: Fri, 07 Jan 2022 04:09:51 GMT  
		Size: 10.1 MB (10122325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e9e46bfc95a35ea1b942d69afc2a3fbf24dd8fa471d9d9a811a9f2a0077fe5c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.3 MB (422268043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3b8dcf7bccb885e71b617b604041eb57d7c9f23880c794b928d562c6cf6cb0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:10:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:10:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:10:35 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:10:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:10:37 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:12:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:12:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:12:07 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:12:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:13:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7cb05d07ef46feac0fe88a2a5076e86982a4783b2bd17c98cf09974e499fd`  
		Last Modified: Fri, 07 Jan 2022 03:33:03 GMT  
		Size: 839.7 KB (839701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26bd7d783afca747fac46c5c9e260d26c390e10997bb98aa9916c1d64e138`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 4.3 MB (4263976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1962a21cee4ae01758aa1e7590e18d5b4447a0367015777fee7c81f8b7eac5`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e8179c314f217515dcf0a6d2885f2052277608fa6a674eb34d27d962d73c40`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992366677b7dcdca6e06367d0f8144bd2730dd68ae4a3ada2877eb399f28bd86`  
		Last Modified: Fri, 07 Jan 2022 03:33:38 GMT  
		Size: 252.4 MB (252357211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c0fcb5d49558d6ca44a8e0671e4bf31db08a187b90278eddda3cd6b18a564`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26ee3aa7ab81e1ae02f90c68840af00275e514a1856ea2c341aa79a0f38e9e7`  
		Last Modified: Fri, 07 Jan 2022 03:34:00 GMT  
		Size: 63.1 MB (63067247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ed727ae92cb44ed96c637dde8e913fb1a0dfc87c6a50ad27fbbf7ad7ebda77`  
		Last Modified: Fri, 07 Jan 2022 03:33:52 GMT  
		Size: 275.8 KB (275812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9649eedfe287e53fba655551c5e75655c3096639775d06d0f681cf3e075642`  
		Last Modified: Fri, 07 Jan 2022 03:34:02 GMT  
		Size: 67.0 MB (67002406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a36c4740c77d215b30d016e7905093904031a7bee0d551c938da8297ccb4afc`  
		Last Modified: Fri, 07 Jan 2022 03:34:19 GMT  
		Size: 10.7 MB (10732405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:9270874f94d17b69d8aeda024b1af616d32cd1266de511c566dad07d7df49fe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:8109753fd1fdadc3d85a56e0ed993c1935ebfdadc207f76374642bc1997b91e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448458268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67bb694c09b4d919aa09a294c4a269aca790768242a1dc884e9129ed6a9333e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:55:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:59:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:59:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:59:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:00:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:00:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:02:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbf856ad4adc3f793ce064ea3fda7e4706e6e0d4b80ca4fe027d96f13a87dab`  
		Last Modified: Fri, 07 Jan 2022 04:32:02 GMT  
		Size: 839.5 KB (839500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19d9c773a8e3aa88af3da94878762a541aab51a81f76bb243ce22986621397`  
		Last Modified: Fri, 07 Jan 2022 04:32:00 GMT  
		Size: 4.9 MB (4872675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56d181a6951ac02f2348017091a5ea75f9c9b179c5aca8afec0a206090b6e3`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089e5a8628e7bc56e73d03702ed0336e18cdf2376719b4c9bc41aaf9f4feb69e`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb0fe2a049369c3aa544eb6b4f7c1f9f7a40074b0d95e8c5d4c8aae1b3995e9`  
		Last Modified: Fri, 07 Jan 2022 04:32:47 GMT  
		Size: 259.4 MB (259449273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3ff65a6b590db242ed4d09391158922c6d1e24a633dd27d58482854501332`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654ab1c4144dbdbf70fdd206f268a6b0c73e0d75aa43c7ae81675a3f1a469003`  
		Last Modified: Fri, 07 Jan 2022 04:33:10 GMT  
		Size: 70.2 MB (70235637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef173f71564f9fa83bd3290bf69987840b7b26a538f67ae46de90934396ea83e`  
		Last Modified: Fri, 07 Jan 2022 04:32:59 GMT  
		Size: 275.9 KB (275867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fd5992e383f303d239a085959c8f07efbe0bdd1cf70c5d4aee0eeafc428dec`  
		Last Modified: Fri, 07 Jan 2022 04:33:15 GMT  
		Size: 75.0 MB (74994999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4211cd1404d0df620af49b32d4ef72abf5e406df483e7e65927aa27f5adee03`  
		Last Modified: Fri, 07 Jan 2022 04:33:30 GMT  
		Size: 11.1 MB (11082876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:318a1fe70bcf6470e59df44c4860dee6b23af1fb3090ce25b3360fa15daf6bfb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396001804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1680f73911ea21499e95b328ab6e559159394a8d1c3816e046e0ab0a869595cc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:03 GMT
ADD file:04c050ae3b998115f9e3f0da295a93a62bdff5d2efc3c37e792665d263cbf804 in / 
# Fri, 07 Jan 2022 02:26:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:41:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:41:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:41:59 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:45:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:45:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:46:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:46:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:48:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db4feefed17933b9e08cd0d0fd6c63db5c115552848576f2bc2062c8c5f69628`  
		Last Modified: Fri, 07 Jan 2022 02:30:10 GMT  
		Size: 22.3 MB (22303634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b5a1a2a0cd898e6a263e2752a2a0c70e3b9f18aca5e6dd0d1fc3bd11e2fc05`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 840.2 KB (840158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc89e947a0da5dceeebc4b92b77167fc247cb9805bffda1d5b6dc231c4f780`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 4.1 MB (4086107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb0ea1bc505b6e24af6dfd211660f3460432820e6b8c1f760bb7ea6c17913d`  
		Last Modified: Fri, 07 Jan 2022 04:05:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09688fa34b6295d2f86dacfd315dcae2bebc5b999531d3c87f78eb9a9a20457d`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977285ff1ff017f6f62e983da18f935bc160be6b6198dbd8624027b4f059a7a`  
		Last Modified: Fri, 07 Jan 2022 04:08:27 GMT  
		Size: 238.9 MB (238920238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b3b7c7ee0ad28b5bf8f651f9dbb344529ec73f21eab872fb5bab652dbf08e`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea142cf00340822a541e62a3c5918346f6f80d2b9ee4b3730c2374cb23b5e8`  
		Last Modified: Fri, 07 Jan 2022 04:09:11 GMT  
		Size: 54.7 MB (54704807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505bd1f0567e09c1ba0faecf71656cbb1d54e9daef574fcca4238df773defe01`  
		Last Modified: Fri, 07 Jan 2022 04:08:42 GMT  
		Size: 275.8 KB (275818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad17b52c3afe2f4e17f6930b9001b9008b8864e9d71ea854774ebcbabaf9dbb`  
		Last Modified: Fri, 07 Jan 2022 04:09:25 GMT  
		Size: 64.7 MB (64746306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4834aeb1ab29cfa8e7ab30d3f3f5b67c6510beace70cdd7869cda04c1e7d5d39`  
		Last Modified: Fri, 07 Jan 2022 04:09:51 GMT  
		Size: 10.1 MB (10122325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e9e46bfc95a35ea1b942d69afc2a3fbf24dd8fa471d9d9a811a9f2a0077fe5c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.3 MB (422268043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3b8dcf7bccb885e71b617b604041eb57d7c9f23880c794b928d562c6cf6cb0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:10:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:10:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:10:35 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:10:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:10:37 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:12:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:12:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:12:07 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:12:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:13:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7cb05d07ef46feac0fe88a2a5076e86982a4783b2bd17c98cf09974e499fd`  
		Last Modified: Fri, 07 Jan 2022 03:33:03 GMT  
		Size: 839.7 KB (839701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26bd7d783afca747fac46c5c9e260d26c390e10997bb98aa9916c1d64e138`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 4.3 MB (4263976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1962a21cee4ae01758aa1e7590e18d5b4447a0367015777fee7c81f8b7eac5`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e8179c314f217515dcf0a6d2885f2052277608fa6a674eb34d27d962d73c40`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992366677b7dcdca6e06367d0f8144bd2730dd68ae4a3ada2877eb399f28bd86`  
		Last Modified: Fri, 07 Jan 2022 03:33:38 GMT  
		Size: 252.4 MB (252357211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c0fcb5d49558d6ca44a8e0671e4bf31db08a187b90278eddda3cd6b18a564`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26ee3aa7ab81e1ae02f90c68840af00275e514a1856ea2c341aa79a0f38e9e7`  
		Last Modified: Fri, 07 Jan 2022 03:34:00 GMT  
		Size: 63.1 MB (63067247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ed727ae92cb44ed96c637dde8e913fb1a0dfc87c6a50ad27fbbf7ad7ebda77`  
		Last Modified: Fri, 07 Jan 2022 03:33:52 GMT  
		Size: 275.8 KB (275812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9649eedfe287e53fba655551c5e75655c3096639775d06d0f681cf3e075642`  
		Last Modified: Fri, 07 Jan 2022 03:34:02 GMT  
		Size: 67.0 MB (67002406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a36c4740c77d215b30d016e7905093904031a7bee0d551c938da8297ccb4afc`  
		Last Modified: Fri, 07 Jan 2022 03:34:19 GMT  
		Size: 10.7 MB (10732405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:05e82fd8df82863e670725c3a06ac5e8e3521db6be5321918202217757ca6eaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:7b541bee2dd035dbb89383d0d08329a3304eb647da512c54eadd40af230f37e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437375392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb5ca5b6529483f2629b6a3e8d38a75090c22d543c77562dacb5c5c6d656ef06`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:55:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:59:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:59:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:59:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:00:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:00:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbf856ad4adc3f793ce064ea3fda7e4706e6e0d4b80ca4fe027d96f13a87dab`  
		Last Modified: Fri, 07 Jan 2022 04:32:02 GMT  
		Size: 839.5 KB (839500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19d9c773a8e3aa88af3da94878762a541aab51a81f76bb243ce22986621397`  
		Last Modified: Fri, 07 Jan 2022 04:32:00 GMT  
		Size: 4.9 MB (4872675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56d181a6951ac02f2348017091a5ea75f9c9b179c5aca8afec0a206090b6e3`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089e5a8628e7bc56e73d03702ed0336e18cdf2376719b4c9bc41aaf9f4feb69e`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb0fe2a049369c3aa544eb6b4f7c1f9f7a40074b0d95e8c5d4c8aae1b3995e9`  
		Last Modified: Fri, 07 Jan 2022 04:32:47 GMT  
		Size: 259.4 MB (259449273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3ff65a6b590db242ed4d09391158922c6d1e24a633dd27d58482854501332`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654ab1c4144dbdbf70fdd206f268a6b0c73e0d75aa43c7ae81675a3f1a469003`  
		Last Modified: Fri, 07 Jan 2022 04:33:10 GMT  
		Size: 70.2 MB (70235637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef173f71564f9fa83bd3290bf69987840b7b26a538f67ae46de90934396ea83e`  
		Last Modified: Fri, 07 Jan 2022 04:32:59 GMT  
		Size: 275.9 KB (275867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fd5992e383f303d239a085959c8f07efbe0bdd1cf70c5d4aee0eeafc428dec`  
		Last Modified: Fri, 07 Jan 2022 04:33:15 GMT  
		Size: 75.0 MB (74994999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:1698701dbbb4fb1d2820c370b866ca1cfd736eb9ec8be5d83b67ff883c12da31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385879479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e840122aab862341d9c8ff4ffd9f725d70333aac4618b815a2eb95e45ea9d0b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:03 GMT
ADD file:04c050ae3b998115f9e3f0da295a93a62bdff5d2efc3c37e792665d263cbf804 in / 
# Fri, 07 Jan 2022 02:26:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:41:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:41:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:41:59 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:45:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:45:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:46:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:46:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db4feefed17933b9e08cd0d0fd6c63db5c115552848576f2bc2062c8c5f69628`  
		Last Modified: Fri, 07 Jan 2022 02:30:10 GMT  
		Size: 22.3 MB (22303634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b5a1a2a0cd898e6a263e2752a2a0c70e3b9f18aca5e6dd0d1fc3bd11e2fc05`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 840.2 KB (840158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc89e947a0da5dceeebc4b92b77167fc247cb9805bffda1d5b6dc231c4f780`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 4.1 MB (4086107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb0ea1bc505b6e24af6dfd211660f3460432820e6b8c1f760bb7ea6c17913d`  
		Last Modified: Fri, 07 Jan 2022 04:05:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09688fa34b6295d2f86dacfd315dcae2bebc5b999531d3c87f78eb9a9a20457d`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977285ff1ff017f6f62e983da18f935bc160be6b6198dbd8624027b4f059a7a`  
		Last Modified: Fri, 07 Jan 2022 04:08:27 GMT  
		Size: 238.9 MB (238920238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b3b7c7ee0ad28b5bf8f651f9dbb344529ec73f21eab872fb5bab652dbf08e`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea142cf00340822a541e62a3c5918346f6f80d2b9ee4b3730c2374cb23b5e8`  
		Last Modified: Fri, 07 Jan 2022 04:09:11 GMT  
		Size: 54.7 MB (54704807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505bd1f0567e09c1ba0faecf71656cbb1d54e9daef574fcca4238df773defe01`  
		Last Modified: Fri, 07 Jan 2022 04:08:42 GMT  
		Size: 275.8 KB (275818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad17b52c3afe2f4e17f6930b9001b9008b8864e9d71ea854774ebcbabaf9dbb`  
		Last Modified: Fri, 07 Jan 2022 04:09:25 GMT  
		Size: 64.7 MB (64746306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bbb1ffc350458f77e3acb322553eac1333fa186131f11164517efc40fe532a0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.5 MB (411535638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b79a6f7bc4df605028d8554e55d499fad95c222cfd69f5478d8e581fb74e3e93`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:10:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:10:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:10:35 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:10:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:10:37 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:12:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:12:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:12:07 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:12:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:13:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7cb05d07ef46feac0fe88a2a5076e86982a4783b2bd17c98cf09974e499fd`  
		Last Modified: Fri, 07 Jan 2022 03:33:03 GMT  
		Size: 839.7 KB (839701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26bd7d783afca747fac46c5c9e260d26c390e10997bb98aa9916c1d64e138`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 4.3 MB (4263976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1962a21cee4ae01758aa1e7590e18d5b4447a0367015777fee7c81f8b7eac5`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e8179c314f217515dcf0a6d2885f2052277608fa6a674eb34d27d962d73c40`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992366677b7dcdca6e06367d0f8144bd2730dd68ae4a3ada2877eb399f28bd86`  
		Last Modified: Fri, 07 Jan 2022 03:33:38 GMT  
		Size: 252.4 MB (252357211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c0fcb5d49558d6ca44a8e0671e4bf31db08a187b90278eddda3cd6b18a564`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26ee3aa7ab81e1ae02f90c68840af00275e514a1856ea2c341aa79a0f38e9e7`  
		Last Modified: Fri, 07 Jan 2022 03:34:00 GMT  
		Size: 63.1 MB (63067247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ed727ae92cb44ed96c637dde8e913fb1a0dfc87c6a50ad27fbbf7ad7ebda77`  
		Last Modified: Fri, 07 Jan 2022 03:33:52 GMT  
		Size: 275.8 KB (275812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9649eedfe287e53fba655551c5e75655c3096639775d06d0f681cf3e075642`  
		Last Modified: Fri, 07 Jan 2022 03:34:02 GMT  
		Size: 67.0 MB (67002406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:05e82fd8df82863e670725c3a06ac5e8e3521db6be5321918202217757ca6eaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:7b541bee2dd035dbb89383d0d08329a3304eb647da512c54eadd40af230f37e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437375392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb5ca5b6529483f2629b6a3e8d38a75090c22d543c77562dacb5c5c6d656ef06`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:55:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:59:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:59:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:59:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:00:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:00:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbf856ad4adc3f793ce064ea3fda7e4706e6e0d4b80ca4fe027d96f13a87dab`  
		Last Modified: Fri, 07 Jan 2022 04:32:02 GMT  
		Size: 839.5 KB (839500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19d9c773a8e3aa88af3da94878762a541aab51a81f76bb243ce22986621397`  
		Last Modified: Fri, 07 Jan 2022 04:32:00 GMT  
		Size: 4.9 MB (4872675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56d181a6951ac02f2348017091a5ea75f9c9b179c5aca8afec0a206090b6e3`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089e5a8628e7bc56e73d03702ed0336e18cdf2376719b4c9bc41aaf9f4feb69e`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb0fe2a049369c3aa544eb6b4f7c1f9f7a40074b0d95e8c5d4c8aae1b3995e9`  
		Last Modified: Fri, 07 Jan 2022 04:32:47 GMT  
		Size: 259.4 MB (259449273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3ff65a6b590db242ed4d09391158922c6d1e24a633dd27d58482854501332`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654ab1c4144dbdbf70fdd206f268a6b0c73e0d75aa43c7ae81675a3f1a469003`  
		Last Modified: Fri, 07 Jan 2022 04:33:10 GMT  
		Size: 70.2 MB (70235637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef173f71564f9fa83bd3290bf69987840b7b26a538f67ae46de90934396ea83e`  
		Last Modified: Fri, 07 Jan 2022 04:32:59 GMT  
		Size: 275.9 KB (275867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fd5992e383f303d239a085959c8f07efbe0bdd1cf70c5d4aee0eeafc428dec`  
		Last Modified: Fri, 07 Jan 2022 04:33:15 GMT  
		Size: 75.0 MB (74994999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:1698701dbbb4fb1d2820c370b866ca1cfd736eb9ec8be5d83b67ff883c12da31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385879479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e840122aab862341d9c8ff4ffd9f725d70333aac4618b815a2eb95e45ea9d0b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:03 GMT
ADD file:04c050ae3b998115f9e3f0da295a93a62bdff5d2efc3c37e792665d263cbf804 in / 
# Fri, 07 Jan 2022 02:26:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:41:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:41:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:41:59 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:45:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:45:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:46:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:46:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db4feefed17933b9e08cd0d0fd6c63db5c115552848576f2bc2062c8c5f69628`  
		Last Modified: Fri, 07 Jan 2022 02:30:10 GMT  
		Size: 22.3 MB (22303634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b5a1a2a0cd898e6a263e2752a2a0c70e3b9f18aca5e6dd0d1fc3bd11e2fc05`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 840.2 KB (840158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc89e947a0da5dceeebc4b92b77167fc247cb9805bffda1d5b6dc231c4f780`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 4.1 MB (4086107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb0ea1bc505b6e24af6dfd211660f3460432820e6b8c1f760bb7ea6c17913d`  
		Last Modified: Fri, 07 Jan 2022 04:05:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09688fa34b6295d2f86dacfd315dcae2bebc5b999531d3c87f78eb9a9a20457d`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977285ff1ff017f6f62e983da18f935bc160be6b6198dbd8624027b4f059a7a`  
		Last Modified: Fri, 07 Jan 2022 04:08:27 GMT  
		Size: 238.9 MB (238920238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b3b7c7ee0ad28b5bf8f651f9dbb344529ec73f21eab872fb5bab652dbf08e`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea142cf00340822a541e62a3c5918346f6f80d2b9ee4b3730c2374cb23b5e8`  
		Last Modified: Fri, 07 Jan 2022 04:09:11 GMT  
		Size: 54.7 MB (54704807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505bd1f0567e09c1ba0faecf71656cbb1d54e9daef574fcca4238df773defe01`  
		Last Modified: Fri, 07 Jan 2022 04:08:42 GMT  
		Size: 275.8 KB (275818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad17b52c3afe2f4e17f6930b9001b9008b8864e9d71ea854774ebcbabaf9dbb`  
		Last Modified: Fri, 07 Jan 2022 04:09:25 GMT  
		Size: 64.7 MB (64746306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bbb1ffc350458f77e3acb322553eac1333fa186131f11164517efc40fe532a0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.5 MB (411535638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b79a6f7bc4df605028d8554e55d499fad95c222cfd69f5478d8e581fb74e3e93`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:10:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:10:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:10:35 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:10:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:10:37 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:12:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:12:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:12:07 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:12:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:13:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7cb05d07ef46feac0fe88a2a5076e86982a4783b2bd17c98cf09974e499fd`  
		Last Modified: Fri, 07 Jan 2022 03:33:03 GMT  
		Size: 839.7 KB (839701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26bd7d783afca747fac46c5c9e260d26c390e10997bb98aa9916c1d64e138`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 4.3 MB (4263976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1962a21cee4ae01758aa1e7590e18d5b4447a0367015777fee7c81f8b7eac5`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e8179c314f217515dcf0a6d2885f2052277608fa6a674eb34d27d962d73c40`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992366677b7dcdca6e06367d0f8144bd2730dd68ae4a3ada2877eb399f28bd86`  
		Last Modified: Fri, 07 Jan 2022 03:33:38 GMT  
		Size: 252.4 MB (252357211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c0fcb5d49558d6ca44a8e0671e4bf31db08a187b90278eddda3cd6b18a564`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26ee3aa7ab81e1ae02f90c68840af00275e514a1856ea2c341aa79a0f38e9e7`  
		Last Modified: Fri, 07 Jan 2022 03:34:00 GMT  
		Size: 63.1 MB (63067247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ed727ae92cb44ed96c637dde8e913fb1a0dfc87c6a50ad27fbbf7ad7ebda77`  
		Last Modified: Fri, 07 Jan 2022 03:33:52 GMT  
		Size: 275.8 KB (275812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9649eedfe287e53fba655551c5e75655c3096639775d06d0f681cf3e075642`  
		Last Modified: Fri, 07 Jan 2022 03:34:02 GMT  
		Size: 67.0 MB (67002406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:50f269b0b49d03ccd82ccbb218f67d8c2d5c4cfa31653a9244aadbb2f4f7c034
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:bb3438831733d7259a71546d7ab92a3b3ad1ff0c1326aaf1d5abd4536fb52a4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291868889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75506b391d30e869af6d027c5baaba17b6ef62ac7fa7b670dad24d207c337744`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:55:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:59:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:59:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:59:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbf856ad4adc3f793ce064ea3fda7e4706e6e0d4b80ca4fe027d96f13a87dab`  
		Last Modified: Fri, 07 Jan 2022 04:32:02 GMT  
		Size: 839.5 KB (839500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19d9c773a8e3aa88af3da94878762a541aab51a81f76bb243ce22986621397`  
		Last Modified: Fri, 07 Jan 2022 04:32:00 GMT  
		Size: 4.9 MB (4872675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56d181a6951ac02f2348017091a5ea75f9c9b179c5aca8afec0a206090b6e3`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089e5a8628e7bc56e73d03702ed0336e18cdf2376719b4c9bc41aaf9f4feb69e`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb0fe2a049369c3aa544eb6b4f7c1f9f7a40074b0d95e8c5d4c8aae1b3995e9`  
		Last Modified: Fri, 07 Jan 2022 04:32:47 GMT  
		Size: 259.4 MB (259449273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3ff65a6b590db242ed4d09391158922c6d1e24a633dd27d58482854501332`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:636f37a5d033d998428a18ab30152404825f8c7f2dde56d586c35987b8c10935
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266152548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5aa91d6c4305b8309cd446a9cbc96c231d2da7ffd19240a281d546e9709a63c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:03 GMT
ADD file:04c050ae3b998115f9e3f0da295a93a62bdff5d2efc3c37e792665d263cbf804 in / 
# Fri, 07 Jan 2022 02:26:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:41:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:41:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:41:59 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:45:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:45:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:db4feefed17933b9e08cd0d0fd6c63db5c115552848576f2bc2062c8c5f69628`  
		Last Modified: Fri, 07 Jan 2022 02:30:10 GMT  
		Size: 22.3 MB (22303634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b5a1a2a0cd898e6a263e2752a2a0c70e3b9f18aca5e6dd0d1fc3bd11e2fc05`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 840.2 KB (840158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc89e947a0da5dceeebc4b92b77167fc247cb9805bffda1d5b6dc231c4f780`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 4.1 MB (4086107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb0ea1bc505b6e24af6dfd211660f3460432820e6b8c1f760bb7ea6c17913d`  
		Last Modified: Fri, 07 Jan 2022 04:05:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09688fa34b6295d2f86dacfd315dcae2bebc5b999531d3c87f78eb9a9a20457d`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977285ff1ff017f6f62e983da18f935bc160be6b6198dbd8624027b4f059a7a`  
		Last Modified: Fri, 07 Jan 2022 04:08:27 GMT  
		Size: 238.9 MB (238920238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b3b7c7ee0ad28b5bf8f651f9dbb344529ec73f21eab872fb5bab652dbf08e`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:56d06aefa375942722d64ad261ee56402ec50704cc0e60414a7115b645f57b97
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281190173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92f626f8ecb30009f8a752384bce5a1626cbd813f7f29ccf4e4f3d3d8774d5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:10:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:10:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:10:35 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:10:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:10:37 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:12:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:12:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:12:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7cb05d07ef46feac0fe88a2a5076e86982a4783b2bd17c98cf09974e499fd`  
		Last Modified: Fri, 07 Jan 2022 03:33:03 GMT  
		Size: 839.7 KB (839701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26bd7d783afca747fac46c5c9e260d26c390e10997bb98aa9916c1d64e138`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 4.3 MB (4263976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1962a21cee4ae01758aa1e7590e18d5b4447a0367015777fee7c81f8b7eac5`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e8179c314f217515dcf0a6d2885f2052277608fa6a674eb34d27d962d73c40`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992366677b7dcdca6e06367d0f8144bd2730dd68ae4a3ada2877eb399f28bd86`  
		Last Modified: Fri, 07 Jan 2022 03:33:38 GMT  
		Size: 252.4 MB (252357211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c0fcb5d49558d6ca44a8e0671e4bf31db08a187b90278eddda3cd6b18a564`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:50f269b0b49d03ccd82ccbb218f67d8c2d5c4cfa31653a9244aadbb2f4f7c034
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:bb3438831733d7259a71546d7ab92a3b3ad1ff0c1326aaf1d5abd4536fb52a4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291868889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75506b391d30e869af6d027c5baaba17b6ef62ac7fa7b670dad24d207c337744`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:55:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:55:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:55:32 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:59:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:59:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:59:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbf856ad4adc3f793ce064ea3fda7e4706e6e0d4b80ca4fe027d96f13a87dab`  
		Last Modified: Fri, 07 Jan 2022 04:32:02 GMT  
		Size: 839.5 KB (839500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d19d9c773a8e3aa88af3da94878762a541aab51a81f76bb243ce22986621397`  
		Last Modified: Fri, 07 Jan 2022 04:32:00 GMT  
		Size: 4.9 MB (4872675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56d181a6951ac02f2348017091a5ea75f9c9b179c5aca8afec0a206090b6e3`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089e5a8628e7bc56e73d03702ed0336e18cdf2376719b4c9bc41aaf9f4feb69e`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb0fe2a049369c3aa544eb6b4f7c1f9f7a40074b0d95e8c5d4c8aae1b3995e9`  
		Last Modified: Fri, 07 Jan 2022 04:32:47 GMT  
		Size: 259.4 MB (259449273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3ff65a6b590db242ed4d09391158922c6d1e24a633dd27d58482854501332`  
		Last Modified: Fri, 07 Jan 2022 04:31:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:636f37a5d033d998428a18ab30152404825f8c7f2dde56d586c35987b8c10935
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266152548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5aa91d6c4305b8309cd446a9cbc96c231d2da7ffd19240a281d546e9709a63c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:03 GMT
ADD file:04c050ae3b998115f9e3f0da295a93a62bdff5d2efc3c37e792665d263cbf804 in / 
# Fri, 07 Jan 2022 02:26:04 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:41:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:41:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:41:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:41:59 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:42:00 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:45:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:45:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:45:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:db4feefed17933b9e08cd0d0fd6c63db5c115552848576f2bc2062c8c5f69628`  
		Last Modified: Fri, 07 Jan 2022 02:30:10 GMT  
		Size: 22.3 MB (22303634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b5a1a2a0cd898e6a263e2752a2a0c70e3b9f18aca5e6dd0d1fc3bd11e2fc05`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 840.2 KB (840158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc89e947a0da5dceeebc4b92b77167fc247cb9805bffda1d5b6dc231c4f780`  
		Last Modified: Fri, 07 Jan 2022 04:06:00 GMT  
		Size: 4.1 MB (4086107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb0ea1bc505b6e24af6dfd211660f3460432820e6b8c1f760bb7ea6c17913d`  
		Last Modified: Fri, 07 Jan 2022 04:05:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09688fa34b6295d2f86dacfd315dcae2bebc5b999531d3c87f78eb9a9a20457d`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977285ff1ff017f6f62e983da18f935bc160be6b6198dbd8624027b4f059a7a`  
		Last Modified: Fri, 07 Jan 2022 04:08:27 GMT  
		Size: 238.9 MB (238920238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b3b7c7ee0ad28b5bf8f651f9dbb344529ec73f21eab872fb5bab652dbf08e`  
		Last Modified: Fri, 07 Jan 2022 04:05:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:56d06aefa375942722d64ad261ee56402ec50704cc0e60414a7115b645f57b97
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281190173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92f626f8ecb30009f8a752384bce5a1626cbd813f7f29ccf4e4f3d3d8774d5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:10:13 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:23 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:10:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:10:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:10:35 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:10:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:10:37 GMT
ENV ROS_DISTRO=melodic
# Fri, 07 Jan 2022 03:12:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:12:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:12:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:12:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f7cb05d07ef46feac0fe88a2a5076e86982a4783b2bd17c98cf09974e499fd`  
		Last Modified: Fri, 07 Jan 2022 03:33:03 GMT  
		Size: 839.7 KB (839701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a26bd7d783afca747fac46c5c9e260d26c390e10997bb98aa9916c1d64e138`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 4.3 MB (4263976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1962a21cee4ae01758aa1e7590e18d5b4447a0367015777fee7c81f8b7eac5`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e8179c314f217515dcf0a6d2885f2052277608fa6a674eb34d27d962d73c40`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992366677b7dcdca6e06367d0f8144bd2730dd68ae4a3ada2877eb399f28bd86`  
		Last Modified: Fri, 07 Jan 2022 03:33:38 GMT  
		Size: 252.4 MB (252357211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c0fcb5d49558d6ca44a8e0671e4bf31db08a187b90278eddda3cd6b18a564`  
		Last Modified: Fri, 07 Jan 2022 03:33:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:9c5c4876665c915a2188fff45aa3787780df0fcfbb36f8b02bf99626f5be2269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:cdb6dd43fd7180cf8be3bdecb65efc01c33e3c8325a71d2be4f491ae3a1c8f9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.3 MB (339348363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b54a33fb042ad416736d85acecaebe856430501f69b01ed3fe50929694c31e4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:09:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 04:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 04:12:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:12:09 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:12:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c70e9658293d6c6994b6a7c4cdaa6377ff6c88e8aacb0cc925a437b7f64d`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b560e1d79dbdd0e1849bd0bf9e744605e7fac17d52d9eae6a2eb85191f795c`  
		Last Modified: Fri, 07 Jan 2022 04:34:46 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19690a1594bd61dff284097ca83119bb45eb8440545c32da4c0922132b07a310`  
		Last Modified: Fri, 07 Jan 2022 04:35:27 GMT  
		Size: 176.9 MB (176882711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1f25217df1dd04bb397f3964b212a7132b0589c74df28014755ac8a8242d39`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ffdfe95d3dd2037023009ce14081cded135d4297f961ccfeefd666265cc7a`  
		Last Modified: Fri, 07 Jan 2022 04:35:51 GMT  
		Size: 47.3 MB (47259832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a460a4cc48907ba7a3f48875ff90081588a2252332a03cd88eaa72be2ae16c0`  
		Last Modified: Fri, 07 Jan 2022 04:35:43 GMT  
		Size: 305.2 KB (305157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406044e053161a2f909c8a24c374019c518eb7ecc7541ad0de4b194271415c57`  
		Last Modified: Fri, 07 Jan 2022 04:35:55 GMT  
		Size: 79.6 MB (79602648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:e66897669f09dd7c3d68ea4c4fe34df26ca125964acb093d94837a7b2e1f8475
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.8 MB (284829867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24a354a8ad393a77a9d504c5970f4f9e95ae30b040be31b115e757aa416ef4fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:25 GMT
ADD file:ac83e0dc7e48a0dc1805c0fd7b71b8eb119b3eeafd1fdcab93e11fbc9c0bcda0 in / 
# Fri, 07 Jan 2022 02:26:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:53:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:53:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:53:38 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:56:18 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:56:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:57:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b8080fa0945580f29aa3abed4664f8ab849229eca04510b5d259a9e29616064`  
		Last Modified: Fri, 07 Jan 2022 02:30:39 GMT  
		Size: 24.1 MB (24064434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4542f65e85cdaf2541613579d209e8ddfa8b797d8edd23c4b1b3e430580dfb8c`  
		Last Modified: Fri, 07 Jan 2022 04:13:02 GMT  
		Size: 1.2 MB (1183516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc20ad2d3acd4173d1357bb75d2d434c2cf628930746de1b638775ce5b3f169`  
		Last Modified: Fri, 07 Jan 2022 04:13:01 GMT  
		Size: 4.7 MB (4676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038a958a9812e6ad8943ca985ee5fc0fa712bd2bb652825668f1e805642250bb`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14895cbe261aa62a0bacb72a62e26758d9c4917efcc5e712fc9f8a815cc2b2df`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05603c4fd7f49169b1f830d906412ac1eb62f339ab3b8518b04e0d0df814b72`  
		Last Modified: Fri, 07 Jan 2022 04:15:07 GMT  
		Size: 157.4 MB (157422125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4937926a5187427a5b557119d517c0cb7b07dd1ec423d7aa471bbf95e1fcfe8`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c707c45473b692c29e259d0c26776db6360563b1a2d369a2e46e30f9e6f053`  
		Last Modified: Fri, 07 Jan 2022 04:15:41 GMT  
		Size: 36.7 MB (36693115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4d7df5c0cc0093b02360bb46f1cf1e7f633acd03cf4ce2cc15d489a0039acb`  
		Last Modified: Fri, 07 Jan 2022 04:15:22 GMT  
		Size: 305.2 KB (305155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9129d7514384ec5dc914d6cc465ffc40283fc596a024219bbd74ecb6ecf66c50`  
		Last Modified: Fri, 07 Jan 2022 04:16:01 GMT  
		Size: 60.5 MB (60482237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e06329d279bf417cd354a1f84def2aaa84138eaab33b5c2e3cbc07a61c414734
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.4 MB (318371559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae709f5f9cd5d04bf4f12d3cdf79edc876767938a542b3fb39c09b88ae598037`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:16:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:16:02 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:16:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:16:04 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:17:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:17:08 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:17:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3843c054baee6fdbb1122ab1ef12464d44642d23fcccbdf9dcb77a02e41bfc7a`  
		Last Modified: Fri, 07 Jan 2022 03:35:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f924ca980605e9e62baf57692a5657c36e9189d8794573f729f971c5ed32bb`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b0eece4cf7bea41c5acd111a551c273d6e153407fcc2744b14a155e05366b`  
		Last Modified: Fri, 07 Jan 2022 03:35:57 GMT  
		Size: 171.3 MB (171326015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a972d654bf4928ae873620e2c0012b7fb3d477f39d368d27ad70a7083fd8a2`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc978c5c6ccf265e99aa4eafe327bc1a79aca0405c567834589c5f2eb1f4a7da`  
		Last Modified: Fri, 07 Jan 2022 03:36:15 GMT  
		Size: 41.3 MB (41306233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587d30d9aed449ad7397931e249b18f034edf5cc07d2ee00610e1972a388f9a`  
		Last Modified: Fri, 07 Jan 2022 03:36:09 GMT  
		Size: 305.1 KB (305107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5814684186464d45ad335516ea3732d0f22a6b4c201319d425fd6324ba9a5e67`  
		Last Modified: Fri, 07 Jan 2022 03:36:19 GMT  
		Size: 71.8 MB (71753993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:0c7f8ff67f8ba3997601c3023352dd5c3143717282f876a81b899620f31866ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:ae7a9381ec90cabd6293626b4d4dc7a7c3a2928b05d259df1398e749a767f310
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **830.5 MB (830492053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22e4a30e7a04b988ce6dd6d676724f1d468aaee1c114880010b2491af6e0c814`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:09:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 04:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 04:12:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:12:09 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:12:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c70e9658293d6c6994b6a7c4cdaa6377ff6c88e8aacb0cc925a437b7f64d`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b560e1d79dbdd0e1849bd0bf9e744605e7fac17d52d9eae6a2eb85191f795c`  
		Last Modified: Fri, 07 Jan 2022 04:34:46 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19690a1594bd61dff284097ca83119bb45eb8440545c32da4c0922132b07a310`  
		Last Modified: Fri, 07 Jan 2022 04:35:27 GMT  
		Size: 176.9 MB (176882711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1f25217df1dd04bb397f3964b212a7132b0589c74df28014755ac8a8242d39`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ffdfe95d3dd2037023009ce14081cded135d4297f961ccfeefd666265cc7a`  
		Last Modified: Fri, 07 Jan 2022 04:35:51 GMT  
		Size: 47.3 MB (47259832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a460a4cc48907ba7a3f48875ff90081588a2252332a03cd88eaa72be2ae16c0`  
		Last Modified: Fri, 07 Jan 2022 04:35:43 GMT  
		Size: 305.2 KB (305157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406044e053161a2f909c8a24c374019c518eb7ecc7541ad0de4b194271415c57`  
		Last Modified: Fri, 07 Jan 2022 04:35:55 GMT  
		Size: 79.6 MB (79602648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1ce7466821e5a5d0e3561de4e5a4cc3a4aa853d74586fa50d9c8fe7ac4bbe3`  
		Last Modified: Fri, 07 Jan 2022 04:37:32 GMT  
		Size: 491.1 MB (491143690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:7c6c88a1d0bb98f2392fd70c79935ee6767576383924a1a13fbbb4d36922a4f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **721.1 MB (721109316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6028632106c6e4cb54ec03431de5a4e7ca6cd0ab5f3cfd24dc29340ef38c668f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:25 GMT
ADD file:ac83e0dc7e48a0dc1805c0fd7b71b8eb119b3eeafd1fdcab93e11fbc9c0bcda0 in / 
# Fri, 07 Jan 2022 02:26:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:53:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:53:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:53:38 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:56:18 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:56:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:57:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:04:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b8080fa0945580f29aa3abed4664f8ab849229eca04510b5d259a9e29616064`  
		Last Modified: Fri, 07 Jan 2022 02:30:39 GMT  
		Size: 24.1 MB (24064434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4542f65e85cdaf2541613579d209e8ddfa8b797d8edd23c4b1b3e430580dfb8c`  
		Last Modified: Fri, 07 Jan 2022 04:13:02 GMT  
		Size: 1.2 MB (1183516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc20ad2d3acd4173d1357bb75d2d434c2cf628930746de1b638775ce5b3f169`  
		Last Modified: Fri, 07 Jan 2022 04:13:01 GMT  
		Size: 4.7 MB (4676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038a958a9812e6ad8943ca985ee5fc0fa712bd2bb652825668f1e805642250bb`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14895cbe261aa62a0bacb72a62e26758d9c4917efcc5e712fc9f8a815cc2b2df`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05603c4fd7f49169b1f830d906412ac1eb62f339ab3b8518b04e0d0df814b72`  
		Last Modified: Fri, 07 Jan 2022 04:15:07 GMT  
		Size: 157.4 MB (157422125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4937926a5187427a5b557119d517c0cb7b07dd1ec423d7aa471bbf95e1fcfe8`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c707c45473b692c29e259d0c26776db6360563b1a2d369a2e46e30f9e6f053`  
		Last Modified: Fri, 07 Jan 2022 04:15:41 GMT  
		Size: 36.7 MB (36693115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4d7df5c0cc0093b02360bb46f1cf1e7f633acd03cf4ce2cc15d489a0039acb`  
		Last Modified: Fri, 07 Jan 2022 04:15:22 GMT  
		Size: 305.2 KB (305155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9129d7514384ec5dc914d6cc465ffc40283fc596a024219bbd74ecb6ecf66c50`  
		Last Modified: Fri, 07 Jan 2022 04:16:01 GMT  
		Size: 60.5 MB (60482237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717ce4b02e355c16404348953d4d926519f98473bccc7cb58ac5c30b8e18b3c7`  
		Last Modified: Fri, 07 Jan 2022 04:21:08 GMT  
		Size: 436.3 MB (436279449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:eb5d4d883e52520819da468f310545e580d9b8d063f73e8573f3addd710ae069
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **780.1 MB (780106767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa9a0b5f335bd160a4a319a25f1c844783f88048a4d4b6b03841d19e16757cb0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:16:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:16:02 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:16:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:16:04 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:17:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:17:08 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:17:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:20:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3843c054baee6fdbb1122ab1ef12464d44642d23fcccbdf9dcb77a02e41bfc7a`  
		Last Modified: Fri, 07 Jan 2022 03:35:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f924ca980605e9e62baf57692a5657c36e9189d8794573f729f971c5ed32bb`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b0eece4cf7bea41c5acd111a551c273d6e153407fcc2744b14a155e05366b`  
		Last Modified: Fri, 07 Jan 2022 03:35:57 GMT  
		Size: 171.3 MB (171326015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a972d654bf4928ae873620e2c0012b7fb3d477f39d368d27ad70a7083fd8a2`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc978c5c6ccf265e99aa4eafe327bc1a79aca0405c567834589c5f2eb1f4a7da`  
		Last Modified: Fri, 07 Jan 2022 03:36:15 GMT  
		Size: 41.3 MB (41306233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587d30d9aed449ad7397931e249b18f034edf5cc07d2ee00610e1972a388f9a`  
		Last Modified: Fri, 07 Jan 2022 03:36:09 GMT  
		Size: 305.1 KB (305107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5814684186464d45ad335516ea3732d0f22a6b4c201319d425fd6324ba9a5e67`  
		Last Modified: Fri, 07 Jan 2022 03:36:19 GMT  
		Size: 71.8 MB (71753993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce42ea2594c2658568488e507dbab59fc44b7afbf9177364a2502ca7a4e60d`  
		Last Modified: Fri, 07 Jan 2022 03:37:57 GMT  
		Size: 461.7 MB (461735208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:167b7b6f358b174b368f4ac11c5be378a23ac75804aa513140beda90224ee835
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:660563293fe042432f396c8ac933fd204d73e5b24f151487eb7728f6c2ab39d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.3 MB (951250673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdde8d2d8755a07c3c5da3e93fc5ea727ef066ad786848c2d224e4826b107c4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:56:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:56:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 21 Dec 2021 23:56:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LC_ALL=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV ROS_DISTRO=noetic
# Tue, 21 Dec 2021 23:57:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:57:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 21 Dec 2021 23:57:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 21 Dec 2021 23:57:28 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:58:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:58:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 21 Dec 2021 23:58:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 00:01:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a21eb75d0e3012979c6611472ad2ce77f9603178d355b33e3a29b873c09cd17`  
		Last Modified: Wed, 22 Dec 2021 00:03:48 GMT  
		Size: 10.9 MB (10891938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8a0355b4bb6623abb06a5060650fda200f613e82ff0c1660f1dd412468468d`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428381b1469052a8549b56c928ac7628c4b0b3212ab6a0e15cd9a7cb0836f7cb`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb2dc8dfc87f5650375873e92661d1220cf0d1ef485c60f8350795669a60fb`  
		Last Modified: Wed, 22 Dec 2021 00:04:21 GMT  
		Size: 239.1 MB (239089267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5280b24f54ae8eeabff880a2eab6ce4c01ea397fe51e158a984ddcc9b1812a`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384ffdd3a88cfad1dba9934a89583cde7175d36b67c35c33b81f4c51b4929654`  
		Last Modified: Wed, 22 Dec 2021 00:04:42 GMT  
		Size: 86.6 MB (86566404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e7347f2acf99a04e2a51ce3ab3a4fdf9b42d547819a739899ee16bd110ff06`  
		Last Modified: Wed, 22 Dec 2021 00:04:28 GMT  
		Size: 299.5 KB (299501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2bbb76c6ff423ad3e4b2298c17b2c64a171419f8c2c1ad315e018fcc912963`  
		Last Modified: Wed, 22 Dec 2021 00:04:40 GMT  
		Size: 76.0 MB (75976617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0556db625d721c637145645d2c1eca3cf524fb0c426003beefeafa8f07487bf2`  
		Last Modified: Wed, 22 Dec 2021 00:06:43 GMT  
		Size: 488.0 MB (487987395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:20cc80458c2dd04979d9251a7ec5f326f97ca31d04ec56257c25fb04221c0839
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **867.4 MB (867435386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65f8851bcebeee3a4a6d2a5bc6d59f0ff175f3c398641b0c1ff6aa94b4fe83d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:43:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:43:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 26 Jan 2022 07:43:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 26 Jan 2022 07:43:57 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 07:43:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 26 Jan 2022 07:43:59 GMT
ENV ROS_DISTRO=noetic
# Wed, 26 Jan 2022 07:45:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:45:12 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 26 Jan 2022 07:45:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 26 Jan 2022 07:45:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:45:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:45:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 26 Jan 2022 07:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:50:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646734dd4c9771207c4468eadc7ddcededd306975b1af9c589d4cdcda9b7c07b`  
		Last Modified: Wed, 26 Jan 2022 07:52:46 GMT  
		Size: 10.7 MB (10688073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3aad39826b43f6faf1264f98a0a52a206ef90890c6834072d8d9f87d882868d`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed8a7e03b40bfdb16508119c9ee410dd3684b3a5cf4bc31f5f6dd1597a12fee`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32e34cb56b02431259e0ed70e5f2a62c5cbae86038cc51c240276d1c687014f`  
		Last Modified: Wed, 26 Jan 2022 07:53:15 GMT  
		Size: 184.3 MB (184306695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86270cb85ef2ff4c03d623ecfac134b2c9cc1bbd6a17a0d9a16eb961841ab45`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead2d175559e1deb0533f1a26d062151a70ee020c83b271d672febcae2962201`  
		Last Modified: Wed, 26 Jan 2022 07:53:34 GMT  
		Size: 84.4 MB (84350117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ee083a5f0a1bb7f96a6fa942a09843a7a85dd23f6c421fc1030cc2233c1fb0`  
		Last Modified: Wed, 26 Jan 2022 07:53:24 GMT  
		Size: 301.2 KB (301224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f310f444237727027c0400435c277b87c69c67df7b68e96da508934404d5a1`  
		Last Modified: Wed, 26 Jan 2022 07:53:34 GMT  
		Size: 73.9 MB (73864375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25c3ada56186c8e10baa41dd6c8ee8692cba6677a7e6d213bcde8400e096e56`  
		Last Modified: Wed, 26 Jan 2022 07:55:03 GMT  
		Size: 464.7 MB (464699490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:0c7f8ff67f8ba3997601c3023352dd5c3143717282f876a81b899620f31866ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:ae7a9381ec90cabd6293626b4d4dc7a7c3a2928b05d259df1398e749a767f310
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **830.5 MB (830492053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22e4a30e7a04b988ce6dd6d676724f1d468aaee1c114880010b2491af6e0c814`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:09:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 04:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 04:12:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:12:09 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:12:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c70e9658293d6c6994b6a7c4cdaa6377ff6c88e8aacb0cc925a437b7f64d`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b560e1d79dbdd0e1849bd0bf9e744605e7fac17d52d9eae6a2eb85191f795c`  
		Last Modified: Fri, 07 Jan 2022 04:34:46 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19690a1594bd61dff284097ca83119bb45eb8440545c32da4c0922132b07a310`  
		Last Modified: Fri, 07 Jan 2022 04:35:27 GMT  
		Size: 176.9 MB (176882711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1f25217df1dd04bb397f3964b212a7132b0589c74df28014755ac8a8242d39`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ffdfe95d3dd2037023009ce14081cded135d4297f961ccfeefd666265cc7a`  
		Last Modified: Fri, 07 Jan 2022 04:35:51 GMT  
		Size: 47.3 MB (47259832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a460a4cc48907ba7a3f48875ff90081588a2252332a03cd88eaa72be2ae16c0`  
		Last Modified: Fri, 07 Jan 2022 04:35:43 GMT  
		Size: 305.2 KB (305157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406044e053161a2f909c8a24c374019c518eb7ecc7541ad0de4b194271415c57`  
		Last Modified: Fri, 07 Jan 2022 04:35:55 GMT  
		Size: 79.6 MB (79602648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1ce7466821e5a5d0e3561de4e5a4cc3a4aa853d74586fa50d9c8fe7ac4bbe3`  
		Last Modified: Fri, 07 Jan 2022 04:37:32 GMT  
		Size: 491.1 MB (491143690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:7c6c88a1d0bb98f2392fd70c79935ee6767576383924a1a13fbbb4d36922a4f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **721.1 MB (721109316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6028632106c6e4cb54ec03431de5a4e7ca6cd0ab5f3cfd24dc29340ef38c668f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:25 GMT
ADD file:ac83e0dc7e48a0dc1805c0fd7b71b8eb119b3eeafd1fdcab93e11fbc9c0bcda0 in / 
# Fri, 07 Jan 2022 02:26:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:53:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:53:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:53:38 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:56:18 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:56:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:57:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:04:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b8080fa0945580f29aa3abed4664f8ab849229eca04510b5d259a9e29616064`  
		Last Modified: Fri, 07 Jan 2022 02:30:39 GMT  
		Size: 24.1 MB (24064434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4542f65e85cdaf2541613579d209e8ddfa8b797d8edd23c4b1b3e430580dfb8c`  
		Last Modified: Fri, 07 Jan 2022 04:13:02 GMT  
		Size: 1.2 MB (1183516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc20ad2d3acd4173d1357bb75d2d434c2cf628930746de1b638775ce5b3f169`  
		Last Modified: Fri, 07 Jan 2022 04:13:01 GMT  
		Size: 4.7 MB (4676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038a958a9812e6ad8943ca985ee5fc0fa712bd2bb652825668f1e805642250bb`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14895cbe261aa62a0bacb72a62e26758d9c4917efcc5e712fc9f8a815cc2b2df`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05603c4fd7f49169b1f830d906412ac1eb62f339ab3b8518b04e0d0df814b72`  
		Last Modified: Fri, 07 Jan 2022 04:15:07 GMT  
		Size: 157.4 MB (157422125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4937926a5187427a5b557119d517c0cb7b07dd1ec423d7aa471bbf95e1fcfe8`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c707c45473b692c29e259d0c26776db6360563b1a2d369a2e46e30f9e6f053`  
		Last Modified: Fri, 07 Jan 2022 04:15:41 GMT  
		Size: 36.7 MB (36693115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4d7df5c0cc0093b02360bb46f1cf1e7f633acd03cf4ce2cc15d489a0039acb`  
		Last Modified: Fri, 07 Jan 2022 04:15:22 GMT  
		Size: 305.2 KB (305155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9129d7514384ec5dc914d6cc465ffc40283fc596a024219bbd74ecb6ecf66c50`  
		Last Modified: Fri, 07 Jan 2022 04:16:01 GMT  
		Size: 60.5 MB (60482237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717ce4b02e355c16404348953d4d926519f98473bccc7cb58ac5c30b8e18b3c7`  
		Last Modified: Fri, 07 Jan 2022 04:21:08 GMT  
		Size: 436.3 MB (436279449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:eb5d4d883e52520819da468f310545e580d9b8d063f73e8573f3addd710ae069
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **780.1 MB (780106767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa9a0b5f335bd160a4a319a25f1c844783f88048a4d4b6b03841d19e16757cb0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:16:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:16:02 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:16:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:16:04 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:17:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:17:08 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:17:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:20:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3843c054baee6fdbb1122ab1ef12464d44642d23fcccbdf9dcb77a02e41bfc7a`  
		Last Modified: Fri, 07 Jan 2022 03:35:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f924ca980605e9e62baf57692a5657c36e9189d8794573f729f971c5ed32bb`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b0eece4cf7bea41c5acd111a551c273d6e153407fcc2744b14a155e05366b`  
		Last Modified: Fri, 07 Jan 2022 03:35:57 GMT  
		Size: 171.3 MB (171326015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a972d654bf4928ae873620e2c0012b7fb3d477f39d368d27ad70a7083fd8a2`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc978c5c6ccf265e99aa4eafe327bc1a79aca0405c567834589c5f2eb1f4a7da`  
		Last Modified: Fri, 07 Jan 2022 03:36:15 GMT  
		Size: 41.3 MB (41306233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587d30d9aed449ad7397931e249b18f034edf5cc07d2ee00610e1972a388f9a`  
		Last Modified: Fri, 07 Jan 2022 03:36:09 GMT  
		Size: 305.1 KB (305107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5814684186464d45ad335516ea3732d0f22a6b4c201319d425fd6324ba9a5e67`  
		Last Modified: Fri, 07 Jan 2022 03:36:19 GMT  
		Size: 71.8 MB (71753993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce42ea2594c2658568488e507dbab59fc44b7afbf9177364a2502ca7a4e60d`  
		Last Modified: Fri, 07 Jan 2022 03:37:57 GMT  
		Size: 461.7 MB (461735208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:59eacbe2019555b2140e52064fc136503de4c92224e8800260c9cafd921671b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:8c72ddfbb32990b47c330b1e3460edb1364a9fa14a09076aa5badfdd028f0d1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.1 MB (355096287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5feb1a7d49e7caff9438639adfed891fb866423159f1d2e7a94cac6c35c991cf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:09:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 04:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 04:12:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:12:09 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:12:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:15:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c70e9658293d6c6994b6a7c4cdaa6377ff6c88e8aacb0cc925a437b7f64d`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b560e1d79dbdd0e1849bd0bf9e744605e7fac17d52d9eae6a2eb85191f795c`  
		Last Modified: Fri, 07 Jan 2022 04:34:46 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19690a1594bd61dff284097ca83119bb45eb8440545c32da4c0922132b07a310`  
		Last Modified: Fri, 07 Jan 2022 04:35:27 GMT  
		Size: 176.9 MB (176882711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1f25217df1dd04bb397f3964b212a7132b0589c74df28014755ac8a8242d39`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ffdfe95d3dd2037023009ce14081cded135d4297f961ccfeefd666265cc7a`  
		Last Modified: Fri, 07 Jan 2022 04:35:51 GMT  
		Size: 47.3 MB (47259832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a460a4cc48907ba7a3f48875ff90081588a2252332a03cd88eaa72be2ae16c0`  
		Last Modified: Fri, 07 Jan 2022 04:35:43 GMT  
		Size: 305.2 KB (305157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406044e053161a2f909c8a24c374019c518eb7ecc7541ad0de4b194271415c57`  
		Last Modified: Fri, 07 Jan 2022 04:35:55 GMT  
		Size: 79.6 MB (79602648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c62d3edd88a3423f9d25b1fd55d069da77aa39216107cd15ae597095a5eec19`  
		Last Modified: Fri, 07 Jan 2022 04:36:11 GMT  
		Size: 15.7 MB (15747924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:b9786f018554e63eb35b049128513bc48960fcfbdccd2a1d2aaf77ba20f9272e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.8 MB (298795161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eba79af9952a9a631801829b405b79b7d26778ab1867a069101dbd9668dd741`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:25 GMT
ADD file:ac83e0dc7e48a0dc1805c0fd7b71b8eb119b3eeafd1fdcab93e11fbc9c0bcda0 in / 
# Fri, 07 Jan 2022 02:26:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:53:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:53:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:53:38 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:56:18 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:56:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:57:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:58:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b8080fa0945580f29aa3abed4664f8ab849229eca04510b5d259a9e29616064`  
		Last Modified: Fri, 07 Jan 2022 02:30:39 GMT  
		Size: 24.1 MB (24064434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4542f65e85cdaf2541613579d209e8ddfa8b797d8edd23c4b1b3e430580dfb8c`  
		Last Modified: Fri, 07 Jan 2022 04:13:02 GMT  
		Size: 1.2 MB (1183516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc20ad2d3acd4173d1357bb75d2d434c2cf628930746de1b638775ce5b3f169`  
		Last Modified: Fri, 07 Jan 2022 04:13:01 GMT  
		Size: 4.7 MB (4676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038a958a9812e6ad8943ca985ee5fc0fa712bd2bb652825668f1e805642250bb`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14895cbe261aa62a0bacb72a62e26758d9c4917efcc5e712fc9f8a815cc2b2df`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05603c4fd7f49169b1f830d906412ac1eb62f339ab3b8518b04e0d0df814b72`  
		Last Modified: Fri, 07 Jan 2022 04:15:07 GMT  
		Size: 157.4 MB (157422125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4937926a5187427a5b557119d517c0cb7b07dd1ec423d7aa471bbf95e1fcfe8`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c707c45473b692c29e259d0c26776db6360563b1a2d369a2e46e30f9e6f053`  
		Last Modified: Fri, 07 Jan 2022 04:15:41 GMT  
		Size: 36.7 MB (36693115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4d7df5c0cc0093b02360bb46f1cf1e7f633acd03cf4ce2cc15d489a0039acb`  
		Last Modified: Fri, 07 Jan 2022 04:15:22 GMT  
		Size: 305.2 KB (305155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9129d7514384ec5dc914d6cc465ffc40283fc596a024219bbd74ecb6ecf66c50`  
		Last Modified: Fri, 07 Jan 2022 04:16:01 GMT  
		Size: 60.5 MB (60482237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc05c61280ccbee68d9725b732b7601a0fc03e0f2edd5d5176e4e66579cec80`  
		Last Modified: Fri, 07 Jan 2022 04:16:27 GMT  
		Size: 14.0 MB (13965294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a90081f9ec434c8185ea5c679fab8b30c463b151fece201252a7da9d273fd1af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.7 MB (333719916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8403c60ca7b25d291234e6a029a14cb558858be7fcdb0b4a0e01171a4f7fcaf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:16:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:16:02 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:16:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:16:04 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:17:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:17:08 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:17:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:18:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3843c054baee6fdbb1122ab1ef12464d44642d23fcccbdf9dcb77a02e41bfc7a`  
		Last Modified: Fri, 07 Jan 2022 03:35:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f924ca980605e9e62baf57692a5657c36e9189d8794573f729f971c5ed32bb`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b0eece4cf7bea41c5acd111a551c273d6e153407fcc2744b14a155e05366b`  
		Last Modified: Fri, 07 Jan 2022 03:35:57 GMT  
		Size: 171.3 MB (171326015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a972d654bf4928ae873620e2c0012b7fb3d477f39d368d27ad70a7083fd8a2`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc978c5c6ccf265e99aa4eafe327bc1a79aca0405c567834589c5f2eb1f4a7da`  
		Last Modified: Fri, 07 Jan 2022 03:36:15 GMT  
		Size: 41.3 MB (41306233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587d30d9aed449ad7397931e249b18f034edf5cc07d2ee00610e1972a388f9a`  
		Last Modified: Fri, 07 Jan 2022 03:36:09 GMT  
		Size: 305.1 KB (305107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5814684186464d45ad335516ea3732d0f22a6b4c201319d425fd6324ba9a5e67`  
		Last Modified: Fri, 07 Jan 2022 03:36:19 GMT  
		Size: 71.8 MB (71753993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481e7053bd5452e8f9174b8d9f5d2b1e2128d338ac9cd6c5feede39785fb7a9`  
		Last Modified: Fri, 07 Jan 2022 03:36:38 GMT  
		Size: 15.3 MB (15348357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:19da1b920fa47f82f337414a8de7a731a9fee1a1dfa00d22d857b2e512e9f466
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:c366ff1f433aa6ca7017a717986d559bb76bf00e43c9f29f9824078a0cd5511b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.5 MB (484488286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640ec9b1d22a9db7b28b026a3c95a12096021c1daf92a247d3ea7a723a2569c8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:56:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:56:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 21 Dec 2021 23:56:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LC_ALL=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV ROS_DISTRO=noetic
# Tue, 21 Dec 2021 23:57:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:57:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 21 Dec 2021 23:57:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 21 Dec 2021 23:57:28 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:58:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:58:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 21 Dec 2021 23:58:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:58:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a21eb75d0e3012979c6611472ad2ce77f9603178d355b33e3a29b873c09cd17`  
		Last Modified: Wed, 22 Dec 2021 00:03:48 GMT  
		Size: 10.9 MB (10891938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8a0355b4bb6623abb06a5060650fda200f613e82ff0c1660f1dd412468468d`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428381b1469052a8549b56c928ac7628c4b0b3212ab6a0e15cd9a7cb0836f7cb`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb2dc8dfc87f5650375873e92661d1220cf0d1ef485c60f8350795669a60fb`  
		Last Modified: Wed, 22 Dec 2021 00:04:21 GMT  
		Size: 239.1 MB (239089267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5280b24f54ae8eeabff880a2eab6ce4c01ea397fe51e158a984ddcc9b1812a`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384ffdd3a88cfad1dba9934a89583cde7175d36b67c35c33b81f4c51b4929654`  
		Last Modified: Wed, 22 Dec 2021 00:04:42 GMT  
		Size: 86.6 MB (86566404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e7347f2acf99a04e2a51ce3ab3a4fdf9b42d547819a739899ee16bd110ff06`  
		Last Modified: Wed, 22 Dec 2021 00:04:28 GMT  
		Size: 299.5 KB (299501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2bbb76c6ff423ad3e4b2298c17b2c64a171419f8c2c1ad315e018fcc912963`  
		Last Modified: Wed, 22 Dec 2021 00:04:40 GMT  
		Size: 76.0 MB (75976617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507642102fd99860c1c0b68aeaa4d2e857b5de0b2a270bf81e5c3e6487153118`  
		Last Modified: Wed, 22 Dec 2021 00:04:53 GMT  
		Size: 21.2 MB (21225008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:576fa82187bd220314afd85c2dec1edd5a3dbff7ab9760bb708d809a53b36fa1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.8 MB (423837943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9c26c1d05bf8b845e9a78785db8b6c44eecb7d35712cae34868c7bace68ac4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:43:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:43:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 26 Jan 2022 07:43:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 26 Jan 2022 07:43:57 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 07:43:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 26 Jan 2022 07:43:59 GMT
ENV ROS_DISTRO=noetic
# Wed, 26 Jan 2022 07:45:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:45:12 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 26 Jan 2022 07:45:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 26 Jan 2022 07:45:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:45:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:45:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 26 Jan 2022 07:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:47:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646734dd4c9771207c4468eadc7ddcededd306975b1af9c589d4cdcda9b7c07b`  
		Last Modified: Wed, 26 Jan 2022 07:52:46 GMT  
		Size: 10.7 MB (10688073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3aad39826b43f6faf1264f98a0a52a206ef90890c6834072d8d9f87d882868d`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed8a7e03b40bfdb16508119c9ee410dd3684b3a5cf4bc31f5f6dd1597a12fee`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32e34cb56b02431259e0ed70e5f2a62c5cbae86038cc51c240276d1c687014f`  
		Last Modified: Wed, 26 Jan 2022 07:53:15 GMT  
		Size: 184.3 MB (184306695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86270cb85ef2ff4c03d623ecfac134b2c9cc1bbd6a17a0d9a16eb961841ab45`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead2d175559e1deb0533f1a26d062151a70ee020c83b271d672febcae2962201`  
		Last Modified: Wed, 26 Jan 2022 07:53:34 GMT  
		Size: 84.4 MB (84350117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ee083a5f0a1bb7f96a6fa942a09843a7a85dd23f6c421fc1030cc2233c1fb0`  
		Last Modified: Wed, 26 Jan 2022 07:53:24 GMT  
		Size: 301.2 KB (301224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f310f444237727027c0400435c277b87c69c67df7b68e96da508934404d5a1`  
		Last Modified: Wed, 26 Jan 2022 07:53:34 GMT  
		Size: 73.9 MB (73864375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d183952954eb4bb2037eb954eb068a02e117f48638cb6a216bd8ae16200ca0`  
		Last Modified: Wed, 26 Jan 2022 07:53:46 GMT  
		Size: 21.1 MB (21102047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:59eacbe2019555b2140e52064fc136503de4c92224e8800260c9cafd921671b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:8c72ddfbb32990b47c330b1e3460edb1364a9fa14a09076aa5badfdd028f0d1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.1 MB (355096287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5feb1a7d49e7caff9438639adfed891fb866423159f1d2e7a94cac6c35c991cf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:09:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 04:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 04:12:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:12:09 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:12:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:15:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c70e9658293d6c6994b6a7c4cdaa6377ff6c88e8aacb0cc925a437b7f64d`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b560e1d79dbdd0e1849bd0bf9e744605e7fac17d52d9eae6a2eb85191f795c`  
		Last Modified: Fri, 07 Jan 2022 04:34:46 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19690a1594bd61dff284097ca83119bb45eb8440545c32da4c0922132b07a310`  
		Last Modified: Fri, 07 Jan 2022 04:35:27 GMT  
		Size: 176.9 MB (176882711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1f25217df1dd04bb397f3964b212a7132b0589c74df28014755ac8a8242d39`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ffdfe95d3dd2037023009ce14081cded135d4297f961ccfeefd666265cc7a`  
		Last Modified: Fri, 07 Jan 2022 04:35:51 GMT  
		Size: 47.3 MB (47259832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a460a4cc48907ba7a3f48875ff90081588a2252332a03cd88eaa72be2ae16c0`  
		Last Modified: Fri, 07 Jan 2022 04:35:43 GMT  
		Size: 305.2 KB (305157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406044e053161a2f909c8a24c374019c518eb7ecc7541ad0de4b194271415c57`  
		Last Modified: Fri, 07 Jan 2022 04:35:55 GMT  
		Size: 79.6 MB (79602648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c62d3edd88a3423f9d25b1fd55d069da77aa39216107cd15ae597095a5eec19`  
		Last Modified: Fri, 07 Jan 2022 04:36:11 GMT  
		Size: 15.7 MB (15747924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:b9786f018554e63eb35b049128513bc48960fcfbdccd2a1d2aaf77ba20f9272e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.8 MB (298795161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eba79af9952a9a631801829b405b79b7d26778ab1867a069101dbd9668dd741`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:25 GMT
ADD file:ac83e0dc7e48a0dc1805c0fd7b71b8eb119b3eeafd1fdcab93e11fbc9c0bcda0 in / 
# Fri, 07 Jan 2022 02:26:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:53:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:53:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:53:38 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:56:18 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:56:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:57:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:58:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b8080fa0945580f29aa3abed4664f8ab849229eca04510b5d259a9e29616064`  
		Last Modified: Fri, 07 Jan 2022 02:30:39 GMT  
		Size: 24.1 MB (24064434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4542f65e85cdaf2541613579d209e8ddfa8b797d8edd23c4b1b3e430580dfb8c`  
		Last Modified: Fri, 07 Jan 2022 04:13:02 GMT  
		Size: 1.2 MB (1183516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc20ad2d3acd4173d1357bb75d2d434c2cf628930746de1b638775ce5b3f169`  
		Last Modified: Fri, 07 Jan 2022 04:13:01 GMT  
		Size: 4.7 MB (4676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038a958a9812e6ad8943ca985ee5fc0fa712bd2bb652825668f1e805642250bb`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14895cbe261aa62a0bacb72a62e26758d9c4917efcc5e712fc9f8a815cc2b2df`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05603c4fd7f49169b1f830d906412ac1eb62f339ab3b8518b04e0d0df814b72`  
		Last Modified: Fri, 07 Jan 2022 04:15:07 GMT  
		Size: 157.4 MB (157422125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4937926a5187427a5b557119d517c0cb7b07dd1ec423d7aa471bbf95e1fcfe8`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c707c45473b692c29e259d0c26776db6360563b1a2d369a2e46e30f9e6f053`  
		Last Modified: Fri, 07 Jan 2022 04:15:41 GMT  
		Size: 36.7 MB (36693115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4d7df5c0cc0093b02360bb46f1cf1e7f633acd03cf4ce2cc15d489a0039acb`  
		Last Modified: Fri, 07 Jan 2022 04:15:22 GMT  
		Size: 305.2 KB (305155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9129d7514384ec5dc914d6cc465ffc40283fc596a024219bbd74ecb6ecf66c50`  
		Last Modified: Fri, 07 Jan 2022 04:16:01 GMT  
		Size: 60.5 MB (60482237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc05c61280ccbee68d9725b732b7601a0fc03e0f2edd5d5176e4e66579cec80`  
		Last Modified: Fri, 07 Jan 2022 04:16:27 GMT  
		Size: 14.0 MB (13965294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a90081f9ec434c8185ea5c679fab8b30c463b151fece201252a7da9d273fd1af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.7 MB (333719916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8403c60ca7b25d291234e6a029a14cb558858be7fcdb0b4a0e01171a4f7fcaf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:16:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:16:02 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:16:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:16:04 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:17:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:17:08 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:17:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:18:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3843c054baee6fdbb1122ab1ef12464d44642d23fcccbdf9dcb77a02e41bfc7a`  
		Last Modified: Fri, 07 Jan 2022 03:35:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f924ca980605e9e62baf57692a5657c36e9189d8794573f729f971c5ed32bb`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b0eece4cf7bea41c5acd111a551c273d6e153407fcc2744b14a155e05366b`  
		Last Modified: Fri, 07 Jan 2022 03:35:57 GMT  
		Size: 171.3 MB (171326015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a972d654bf4928ae873620e2c0012b7fb3d477f39d368d27ad70a7083fd8a2`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc978c5c6ccf265e99aa4eafe327bc1a79aca0405c567834589c5f2eb1f4a7da`  
		Last Modified: Fri, 07 Jan 2022 03:36:15 GMT  
		Size: 41.3 MB (41306233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587d30d9aed449ad7397931e249b18f034edf5cc07d2ee00610e1972a388f9a`  
		Last Modified: Fri, 07 Jan 2022 03:36:09 GMT  
		Size: 305.1 KB (305107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5814684186464d45ad335516ea3732d0f22a6b4c201319d425fd6324ba9a5e67`  
		Last Modified: Fri, 07 Jan 2022 03:36:19 GMT  
		Size: 71.8 MB (71753993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481e7053bd5452e8f9174b8d9f5d2b1e2128d338ac9cd6c5feede39785fb7a9`  
		Last Modified: Fri, 07 Jan 2022 03:36:38 GMT  
		Size: 15.3 MB (15348357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:9c5c4876665c915a2188fff45aa3787780df0fcfbb36f8b02bf99626f5be2269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:cdb6dd43fd7180cf8be3bdecb65efc01c33e3c8325a71d2be4f491ae3a1c8f9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.3 MB (339348363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b54a33fb042ad416736d85acecaebe856430501f69b01ed3fe50929694c31e4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:09:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 04:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 04:12:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:12:09 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:12:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c70e9658293d6c6994b6a7c4cdaa6377ff6c88e8aacb0cc925a437b7f64d`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b560e1d79dbdd0e1849bd0bf9e744605e7fac17d52d9eae6a2eb85191f795c`  
		Last Modified: Fri, 07 Jan 2022 04:34:46 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19690a1594bd61dff284097ca83119bb45eb8440545c32da4c0922132b07a310`  
		Last Modified: Fri, 07 Jan 2022 04:35:27 GMT  
		Size: 176.9 MB (176882711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1f25217df1dd04bb397f3964b212a7132b0589c74df28014755ac8a8242d39`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ffdfe95d3dd2037023009ce14081cded135d4297f961ccfeefd666265cc7a`  
		Last Modified: Fri, 07 Jan 2022 04:35:51 GMT  
		Size: 47.3 MB (47259832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a460a4cc48907ba7a3f48875ff90081588a2252332a03cd88eaa72be2ae16c0`  
		Last Modified: Fri, 07 Jan 2022 04:35:43 GMT  
		Size: 305.2 KB (305157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406044e053161a2f909c8a24c374019c518eb7ecc7541ad0de4b194271415c57`  
		Last Modified: Fri, 07 Jan 2022 04:35:55 GMT  
		Size: 79.6 MB (79602648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:e66897669f09dd7c3d68ea4c4fe34df26ca125964acb093d94837a7b2e1f8475
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.8 MB (284829867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24a354a8ad393a77a9d504c5970f4f9e95ae30b040be31b115e757aa416ef4fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:25 GMT
ADD file:ac83e0dc7e48a0dc1805c0fd7b71b8eb119b3eeafd1fdcab93e11fbc9c0bcda0 in / 
# Fri, 07 Jan 2022 02:26:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:53:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:53:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:53:38 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:56:18 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:56:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:57:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b8080fa0945580f29aa3abed4664f8ab849229eca04510b5d259a9e29616064`  
		Last Modified: Fri, 07 Jan 2022 02:30:39 GMT  
		Size: 24.1 MB (24064434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4542f65e85cdaf2541613579d209e8ddfa8b797d8edd23c4b1b3e430580dfb8c`  
		Last Modified: Fri, 07 Jan 2022 04:13:02 GMT  
		Size: 1.2 MB (1183516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc20ad2d3acd4173d1357bb75d2d434c2cf628930746de1b638775ce5b3f169`  
		Last Modified: Fri, 07 Jan 2022 04:13:01 GMT  
		Size: 4.7 MB (4676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038a958a9812e6ad8943ca985ee5fc0fa712bd2bb652825668f1e805642250bb`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14895cbe261aa62a0bacb72a62e26758d9c4917efcc5e712fc9f8a815cc2b2df`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05603c4fd7f49169b1f830d906412ac1eb62f339ab3b8518b04e0d0df814b72`  
		Last Modified: Fri, 07 Jan 2022 04:15:07 GMT  
		Size: 157.4 MB (157422125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4937926a5187427a5b557119d517c0cb7b07dd1ec423d7aa471bbf95e1fcfe8`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c707c45473b692c29e259d0c26776db6360563b1a2d369a2e46e30f9e6f053`  
		Last Modified: Fri, 07 Jan 2022 04:15:41 GMT  
		Size: 36.7 MB (36693115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4d7df5c0cc0093b02360bb46f1cf1e7f633acd03cf4ce2cc15d489a0039acb`  
		Last Modified: Fri, 07 Jan 2022 04:15:22 GMT  
		Size: 305.2 KB (305155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9129d7514384ec5dc914d6cc465ffc40283fc596a024219bbd74ecb6ecf66c50`  
		Last Modified: Fri, 07 Jan 2022 04:16:01 GMT  
		Size: 60.5 MB (60482237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e06329d279bf417cd354a1f84def2aaa84138eaab33b5c2e3cbc07a61c414734
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.4 MB (318371559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae709f5f9cd5d04bf4f12d3cdf79edc876767938a542b3fb39c09b88ae598037`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:16:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:16:02 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:16:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:16:04 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:17:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:17:08 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:17:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3843c054baee6fdbb1122ab1ef12464d44642d23fcccbdf9dcb77a02e41bfc7a`  
		Last Modified: Fri, 07 Jan 2022 03:35:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f924ca980605e9e62baf57692a5657c36e9189d8794573f729f971c5ed32bb`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b0eece4cf7bea41c5acd111a551c273d6e153407fcc2744b14a155e05366b`  
		Last Modified: Fri, 07 Jan 2022 03:35:57 GMT  
		Size: 171.3 MB (171326015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a972d654bf4928ae873620e2c0012b7fb3d477f39d368d27ad70a7083fd8a2`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc978c5c6ccf265e99aa4eafe327bc1a79aca0405c567834589c5f2eb1f4a7da`  
		Last Modified: Fri, 07 Jan 2022 03:36:15 GMT  
		Size: 41.3 MB (41306233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587d30d9aed449ad7397931e249b18f034edf5cc07d2ee00610e1972a388f9a`  
		Last Modified: Fri, 07 Jan 2022 03:36:09 GMT  
		Size: 305.1 KB (305107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5814684186464d45ad335516ea3732d0f22a6b4c201319d425fd6324ba9a5e67`  
		Last Modified: Fri, 07 Jan 2022 03:36:19 GMT  
		Size: 71.8 MB (71753993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:5ad7dc461716c49ba524307c74df5605df471b66356ca46996311139d625b49b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:f289e65e384ac984d82fb032f56a6f95129aade492622c6f1b0a6a0e5b184f1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.3 MB (463263278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:903008d9ac6b3bdf3a598858fe90a23c9a9b461835734c25c70f8e972a09fcae`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:56:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:56:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 21 Dec 2021 23:56:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LC_ALL=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV ROS_DISTRO=noetic
# Tue, 21 Dec 2021 23:57:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:57:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 21 Dec 2021 23:57:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 21 Dec 2021 23:57:28 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:58:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:58:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 21 Dec 2021 23:58:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a21eb75d0e3012979c6611472ad2ce77f9603178d355b33e3a29b873c09cd17`  
		Last Modified: Wed, 22 Dec 2021 00:03:48 GMT  
		Size: 10.9 MB (10891938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8a0355b4bb6623abb06a5060650fda200f613e82ff0c1660f1dd412468468d`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428381b1469052a8549b56c928ac7628c4b0b3212ab6a0e15cd9a7cb0836f7cb`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb2dc8dfc87f5650375873e92661d1220cf0d1ef485c60f8350795669a60fb`  
		Last Modified: Wed, 22 Dec 2021 00:04:21 GMT  
		Size: 239.1 MB (239089267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5280b24f54ae8eeabff880a2eab6ce4c01ea397fe51e158a984ddcc9b1812a`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384ffdd3a88cfad1dba9934a89583cde7175d36b67c35c33b81f4c51b4929654`  
		Last Modified: Wed, 22 Dec 2021 00:04:42 GMT  
		Size: 86.6 MB (86566404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e7347f2acf99a04e2a51ce3ab3a4fdf9b42d547819a739899ee16bd110ff06`  
		Last Modified: Wed, 22 Dec 2021 00:04:28 GMT  
		Size: 299.5 KB (299501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2bbb76c6ff423ad3e4b2298c17b2c64a171419f8c2c1ad315e018fcc912963`  
		Last Modified: Wed, 22 Dec 2021 00:04:40 GMT  
		Size: 76.0 MB (75976617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c93ca6155cb88a8496cea67ea2eeec68b6d4541e0fee83b1f301a84cc71a793d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.7 MB (402735896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e7479069555b7b81015b03ef73244324cb06a7307c9b7be05520d892cb2b3c4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:43:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:43:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 26 Jan 2022 07:43:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 26 Jan 2022 07:43:57 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 07:43:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 26 Jan 2022 07:43:59 GMT
ENV ROS_DISTRO=noetic
# Wed, 26 Jan 2022 07:45:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:45:12 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 26 Jan 2022 07:45:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 26 Jan 2022 07:45:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:45:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:45:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 26 Jan 2022 07:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646734dd4c9771207c4468eadc7ddcededd306975b1af9c589d4cdcda9b7c07b`  
		Last Modified: Wed, 26 Jan 2022 07:52:46 GMT  
		Size: 10.7 MB (10688073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3aad39826b43f6faf1264f98a0a52a206ef90890c6834072d8d9f87d882868d`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed8a7e03b40bfdb16508119c9ee410dd3684b3a5cf4bc31f5f6dd1597a12fee`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32e34cb56b02431259e0ed70e5f2a62c5cbae86038cc51c240276d1c687014f`  
		Last Modified: Wed, 26 Jan 2022 07:53:15 GMT  
		Size: 184.3 MB (184306695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86270cb85ef2ff4c03d623ecfac134b2c9cc1bbd6a17a0d9a16eb961841ab45`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead2d175559e1deb0533f1a26d062151a70ee020c83b271d672febcae2962201`  
		Last Modified: Wed, 26 Jan 2022 07:53:34 GMT  
		Size: 84.4 MB (84350117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ee083a5f0a1bb7f96a6fa942a09843a7a85dd23f6c421fc1030cc2233c1fb0`  
		Last Modified: Wed, 26 Jan 2022 07:53:24 GMT  
		Size: 301.2 KB (301224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f310f444237727027c0400435c277b87c69c67df7b68e96da508934404d5a1`  
		Last Modified: Wed, 26 Jan 2022 07:53:34 GMT  
		Size: 73.9 MB (73864375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:9c5c4876665c915a2188fff45aa3787780df0fcfbb36f8b02bf99626f5be2269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:cdb6dd43fd7180cf8be3bdecb65efc01c33e3c8325a71d2be4f491ae3a1c8f9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.3 MB (339348363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b54a33fb042ad416736d85acecaebe856430501f69b01ed3fe50929694c31e4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:09:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 04:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 04:12:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:12:09 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:12:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c70e9658293d6c6994b6a7c4cdaa6377ff6c88e8aacb0cc925a437b7f64d`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b560e1d79dbdd0e1849bd0bf9e744605e7fac17d52d9eae6a2eb85191f795c`  
		Last Modified: Fri, 07 Jan 2022 04:34:46 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19690a1594bd61dff284097ca83119bb45eb8440545c32da4c0922132b07a310`  
		Last Modified: Fri, 07 Jan 2022 04:35:27 GMT  
		Size: 176.9 MB (176882711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1f25217df1dd04bb397f3964b212a7132b0589c74df28014755ac8a8242d39`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ffdfe95d3dd2037023009ce14081cded135d4297f961ccfeefd666265cc7a`  
		Last Modified: Fri, 07 Jan 2022 04:35:51 GMT  
		Size: 47.3 MB (47259832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a460a4cc48907ba7a3f48875ff90081588a2252332a03cd88eaa72be2ae16c0`  
		Last Modified: Fri, 07 Jan 2022 04:35:43 GMT  
		Size: 305.2 KB (305157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406044e053161a2f909c8a24c374019c518eb7ecc7541ad0de4b194271415c57`  
		Last Modified: Fri, 07 Jan 2022 04:35:55 GMT  
		Size: 79.6 MB (79602648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:e66897669f09dd7c3d68ea4c4fe34df26ca125964acb093d94837a7b2e1f8475
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.8 MB (284829867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24a354a8ad393a77a9d504c5970f4f9e95ae30b040be31b115e757aa416ef4fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:25 GMT
ADD file:ac83e0dc7e48a0dc1805c0fd7b71b8eb119b3eeafd1fdcab93e11fbc9c0bcda0 in / 
# Fri, 07 Jan 2022 02:26:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:53:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:53:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:53:38 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:56:18 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:56:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:57:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b8080fa0945580f29aa3abed4664f8ab849229eca04510b5d259a9e29616064`  
		Last Modified: Fri, 07 Jan 2022 02:30:39 GMT  
		Size: 24.1 MB (24064434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4542f65e85cdaf2541613579d209e8ddfa8b797d8edd23c4b1b3e430580dfb8c`  
		Last Modified: Fri, 07 Jan 2022 04:13:02 GMT  
		Size: 1.2 MB (1183516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc20ad2d3acd4173d1357bb75d2d434c2cf628930746de1b638775ce5b3f169`  
		Last Modified: Fri, 07 Jan 2022 04:13:01 GMT  
		Size: 4.7 MB (4676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038a958a9812e6ad8943ca985ee5fc0fa712bd2bb652825668f1e805642250bb`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14895cbe261aa62a0bacb72a62e26758d9c4917efcc5e712fc9f8a815cc2b2df`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05603c4fd7f49169b1f830d906412ac1eb62f339ab3b8518b04e0d0df814b72`  
		Last Modified: Fri, 07 Jan 2022 04:15:07 GMT  
		Size: 157.4 MB (157422125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4937926a5187427a5b557119d517c0cb7b07dd1ec423d7aa471bbf95e1fcfe8`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c707c45473b692c29e259d0c26776db6360563b1a2d369a2e46e30f9e6f053`  
		Last Modified: Fri, 07 Jan 2022 04:15:41 GMT  
		Size: 36.7 MB (36693115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4d7df5c0cc0093b02360bb46f1cf1e7f633acd03cf4ce2cc15d489a0039acb`  
		Last Modified: Fri, 07 Jan 2022 04:15:22 GMT  
		Size: 305.2 KB (305155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9129d7514384ec5dc914d6cc465ffc40283fc596a024219bbd74ecb6ecf66c50`  
		Last Modified: Fri, 07 Jan 2022 04:16:01 GMT  
		Size: 60.5 MB (60482237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e06329d279bf417cd354a1f84def2aaa84138eaab33b5c2e3cbc07a61c414734
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.4 MB (318371559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae709f5f9cd5d04bf4f12d3cdf79edc876767938a542b3fb39c09b88ae598037`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:16:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:16:02 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:16:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:16:04 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:17:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:17:08 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:17:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3843c054baee6fdbb1122ab1ef12464d44642d23fcccbdf9dcb77a02e41bfc7a`  
		Last Modified: Fri, 07 Jan 2022 03:35:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f924ca980605e9e62baf57692a5657c36e9189d8794573f729f971c5ed32bb`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b0eece4cf7bea41c5acd111a551c273d6e153407fcc2744b14a155e05366b`  
		Last Modified: Fri, 07 Jan 2022 03:35:57 GMT  
		Size: 171.3 MB (171326015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a972d654bf4928ae873620e2c0012b7fb3d477f39d368d27ad70a7083fd8a2`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc978c5c6ccf265e99aa4eafe327bc1a79aca0405c567834589c5f2eb1f4a7da`  
		Last Modified: Fri, 07 Jan 2022 03:36:15 GMT  
		Size: 41.3 MB (41306233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587d30d9aed449ad7397931e249b18f034edf5cc07d2ee00610e1972a388f9a`  
		Last Modified: Fri, 07 Jan 2022 03:36:09 GMT  
		Size: 305.1 KB (305107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5814684186464d45ad335516ea3732d0f22a6b4c201319d425fd6324ba9a5e67`  
		Last Modified: Fri, 07 Jan 2022 03:36:19 GMT  
		Size: 71.8 MB (71753993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:e6455e8da194d713f90ee69ba8263a333ee315ff712398df56c0ba434562b38a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:629dd30ed0719de11a77103640105da48dcf537b5628659245091f33bc4dc7a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212180726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a3613b0fe30d1f279505bbc2ebae66b4ab10f2ff86d42c32b4d0993b1af5aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:09:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 04:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 04:12:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:12:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c70e9658293d6c6994b6a7c4cdaa6377ff6c88e8aacb0cc925a437b7f64d`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b560e1d79dbdd0e1849bd0bf9e744605e7fac17d52d9eae6a2eb85191f795c`  
		Last Modified: Fri, 07 Jan 2022 04:34:46 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19690a1594bd61dff284097ca83119bb45eb8440545c32da4c0922132b07a310`  
		Last Modified: Fri, 07 Jan 2022 04:35:27 GMT  
		Size: 176.9 MB (176882711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1f25217df1dd04bb397f3964b212a7132b0589c74df28014755ac8a8242d39`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:463131cee2ac3150a66ed4153e3cb51ca06c31fb26c2d74c74b07d8f73f17e34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.3 MB (187349360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa0ce674f6acd0d31658f0b4c65223ff5aef42686adb5a8e0d30780b5a71163`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:25 GMT
ADD file:ac83e0dc7e48a0dc1805c0fd7b71b8eb119b3eeafd1fdcab93e11fbc9c0bcda0 in / 
# Fri, 07 Jan 2022 02:26:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:53:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:53:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:53:38 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:56:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9b8080fa0945580f29aa3abed4664f8ab849229eca04510b5d259a9e29616064`  
		Last Modified: Fri, 07 Jan 2022 02:30:39 GMT  
		Size: 24.1 MB (24064434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4542f65e85cdaf2541613579d209e8ddfa8b797d8edd23c4b1b3e430580dfb8c`  
		Last Modified: Fri, 07 Jan 2022 04:13:02 GMT  
		Size: 1.2 MB (1183516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc20ad2d3acd4173d1357bb75d2d434c2cf628930746de1b638775ce5b3f169`  
		Last Modified: Fri, 07 Jan 2022 04:13:01 GMT  
		Size: 4.7 MB (4676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038a958a9812e6ad8943ca985ee5fc0fa712bd2bb652825668f1e805642250bb`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14895cbe261aa62a0bacb72a62e26758d9c4917efcc5e712fc9f8a815cc2b2df`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05603c4fd7f49169b1f830d906412ac1eb62f339ab3b8518b04e0d0df814b72`  
		Last Modified: Fri, 07 Jan 2022 04:15:07 GMT  
		Size: 157.4 MB (157422125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4937926a5187427a5b557119d517c0cb7b07dd1ec423d7aa471bbf95e1fcfe8`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f14979b3e99f29bf1433552bfd1a3b683b87660395033f7902fcee9aa638f885
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205006226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c09f3f2de1c4fd7d1bc2f95e4fd45246005bac5a53c7c7b7d116a909d1caba`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:16:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:16:02 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:16:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:16:04 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:17:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:17:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3843c054baee6fdbb1122ab1ef12464d44642d23fcccbdf9dcb77a02e41bfc7a`  
		Last Modified: Fri, 07 Jan 2022 03:35:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f924ca980605e9e62baf57692a5657c36e9189d8794573f729f971c5ed32bb`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b0eece4cf7bea41c5acd111a551c273d6e153407fcc2744b14a155e05366b`  
		Last Modified: Fri, 07 Jan 2022 03:35:57 GMT  
		Size: 171.3 MB (171326015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a972d654bf4928ae873620e2c0012b7fb3d477f39d368d27ad70a7083fd8a2`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:6867c07656c40c42f0208d81c148257da0bee194063bcaf3e331a0dca39acdd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:0e72063b55d6fd36382fe96279a3521dab05eba87af044036a4579cb3833d923
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300420756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:843649105be24214e63135218c4d1bb8d004608854be280bc2defe7bdffc3bff`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:56:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:56:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 21 Dec 2021 23:56:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LC_ALL=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV ROS_DISTRO=noetic
# Tue, 21 Dec 2021 23:57:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:57:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 21 Dec 2021 23:57:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 21 Dec 2021 23:57:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a21eb75d0e3012979c6611472ad2ce77f9603178d355b33e3a29b873c09cd17`  
		Last Modified: Wed, 22 Dec 2021 00:03:48 GMT  
		Size: 10.9 MB (10891938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8a0355b4bb6623abb06a5060650fda200f613e82ff0c1660f1dd412468468d`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428381b1469052a8549b56c928ac7628c4b0b3212ab6a0e15cd9a7cb0836f7cb`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb2dc8dfc87f5650375873e92661d1220cf0d1ef485c60f8350795669a60fb`  
		Last Modified: Wed, 22 Dec 2021 00:04:21 GMT  
		Size: 239.1 MB (239089267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5280b24f54ae8eeabff880a2eab6ce4c01ea397fe51e158a984ddcc9b1812a`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2d075a0e610755518d794e4ff53116825d0b300e5d4a0ab579f9558caa7e0627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244220180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b860d538b83d7e7e97f1e6ff32625c75474097c781fb5b6c9120a371393f4a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:43:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:43:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 26 Jan 2022 07:43:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 26 Jan 2022 07:43:57 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 07:43:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 26 Jan 2022 07:43:59 GMT
ENV ROS_DISTRO=noetic
# Wed, 26 Jan 2022 07:45:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:45:12 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 26 Jan 2022 07:45:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 26 Jan 2022 07:45:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646734dd4c9771207c4468eadc7ddcededd306975b1af9c589d4cdcda9b7c07b`  
		Last Modified: Wed, 26 Jan 2022 07:52:46 GMT  
		Size: 10.7 MB (10688073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3aad39826b43f6faf1264f98a0a52a206ef90890c6834072d8d9f87d882868d`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed8a7e03b40bfdb16508119c9ee410dd3684b3a5cf4bc31f5f6dd1597a12fee`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32e34cb56b02431259e0ed70e5f2a62c5cbae86038cc51c240276d1c687014f`  
		Last Modified: Wed, 26 Jan 2022 07:53:15 GMT  
		Size: 184.3 MB (184306695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86270cb85ef2ff4c03d623ecfac134b2c9cc1bbd6a17a0d9a16eb961841ab45`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:e6455e8da194d713f90ee69ba8263a333ee315ff712398df56c0ba434562b38a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:629dd30ed0719de11a77103640105da48dcf537b5628659245091f33bc4dc7a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212180726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a3613b0fe30d1f279505bbc2ebae66b4ab10f2ff86d42c32b4d0993b1af5aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:09:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 04:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 04:12:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:12:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c70e9658293d6c6994b6a7c4cdaa6377ff6c88e8aacb0cc925a437b7f64d`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b560e1d79dbdd0e1849bd0bf9e744605e7fac17d52d9eae6a2eb85191f795c`  
		Last Modified: Fri, 07 Jan 2022 04:34:46 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19690a1594bd61dff284097ca83119bb45eb8440545c32da4c0922132b07a310`  
		Last Modified: Fri, 07 Jan 2022 04:35:27 GMT  
		Size: 176.9 MB (176882711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1f25217df1dd04bb397f3964b212a7132b0589c74df28014755ac8a8242d39`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:463131cee2ac3150a66ed4153e3cb51ca06c31fb26c2d74c74b07d8f73f17e34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.3 MB (187349360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa0ce674f6acd0d31658f0b4c65223ff5aef42686adb5a8e0d30780b5a71163`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:25 GMT
ADD file:ac83e0dc7e48a0dc1805c0fd7b71b8eb119b3eeafd1fdcab93e11fbc9c0bcda0 in / 
# Fri, 07 Jan 2022 02:26:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:53:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:53:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:53:38 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:56:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9b8080fa0945580f29aa3abed4664f8ab849229eca04510b5d259a9e29616064`  
		Last Modified: Fri, 07 Jan 2022 02:30:39 GMT  
		Size: 24.1 MB (24064434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4542f65e85cdaf2541613579d209e8ddfa8b797d8edd23c4b1b3e430580dfb8c`  
		Last Modified: Fri, 07 Jan 2022 04:13:02 GMT  
		Size: 1.2 MB (1183516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc20ad2d3acd4173d1357bb75d2d434c2cf628930746de1b638775ce5b3f169`  
		Last Modified: Fri, 07 Jan 2022 04:13:01 GMT  
		Size: 4.7 MB (4676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038a958a9812e6ad8943ca985ee5fc0fa712bd2bb652825668f1e805642250bb`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14895cbe261aa62a0bacb72a62e26758d9c4917efcc5e712fc9f8a815cc2b2df`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05603c4fd7f49169b1f830d906412ac1eb62f339ab3b8518b04e0d0df814b72`  
		Last Modified: Fri, 07 Jan 2022 04:15:07 GMT  
		Size: 157.4 MB (157422125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4937926a5187427a5b557119d517c0cb7b07dd1ec423d7aa471bbf95e1fcfe8`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f14979b3e99f29bf1433552bfd1a3b683b87660395033f7902fcee9aa638f885
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205006226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c09f3f2de1c4fd7d1bc2f95e4fd45246005bac5a53c7c7b7d116a909d1caba`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:16:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:16:02 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:16:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:16:04 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:17:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:17:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3843c054baee6fdbb1122ab1ef12464d44642d23fcccbdf9dcb77a02e41bfc7a`  
		Last Modified: Fri, 07 Jan 2022 03:35:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f924ca980605e9e62baf57692a5657c36e9189d8794573f729f971c5ed32bb`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b0eece4cf7bea41c5acd111a551c273d6e153407fcc2744b14a155e05366b`  
		Last Modified: Fri, 07 Jan 2022 03:35:57 GMT  
		Size: 171.3 MB (171326015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a972d654bf4928ae873620e2c0012b7fb3d477f39d368d27ad70a7083fd8a2`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:3135eeb8454570c78472702dde8d4323245870160d013d2ff865201c29ca57e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:89b005299b79f90191e5e05b9749075c43a0d8de33ef3dd19399729e5bf6a6af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233185857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:770989ecc5d33a69d068d6ebe689478b105fea329648b33abc4fc85993657f2b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:28:39 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 04:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:29:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:29:23 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:29:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:30:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a16336f1ed977ade36c23a1558b9a63ce42588d7ec9f6421a6204b11721d61`  
		Last Modified: Fri, 07 Jan 2022 04:40:44 GMT  
		Size: 104.3 MB (104309484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8808400f29e297aedb3c763cf8095eac61233ac3447a40c594d7b609d5e39737`  
		Last Modified: Fri, 07 Jan 2022 04:40:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975a65f4140cd95ee881ea97ea69c6a4281b69ecedb9e71cfc8facffcd4fced`  
		Last Modified: Fri, 07 Jan 2022 04:41:04 GMT  
		Size: 70.8 MB (70809014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4aa7e9a462136248a1bab745e0ef3700e8455754a798add890def6b37a005b`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 250.8 KB (250795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d26a9439e09a0948d815314f26bf67505a8c65acc36c1488d8811573545c1f7`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 2.1 KB (2077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df1f316243ac1be85ac6dfa37b569d24ecef99f9ea08145931fc5a90b217258`  
		Last Modified: Fri, 07 Jan 2022 04:40:57 GMT  
		Size: 22.5 MB (22516472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:31048e3e6eca6b8a0de444148409fdf6862910a64e1d06aa83fae0858ca0e77d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221400509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a9c8565c265d25d911f5e30b8210deed74afe9cd8c73ee6fc1cb21a2076e4a2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:28:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 03:29:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:29:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:29:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:29:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:30:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe9c88c8c6bc1b55f02a9a0056d819accb8c03fe0b7e232ef7fd19b4dcb608`  
		Last Modified: Fri, 07 Jan 2022 03:41:17 GMT  
		Size: 100.7 MB (100701530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d5b527a61b8422fad766a9a8046afd6d70ee8cf7791b05ddd5a53375746cc8`  
		Last Modified: Fri, 07 Jan 2022 03:40:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30c74104597caa34b1cf8dbae71571ea6b16babbfd42dc0307090ca2fc8bcb6`  
		Last Modified: Fri, 07 Jan 2022 03:41:37 GMT  
		Size: 64.9 MB (64932455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba76342cba00f5b67fb766da3e232f9c1315ec60d929e502e588ffc1c13a0db`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 250.7 KB (250740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953fe848460e818385e527aacdaedad1d93510afdd9191a5ae514aa49666452a`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83f842b26fd064cb8a18f71dd7718b127b2c05f1c484e87d46e363d70879d09`  
		Last Modified: Fri, 07 Jan 2022 03:41:31 GMT  
		Size: 21.8 MB (21833517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:3135eeb8454570c78472702dde8d4323245870160d013d2ff865201c29ca57e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:89b005299b79f90191e5e05b9749075c43a0d8de33ef3dd19399729e5bf6a6af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233185857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:770989ecc5d33a69d068d6ebe689478b105fea329648b33abc4fc85993657f2b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:28:39 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 04:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:29:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:29:23 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:29:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:30:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a16336f1ed977ade36c23a1558b9a63ce42588d7ec9f6421a6204b11721d61`  
		Last Modified: Fri, 07 Jan 2022 04:40:44 GMT  
		Size: 104.3 MB (104309484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8808400f29e297aedb3c763cf8095eac61233ac3447a40c594d7b609d5e39737`  
		Last Modified: Fri, 07 Jan 2022 04:40:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975a65f4140cd95ee881ea97ea69c6a4281b69ecedb9e71cfc8facffcd4fced`  
		Last Modified: Fri, 07 Jan 2022 04:41:04 GMT  
		Size: 70.8 MB (70809014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4aa7e9a462136248a1bab745e0ef3700e8455754a798add890def6b37a005b`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 250.8 KB (250795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d26a9439e09a0948d815314f26bf67505a8c65acc36c1488d8811573545c1f7`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 2.1 KB (2077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df1f316243ac1be85ac6dfa37b569d24ecef99f9ea08145931fc5a90b217258`  
		Last Modified: Fri, 07 Jan 2022 04:40:57 GMT  
		Size: 22.5 MB (22516472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:31048e3e6eca6b8a0de444148409fdf6862910a64e1d06aa83fae0858ca0e77d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221400509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a9c8565c265d25d911f5e30b8210deed74afe9cd8c73ee6fc1cb21a2076e4a2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:28:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 03:29:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:29:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:29:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:29:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:30:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe9c88c8c6bc1b55f02a9a0056d819accb8c03fe0b7e232ef7fd19b4dcb608`  
		Last Modified: Fri, 07 Jan 2022 03:41:17 GMT  
		Size: 100.7 MB (100701530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d5b527a61b8422fad766a9a8046afd6d70ee8cf7791b05ddd5a53375746cc8`  
		Last Modified: Fri, 07 Jan 2022 03:40:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30c74104597caa34b1cf8dbae71571ea6b16babbfd42dc0307090ca2fc8bcb6`  
		Last Modified: Fri, 07 Jan 2022 03:41:37 GMT  
		Size: 64.9 MB (64932455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba76342cba00f5b67fb766da3e232f9c1315ec60d929e502e588ffc1c13a0db`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 250.7 KB (250740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953fe848460e818385e527aacdaedad1d93510afdd9191a5ae514aa49666452a`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83f842b26fd064cb8a18f71dd7718b127b2c05f1c484e87d46e363d70879d09`  
		Last Modified: Fri, 07 Jan 2022 03:41:31 GMT  
		Size: 21.8 MB (21833517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-focal`

```console
$ docker pull ros@sha256:3135eeb8454570c78472702dde8d4323245870160d013d2ff865201c29ca57e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:89b005299b79f90191e5e05b9749075c43a0d8de33ef3dd19399729e5bf6a6af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233185857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:770989ecc5d33a69d068d6ebe689478b105fea329648b33abc4fc85993657f2b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:28:39 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 04:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:29:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:29:23 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:29:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:30:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a16336f1ed977ade36c23a1558b9a63ce42588d7ec9f6421a6204b11721d61`  
		Last Modified: Fri, 07 Jan 2022 04:40:44 GMT  
		Size: 104.3 MB (104309484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8808400f29e297aedb3c763cf8095eac61233ac3447a40c594d7b609d5e39737`  
		Last Modified: Fri, 07 Jan 2022 04:40:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975a65f4140cd95ee881ea97ea69c6a4281b69ecedb9e71cfc8facffcd4fced`  
		Last Modified: Fri, 07 Jan 2022 04:41:04 GMT  
		Size: 70.8 MB (70809014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4aa7e9a462136248a1bab745e0ef3700e8455754a798add890def6b37a005b`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 250.8 KB (250795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d26a9439e09a0948d815314f26bf67505a8c65acc36c1488d8811573545c1f7`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 2.1 KB (2077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df1f316243ac1be85ac6dfa37b569d24ecef99f9ea08145931fc5a90b217258`  
		Last Modified: Fri, 07 Jan 2022 04:40:57 GMT  
		Size: 22.5 MB (22516472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:31048e3e6eca6b8a0de444148409fdf6862910a64e1d06aa83fae0858ca0e77d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221400509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a9c8565c265d25d911f5e30b8210deed74afe9cd8c73ee6fc1cb21a2076e4a2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:28:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 03:29:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:29:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:29:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:29:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:30:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe9c88c8c6bc1b55f02a9a0056d819accb8c03fe0b7e232ef7fd19b4dcb608`  
		Last Modified: Fri, 07 Jan 2022 03:41:17 GMT  
		Size: 100.7 MB (100701530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d5b527a61b8422fad766a9a8046afd6d70ee8cf7791b05ddd5a53375746cc8`  
		Last Modified: Fri, 07 Jan 2022 03:40:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30c74104597caa34b1cf8dbae71571ea6b16babbfd42dc0307090ca2fc8bcb6`  
		Last Modified: Fri, 07 Jan 2022 03:41:37 GMT  
		Size: 64.9 MB (64932455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba76342cba00f5b67fb766da3e232f9c1315ec60d929e502e588ffc1c13a0db`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 250.7 KB (250740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953fe848460e818385e527aacdaedad1d93510afdd9191a5ae514aa49666452a`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83f842b26fd064cb8a18f71dd7718b127b2c05f1c484e87d46e363d70879d09`  
		Last Modified: Fri, 07 Jan 2022 03:41:31 GMT  
		Size: 21.8 MB (21833517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:f53adada991ef778932e2e8a64f121bfde7adfa8fae3c061242d4f215f07c550
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:4170c331c8d4dfe00e10bdd564761f077242a150b2db7ff1f19269bc3b1f226e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139607499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc29bc7d7a3be036caab99a9e97437881208ea1a4f0ded9d17aef3b434d8a075`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:28:39 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 04:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:29:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:29:23 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a16336f1ed977ade36c23a1558b9a63ce42588d7ec9f6421a6204b11721d61`  
		Last Modified: Fri, 07 Jan 2022 04:40:44 GMT  
		Size: 104.3 MB (104309484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8808400f29e297aedb3c763cf8095eac61233ac3447a40c594d7b609d5e39737`  
		Last Modified: Fri, 07 Jan 2022 04:40:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:efa75c4f20c2c673a75f8a5f8b8aa9d25937af7745e36f8e5f2b2f8937b6acb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134381742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6a14080b93b443cce9f307c79d815e95c32475a4fcefeffab39dcf338730fee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:28:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 03:29:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:29:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:29:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe9c88c8c6bc1b55f02a9a0056d819accb8c03fe0b7e232ef7fd19b4dcb608`  
		Last Modified: Fri, 07 Jan 2022 03:41:17 GMT  
		Size: 100.7 MB (100701530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d5b527a61b8422fad766a9a8046afd6d70ee8cf7791b05ddd5a53375746cc8`  
		Last Modified: Fri, 07 Jan 2022 03:40:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-focal`

```console
$ docker pull ros@sha256:f53adada991ef778932e2e8a64f121bfde7adfa8fae3c061242d4f215f07c550
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:4170c331c8d4dfe00e10bdd564761f077242a150b2db7ff1f19269bc3b1f226e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139607499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc29bc7d7a3be036caab99a9e97437881208ea1a4f0ded9d17aef3b434d8a075`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:28:39 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 04:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:29:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:29:23 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a16336f1ed977ade36c23a1558b9a63ce42588d7ec9f6421a6204b11721d61`  
		Last Modified: Fri, 07 Jan 2022 04:40:44 GMT  
		Size: 104.3 MB (104309484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8808400f29e297aedb3c763cf8095eac61233ac3447a40c594d7b609d5e39737`  
		Last Modified: Fri, 07 Jan 2022 04:40:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:efa75c4f20c2c673a75f8a5f8b8aa9d25937af7745e36f8e5f2b2f8937b6acb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134381742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6a14080b93b443cce9f307c79d815e95c32475a4fcefeffab39dcf338730fee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:28:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 03:29:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:29:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:29:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe9c88c8c6bc1b55f02a9a0056d819accb8c03fe0b7e232ef7fd19b4dcb608`  
		Last Modified: Fri, 07 Jan 2022 03:41:17 GMT  
		Size: 100.7 MB (100701530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d5b527a61b8422fad766a9a8046afd6d70ee8cf7791b05ddd5a53375746cc8`  
		Last Modified: Fri, 07 Jan 2022 03:40:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge`

```console
$ docker pull ros@sha256:0778b8b9db57165a0661d32b3d18c2d64732d8127cba022d5843cb9ed1bf38e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:e4a6c4c501f1c72e281297621d00591e282317a5ead0f2a093699fdc397531e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.4 MB (329435838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19767d8504e063807a9e78a20529447c536b3e226aaa36204046d022b9beab46`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:28:39 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 04:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:29:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:29:23 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:29:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:30:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:30:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:30:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:30:25 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 04:30:25 GMT
ENV ROS2_DISTRO=rolling
# Mon, 24 Jan 2022 19:56:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:56:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.18.0-1*     ros-rolling-demo-nodes-py=0.18.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:56:53 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a16336f1ed977ade36c23a1558b9a63ce42588d7ec9f6421a6204b11721d61`  
		Last Modified: Fri, 07 Jan 2022 04:40:44 GMT  
		Size: 104.3 MB (104309484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8808400f29e297aedb3c763cf8095eac61233ac3447a40c594d7b609d5e39737`  
		Last Modified: Fri, 07 Jan 2022 04:40:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975a65f4140cd95ee881ea97ea69c6a4281b69ecedb9e71cfc8facffcd4fced`  
		Last Modified: Fri, 07 Jan 2022 04:41:04 GMT  
		Size: 70.8 MB (70809014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4aa7e9a462136248a1bab745e0ef3700e8455754a798add890def6b37a005b`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 250.8 KB (250795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d26a9439e09a0948d815314f26bf67505a8c65acc36c1488d8811573545c1f7`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 2.1 KB (2077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df1f316243ac1be85ac6dfa37b569d24ecef99f9ea08145931fc5a90b217258`  
		Last Modified: Fri, 07 Jan 2022 04:40:57 GMT  
		Size: 22.5 MB (22516472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda97e6ba89e5697ee900949aca16772f1798a21c3efb4ec433b8358ffa49841`  
		Last Modified: Fri, 07 Jan 2022 04:41:19 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2506852a7d2749b096216e1eadd03cbdfb60e96c86df52beb9295501d72641cc`  
		Last Modified: Fri, 07 Jan 2022 04:41:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1dd8d73d459b2c9a8c6898909ed932e48aad2b3a64f6109c195e8ae3f5d6b4`  
		Last Modified: Mon, 24 Jan 2022 20:00:42 GMT  
		Size: 78.6 MB (78597529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f338de7051819ed2e278870e898216bfc5290534dc24e767faae0a10b7f85b57`  
		Last Modified: Mon, 24 Jan 2022 20:00:31 GMT  
		Size: 17.7 MB (17651827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd85f74ec819791a564ce0b97b121d82dbfb812df7c39cb54ec76cdbea1e9d35`  
		Last Modified: Mon, 24 Jan 2022 20:00:27 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7a7d8b62a27e0cab8c2afd745f6ad7feb4438eff84fb09fbc38b866c1c0a60fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.6 MB (316631765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c13dc2c55d8648752a15072b69826fced63c08e8fe4fab9d8464730d4ae5826`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:28:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 03:29:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:29:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:29:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:29:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:30:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:30:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:30:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:30:31 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 03:30:32 GMT
ENV ROS2_DISTRO=rolling
# Mon, 24 Jan 2022 19:45:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:45:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.18.0-1*     ros-rolling-demo-nodes-py=0.18.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:45:39 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe9c88c8c6bc1b55f02a9a0056d819accb8c03fe0b7e232ef7fd19b4dcb608`  
		Last Modified: Fri, 07 Jan 2022 03:41:17 GMT  
		Size: 100.7 MB (100701530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d5b527a61b8422fad766a9a8046afd6d70ee8cf7791b05ddd5a53375746cc8`  
		Last Modified: Fri, 07 Jan 2022 03:40:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30c74104597caa34b1cf8dbae71571ea6b16babbfd42dc0307090ca2fc8bcb6`  
		Last Modified: Fri, 07 Jan 2022 03:41:37 GMT  
		Size: 64.9 MB (64932455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba76342cba00f5b67fb766da3e232f9c1315ec60d929e502e588ffc1c13a0db`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 250.7 KB (250740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953fe848460e818385e527aacdaedad1d93510afdd9191a5ae514aa49666452a`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83f842b26fd064cb8a18f71dd7718b127b2c05f1c484e87d46e363d70879d09`  
		Last Modified: Fri, 07 Jan 2022 03:41:31 GMT  
		Size: 21.8 MB (21833517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6032ab55393eb2858b6d6a300bcfc7028fa5224f31798295a76cc740f40924db`  
		Last Modified: Fri, 07 Jan 2022 03:41:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d4921a80464defe3e5c2f82505e18c5cc22accac8f0c84969bd1ccd776ab6d`  
		Last Modified: Mon, 24 Jan 2022 19:48:51 GMT  
		Size: 78.3 MB (78323680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f14f53f0ec1a86d046cbea5cdf971a94bc92116e822542905d60d21a2ef58f3`  
		Last Modified: Mon, 24 Jan 2022 19:48:39 GMT  
		Size: 16.9 MB (16907107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae18178ed177519dbbb637b2b9807d6a2aa5105b50452e5c62be7be54a184c8b`  
		Last Modified: Mon, 24 Jan 2022 19:48:35 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:0778b8b9db57165a0661d32b3d18c2d64732d8127cba022d5843cb9ed1bf38e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:e4a6c4c501f1c72e281297621d00591e282317a5ead0f2a093699fdc397531e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.4 MB (329435838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19767d8504e063807a9e78a20529447c536b3e226aaa36204046d022b9beab46`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:49 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 04:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:22:58 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:28:39 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 04:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:22 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 04:29:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:29:23 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:29:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:29:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 04:30:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:30:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:30:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:30:25 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 04:30:25 GMT
ENV ROS2_DISTRO=rolling
# Mon, 24 Jan 2022 19:56:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:56:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.18.0-1*     ros-rolling-demo-nodes-py=0.18.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:56:53 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9703d7991cf24346be83227ed5301b773e0d61d93effd34a9263fd4c67504f`  
		Last Modified: Fri, 07 Jan 2022 04:37:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ee04ca82bf5b24a9b55f2bdbfb80b5ea009b8419a3e8611d2d0a551404face`  
		Last Modified: Fri, 07 Jan 2022 04:37:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a16336f1ed977ade36c23a1558b9a63ce42588d7ec9f6421a6204b11721d61`  
		Last Modified: Fri, 07 Jan 2022 04:40:44 GMT  
		Size: 104.3 MB (104309484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8808400f29e297aedb3c763cf8095eac61233ac3447a40c594d7b609d5e39737`  
		Last Modified: Fri, 07 Jan 2022 04:40:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975a65f4140cd95ee881ea97ea69c6a4281b69ecedb9e71cfc8facffcd4fced`  
		Last Modified: Fri, 07 Jan 2022 04:41:04 GMT  
		Size: 70.8 MB (70809014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4aa7e9a462136248a1bab745e0ef3700e8455754a798add890def6b37a005b`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 250.8 KB (250795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d26a9439e09a0948d815314f26bf67505a8c65acc36c1488d8811573545c1f7`  
		Last Modified: Fri, 07 Jan 2022 04:40:54 GMT  
		Size: 2.1 KB (2077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df1f316243ac1be85ac6dfa37b569d24ecef99f9ea08145931fc5a90b217258`  
		Last Modified: Fri, 07 Jan 2022 04:40:57 GMT  
		Size: 22.5 MB (22516472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda97e6ba89e5697ee900949aca16772f1798a21c3efb4ec433b8358ffa49841`  
		Last Modified: Fri, 07 Jan 2022 04:41:19 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2506852a7d2749b096216e1eadd03cbdfb60e96c86df52beb9295501d72641cc`  
		Last Modified: Fri, 07 Jan 2022 04:41:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1dd8d73d459b2c9a8c6898909ed932e48aad2b3a64f6109c195e8ae3f5d6b4`  
		Last Modified: Mon, 24 Jan 2022 20:00:42 GMT  
		Size: 78.6 MB (78597529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f338de7051819ed2e278870e898216bfc5290534dc24e767faae0a10b7f85b57`  
		Last Modified: Mon, 24 Jan 2022 20:00:31 GMT  
		Size: 17.7 MB (17651827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd85f74ec819791a564ce0b97b121d82dbfb812df7c39cb54ec76cdbea1e9d35`  
		Last Modified: Mon, 24 Jan 2022 20:00:27 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7a7d8b62a27e0cab8c2afd745f6ad7feb4438eff84fb09fbc38b866c1c0a60fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.6 MB (316631765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c13dc2c55d8648752a15072b69826fced63c08e8fe4fab9d8464730d4ae5826`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:21:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 07 Jan 2022 03:21:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:21:31 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:21:32 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:28:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 07 Jan 2022 03:29:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 07 Jan 2022 03:29:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:29:14 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:29:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:29:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 07 Jan 2022 03:30:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:30:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:30:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:30:31 GMT
ENV ROS1_DISTRO=noetic
# Fri, 07 Jan 2022 03:30:32 GMT
ENV ROS2_DISTRO=rolling
# Mon, 24 Jan 2022 19:45:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:45:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.18.0-1*     ros-rolling-demo-nodes-py=0.18.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 24 Jan 2022 19:45:39 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad9922ff69bb25ec018c299f28319acded05b5533ed0199dcde7dfdaf6f38d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f333e9ff5288dcdc1fe0dd0332bc451df49b84edb59aba98cfd562e29f254d`  
		Last Modified: Fri, 07 Jan 2022 03:38:13 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe9c88c8c6bc1b55f02a9a0056d819accb8c03fe0b7e232ef7fd19b4dcb608`  
		Last Modified: Fri, 07 Jan 2022 03:41:17 GMT  
		Size: 100.7 MB (100701530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d5b527a61b8422fad766a9a8046afd6d70ee8cf7791b05ddd5a53375746cc8`  
		Last Modified: Fri, 07 Jan 2022 03:40:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30c74104597caa34b1cf8dbae71571ea6b16babbfd42dc0307090ca2fc8bcb6`  
		Last Modified: Fri, 07 Jan 2022 03:41:37 GMT  
		Size: 64.9 MB (64932455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba76342cba00f5b67fb766da3e232f9c1315ec60d929e502e588ffc1c13a0db`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 250.7 KB (250740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953fe848460e818385e527aacdaedad1d93510afdd9191a5ae514aa49666452a`  
		Last Modified: Fri, 07 Jan 2022 03:41:28 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83f842b26fd064cb8a18f71dd7718b127b2c05f1c484e87d46e363d70879d09`  
		Last Modified: Fri, 07 Jan 2022 03:41:31 GMT  
		Size: 21.8 MB (21833517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6032ab55393eb2858b6d6a300bcfc7028fa5224f31798295a76cc740f40924db`  
		Last Modified: Fri, 07 Jan 2022 03:41:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d4921a80464defe3e5c2f82505e18c5cc22accac8f0c84969bd1ccd776ab6d`  
		Last Modified: Mon, 24 Jan 2022 19:48:51 GMT  
		Size: 78.3 MB (78323680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f14f53f0ec1a86d046cbea5cdf971a94bc92116e822542905d60d21a2ef58f3`  
		Last Modified: Mon, 24 Jan 2022 19:48:39 GMT  
		Size: 16.9 MB (16907107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae18178ed177519dbbb637b2b9807d6a2aa5105b50452e5c62be7be54a184c8b`  
		Last Modified: Mon, 24 Jan 2022 19:48:35 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
