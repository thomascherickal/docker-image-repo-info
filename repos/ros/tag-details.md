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
$ docker pull ros@sha256:fcef2c631a908d0672dba3ee673b7623d862077edbadaf38deef6e8bef0e84ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:192d069ec555bb7fa52b9b468571ff03542e49b7b75b70ce1ae38b3ab0248d0d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236639853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6956e340e28562d8ce15e57d391ac9e83e082918b0c5e3d4c1894d69be7f4fa6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 02:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:21:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:21:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:21:56 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:22:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:22:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:22:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:22:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0234a258528781c42e63827528d6c7a315cd1e2ef8b46e71d99a78a4d59dcbf`  
		Last Modified: Wed, 14 Jul 2021 02:35:59 GMT  
		Size: 120.0 MB (119975945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a5c449e69efd0e9e1b61ad7020778546ff3ff603b1a5197fb7ed9fea0fc614`  
		Last Modified: Wed, 14 Jul 2021 02:35:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3518431585e3e9557943646c1eef2077e9854ffa950319b78fd2d7fbd70ee5c2`  
		Last Modified: Wed, 14 Jul 2021 02:36:22 GMT  
		Size: 70.8 MB (70843631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc7d862b9c0b2ddcaa3389e4e27ea079df944ebe07ee31c85f0221d7fc40156`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 237.6 KB (237580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d88a8f795e64184b90f11dc03bc03cb4ffd96b9f975bb2d5aafe8bab9d002c`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3dd3d1d4cf2a91fd64ca57a400ed7e23bd83a036bab0ccc75f7eb61f62443f`  
		Last Modified: Wed, 14 Jul 2021 02:36:13 GMT  
		Size: 10.3 MB (10283054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e67ac993be54f63b4f0a99b7a220d970d4fe8d00b304ccefd9bf1be36a66e41c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212756674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1225d3458fd9765460e5d38bdeceaa63debf7aca992d789d08bad856908f3e2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:36:23 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 00:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:37:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:37:14 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:37:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936cb23bc42354dbb71d877748e552cb73f6dbf41c5e08bd865fa3c114aef35`  
		Last Modified: Wed, 14 Jul 2021 00:54:55 GMT  
		Size: 104.2 MB (104167359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36347bc4a56f51f846093441b8546ecc164f1d40d01326b7cdfac922c21d1660`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe5bdfae75c50aed283bd88d5625a1b4a326f2dad0668653a33362999ed4290`  
		Last Modified: Wed, 14 Jul 2021 00:55:25 GMT  
		Size: 65.2 MB (65182930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe6efd0ae55b568c611184eb4bda1a365d729b0b7f3c761f3ba136411113de6`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 237.6 KB (237581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8719e38b9194bbb114aae02ae4bf47e945e0884bc0ec16f781999d2e1a291b25`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd38204e6bd09c8eda1fcccc293da1cd0104bdc98d5b7c857c9ebf5502ff0f14`  
		Last Modified: Wed, 14 Jul 2021 00:55:10 GMT  
		Size: 9.3 MB (9298848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:fcef2c631a908d0672dba3ee673b7623d862077edbadaf38deef6e8bef0e84ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:192d069ec555bb7fa52b9b468571ff03542e49b7b75b70ce1ae38b3ab0248d0d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236639853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6956e340e28562d8ce15e57d391ac9e83e082918b0c5e3d4c1894d69be7f4fa6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 02:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:21:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:21:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:21:56 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:22:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:22:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:22:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:22:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0234a258528781c42e63827528d6c7a315cd1e2ef8b46e71d99a78a4d59dcbf`  
		Last Modified: Wed, 14 Jul 2021 02:35:59 GMT  
		Size: 120.0 MB (119975945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a5c449e69efd0e9e1b61ad7020778546ff3ff603b1a5197fb7ed9fea0fc614`  
		Last Modified: Wed, 14 Jul 2021 02:35:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3518431585e3e9557943646c1eef2077e9854ffa950319b78fd2d7fbd70ee5c2`  
		Last Modified: Wed, 14 Jul 2021 02:36:22 GMT  
		Size: 70.8 MB (70843631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc7d862b9c0b2ddcaa3389e4e27ea079df944ebe07ee31c85f0221d7fc40156`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 237.6 KB (237580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d88a8f795e64184b90f11dc03bc03cb4ffd96b9f975bb2d5aafe8bab9d002c`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3dd3d1d4cf2a91fd64ca57a400ed7e23bd83a036bab0ccc75f7eb61f62443f`  
		Last Modified: Wed, 14 Jul 2021 02:36:13 GMT  
		Size: 10.3 MB (10283054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e67ac993be54f63b4f0a99b7a220d970d4fe8d00b304ccefd9bf1be36a66e41c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212756674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1225d3458fd9765460e5d38bdeceaa63debf7aca992d789d08bad856908f3e2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:36:23 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 00:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:37:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:37:14 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:37:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936cb23bc42354dbb71d877748e552cb73f6dbf41c5e08bd865fa3c114aef35`  
		Last Modified: Wed, 14 Jul 2021 00:54:55 GMT  
		Size: 104.2 MB (104167359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36347bc4a56f51f846093441b8546ecc164f1d40d01326b7cdfac922c21d1660`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe5bdfae75c50aed283bd88d5625a1b4a326f2dad0668653a33362999ed4290`  
		Last Modified: Wed, 14 Jul 2021 00:55:25 GMT  
		Size: 65.2 MB (65182930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe6efd0ae55b568c611184eb4bda1a365d729b0b7f3c761f3ba136411113de6`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 237.6 KB (237581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8719e38b9194bbb114aae02ae4bf47e945e0884bc0ec16f781999d2e1a291b25`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd38204e6bd09c8eda1fcccc293da1cd0104bdc98d5b7c857c9ebf5502ff0f14`  
		Last Modified: Wed, 14 Jul 2021 00:55:10 GMT  
		Size: 9.3 MB (9298848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:fcef2c631a908d0672dba3ee673b7623d862077edbadaf38deef6e8bef0e84ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:192d069ec555bb7fa52b9b468571ff03542e49b7b75b70ce1ae38b3ab0248d0d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236639853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6956e340e28562d8ce15e57d391ac9e83e082918b0c5e3d4c1894d69be7f4fa6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 02:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:21:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:21:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:21:56 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:22:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:22:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:22:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:22:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0234a258528781c42e63827528d6c7a315cd1e2ef8b46e71d99a78a4d59dcbf`  
		Last Modified: Wed, 14 Jul 2021 02:35:59 GMT  
		Size: 120.0 MB (119975945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a5c449e69efd0e9e1b61ad7020778546ff3ff603b1a5197fb7ed9fea0fc614`  
		Last Modified: Wed, 14 Jul 2021 02:35:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3518431585e3e9557943646c1eef2077e9854ffa950319b78fd2d7fbd70ee5c2`  
		Last Modified: Wed, 14 Jul 2021 02:36:22 GMT  
		Size: 70.8 MB (70843631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc7d862b9c0b2ddcaa3389e4e27ea079df944ebe07ee31c85f0221d7fc40156`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 237.6 KB (237580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d88a8f795e64184b90f11dc03bc03cb4ffd96b9f975bb2d5aafe8bab9d002c`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3dd3d1d4cf2a91fd64ca57a400ed7e23bd83a036bab0ccc75f7eb61f62443f`  
		Last Modified: Wed, 14 Jul 2021 02:36:13 GMT  
		Size: 10.3 MB (10283054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e67ac993be54f63b4f0a99b7a220d970d4fe8d00b304ccefd9bf1be36a66e41c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212756674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1225d3458fd9765460e5d38bdeceaa63debf7aca992d789d08bad856908f3e2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:36:23 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 00:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:37:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:37:14 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:37:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936cb23bc42354dbb71d877748e552cb73f6dbf41c5e08bd865fa3c114aef35`  
		Last Modified: Wed, 14 Jul 2021 00:54:55 GMT  
		Size: 104.2 MB (104167359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36347bc4a56f51f846093441b8546ecc164f1d40d01326b7cdfac922c21d1660`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe5bdfae75c50aed283bd88d5625a1b4a326f2dad0668653a33362999ed4290`  
		Last Modified: Wed, 14 Jul 2021 00:55:25 GMT  
		Size: 65.2 MB (65182930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe6efd0ae55b568c611184eb4bda1a365d729b0b7f3c761f3ba136411113de6`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 237.6 KB (237581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8719e38b9194bbb114aae02ae4bf47e945e0884bc0ec16f781999d2e1a291b25`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd38204e6bd09c8eda1fcccc293da1cd0104bdc98d5b7c857c9ebf5502ff0f14`  
		Last Modified: Wed, 14 Jul 2021 00:55:10 GMT  
		Size: 9.3 MB (9298848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:d462c3c12d8ff4f4e46269e4baf48a799a29313c879846a8930370fb8d2eb67f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:b014589ce3e513c7939b225eeba8f009079adacf867e39b60cbbdeca6e2507a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155273537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d20d1d8f20d96774aa9db18c4da47021319b49a28fe9a2ce131e6c80845d6a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 02:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:21:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:21:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:21:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0234a258528781c42e63827528d6c7a315cd1e2ef8b46e71d99a78a4d59dcbf`  
		Last Modified: Wed, 14 Jul 2021 02:35:59 GMT  
		Size: 120.0 MB (119975945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a5c449e69efd0e9e1b61ad7020778546ff3ff603b1a5197fb7ed9fea0fc614`  
		Last Modified: Wed, 14 Jul 2021 02:35:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4a9a0c120627766bf0397059d4136039893d2b239edf4727c06402474df72316
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138035287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911278af67a82e63b6a724a16c5780249e047a5e396b02a7aeec19a4d22e297`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:36:23 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 00:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:37:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:37:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936cb23bc42354dbb71d877748e552cb73f6dbf41c5e08bd865fa3c114aef35`  
		Last Modified: Wed, 14 Jul 2021 00:54:55 GMT  
		Size: 104.2 MB (104167359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36347bc4a56f51f846093441b8546ecc164f1d40d01326b7cdfac922c21d1660`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:d462c3c12d8ff4f4e46269e4baf48a799a29313c879846a8930370fb8d2eb67f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:b014589ce3e513c7939b225eeba8f009079adacf867e39b60cbbdeca6e2507a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155273537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d20d1d8f20d96774aa9db18c4da47021319b49a28fe9a2ce131e6c80845d6a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 02:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:21:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:21:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:21:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0234a258528781c42e63827528d6c7a315cd1e2ef8b46e71d99a78a4d59dcbf`  
		Last Modified: Wed, 14 Jul 2021 02:35:59 GMT  
		Size: 120.0 MB (119975945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a5c449e69efd0e9e1b61ad7020778546ff3ff603b1a5197fb7ed9fea0fc614`  
		Last Modified: Wed, 14 Jul 2021 02:35:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4a9a0c120627766bf0397059d4136039893d2b239edf4727c06402474df72316
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138035287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911278af67a82e63b6a724a16c5780249e047a5e396b02a7aeec19a4d22e297`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:36:23 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 00:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:37:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:37:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936cb23bc42354dbb71d877748e552cb73f6dbf41c5e08bd865fa3c114aef35`  
		Last Modified: Wed, 14 Jul 2021 00:54:55 GMT  
		Size: 104.2 MB (104167359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36347bc4a56f51f846093441b8546ecc164f1d40d01326b7cdfac922c21d1660`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:ccb6732ea22333c2027ed771d46b29a08cde9d96c7cbc2fae9a382e5792a06d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:1d6b89577432ca2593141f7c0753f2ab0ae062cf9987d9f9c4e440f290b3c872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.5 MB (345498966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4028ccf5e28817b3038d03f2b422e92a55b53c019d3112cf0aee9a67a4beafa9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 02:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:21:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:21:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:21:56 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:22:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:22:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:22:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:22:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:22:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:22:58 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 02:22:59 GMT
ENV ROS2_DISTRO=foxy
# Wed, 14 Jul 2021 02:23:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:23:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:23:40 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0234a258528781c42e63827528d6c7a315cd1e2ef8b46e71d99a78a4d59dcbf`  
		Last Modified: Wed, 14 Jul 2021 02:35:59 GMT  
		Size: 120.0 MB (119975945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a5c449e69efd0e9e1b61ad7020778546ff3ff603b1a5197fb7ed9fea0fc614`  
		Last Modified: Wed, 14 Jul 2021 02:35:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3518431585e3e9557943646c1eef2077e9854ffa950319b78fd2d7fbd70ee5c2`  
		Last Modified: Wed, 14 Jul 2021 02:36:22 GMT  
		Size: 70.8 MB (70843631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc7d862b9c0b2ddcaa3389e4e27ea079df944ebe07ee31c85f0221d7fc40156`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 237.6 KB (237580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d88a8f795e64184b90f11dc03bc03cb4ffd96b9f975bb2d5aafe8bab9d002c`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3dd3d1d4cf2a91fd64ca57a400ed7e23bd83a036bab0ccc75f7eb61f62443f`  
		Last Modified: Wed, 14 Jul 2021 02:36:13 GMT  
		Size: 10.3 MB (10283054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e347f15045e3e88d4ad189addc66be81c4c63316255d777b898a13d20b4744`  
		Last Modified: Wed, 14 Jul 2021 02:36:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ac25308bd6733fea269c23e8c098517fef5f615dffd23ef7de28fcc4d9bcb8`  
		Last Modified: Wed, 14 Jul 2021 02:36:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49f0b730b7fc10217137ff01e118be98061ab6d2ad0bcd36d54a46a1af3ec0e`  
		Last Modified: Wed, 14 Jul 2021 02:37:00 GMT  
		Size: 76.1 MB (76123398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63af41c6faaa55b9f2ee8e449a74ce20f9f11f32fc1dd0394356e9fb8c2437cf`  
		Last Modified: Wed, 14 Jul 2021 02:36:47 GMT  
		Size: 32.7 MB (32735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25f21aa5ee8fbbe32d95305938c99daa615bee725625c4128c438b596bf631d`  
		Last Modified: Wed, 14 Jul 2021 02:36:39 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:eb65f9806e158f725ec1a054294296ea093dbef7325110b5e33637abc5e64a3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (314018847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86881289b194f2f9681ec937a2d8bbbee046461ff503e09842b6bd0bb51460c9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:36:23 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 00:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:37:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:37:14 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:37:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:38:14 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:38:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:38:17 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 00:38:17 GMT
ENV ROS2_DISTRO=foxy
# Wed, 14 Jul 2021 00:38:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:39:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:39:09 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936cb23bc42354dbb71d877748e552cb73f6dbf41c5e08bd865fa3c114aef35`  
		Last Modified: Wed, 14 Jul 2021 00:54:55 GMT  
		Size: 104.2 MB (104167359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36347bc4a56f51f846093441b8546ecc164f1d40d01326b7cdfac922c21d1660`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe5bdfae75c50aed283bd88d5625a1b4a326f2dad0668653a33362999ed4290`  
		Last Modified: Wed, 14 Jul 2021 00:55:25 GMT  
		Size: 65.2 MB (65182930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe6efd0ae55b568c611184eb4bda1a365d729b0b7f3c761f3ba136411113de6`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 237.6 KB (237581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8719e38b9194bbb114aae02ae4bf47e945e0884bc0ec16f781999d2e1a291b25`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd38204e6bd09c8eda1fcccc293da1cd0104bdc98d5b7c857c9ebf5502ff0f14`  
		Last Modified: Wed, 14 Jul 2021 00:55:10 GMT  
		Size: 9.3 MB (9298848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee855d2693cfa3c761f057e595d952f3ad9aa28baec4fdb6c7c6aeccebe5253`  
		Last Modified: Wed, 14 Jul 2021 00:55:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c771a7d94ba5d8af44e03039cf751b24155eae28d23719588728df573466ec3a`  
		Last Modified: Wed, 14 Jul 2021 00:55:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0225905d7fa4ba83b5c82c7276fb856b5a60056229687c75ed8f7a862dd5a5b`  
		Last Modified: Wed, 14 Jul 2021 00:56:08 GMT  
		Size: 76.2 MB (76152200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ef894e724d511fd316fd252172ad77ab6c931f19686507871ff43a2d62505a`  
		Last Modified: Wed, 14 Jul 2021 00:55:51 GMT  
		Size: 25.1 MB (25109348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7b814322b4878b354087da9e952e45c63772416117a07772baedd7d5239ff0`  
		Last Modified: Wed, 14 Jul 2021 00:55:45 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:ccb6732ea22333c2027ed771d46b29a08cde9d96c7cbc2fae9a382e5792a06d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:1d6b89577432ca2593141f7c0753f2ab0ae062cf9987d9f9c4e440f290b3c872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.5 MB (345498966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4028ccf5e28817b3038d03f2b422e92a55b53c019d3112cf0aee9a67a4beafa9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 02:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:21:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:21:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:21:56 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:22:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:22:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:22:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:22:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:22:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:22:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:22:58 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 02:22:59 GMT
ENV ROS2_DISTRO=foxy
# Wed, 14 Jul 2021 02:23:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:23:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:23:40 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0234a258528781c42e63827528d6c7a315cd1e2ef8b46e71d99a78a4d59dcbf`  
		Last Modified: Wed, 14 Jul 2021 02:35:59 GMT  
		Size: 120.0 MB (119975945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a5c449e69efd0e9e1b61ad7020778546ff3ff603b1a5197fb7ed9fea0fc614`  
		Last Modified: Wed, 14 Jul 2021 02:35:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3518431585e3e9557943646c1eef2077e9854ffa950319b78fd2d7fbd70ee5c2`  
		Last Modified: Wed, 14 Jul 2021 02:36:22 GMT  
		Size: 70.8 MB (70843631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc7d862b9c0b2ddcaa3389e4e27ea079df944ebe07ee31c85f0221d7fc40156`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 237.6 KB (237580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d88a8f795e64184b90f11dc03bc03cb4ffd96b9f975bb2d5aafe8bab9d002c`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3dd3d1d4cf2a91fd64ca57a400ed7e23bd83a036bab0ccc75f7eb61f62443f`  
		Last Modified: Wed, 14 Jul 2021 02:36:13 GMT  
		Size: 10.3 MB (10283054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e347f15045e3e88d4ad189addc66be81c4c63316255d777b898a13d20b4744`  
		Last Modified: Wed, 14 Jul 2021 02:36:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ac25308bd6733fea269c23e8c098517fef5f615dffd23ef7de28fcc4d9bcb8`  
		Last Modified: Wed, 14 Jul 2021 02:36:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49f0b730b7fc10217137ff01e118be98061ab6d2ad0bcd36d54a46a1af3ec0e`  
		Last Modified: Wed, 14 Jul 2021 02:37:00 GMT  
		Size: 76.1 MB (76123398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63af41c6faaa55b9f2ee8e449a74ce20f9f11f32fc1dd0394356e9fb8c2437cf`  
		Last Modified: Wed, 14 Jul 2021 02:36:47 GMT  
		Size: 32.7 MB (32735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25f21aa5ee8fbbe32d95305938c99daa615bee725625c4128c438b596bf631d`  
		Last Modified: Wed, 14 Jul 2021 02:36:39 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:eb65f9806e158f725ec1a054294296ea093dbef7325110b5e33637abc5e64a3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (314018847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86881289b194f2f9681ec937a2d8bbbee046461ff503e09842b6bd0bb51460c9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:36:23 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 00:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:37:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:37:14 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:37:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:38:14 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:38:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:38:17 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 00:38:17 GMT
ENV ROS2_DISTRO=foxy
# Wed, 14 Jul 2021 00:38:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:39:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:39:09 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936cb23bc42354dbb71d877748e552cb73f6dbf41c5e08bd865fa3c114aef35`  
		Last Modified: Wed, 14 Jul 2021 00:54:55 GMT  
		Size: 104.2 MB (104167359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36347bc4a56f51f846093441b8546ecc164f1d40d01326b7cdfac922c21d1660`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe5bdfae75c50aed283bd88d5625a1b4a326f2dad0668653a33362999ed4290`  
		Last Modified: Wed, 14 Jul 2021 00:55:25 GMT  
		Size: 65.2 MB (65182930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe6efd0ae55b568c611184eb4bda1a365d729b0b7f3c761f3ba136411113de6`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 237.6 KB (237581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8719e38b9194bbb114aae02ae4bf47e945e0884bc0ec16f781999d2e1a291b25`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd38204e6bd09c8eda1fcccc293da1cd0104bdc98d5b7c857c9ebf5502ff0f14`  
		Last Modified: Wed, 14 Jul 2021 00:55:10 GMT  
		Size: 9.3 MB (9298848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee855d2693cfa3c761f057e595d952f3ad9aa28baec4fdb6c7c6aeccebe5253`  
		Last Modified: Wed, 14 Jul 2021 00:55:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c771a7d94ba5d8af44e03039cf751b24155eae28d23719588728df573466ec3a`  
		Last Modified: Wed, 14 Jul 2021 00:55:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0225905d7fa4ba83b5c82c7276fb856b5a60056229687c75ed8f7a862dd5a5b`  
		Last Modified: Wed, 14 Jul 2021 00:56:08 GMT  
		Size: 76.2 MB (76152200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ef894e724d511fd316fd252172ad77ab6c931f19686507871ff43a2d62505a`  
		Last Modified: Wed, 14 Jul 2021 00:55:51 GMT  
		Size: 25.1 MB (25109348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7b814322b4878b354087da9e952e45c63772416117a07772baedd7d5239ff0`  
		Last Modified: Wed, 14 Jul 2021 00:55:45 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:d0699e4ade0748bda3c9325cc821e27670dd4714a13ebe035cfe8d79a9c87cf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:28ca84182f0ee87aca4d0f87192387544549540246bac34f56c34d2848fc6323
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232051568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a167de5fe893c22c072d577ac26b70b9b56edf708870f19f5ba6a7775875e9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:23:46 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 02:24:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:24:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:24:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:24:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:24:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:25:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:25:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:25:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1930f841acbb1a21ad4211eba32f7bab4659cd8529a3350114543d86c09d7e4d`  
		Last Modified: Wed, 14 Jul 2021 02:37:35 GMT  
		Size: 103.6 MB (103620758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855c1ac82a78d10ac251447548fddc6d48a5e2095ac346519a299915af8a828f`  
		Last Modified: Wed, 14 Jul 2021 02:37:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7965e0f107cc789a111cb3aa5eeccbd0301fed15c9b12b6ef20f7189fdcb19`  
		Last Modified: Wed, 14 Jul 2021 02:37:58 GMT  
		Size: 70.8 MB (70796695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cb6f6e6066357111dc70ca230ecf7ee7fc275ffb6d673b41ca24523aa05447`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 239.1 KB (239064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a695aa247c643fba1c6637b4e18f867bff6915c0e30aeec58fb120791bf6eeeb`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26ef9d4a7fb46254a46a0a519d9b72965918875f359d7528c7a0fc75c884477`  
		Last Modified: Wed, 14 Jul 2021 02:37:51 GMT  
		Size: 22.1 MB (22095400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:abc211eed9fdf36bd18f37531c639173ac8d34a937e7565fb52bfda545945916
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220687765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0654be371efbe96156b89adf874e1665812be939aa6d7e21c3b8cc380913ff06`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:39:17 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 00:40:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:04 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:40:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:40:05 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:40:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:40:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:41:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a358bcd5244082729aa86f97ceebc1bafc117cd6bda738048993019c725c4aa`  
		Last Modified: Wed, 14 Jul 2021 00:56:46 GMT  
		Size: 100.0 MB (100009983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc183ac09899a507fd7a493ef7df17da81f347a2e6656d73250011f04ce4ea7d`  
		Last Modified: Wed, 14 Jul 2021 00:56:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bc7b547b1afd452e0d2e6117cd8fb371f9a1c04ff419c3c949a00748326947`  
		Last Modified: Wed, 14 Jul 2021 00:57:10 GMT  
		Size: 65.1 MB (65138013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd221fea38277681133e26873bca9e0142c8f29da55e477c907eacf6ceb83db`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 239.1 KB (239067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb57708f3ffa9cb8661054de506d3c0785274f18cc66559add5c8e54cd7521d2`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 2.0 KB (2010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0aa6988dfd8634883841d16c2fa96fb2add5d6b9cce72d9fe8f66b3d5e4200`  
		Last Modified: Wed, 14 Jul 2021 00:57:02 GMT  
		Size: 21.4 MB (21430764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:d0699e4ade0748bda3c9325cc821e27670dd4714a13ebe035cfe8d79a9c87cf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:28ca84182f0ee87aca4d0f87192387544549540246bac34f56c34d2848fc6323
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232051568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a167de5fe893c22c072d577ac26b70b9b56edf708870f19f5ba6a7775875e9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:23:46 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 02:24:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:24:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:24:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:24:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:24:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:25:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:25:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:25:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1930f841acbb1a21ad4211eba32f7bab4659cd8529a3350114543d86c09d7e4d`  
		Last Modified: Wed, 14 Jul 2021 02:37:35 GMT  
		Size: 103.6 MB (103620758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855c1ac82a78d10ac251447548fddc6d48a5e2095ac346519a299915af8a828f`  
		Last Modified: Wed, 14 Jul 2021 02:37:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7965e0f107cc789a111cb3aa5eeccbd0301fed15c9b12b6ef20f7189fdcb19`  
		Last Modified: Wed, 14 Jul 2021 02:37:58 GMT  
		Size: 70.8 MB (70796695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cb6f6e6066357111dc70ca230ecf7ee7fc275ffb6d673b41ca24523aa05447`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 239.1 KB (239064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a695aa247c643fba1c6637b4e18f867bff6915c0e30aeec58fb120791bf6eeeb`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26ef9d4a7fb46254a46a0a519d9b72965918875f359d7528c7a0fc75c884477`  
		Last Modified: Wed, 14 Jul 2021 02:37:51 GMT  
		Size: 22.1 MB (22095400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:abc211eed9fdf36bd18f37531c639173ac8d34a937e7565fb52bfda545945916
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220687765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0654be371efbe96156b89adf874e1665812be939aa6d7e21c3b8cc380913ff06`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:39:17 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 00:40:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:04 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:40:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:40:05 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:40:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:40:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:41:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a358bcd5244082729aa86f97ceebc1bafc117cd6bda738048993019c725c4aa`  
		Last Modified: Wed, 14 Jul 2021 00:56:46 GMT  
		Size: 100.0 MB (100009983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc183ac09899a507fd7a493ef7df17da81f347a2e6656d73250011f04ce4ea7d`  
		Last Modified: Wed, 14 Jul 2021 00:56:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bc7b547b1afd452e0d2e6117cd8fb371f9a1c04ff419c3c949a00748326947`  
		Last Modified: Wed, 14 Jul 2021 00:57:10 GMT  
		Size: 65.1 MB (65138013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd221fea38277681133e26873bca9e0142c8f29da55e477c907eacf6ceb83db`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 239.1 KB (239067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb57708f3ffa9cb8661054de506d3c0785274f18cc66559add5c8e54cd7521d2`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 2.0 KB (2010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0aa6988dfd8634883841d16c2fa96fb2add5d6b9cce72d9fe8f66b3d5e4200`  
		Last Modified: Wed, 14 Jul 2021 00:57:02 GMT  
		Size: 21.4 MB (21430764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:d0699e4ade0748bda3c9325cc821e27670dd4714a13ebe035cfe8d79a9c87cf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:28ca84182f0ee87aca4d0f87192387544549540246bac34f56c34d2848fc6323
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232051568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a167de5fe893c22c072d577ac26b70b9b56edf708870f19f5ba6a7775875e9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:23:46 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 02:24:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:24:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:24:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:24:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:24:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:25:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:25:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:25:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1930f841acbb1a21ad4211eba32f7bab4659cd8529a3350114543d86c09d7e4d`  
		Last Modified: Wed, 14 Jul 2021 02:37:35 GMT  
		Size: 103.6 MB (103620758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855c1ac82a78d10ac251447548fddc6d48a5e2095ac346519a299915af8a828f`  
		Last Modified: Wed, 14 Jul 2021 02:37:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7965e0f107cc789a111cb3aa5eeccbd0301fed15c9b12b6ef20f7189fdcb19`  
		Last Modified: Wed, 14 Jul 2021 02:37:58 GMT  
		Size: 70.8 MB (70796695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cb6f6e6066357111dc70ca230ecf7ee7fc275ffb6d673b41ca24523aa05447`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 239.1 KB (239064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a695aa247c643fba1c6637b4e18f867bff6915c0e30aeec58fb120791bf6eeeb`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26ef9d4a7fb46254a46a0a519d9b72965918875f359d7528c7a0fc75c884477`  
		Last Modified: Wed, 14 Jul 2021 02:37:51 GMT  
		Size: 22.1 MB (22095400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:abc211eed9fdf36bd18f37531c639173ac8d34a937e7565fb52bfda545945916
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220687765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0654be371efbe96156b89adf874e1665812be939aa6d7e21c3b8cc380913ff06`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:39:17 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 00:40:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:04 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:40:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:40:05 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:40:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:40:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:41:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a358bcd5244082729aa86f97ceebc1bafc117cd6bda738048993019c725c4aa`  
		Last Modified: Wed, 14 Jul 2021 00:56:46 GMT  
		Size: 100.0 MB (100009983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc183ac09899a507fd7a493ef7df17da81f347a2e6656d73250011f04ce4ea7d`  
		Last Modified: Wed, 14 Jul 2021 00:56:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bc7b547b1afd452e0d2e6117cd8fb371f9a1c04ff419c3c949a00748326947`  
		Last Modified: Wed, 14 Jul 2021 00:57:10 GMT  
		Size: 65.1 MB (65138013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd221fea38277681133e26873bca9e0142c8f29da55e477c907eacf6ceb83db`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 239.1 KB (239067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb57708f3ffa9cb8661054de506d3c0785274f18cc66559add5c8e54cd7521d2`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 2.0 KB (2010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0aa6988dfd8634883841d16c2fa96fb2add5d6b9cce72d9fe8f66b3d5e4200`  
		Last Modified: Wed, 14 Jul 2021 00:57:02 GMT  
		Size: 21.4 MB (21430764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:06f3ec1886f3e97dd01d34a4e66a7eb2adbcda5b430008cc41b4d0035f0df3d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:0ca700ff0556ea9ef31665ebe0560ec619c94399af156731c16199124e95499a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138918351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d761fffa1723d4ac1d97c6dcb00d9b161923919f841a6a64159eb26348492d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:23:46 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 02:24:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:24:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:24:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:24:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1930f841acbb1a21ad4211eba32f7bab4659cd8529a3350114543d86c09d7e4d`  
		Last Modified: Wed, 14 Jul 2021 02:37:35 GMT  
		Size: 103.6 MB (103620758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855c1ac82a78d10ac251447548fddc6d48a5e2095ac346519a299915af8a828f`  
		Last Modified: Wed, 14 Jul 2021 02:37:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:21f870e1fd8a44f001954ccb0e8e7c6ae9f0deea556fad286cd0d7c2bb43307b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133877911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c674924ac49f284ceb1ed0f8e2764451d9cf120e41cbe990624d9ffb965ab2d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:39:17 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 00:40:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:04 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:40:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:40:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a358bcd5244082729aa86f97ceebc1bafc117cd6bda738048993019c725c4aa`  
		Last Modified: Wed, 14 Jul 2021 00:56:46 GMT  
		Size: 100.0 MB (100009983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc183ac09899a507fd7a493ef7df17da81f347a2e6656d73250011f04ce4ea7d`  
		Last Modified: Wed, 14 Jul 2021 00:56:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:06f3ec1886f3e97dd01d34a4e66a7eb2adbcda5b430008cc41b4d0035f0df3d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:0ca700ff0556ea9ef31665ebe0560ec619c94399af156731c16199124e95499a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138918351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d761fffa1723d4ac1d97c6dcb00d9b161923919f841a6a64159eb26348492d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:23:46 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 02:24:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:24:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:24:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:24:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1930f841acbb1a21ad4211eba32f7bab4659cd8529a3350114543d86c09d7e4d`  
		Last Modified: Wed, 14 Jul 2021 02:37:35 GMT  
		Size: 103.6 MB (103620758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855c1ac82a78d10ac251447548fddc6d48a5e2095ac346519a299915af8a828f`  
		Last Modified: Wed, 14 Jul 2021 02:37:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:21f870e1fd8a44f001954ccb0e8e7c6ae9f0deea556fad286cd0d7c2bb43307b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133877911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c674924ac49f284ceb1ed0f8e2764451d9cf120e41cbe990624d9ffb965ab2d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:39:17 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 00:40:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:04 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:40:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:40:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a358bcd5244082729aa86f97ceebc1bafc117cd6bda738048993019c725c4aa`  
		Last Modified: Wed, 14 Jul 2021 00:56:46 GMT  
		Size: 100.0 MB (100009983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc183ac09899a507fd7a493ef7df17da81f347a2e6656d73250011f04ce4ea7d`  
		Last Modified: Wed, 14 Jul 2021 00:56:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:3a0234080fa126ca4db17a9a1b0e3a5cbf85e1fcc44a8e1abdebac009d4778af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:5fba93fc00fcd75ec53458d3d2b68442bd8807a0509062d3e8edc0fb498050b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.8 MB (326825424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939db889d7a764b6ba9a4af65a94f0fd309bf9d7fba112373174753d07a19190`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:23:46 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 02:24:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:24:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:24:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:24:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:24:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:25:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:25:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:25:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:25:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:25:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:25:30 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 02:25:30 GMT
ENV ROS2_DISTRO=galactic
# Wed, 14 Jul 2021 02:25:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:04 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1930f841acbb1a21ad4211eba32f7bab4659cd8529a3350114543d86c09d7e4d`  
		Last Modified: Wed, 14 Jul 2021 02:37:35 GMT  
		Size: 103.6 MB (103620758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855c1ac82a78d10ac251447548fddc6d48a5e2095ac346519a299915af8a828f`  
		Last Modified: Wed, 14 Jul 2021 02:37:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7965e0f107cc789a111cb3aa5eeccbd0301fed15c9b12b6ef20f7189fdcb19`  
		Last Modified: Wed, 14 Jul 2021 02:37:58 GMT  
		Size: 70.8 MB (70796695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cb6f6e6066357111dc70ca230ecf7ee7fc275ffb6d673b41ca24523aa05447`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 239.1 KB (239064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a695aa247c643fba1c6637b4e18f867bff6915c0e30aeec58fb120791bf6eeeb`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26ef9d4a7fb46254a46a0a519d9b72965918875f359d7528c7a0fc75c884477`  
		Last Modified: Wed, 14 Jul 2021 02:37:51 GMT  
		Size: 22.1 MB (22095400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf1ad79a001e7cd5f7de9c17dd1484424d709487bf00b4beefc3c250d8ac0f7`  
		Last Modified: Wed, 14 Jul 2021 02:38:12 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2390c5c32a930568c0996b626861dee58da7cb059ac4c5a52a90dc6853ab4e5`  
		Last Modified: Wed, 14 Jul 2021 02:38:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e2df934bcf149c56e84a5a5bd5e66c21a296ac99898b13ec7033d6e7dbeb8`  
		Last Modified: Wed, 14 Jul 2021 02:38:34 GMT  
		Size: 78.4 MB (78410908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8def3824423f333ccb68e18168231f3460505a001ecc0e8223472586fe3c072`  
		Last Modified: Wed, 14 Jul 2021 02:38:16 GMT  
		Size: 16.4 MB (16362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf674ebf6056dbaeac1a5bec5a0668737b2828b2f7a03ffa4c6330b36b2813ad`  
		Last Modified: Wed, 14 Jul 2021 02:38:13 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:21dbd174709b05d963c775428d818c6859e7e0333569017dde41c553d52c9d29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.9 MB (314947249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e1d258435ff91e645e428026031524073e7298d90a9588a3f2cf5869dada9a7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:39:17 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 00:40:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:04 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:40:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:40:05 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:40:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:40:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:41:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:41:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:41:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:41:28 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 00:41:28 GMT
ENV ROS2_DISTRO=galactic
# Wed, 14 Jul 2021 00:41:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:42:09 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a358bcd5244082729aa86f97ceebc1bafc117cd6bda738048993019c725c4aa`  
		Last Modified: Wed, 14 Jul 2021 00:56:46 GMT  
		Size: 100.0 MB (100009983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc183ac09899a507fd7a493ef7df17da81f347a2e6656d73250011f04ce4ea7d`  
		Last Modified: Wed, 14 Jul 2021 00:56:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bc7b547b1afd452e0d2e6117cd8fb371f9a1c04ff419c3c949a00748326947`  
		Last Modified: Wed, 14 Jul 2021 00:57:10 GMT  
		Size: 65.1 MB (65138013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd221fea38277681133e26873bca9e0142c8f29da55e477c907eacf6ceb83db`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 239.1 KB (239067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb57708f3ffa9cb8661054de506d3c0785274f18cc66559add5c8e54cd7521d2`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 2.0 KB (2010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0aa6988dfd8634883841d16c2fa96fb2add5d6b9cce72d9fe8f66b3d5e4200`  
		Last Modified: Wed, 14 Jul 2021 00:57:02 GMT  
		Size: 21.4 MB (21430764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb317f13463f02047277be9351ec1be0004beab4e6bb9fee342f11ea8f4914`  
		Last Modified: Wed, 14 Jul 2021 00:57:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec27dc4a7abd2df6cdd4705ba4380601e0ba406454fd3a386422f8f07c97ca0`  
		Last Modified: Wed, 14 Jul 2021 00:57:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e453588761a1c6c9d89a74b2f49c7b8bab3629b5665f6cea21489228dddec0f4`  
		Last Modified: Wed, 14 Jul 2021 00:57:49 GMT  
		Size: 78.4 MB (78368862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6447c99abc27d97a49b6e75f2dcd5cfac1bce156b1d593e436a87fef8365e3c9`  
		Last Modified: Wed, 14 Jul 2021 00:57:31 GMT  
		Size: 15.9 MB (15889992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc287c18aa593411cc80a90e25dcad46077e7c0a28af363b9eec15af1ce8dd3`  
		Last Modified: Wed, 14 Jul 2021 00:57:27 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:3a0234080fa126ca4db17a9a1b0e3a5cbf85e1fcc44a8e1abdebac009d4778af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:5fba93fc00fcd75ec53458d3d2b68442bd8807a0509062d3e8edc0fb498050b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.8 MB (326825424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939db889d7a764b6ba9a4af65a94f0fd309bf9d7fba112373174753d07a19190`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:23:46 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 02:24:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:24:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:24:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:24:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:24:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:25:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:25:02 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:25:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:25:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:25:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:25:30 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 02:25:30 GMT
ENV ROS2_DISTRO=galactic
# Wed, 14 Jul 2021 02:25:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:04 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1930f841acbb1a21ad4211eba32f7bab4659cd8529a3350114543d86c09d7e4d`  
		Last Modified: Wed, 14 Jul 2021 02:37:35 GMT  
		Size: 103.6 MB (103620758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855c1ac82a78d10ac251447548fddc6d48a5e2095ac346519a299915af8a828f`  
		Last Modified: Wed, 14 Jul 2021 02:37:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7965e0f107cc789a111cb3aa5eeccbd0301fed15c9b12b6ef20f7189fdcb19`  
		Last Modified: Wed, 14 Jul 2021 02:37:58 GMT  
		Size: 70.8 MB (70796695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cb6f6e6066357111dc70ca230ecf7ee7fc275ffb6d673b41ca24523aa05447`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 239.1 KB (239064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a695aa247c643fba1c6637b4e18f867bff6915c0e30aeec58fb120791bf6eeeb`  
		Last Modified: Wed, 14 Jul 2021 02:37:46 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26ef9d4a7fb46254a46a0a519d9b72965918875f359d7528c7a0fc75c884477`  
		Last Modified: Wed, 14 Jul 2021 02:37:51 GMT  
		Size: 22.1 MB (22095400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf1ad79a001e7cd5f7de9c17dd1484424d709487bf00b4beefc3c250d8ac0f7`  
		Last Modified: Wed, 14 Jul 2021 02:38:12 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2390c5c32a930568c0996b626861dee58da7cb059ac4c5a52a90dc6853ab4e5`  
		Last Modified: Wed, 14 Jul 2021 02:38:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e2df934bcf149c56e84a5a5bd5e66c21a296ac99898b13ec7033d6e7dbeb8`  
		Last Modified: Wed, 14 Jul 2021 02:38:34 GMT  
		Size: 78.4 MB (78410908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8def3824423f333ccb68e18168231f3460505a001ecc0e8223472586fe3c072`  
		Last Modified: Wed, 14 Jul 2021 02:38:16 GMT  
		Size: 16.4 MB (16362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf674ebf6056dbaeac1a5bec5a0668737b2828b2f7a03ffa4c6330b36b2813ad`  
		Last Modified: Wed, 14 Jul 2021 02:38:13 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:21dbd174709b05d963c775428d818c6859e7e0333569017dde41c553d52c9d29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.9 MB (314947249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e1d258435ff91e645e428026031524073e7298d90a9588a3f2cf5869dada9a7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:39:17 GMT
ENV ROS_DISTRO=galactic
# Wed, 14 Jul 2021 00:40:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:04 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:40:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:40:05 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:40:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:40:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:40:49 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:41:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:41:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:41:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:41:28 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 00:41:28 GMT
ENV ROS2_DISTRO=galactic
# Wed, 14 Jul 2021 00:41:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:42:09 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a358bcd5244082729aa86f97ceebc1bafc117cd6bda738048993019c725c4aa`  
		Last Modified: Wed, 14 Jul 2021 00:56:46 GMT  
		Size: 100.0 MB (100009983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc183ac09899a507fd7a493ef7df17da81f347a2e6656d73250011f04ce4ea7d`  
		Last Modified: Wed, 14 Jul 2021 00:56:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bc7b547b1afd452e0d2e6117cd8fb371f9a1c04ff419c3c949a00748326947`  
		Last Modified: Wed, 14 Jul 2021 00:57:10 GMT  
		Size: 65.1 MB (65138013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd221fea38277681133e26873bca9e0142c8f29da55e477c907eacf6ceb83db`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 239.1 KB (239067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb57708f3ffa9cb8661054de506d3c0785274f18cc66559add5c8e54cd7521d2`  
		Last Modified: Wed, 14 Jul 2021 00:56:58 GMT  
		Size: 2.0 KB (2010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0aa6988dfd8634883841d16c2fa96fb2add5d6b9cce72d9fe8f66b3d5e4200`  
		Last Modified: Wed, 14 Jul 2021 00:57:02 GMT  
		Size: 21.4 MB (21430764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb317f13463f02047277be9351ec1be0004beab4e6bb9fee342f11ea8f4914`  
		Last Modified: Wed, 14 Jul 2021 00:57:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec27dc4a7abd2df6cdd4705ba4380601e0ba406454fd3a386422f8f07c97ca0`  
		Last Modified: Wed, 14 Jul 2021 00:57:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e453588761a1c6c9d89a74b2f49c7b8bab3629b5665f6cea21489228dddec0f4`  
		Last Modified: Wed, 14 Jul 2021 00:57:49 GMT  
		Size: 78.4 MB (78368862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6447c99abc27d97a49b6e75f2dcd5cfac1bce156b1d593e436a87fef8365e3c9`  
		Last Modified: Wed, 14 Jul 2021 00:57:31 GMT  
		Size: 15.9 MB (15889992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc287c18aa593411cc80a90e25dcad46077e7c0a28af363b9eec15af1ce8dd3`  
		Last Modified: Wed, 14 Jul 2021 00:57:27 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:fcef2c631a908d0672dba3ee673b7623d862077edbadaf38deef6e8bef0e84ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:192d069ec555bb7fa52b9b468571ff03542e49b7b75b70ce1ae38b3ab0248d0d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.6 MB (236639853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6956e340e28562d8ce15e57d391ac9e83e082918b0c5e3d4c1894d69be7f4fa6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 02:21:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:21:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:21:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:21:56 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:22:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:22:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:22:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:22:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0234a258528781c42e63827528d6c7a315cd1e2ef8b46e71d99a78a4d59dcbf`  
		Last Modified: Wed, 14 Jul 2021 02:35:59 GMT  
		Size: 120.0 MB (119975945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a5c449e69efd0e9e1b61ad7020778546ff3ff603b1a5197fb7ed9fea0fc614`  
		Last Modified: Wed, 14 Jul 2021 02:35:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3518431585e3e9557943646c1eef2077e9854ffa950319b78fd2d7fbd70ee5c2`  
		Last Modified: Wed, 14 Jul 2021 02:36:22 GMT  
		Size: 70.8 MB (70843631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc7d862b9c0b2ddcaa3389e4e27ea079df944ebe07ee31c85f0221d7fc40156`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 237.6 KB (237580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d88a8f795e64184b90f11dc03bc03cb4ffd96b9f975bb2d5aafe8bab9d002c`  
		Last Modified: Wed, 14 Jul 2021 02:36:10 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3dd3d1d4cf2a91fd64ca57a400ed7e23bd83a036bab0ccc75f7eb61f62443f`  
		Last Modified: Wed, 14 Jul 2021 02:36:13 GMT  
		Size: 10.3 MB (10283054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e67ac993be54f63b4f0a99b7a220d970d4fe8d00b304ccefd9bf1be36a66e41c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.8 MB (212756674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1225d3458fd9765460e5d38bdeceaa63debf7aca992d789d08bad856908f3e2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:36:23 GMT
ENV ROS_DISTRO=foxy
# Wed, 14 Jul 2021 00:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:13 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:37:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:37:14 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:37:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:37:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:37:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936cb23bc42354dbb71d877748e552cb73f6dbf41c5e08bd865fa3c114aef35`  
		Last Modified: Wed, 14 Jul 2021 00:54:55 GMT  
		Size: 104.2 MB (104167359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36347bc4a56f51f846093441b8546ecc164f1d40d01326b7cdfac922c21d1660`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe5bdfae75c50aed283bd88d5625a1b4a326f2dad0668653a33362999ed4290`  
		Last Modified: Wed, 14 Jul 2021 00:55:25 GMT  
		Size: 65.2 MB (65182930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe6efd0ae55b568c611184eb4bda1a365d729b0b7f3c761f3ba136411113de6`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 237.6 KB (237581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8719e38b9194bbb114aae02ae4bf47e945e0884bc0ec16f781999d2e1a291b25`  
		Last Modified: Wed, 14 Jul 2021 00:55:08 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd38204e6bd09c8eda1fcccc293da1cd0104bdc98d5b7c857c9ebf5502ff0f14`  
		Last Modified: Wed, 14 Jul 2021 00:55:10 GMT  
		Size: 9.3 MB (9298848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:5cb69d502cff623004c1e4967e8ebe632c136aea7598ec3be25fecf243e588df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:e250575746ce217c6d18bd3369ac85fdd31faa57485b8ca4cfc5b5a71873f5f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437352310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6358b4a94be18f7307dd098afa12f669f6f48f71414a6aac1624946e3e6bb0c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:53:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:53:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 01:57:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:57:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:57:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:58:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:58:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1107129de068a3615596b08dc61d39c6a7722d1f446096ae57c3f28769bfca39`  
		Last Modified: Tue, 13 Jul 2021 23:14:34 GMT  
		Size: 840.8 KB (840788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a7fbbce93b678f9a7ec24c63012d604fef4a9cad8414c5b8a467f2930e4d`  
		Last Modified: Wed, 14 Jul 2021 02:29:23 GMT  
		Size: 4.9 MB (4872342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea558154c977de1713b413508635ea067b8a9cb2caac2c2d33399aa134072c7a`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a009470670a1026f1819627c53fb14edf956e0cc56b9ead79340c9de91ed8`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8abfba080c1ed4e3b4bdc2bf0d8eee89b03d0c97b04d513b964b4b26aa96d`  
		Last Modified: Wed, 14 Jul 2021 02:30:07 GMT  
		Size: 259.4 MB (259436482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906763856d86a129884f2d128bbc8ba73658b2c439deafb32dc704ad6f8f3d3`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e724da914872a99c21d1c752fe003c146cf3fda351f11997235ba7772cdba`  
		Last Modified: Wed, 14 Jul 2021 02:30:31 GMT  
		Size: 70.2 MB (70229653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a2ee178e82d7a724d90e3a8d8e37e8f09ccb10b47b1b62479653c997cb1df0`  
		Last Modified: Wed, 14 Jul 2021 02:30:20 GMT  
		Size: 269.6 KB (269609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b958a59ce23c95988f3219849b668a9b70003fa348726a8d3f88d1f5281a4715`  
		Last Modified: Wed, 14 Jul 2021 02:30:35 GMT  
		Size: 75.0 MB (74994876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:7a8849406ecc1d8f59be615d0df0c6053628ee8b72cf7d1da54e0d14529d6404
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385874432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029b973a5417d0d37ba392315e216308319602737150f61619be6a9aecb32089`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:50:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:50:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:53:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:53:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:53:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:54:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:54:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42872bf962a1c39ef027f457cefdef3c14b61de5a2e4eb23c3cd86de2ddf9554`  
		Last Modified: Wed, 14 Jul 2021 01:11:43 GMT  
		Size: 841.4 KB (841422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86d64b6163277a8faa0275b3fcba0855d5af76a2212503e755cba50cb08d4d`  
		Last Modified: Wed, 14 Jul 2021 01:11:42 GMT  
		Size: 4.1 MB (4085737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c8f9089545ebc81b78035f6c8bcc9757f8574fc623e07301fbc6081e76d1ee`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a241e304ad2761062f5ec7258e0a2490ccfb82ee70d01cca739111e2656605a0`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6434ded48ed96eaf7f1622cc6d4a0d69212f24911da077bb3e36b45f85e1487`  
		Last Modified: Wed, 14 Jul 2021 01:14:19 GMT  
		Size: 238.9 MB (238929302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193577023dae8fd6d36536414dd47eb98a483fdcf9d56fb523ac3cd9b4b80f06`  
		Last Modified: Wed, 14 Jul 2021 01:11:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf1f931a8a0bada54ddb1868696700aed914f2205fcf2d217323a06a12897c`  
		Last Modified: Wed, 14 Jul 2021 01:15:03 GMT  
		Size: 54.7 MB (54695702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dc768f3e4222fe29a227fe190b7dff33b4c25fc8c8423d81dc83f47634fbb3`  
		Last Modified: Wed, 14 Jul 2021 01:14:33 GMT  
		Size: 269.7 KB (269680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e632e952bcaf0807284b647dec165289d61395139d9d50307f600e4ae928d0b`  
		Last Modified: Wed, 14 Jul 2021 01:15:19 GMT  
		Size: 64.7 MB (64746099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1a691b80df54ca92e8384ee974db49cf3bf6c5d91a2d4d82ede19f9a7ba67b76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411937593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aae085ede476478224c506fd8cdb4ec4f6b065badec5e43411705926c7e15ec`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:26:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:26:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:26:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:27:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:27:41 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:28:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:28:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:28:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41769627f180322e716b3023e5ef1ae59239c5ec3ba63d3feb96951d73d5878`  
		Last Modified: Wed, 14 Jul 2021 00:47:53 GMT  
		Size: 841.3 KB (841282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63f135f6f4db75ebf1ed14bf2422b3e612ec51db4bc3162a3a75a8b8df7b1b`  
		Last Modified: Wed, 14 Jul 2021 00:47:51 GMT  
		Size: 4.5 MB (4453635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3d85ee829fbd9be39df324330a8fe50c97a4b0c1247389b35c752404e77956`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c861f823f51f0edd135ae9cfa7425e5069eee2dc8641b3295ac532e11f81a`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0bc4e6e6bc21814066b9ec7467ea608909aead56aaf7d7f6972cc89eefea9f`  
		Last Modified: Wed, 14 Jul 2021 00:48:44 GMT  
		Size: 252.4 MB (252361492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767e94dd377ecd0bbcfb7093ad56d12b9939dcd7e13e05dd7670d173f21a2c5`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757b61452d8eae6c89294b87e561cbfba03e0e55970cafa498482560fb4b149c`  
		Last Modified: Wed, 14 Jul 2021 00:49:13 GMT  
		Size: 63.1 MB (63057473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ae03f3e351dc5e7ad9a7a7326828f929507da72882680dde4eb7b4b257d66a`  
		Last Modified: Wed, 14 Jul 2021 00:49:03 GMT  
		Size: 269.6 KB (269565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd788c193bc11dec6b0622c8def99e36c29b17a5c68360cc67bca0a52b5d74`  
		Last Modified: Wed, 14 Jul 2021 00:49:18 GMT  
		Size: 67.2 MB (67222233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:6d8320110a5c27e31319207fefe8bb5ace856e9aee8a785426d4afd0ab4f1928
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:be4597ce7bc9e89f114baaeb3d9bbfca25d0823264b89bba8493583ebb44b343
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742471468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0abc68b332bea9499a8f5a85bb588fbacb32a320b25ef9d866c1227a98231df9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:53:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:53:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 01:57:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:57:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:57:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:58:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:58:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:05:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1107129de068a3615596b08dc61d39c6a7722d1f446096ae57c3f28769bfca39`  
		Last Modified: Tue, 13 Jul 2021 23:14:34 GMT  
		Size: 840.8 KB (840788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a7fbbce93b678f9a7ec24c63012d604fef4a9cad8414c5b8a467f2930e4d`  
		Last Modified: Wed, 14 Jul 2021 02:29:23 GMT  
		Size: 4.9 MB (4872342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea558154c977de1713b413508635ea067b8a9cb2caac2c2d33399aa134072c7a`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a009470670a1026f1819627c53fb14edf956e0cc56b9ead79340c9de91ed8`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8abfba080c1ed4e3b4bdc2bf0d8eee89b03d0c97b04d513b964b4b26aa96d`  
		Last Modified: Wed, 14 Jul 2021 02:30:07 GMT  
		Size: 259.4 MB (259436482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906763856d86a129884f2d128bbc8ba73658b2c439deafb32dc704ad6f8f3d3`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e724da914872a99c21d1c752fe003c146cf3fda351f11997235ba7772cdba`  
		Last Modified: Wed, 14 Jul 2021 02:30:31 GMT  
		Size: 70.2 MB (70229653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a2ee178e82d7a724d90e3a8d8e37e8f09ccb10b47b1b62479653c997cb1df0`  
		Last Modified: Wed, 14 Jul 2021 02:30:20 GMT  
		Size: 269.6 KB (269609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b958a59ce23c95988f3219849b668a9b70003fa348726a8d3f88d1f5281a4715`  
		Last Modified: Wed, 14 Jul 2021 02:30:35 GMT  
		Size: 75.0 MB (74994876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f8ea3cc6e40968b9269ae85659b70394812d64bc9bf7e41a2e48e7bd47924e`  
		Last Modified: Wed, 14 Jul 2021 02:31:58 GMT  
		Size: 305.1 MB (305119158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:531c5b1f694fe9241b487531af0ad04d0630e2a086eaeb6901a88b84e8b2d24c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.8 MB (645753605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb39a9052fc864479baf00515e9f9873ba014f65779d4143cb70654f3f3a713`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:50:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:50:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:53:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:53:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:53:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:54:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:54:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42872bf962a1c39ef027f457cefdef3c14b61de5a2e4eb23c3cd86de2ddf9554`  
		Last Modified: Wed, 14 Jul 2021 01:11:43 GMT  
		Size: 841.4 KB (841422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86d64b6163277a8faa0275b3fcba0855d5af76a2212503e755cba50cb08d4d`  
		Last Modified: Wed, 14 Jul 2021 01:11:42 GMT  
		Size: 4.1 MB (4085737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c8f9089545ebc81b78035f6c8bcc9757f8574fc623e07301fbc6081e76d1ee`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a241e304ad2761062f5ec7258e0a2490ccfb82ee70d01cca739111e2656605a0`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6434ded48ed96eaf7f1622cc6d4a0d69212f24911da077bb3e36b45f85e1487`  
		Last Modified: Wed, 14 Jul 2021 01:14:19 GMT  
		Size: 238.9 MB (238929302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193577023dae8fd6d36536414dd47eb98a483fdcf9d56fb523ac3cd9b4b80f06`  
		Last Modified: Wed, 14 Jul 2021 01:11:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf1f931a8a0bada54ddb1868696700aed914f2205fcf2d217323a06a12897c`  
		Last Modified: Wed, 14 Jul 2021 01:15:03 GMT  
		Size: 54.7 MB (54695702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dc768f3e4222fe29a227fe190b7dff33b4c25fc8c8423d81dc83f47634fbb3`  
		Last Modified: Wed, 14 Jul 2021 01:14:33 GMT  
		Size: 269.7 KB (269680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e632e952bcaf0807284b647dec165289d61395139d9d50307f600e4ae928d0b`  
		Last Modified: Wed, 14 Jul 2021 01:15:19 GMT  
		Size: 64.7 MB (64746099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4700cd0e55ec4689d10f8da0b292b3b58a8f52b07d10b0ff28072467263a9c39`  
		Last Modified: Wed, 14 Jul 2021 01:18:51 GMT  
		Size: 259.9 MB (259879173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1f13e80d9989dcd03291647cdb26e47ff27b4ce78de2c9e769e79aa931e09f1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.4 MB (703396106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfa94140117f7480b84b81a59d881a5f20db96862994c4d184cada469db967e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:26:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:26:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:26:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:27:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:27:41 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:28:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:28:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:28:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:30:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41769627f180322e716b3023e5ef1ae59239c5ec3ba63d3feb96951d73d5878`  
		Last Modified: Wed, 14 Jul 2021 00:47:53 GMT  
		Size: 841.3 KB (841282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63f135f6f4db75ebf1ed14bf2422b3e612ec51db4bc3162a3a75a8b8df7b1b`  
		Last Modified: Wed, 14 Jul 2021 00:47:51 GMT  
		Size: 4.5 MB (4453635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3d85ee829fbd9be39df324330a8fe50c97a4b0c1247389b35c752404e77956`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c861f823f51f0edd135ae9cfa7425e5069eee2dc8641b3295ac532e11f81a`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0bc4e6e6bc21814066b9ec7467ea608909aead56aaf7d7f6972cc89eefea9f`  
		Last Modified: Wed, 14 Jul 2021 00:48:44 GMT  
		Size: 252.4 MB (252361492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767e94dd377ecd0bbcfb7093ad56d12b9939dcd7e13e05dd7670d173f21a2c5`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757b61452d8eae6c89294b87e561cbfba03e0e55970cafa498482560fb4b149c`  
		Last Modified: Wed, 14 Jul 2021 00:49:13 GMT  
		Size: 63.1 MB (63057473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ae03f3e351dc5e7ad9a7a7326828f929507da72882680dde4eb7b4b257d66a`  
		Last Modified: Wed, 14 Jul 2021 00:49:03 GMT  
		Size: 269.6 KB (269565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd788c193bc11dec6b0622c8def99e36c29b17a5c68360cc67bca0a52b5d74`  
		Last Modified: Wed, 14 Jul 2021 00:49:18 GMT  
		Size: 67.2 MB (67222233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f59ad25c5a9eed6d97c13dd07cd9ffd646f2f4f0963c6ba693f84b64db0a06`  
		Last Modified: Wed, 14 Jul 2021 00:50:50 GMT  
		Size: 291.5 MB (291458513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:6d8320110a5c27e31319207fefe8bb5ace856e9aee8a785426d4afd0ab4f1928
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:be4597ce7bc9e89f114baaeb3d9bbfca25d0823264b89bba8493583ebb44b343
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742471468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0abc68b332bea9499a8f5a85bb588fbacb32a320b25ef9d866c1227a98231df9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:53:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:53:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 01:57:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:57:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:57:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:58:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:58:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:05:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1107129de068a3615596b08dc61d39c6a7722d1f446096ae57c3f28769bfca39`  
		Last Modified: Tue, 13 Jul 2021 23:14:34 GMT  
		Size: 840.8 KB (840788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a7fbbce93b678f9a7ec24c63012d604fef4a9cad8414c5b8a467f2930e4d`  
		Last Modified: Wed, 14 Jul 2021 02:29:23 GMT  
		Size: 4.9 MB (4872342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea558154c977de1713b413508635ea067b8a9cb2caac2c2d33399aa134072c7a`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a009470670a1026f1819627c53fb14edf956e0cc56b9ead79340c9de91ed8`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8abfba080c1ed4e3b4bdc2bf0d8eee89b03d0c97b04d513b964b4b26aa96d`  
		Last Modified: Wed, 14 Jul 2021 02:30:07 GMT  
		Size: 259.4 MB (259436482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906763856d86a129884f2d128bbc8ba73658b2c439deafb32dc704ad6f8f3d3`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e724da914872a99c21d1c752fe003c146cf3fda351f11997235ba7772cdba`  
		Last Modified: Wed, 14 Jul 2021 02:30:31 GMT  
		Size: 70.2 MB (70229653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a2ee178e82d7a724d90e3a8d8e37e8f09ccb10b47b1b62479653c997cb1df0`  
		Last Modified: Wed, 14 Jul 2021 02:30:20 GMT  
		Size: 269.6 KB (269609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b958a59ce23c95988f3219849b668a9b70003fa348726a8d3f88d1f5281a4715`  
		Last Modified: Wed, 14 Jul 2021 02:30:35 GMT  
		Size: 75.0 MB (74994876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f8ea3cc6e40968b9269ae85659b70394812d64bc9bf7e41a2e48e7bd47924e`  
		Last Modified: Wed, 14 Jul 2021 02:31:58 GMT  
		Size: 305.1 MB (305119158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:531c5b1f694fe9241b487531af0ad04d0630e2a086eaeb6901a88b84e8b2d24c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.8 MB (645753605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb39a9052fc864479baf00515e9f9873ba014f65779d4143cb70654f3f3a713`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:50:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:50:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:53:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:53:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:53:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:54:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:54:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42872bf962a1c39ef027f457cefdef3c14b61de5a2e4eb23c3cd86de2ddf9554`  
		Last Modified: Wed, 14 Jul 2021 01:11:43 GMT  
		Size: 841.4 KB (841422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86d64b6163277a8faa0275b3fcba0855d5af76a2212503e755cba50cb08d4d`  
		Last Modified: Wed, 14 Jul 2021 01:11:42 GMT  
		Size: 4.1 MB (4085737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c8f9089545ebc81b78035f6c8bcc9757f8574fc623e07301fbc6081e76d1ee`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a241e304ad2761062f5ec7258e0a2490ccfb82ee70d01cca739111e2656605a0`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6434ded48ed96eaf7f1622cc6d4a0d69212f24911da077bb3e36b45f85e1487`  
		Last Modified: Wed, 14 Jul 2021 01:14:19 GMT  
		Size: 238.9 MB (238929302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193577023dae8fd6d36536414dd47eb98a483fdcf9d56fb523ac3cd9b4b80f06`  
		Last Modified: Wed, 14 Jul 2021 01:11:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf1f931a8a0bada54ddb1868696700aed914f2205fcf2d217323a06a12897c`  
		Last Modified: Wed, 14 Jul 2021 01:15:03 GMT  
		Size: 54.7 MB (54695702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dc768f3e4222fe29a227fe190b7dff33b4c25fc8c8423d81dc83f47634fbb3`  
		Last Modified: Wed, 14 Jul 2021 01:14:33 GMT  
		Size: 269.7 KB (269680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e632e952bcaf0807284b647dec165289d61395139d9d50307f600e4ae928d0b`  
		Last Modified: Wed, 14 Jul 2021 01:15:19 GMT  
		Size: 64.7 MB (64746099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4700cd0e55ec4689d10f8da0b292b3b58a8f52b07d10b0ff28072467263a9c39`  
		Last Modified: Wed, 14 Jul 2021 01:18:51 GMT  
		Size: 259.9 MB (259879173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1f13e80d9989dcd03291647cdb26e47ff27b4ce78de2c9e769e79aa931e09f1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.4 MB (703396106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfa94140117f7480b84b81a59d881a5f20db96862994c4d184cada469db967e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:26:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:26:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:26:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:27:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:27:41 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:28:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:28:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:28:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:30:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41769627f180322e716b3023e5ef1ae59239c5ec3ba63d3feb96951d73d5878`  
		Last Modified: Wed, 14 Jul 2021 00:47:53 GMT  
		Size: 841.3 KB (841282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63f135f6f4db75ebf1ed14bf2422b3e612ec51db4bc3162a3a75a8b8df7b1b`  
		Last Modified: Wed, 14 Jul 2021 00:47:51 GMT  
		Size: 4.5 MB (4453635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3d85ee829fbd9be39df324330a8fe50c97a4b0c1247389b35c752404e77956`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c861f823f51f0edd135ae9cfa7425e5069eee2dc8641b3295ac532e11f81a`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0bc4e6e6bc21814066b9ec7467ea608909aead56aaf7d7f6972cc89eefea9f`  
		Last Modified: Wed, 14 Jul 2021 00:48:44 GMT  
		Size: 252.4 MB (252361492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767e94dd377ecd0bbcfb7093ad56d12b9939dcd7e13e05dd7670d173f21a2c5`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757b61452d8eae6c89294b87e561cbfba03e0e55970cafa498482560fb4b149c`  
		Last Modified: Wed, 14 Jul 2021 00:49:13 GMT  
		Size: 63.1 MB (63057473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ae03f3e351dc5e7ad9a7a7326828f929507da72882680dde4eb7b4b257d66a`  
		Last Modified: Wed, 14 Jul 2021 00:49:03 GMT  
		Size: 269.6 KB (269565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd788c193bc11dec6b0622c8def99e36c29b17a5c68360cc67bca0a52b5d74`  
		Last Modified: Wed, 14 Jul 2021 00:49:18 GMT  
		Size: 67.2 MB (67222233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f59ad25c5a9eed6d97c13dd07cd9ffd646f2f4f0963c6ba693f84b64db0a06`  
		Last Modified: Wed, 14 Jul 2021 00:50:50 GMT  
		Size: 291.5 MB (291458513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:8fb5d5ae193f0e00ae7b88a0b8b8574bba37d5b182d666d5aace3784c2864e97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:4f77b7983751f82229d2167f2601f19ea9dfed600d2add2e4e62144f401f0dcc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448429857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7534e98061854591891289aacefbe4665c302c0e18eb2b95c9b92f7a99f3a9b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:53:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:53:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 01:57:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:57:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:57:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:58:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:58:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:59:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1107129de068a3615596b08dc61d39c6a7722d1f446096ae57c3f28769bfca39`  
		Last Modified: Tue, 13 Jul 2021 23:14:34 GMT  
		Size: 840.8 KB (840788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a7fbbce93b678f9a7ec24c63012d604fef4a9cad8414c5b8a467f2930e4d`  
		Last Modified: Wed, 14 Jul 2021 02:29:23 GMT  
		Size: 4.9 MB (4872342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea558154c977de1713b413508635ea067b8a9cb2caac2c2d33399aa134072c7a`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a009470670a1026f1819627c53fb14edf956e0cc56b9ead79340c9de91ed8`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8abfba080c1ed4e3b4bdc2bf0d8eee89b03d0c97b04d513b964b4b26aa96d`  
		Last Modified: Wed, 14 Jul 2021 02:30:07 GMT  
		Size: 259.4 MB (259436482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906763856d86a129884f2d128bbc8ba73658b2c439deafb32dc704ad6f8f3d3`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e724da914872a99c21d1c752fe003c146cf3fda351f11997235ba7772cdba`  
		Last Modified: Wed, 14 Jul 2021 02:30:31 GMT  
		Size: 70.2 MB (70229653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a2ee178e82d7a724d90e3a8d8e37e8f09ccb10b47b1b62479653c997cb1df0`  
		Last Modified: Wed, 14 Jul 2021 02:30:20 GMT  
		Size: 269.6 KB (269609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b958a59ce23c95988f3219849b668a9b70003fa348726a8d3f88d1f5281a4715`  
		Last Modified: Wed, 14 Jul 2021 02:30:35 GMT  
		Size: 75.0 MB (74994876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d3de5e357728022b59ffac5d209fb766dabf58ab4d6ca073e371d82256056e`  
		Last Modified: Wed, 14 Jul 2021 02:30:52 GMT  
		Size: 11.1 MB (11077547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:61e98cbf3268458279d81c99b2242d25879e5abe6c39488bb5e71de2c2b92a1b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (395994921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79342d85c4ffce61a75fa2d3cbbfee3317b043c12b2543231fd968b32da4cec0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:50:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:50:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:53:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:53:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:53:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:54:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:54:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:56:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42872bf962a1c39ef027f457cefdef3c14b61de5a2e4eb23c3cd86de2ddf9554`  
		Last Modified: Wed, 14 Jul 2021 01:11:43 GMT  
		Size: 841.4 KB (841422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86d64b6163277a8faa0275b3fcba0855d5af76a2212503e755cba50cb08d4d`  
		Last Modified: Wed, 14 Jul 2021 01:11:42 GMT  
		Size: 4.1 MB (4085737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c8f9089545ebc81b78035f6c8bcc9757f8574fc623e07301fbc6081e76d1ee`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a241e304ad2761062f5ec7258e0a2490ccfb82ee70d01cca739111e2656605a0`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6434ded48ed96eaf7f1622cc6d4a0d69212f24911da077bb3e36b45f85e1487`  
		Last Modified: Wed, 14 Jul 2021 01:14:19 GMT  
		Size: 238.9 MB (238929302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193577023dae8fd6d36536414dd47eb98a483fdcf9d56fb523ac3cd9b4b80f06`  
		Last Modified: Wed, 14 Jul 2021 01:11:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf1f931a8a0bada54ddb1868696700aed914f2205fcf2d217323a06a12897c`  
		Last Modified: Wed, 14 Jul 2021 01:15:03 GMT  
		Size: 54.7 MB (54695702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dc768f3e4222fe29a227fe190b7dff33b4c25fc8c8423d81dc83f47634fbb3`  
		Last Modified: Wed, 14 Jul 2021 01:14:33 GMT  
		Size: 269.7 KB (269680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e632e952bcaf0807284b647dec165289d61395139d9d50307f600e4ae928d0b`  
		Last Modified: Wed, 14 Jul 2021 01:15:19 GMT  
		Size: 64.7 MB (64746099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f163f6facf7915ed1361c02ce023903ec332843f27d78246993b5bf15fe0efb`  
		Last Modified: Wed, 14 Jul 2021 01:15:46 GMT  
		Size: 10.1 MB (10120489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bcd6dbc4c225ebbe65b2a969eb95f9197b3c3af9c5c59935cde8b859c1f591b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422669461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b895d9e92f835cb0cb94a210aa510ab0f274f2163a3643c010678ff169b563e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:26:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:26:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:26:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:27:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:27:41 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:28:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:28:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:28:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41769627f180322e716b3023e5ef1ae59239c5ec3ba63d3feb96951d73d5878`  
		Last Modified: Wed, 14 Jul 2021 00:47:53 GMT  
		Size: 841.3 KB (841282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63f135f6f4db75ebf1ed14bf2422b3e612ec51db4bc3162a3a75a8b8df7b1b`  
		Last Modified: Wed, 14 Jul 2021 00:47:51 GMT  
		Size: 4.5 MB (4453635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3d85ee829fbd9be39df324330a8fe50c97a4b0c1247389b35c752404e77956`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c861f823f51f0edd135ae9cfa7425e5069eee2dc8641b3295ac532e11f81a`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0bc4e6e6bc21814066b9ec7467ea608909aead56aaf7d7f6972cc89eefea9f`  
		Last Modified: Wed, 14 Jul 2021 00:48:44 GMT  
		Size: 252.4 MB (252361492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767e94dd377ecd0bbcfb7093ad56d12b9939dcd7e13e05dd7670d173f21a2c5`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757b61452d8eae6c89294b87e561cbfba03e0e55970cafa498482560fb4b149c`  
		Last Modified: Wed, 14 Jul 2021 00:49:13 GMT  
		Size: 63.1 MB (63057473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ae03f3e351dc5e7ad9a7a7326828f929507da72882680dde4eb7b4b257d66a`  
		Last Modified: Wed, 14 Jul 2021 00:49:03 GMT  
		Size: 269.6 KB (269565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd788c193bc11dec6b0622c8def99e36c29b17a5c68360cc67bca0a52b5d74`  
		Last Modified: Wed, 14 Jul 2021 00:49:18 GMT  
		Size: 67.2 MB (67222233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0073605ff6b06de0753d62a4d3f35f3df0d0a298ab337cca5b9e16c8f832543`  
		Last Modified: Wed, 14 Jul 2021 00:49:39 GMT  
		Size: 10.7 MB (10731868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:8fb5d5ae193f0e00ae7b88a0b8b8574bba37d5b182d666d5aace3784c2864e97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:4f77b7983751f82229d2167f2601f19ea9dfed600d2add2e4e62144f401f0dcc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448429857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7534e98061854591891289aacefbe4665c302c0e18eb2b95c9b92f7a99f3a9b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:53:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:53:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 01:57:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:57:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:57:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:58:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:58:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:59:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1107129de068a3615596b08dc61d39c6a7722d1f446096ae57c3f28769bfca39`  
		Last Modified: Tue, 13 Jul 2021 23:14:34 GMT  
		Size: 840.8 KB (840788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a7fbbce93b678f9a7ec24c63012d604fef4a9cad8414c5b8a467f2930e4d`  
		Last Modified: Wed, 14 Jul 2021 02:29:23 GMT  
		Size: 4.9 MB (4872342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea558154c977de1713b413508635ea067b8a9cb2caac2c2d33399aa134072c7a`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a009470670a1026f1819627c53fb14edf956e0cc56b9ead79340c9de91ed8`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8abfba080c1ed4e3b4bdc2bf0d8eee89b03d0c97b04d513b964b4b26aa96d`  
		Last Modified: Wed, 14 Jul 2021 02:30:07 GMT  
		Size: 259.4 MB (259436482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906763856d86a129884f2d128bbc8ba73658b2c439deafb32dc704ad6f8f3d3`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e724da914872a99c21d1c752fe003c146cf3fda351f11997235ba7772cdba`  
		Last Modified: Wed, 14 Jul 2021 02:30:31 GMT  
		Size: 70.2 MB (70229653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a2ee178e82d7a724d90e3a8d8e37e8f09ccb10b47b1b62479653c997cb1df0`  
		Last Modified: Wed, 14 Jul 2021 02:30:20 GMT  
		Size: 269.6 KB (269609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b958a59ce23c95988f3219849b668a9b70003fa348726a8d3f88d1f5281a4715`  
		Last Modified: Wed, 14 Jul 2021 02:30:35 GMT  
		Size: 75.0 MB (74994876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d3de5e357728022b59ffac5d209fb766dabf58ab4d6ca073e371d82256056e`  
		Last Modified: Wed, 14 Jul 2021 02:30:52 GMT  
		Size: 11.1 MB (11077547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:61e98cbf3268458279d81c99b2242d25879e5abe6c39488bb5e71de2c2b92a1b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (395994921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79342d85c4ffce61a75fa2d3cbbfee3317b043c12b2543231fd968b32da4cec0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:50:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:50:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:53:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:53:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:53:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:54:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:54:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:56:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42872bf962a1c39ef027f457cefdef3c14b61de5a2e4eb23c3cd86de2ddf9554`  
		Last Modified: Wed, 14 Jul 2021 01:11:43 GMT  
		Size: 841.4 KB (841422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86d64b6163277a8faa0275b3fcba0855d5af76a2212503e755cba50cb08d4d`  
		Last Modified: Wed, 14 Jul 2021 01:11:42 GMT  
		Size: 4.1 MB (4085737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c8f9089545ebc81b78035f6c8bcc9757f8574fc623e07301fbc6081e76d1ee`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a241e304ad2761062f5ec7258e0a2490ccfb82ee70d01cca739111e2656605a0`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6434ded48ed96eaf7f1622cc6d4a0d69212f24911da077bb3e36b45f85e1487`  
		Last Modified: Wed, 14 Jul 2021 01:14:19 GMT  
		Size: 238.9 MB (238929302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193577023dae8fd6d36536414dd47eb98a483fdcf9d56fb523ac3cd9b4b80f06`  
		Last Modified: Wed, 14 Jul 2021 01:11:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf1f931a8a0bada54ddb1868696700aed914f2205fcf2d217323a06a12897c`  
		Last Modified: Wed, 14 Jul 2021 01:15:03 GMT  
		Size: 54.7 MB (54695702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dc768f3e4222fe29a227fe190b7dff33b4c25fc8c8423d81dc83f47634fbb3`  
		Last Modified: Wed, 14 Jul 2021 01:14:33 GMT  
		Size: 269.7 KB (269680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e632e952bcaf0807284b647dec165289d61395139d9d50307f600e4ae928d0b`  
		Last Modified: Wed, 14 Jul 2021 01:15:19 GMT  
		Size: 64.7 MB (64746099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f163f6facf7915ed1361c02ce023903ec332843f27d78246993b5bf15fe0efb`  
		Last Modified: Wed, 14 Jul 2021 01:15:46 GMT  
		Size: 10.1 MB (10120489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bcd6dbc4c225ebbe65b2a969eb95f9197b3c3af9c5c59935cde8b859c1f591b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422669461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b895d9e92f835cb0cb94a210aa510ab0f274f2163a3643c010678ff169b563e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:26:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:26:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:26:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:27:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:27:41 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:28:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:28:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:28:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41769627f180322e716b3023e5ef1ae59239c5ec3ba63d3feb96951d73d5878`  
		Last Modified: Wed, 14 Jul 2021 00:47:53 GMT  
		Size: 841.3 KB (841282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63f135f6f4db75ebf1ed14bf2422b3e612ec51db4bc3162a3a75a8b8df7b1b`  
		Last Modified: Wed, 14 Jul 2021 00:47:51 GMT  
		Size: 4.5 MB (4453635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3d85ee829fbd9be39df324330a8fe50c97a4b0c1247389b35c752404e77956`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c861f823f51f0edd135ae9cfa7425e5069eee2dc8641b3295ac532e11f81a`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0bc4e6e6bc21814066b9ec7467ea608909aead56aaf7d7f6972cc89eefea9f`  
		Last Modified: Wed, 14 Jul 2021 00:48:44 GMT  
		Size: 252.4 MB (252361492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767e94dd377ecd0bbcfb7093ad56d12b9939dcd7e13e05dd7670d173f21a2c5`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757b61452d8eae6c89294b87e561cbfba03e0e55970cafa498482560fb4b149c`  
		Last Modified: Wed, 14 Jul 2021 00:49:13 GMT  
		Size: 63.1 MB (63057473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ae03f3e351dc5e7ad9a7a7326828f929507da72882680dde4eb7b4b257d66a`  
		Last Modified: Wed, 14 Jul 2021 00:49:03 GMT  
		Size: 269.6 KB (269565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd788c193bc11dec6b0622c8def99e36c29b17a5c68360cc67bca0a52b5d74`  
		Last Modified: Wed, 14 Jul 2021 00:49:18 GMT  
		Size: 67.2 MB (67222233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0073605ff6b06de0753d62a4d3f35f3df0d0a298ab337cca5b9e16c8f832543`  
		Last Modified: Wed, 14 Jul 2021 00:49:39 GMT  
		Size: 10.7 MB (10731868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:5cb69d502cff623004c1e4967e8ebe632c136aea7598ec3be25fecf243e588df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:e250575746ce217c6d18bd3369ac85fdd31faa57485b8ca4cfc5b5a71873f5f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437352310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6358b4a94be18f7307dd098afa12f669f6f48f71414a6aac1624946e3e6bb0c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:53:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:53:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 01:57:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:57:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:57:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:58:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:58:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1107129de068a3615596b08dc61d39c6a7722d1f446096ae57c3f28769bfca39`  
		Last Modified: Tue, 13 Jul 2021 23:14:34 GMT  
		Size: 840.8 KB (840788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a7fbbce93b678f9a7ec24c63012d604fef4a9cad8414c5b8a467f2930e4d`  
		Last Modified: Wed, 14 Jul 2021 02:29:23 GMT  
		Size: 4.9 MB (4872342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea558154c977de1713b413508635ea067b8a9cb2caac2c2d33399aa134072c7a`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a009470670a1026f1819627c53fb14edf956e0cc56b9ead79340c9de91ed8`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8abfba080c1ed4e3b4bdc2bf0d8eee89b03d0c97b04d513b964b4b26aa96d`  
		Last Modified: Wed, 14 Jul 2021 02:30:07 GMT  
		Size: 259.4 MB (259436482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906763856d86a129884f2d128bbc8ba73658b2c439deafb32dc704ad6f8f3d3`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e724da914872a99c21d1c752fe003c146cf3fda351f11997235ba7772cdba`  
		Last Modified: Wed, 14 Jul 2021 02:30:31 GMT  
		Size: 70.2 MB (70229653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a2ee178e82d7a724d90e3a8d8e37e8f09ccb10b47b1b62479653c997cb1df0`  
		Last Modified: Wed, 14 Jul 2021 02:30:20 GMT  
		Size: 269.6 KB (269609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b958a59ce23c95988f3219849b668a9b70003fa348726a8d3f88d1f5281a4715`  
		Last Modified: Wed, 14 Jul 2021 02:30:35 GMT  
		Size: 75.0 MB (74994876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:7a8849406ecc1d8f59be615d0df0c6053628ee8b72cf7d1da54e0d14529d6404
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385874432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029b973a5417d0d37ba392315e216308319602737150f61619be6a9aecb32089`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:50:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:50:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:53:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:53:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:53:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:54:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:54:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42872bf962a1c39ef027f457cefdef3c14b61de5a2e4eb23c3cd86de2ddf9554`  
		Last Modified: Wed, 14 Jul 2021 01:11:43 GMT  
		Size: 841.4 KB (841422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86d64b6163277a8faa0275b3fcba0855d5af76a2212503e755cba50cb08d4d`  
		Last Modified: Wed, 14 Jul 2021 01:11:42 GMT  
		Size: 4.1 MB (4085737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c8f9089545ebc81b78035f6c8bcc9757f8574fc623e07301fbc6081e76d1ee`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a241e304ad2761062f5ec7258e0a2490ccfb82ee70d01cca739111e2656605a0`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6434ded48ed96eaf7f1622cc6d4a0d69212f24911da077bb3e36b45f85e1487`  
		Last Modified: Wed, 14 Jul 2021 01:14:19 GMT  
		Size: 238.9 MB (238929302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193577023dae8fd6d36536414dd47eb98a483fdcf9d56fb523ac3cd9b4b80f06`  
		Last Modified: Wed, 14 Jul 2021 01:11:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf1f931a8a0bada54ddb1868696700aed914f2205fcf2d217323a06a12897c`  
		Last Modified: Wed, 14 Jul 2021 01:15:03 GMT  
		Size: 54.7 MB (54695702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dc768f3e4222fe29a227fe190b7dff33b4c25fc8c8423d81dc83f47634fbb3`  
		Last Modified: Wed, 14 Jul 2021 01:14:33 GMT  
		Size: 269.7 KB (269680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e632e952bcaf0807284b647dec165289d61395139d9d50307f600e4ae928d0b`  
		Last Modified: Wed, 14 Jul 2021 01:15:19 GMT  
		Size: 64.7 MB (64746099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1a691b80df54ca92e8384ee974db49cf3bf6c5d91a2d4d82ede19f9a7ba67b76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411937593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aae085ede476478224c506fd8cdb4ec4f6b065badec5e43411705926c7e15ec`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:26:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:26:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:26:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:27:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:27:41 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:28:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:28:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:28:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41769627f180322e716b3023e5ef1ae59239c5ec3ba63d3feb96951d73d5878`  
		Last Modified: Wed, 14 Jul 2021 00:47:53 GMT  
		Size: 841.3 KB (841282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63f135f6f4db75ebf1ed14bf2422b3e612ec51db4bc3162a3a75a8b8df7b1b`  
		Last Modified: Wed, 14 Jul 2021 00:47:51 GMT  
		Size: 4.5 MB (4453635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3d85ee829fbd9be39df324330a8fe50c97a4b0c1247389b35c752404e77956`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c861f823f51f0edd135ae9cfa7425e5069eee2dc8641b3295ac532e11f81a`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0bc4e6e6bc21814066b9ec7467ea608909aead56aaf7d7f6972cc89eefea9f`  
		Last Modified: Wed, 14 Jul 2021 00:48:44 GMT  
		Size: 252.4 MB (252361492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767e94dd377ecd0bbcfb7093ad56d12b9939dcd7e13e05dd7670d173f21a2c5`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757b61452d8eae6c89294b87e561cbfba03e0e55970cafa498482560fb4b149c`  
		Last Modified: Wed, 14 Jul 2021 00:49:13 GMT  
		Size: 63.1 MB (63057473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ae03f3e351dc5e7ad9a7a7326828f929507da72882680dde4eb7b4b257d66a`  
		Last Modified: Wed, 14 Jul 2021 00:49:03 GMT  
		Size: 269.6 KB (269565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd788c193bc11dec6b0622c8def99e36c29b17a5c68360cc67bca0a52b5d74`  
		Last Modified: Wed, 14 Jul 2021 00:49:18 GMT  
		Size: 67.2 MB (67222233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:5cb69d502cff623004c1e4967e8ebe632c136aea7598ec3be25fecf243e588df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:e250575746ce217c6d18bd3369ac85fdd31faa57485b8ca4cfc5b5a71873f5f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437352310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6358b4a94be18f7307dd098afa12f669f6f48f71414a6aac1624946e3e6bb0c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:53:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:53:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 01:57:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:57:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:57:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:58:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:58:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1107129de068a3615596b08dc61d39c6a7722d1f446096ae57c3f28769bfca39`  
		Last Modified: Tue, 13 Jul 2021 23:14:34 GMT  
		Size: 840.8 KB (840788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a7fbbce93b678f9a7ec24c63012d604fef4a9cad8414c5b8a467f2930e4d`  
		Last Modified: Wed, 14 Jul 2021 02:29:23 GMT  
		Size: 4.9 MB (4872342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea558154c977de1713b413508635ea067b8a9cb2caac2c2d33399aa134072c7a`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a009470670a1026f1819627c53fb14edf956e0cc56b9ead79340c9de91ed8`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8abfba080c1ed4e3b4bdc2bf0d8eee89b03d0c97b04d513b964b4b26aa96d`  
		Last Modified: Wed, 14 Jul 2021 02:30:07 GMT  
		Size: 259.4 MB (259436482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906763856d86a129884f2d128bbc8ba73658b2c439deafb32dc704ad6f8f3d3`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e724da914872a99c21d1c752fe003c146cf3fda351f11997235ba7772cdba`  
		Last Modified: Wed, 14 Jul 2021 02:30:31 GMT  
		Size: 70.2 MB (70229653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a2ee178e82d7a724d90e3a8d8e37e8f09ccb10b47b1b62479653c997cb1df0`  
		Last Modified: Wed, 14 Jul 2021 02:30:20 GMT  
		Size: 269.6 KB (269609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b958a59ce23c95988f3219849b668a9b70003fa348726a8d3f88d1f5281a4715`  
		Last Modified: Wed, 14 Jul 2021 02:30:35 GMT  
		Size: 75.0 MB (74994876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:7a8849406ecc1d8f59be615d0df0c6053628ee8b72cf7d1da54e0d14529d6404
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385874432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029b973a5417d0d37ba392315e216308319602737150f61619be6a9aecb32089`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:50:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:50:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:53:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:53:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:53:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:54:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:54:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42872bf962a1c39ef027f457cefdef3c14b61de5a2e4eb23c3cd86de2ddf9554`  
		Last Modified: Wed, 14 Jul 2021 01:11:43 GMT  
		Size: 841.4 KB (841422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86d64b6163277a8faa0275b3fcba0855d5af76a2212503e755cba50cb08d4d`  
		Last Modified: Wed, 14 Jul 2021 01:11:42 GMT  
		Size: 4.1 MB (4085737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c8f9089545ebc81b78035f6c8bcc9757f8574fc623e07301fbc6081e76d1ee`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a241e304ad2761062f5ec7258e0a2490ccfb82ee70d01cca739111e2656605a0`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6434ded48ed96eaf7f1622cc6d4a0d69212f24911da077bb3e36b45f85e1487`  
		Last Modified: Wed, 14 Jul 2021 01:14:19 GMT  
		Size: 238.9 MB (238929302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193577023dae8fd6d36536414dd47eb98a483fdcf9d56fb523ac3cd9b4b80f06`  
		Last Modified: Wed, 14 Jul 2021 01:11:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf1f931a8a0bada54ddb1868696700aed914f2205fcf2d217323a06a12897c`  
		Last Modified: Wed, 14 Jul 2021 01:15:03 GMT  
		Size: 54.7 MB (54695702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dc768f3e4222fe29a227fe190b7dff33b4c25fc8c8423d81dc83f47634fbb3`  
		Last Modified: Wed, 14 Jul 2021 01:14:33 GMT  
		Size: 269.7 KB (269680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e632e952bcaf0807284b647dec165289d61395139d9d50307f600e4ae928d0b`  
		Last Modified: Wed, 14 Jul 2021 01:15:19 GMT  
		Size: 64.7 MB (64746099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1a691b80df54ca92e8384ee974db49cf3bf6c5d91a2d4d82ede19f9a7ba67b76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.9 MB (411937593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aae085ede476478224c506fd8cdb4ec4f6b065badec5e43411705926c7e15ec`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:26:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:26:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:26:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:27:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:27:41 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:28:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:28:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:28:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41769627f180322e716b3023e5ef1ae59239c5ec3ba63d3feb96951d73d5878`  
		Last Modified: Wed, 14 Jul 2021 00:47:53 GMT  
		Size: 841.3 KB (841282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63f135f6f4db75ebf1ed14bf2422b3e612ec51db4bc3162a3a75a8b8df7b1b`  
		Last Modified: Wed, 14 Jul 2021 00:47:51 GMT  
		Size: 4.5 MB (4453635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3d85ee829fbd9be39df324330a8fe50c97a4b0c1247389b35c752404e77956`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c861f823f51f0edd135ae9cfa7425e5069eee2dc8641b3295ac532e11f81a`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0bc4e6e6bc21814066b9ec7467ea608909aead56aaf7d7f6972cc89eefea9f`  
		Last Modified: Wed, 14 Jul 2021 00:48:44 GMT  
		Size: 252.4 MB (252361492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767e94dd377ecd0bbcfb7093ad56d12b9939dcd7e13e05dd7670d173f21a2c5`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757b61452d8eae6c89294b87e561cbfba03e0e55970cafa498482560fb4b149c`  
		Last Modified: Wed, 14 Jul 2021 00:49:13 GMT  
		Size: 63.1 MB (63057473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ae03f3e351dc5e7ad9a7a7326828f929507da72882680dde4eb7b4b257d66a`  
		Last Modified: Wed, 14 Jul 2021 00:49:03 GMT  
		Size: 269.6 KB (269565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd788c193bc11dec6b0622c8def99e36c29b17a5c68360cc67bca0a52b5d74`  
		Last Modified: Wed, 14 Jul 2021 00:49:18 GMT  
		Size: 67.2 MB (67222233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:bf0eb5f3cf9d7d81e35ecc54a271d49c3f5903b9e14a24766deea46efd77915c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:f4e443c903daa42241d67a65e51e77f738ed53152872aef763cae20229b8aaaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291858172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c5100ec73d9f52ba5c15bc6a39061c920eb76dbc6ad7af7764955f3d025311`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:53:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:53:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 01:57:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:57:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:57:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1107129de068a3615596b08dc61d39c6a7722d1f446096ae57c3f28769bfca39`  
		Last Modified: Tue, 13 Jul 2021 23:14:34 GMT  
		Size: 840.8 KB (840788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a7fbbce93b678f9a7ec24c63012d604fef4a9cad8414c5b8a467f2930e4d`  
		Last Modified: Wed, 14 Jul 2021 02:29:23 GMT  
		Size: 4.9 MB (4872342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea558154c977de1713b413508635ea067b8a9cb2caac2c2d33399aa134072c7a`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a009470670a1026f1819627c53fb14edf956e0cc56b9ead79340c9de91ed8`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8abfba080c1ed4e3b4bdc2bf0d8eee89b03d0c97b04d513b964b4b26aa96d`  
		Last Modified: Wed, 14 Jul 2021 02:30:07 GMT  
		Size: 259.4 MB (259436482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906763856d86a129884f2d128bbc8ba73658b2c439deafb32dc704ad6f8f3d3`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:628bee3532ab9eaa9de73ed73ad31fc0d28da33a63299d0b2813aa962ceac751
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266162951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c3beeef57cc2a97b39b2849049ac5862b35e8308f3dc59355d3e6f022c59a4c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:50:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:50:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:53:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:53:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:53:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42872bf962a1c39ef027f457cefdef3c14b61de5a2e4eb23c3cd86de2ddf9554`  
		Last Modified: Wed, 14 Jul 2021 01:11:43 GMT  
		Size: 841.4 KB (841422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86d64b6163277a8faa0275b3fcba0855d5af76a2212503e755cba50cb08d4d`  
		Last Modified: Wed, 14 Jul 2021 01:11:42 GMT  
		Size: 4.1 MB (4085737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c8f9089545ebc81b78035f6c8bcc9757f8574fc623e07301fbc6081e76d1ee`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a241e304ad2761062f5ec7258e0a2490ccfb82ee70d01cca739111e2656605a0`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6434ded48ed96eaf7f1622cc6d4a0d69212f24911da077bb3e36b45f85e1487`  
		Last Modified: Wed, 14 Jul 2021 01:14:19 GMT  
		Size: 238.9 MB (238929302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193577023dae8fd6d36536414dd47eb98a483fdcf9d56fb523ac3cd9b4b80f06`  
		Last Modified: Wed, 14 Jul 2021 01:11:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:041b574c78ee9baf5989a9cd6250c6f65c718a32c8e960f93e29990ef0d94976
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281388322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80d1bab3903f9becc4925d1bf4e936e185e4904699c4f5484ffdf6fb2c59008f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:26:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:26:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:26:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:27:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:27:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41769627f180322e716b3023e5ef1ae59239c5ec3ba63d3feb96951d73d5878`  
		Last Modified: Wed, 14 Jul 2021 00:47:53 GMT  
		Size: 841.3 KB (841282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63f135f6f4db75ebf1ed14bf2422b3e612ec51db4bc3162a3a75a8b8df7b1b`  
		Last Modified: Wed, 14 Jul 2021 00:47:51 GMT  
		Size: 4.5 MB (4453635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3d85ee829fbd9be39df324330a8fe50c97a4b0c1247389b35c752404e77956`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c861f823f51f0edd135ae9cfa7425e5069eee2dc8641b3295ac532e11f81a`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0bc4e6e6bc21814066b9ec7467ea608909aead56aaf7d7f6972cc89eefea9f`  
		Last Modified: Wed, 14 Jul 2021 00:48:44 GMT  
		Size: 252.4 MB (252361492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767e94dd377ecd0bbcfb7093ad56d12b9939dcd7e13e05dd7670d173f21a2c5`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:bf0eb5f3cf9d7d81e35ecc54a271d49c3f5903b9e14a24766deea46efd77915c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:f4e443c903daa42241d67a65e51e77f738ed53152872aef763cae20229b8aaaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291858172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c5100ec73d9f52ba5c15bc6a39061c920eb76dbc6ad7af7764955f3d025311`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:53:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:53:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 01:57:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:57:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:57:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1107129de068a3615596b08dc61d39c6a7722d1f446096ae57c3f28769bfca39`  
		Last Modified: Tue, 13 Jul 2021 23:14:34 GMT  
		Size: 840.8 KB (840788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a7fbbce93b678f9a7ec24c63012d604fef4a9cad8414c5b8a467f2930e4d`  
		Last Modified: Wed, 14 Jul 2021 02:29:23 GMT  
		Size: 4.9 MB (4872342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea558154c977de1713b413508635ea067b8a9cb2caac2c2d33399aa134072c7a`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a009470670a1026f1819627c53fb14edf956e0cc56b9ead79340c9de91ed8`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8abfba080c1ed4e3b4bdc2bf0d8eee89b03d0c97b04d513b964b4b26aa96d`  
		Last Modified: Wed, 14 Jul 2021 02:30:07 GMT  
		Size: 259.4 MB (259436482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906763856d86a129884f2d128bbc8ba73658b2c439deafb32dc704ad6f8f3d3`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:628bee3532ab9eaa9de73ed73ad31fc0d28da33a63299d0b2813aa962ceac751
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266162951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c3beeef57cc2a97b39b2849049ac5862b35e8308f3dc59355d3e6f022c59a4c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:50:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:50:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:53:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:53:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:53:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42872bf962a1c39ef027f457cefdef3c14b61de5a2e4eb23c3cd86de2ddf9554`  
		Last Modified: Wed, 14 Jul 2021 01:11:43 GMT  
		Size: 841.4 KB (841422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86d64b6163277a8faa0275b3fcba0855d5af76a2212503e755cba50cb08d4d`  
		Last Modified: Wed, 14 Jul 2021 01:11:42 GMT  
		Size: 4.1 MB (4085737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c8f9089545ebc81b78035f6c8bcc9757f8574fc623e07301fbc6081e76d1ee`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a241e304ad2761062f5ec7258e0a2490ccfb82ee70d01cca739111e2656605a0`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6434ded48ed96eaf7f1622cc6d4a0d69212f24911da077bb3e36b45f85e1487`  
		Last Modified: Wed, 14 Jul 2021 01:14:19 GMT  
		Size: 238.9 MB (238929302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193577023dae8fd6d36536414dd47eb98a483fdcf9d56fb523ac3cd9b4b80f06`  
		Last Modified: Wed, 14 Jul 2021 01:11:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:041b574c78ee9baf5989a9cd6250c6f65c718a32c8e960f93e29990ef0d94976
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281388322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80d1bab3903f9becc4925d1bf4e936e185e4904699c4f5484ffdf6fb2c59008f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:26:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:26:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:26:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:27:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:27:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41769627f180322e716b3023e5ef1ae59239c5ec3ba63d3feb96951d73d5878`  
		Last Modified: Wed, 14 Jul 2021 00:47:53 GMT  
		Size: 841.3 KB (841282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63f135f6f4db75ebf1ed14bf2422b3e612ec51db4bc3162a3a75a8b8df7b1b`  
		Last Modified: Wed, 14 Jul 2021 00:47:51 GMT  
		Size: 4.5 MB (4453635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3d85ee829fbd9be39df324330a8fe50c97a4b0c1247389b35c752404e77956`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c861f823f51f0edd135ae9cfa7425e5069eee2dc8641b3295ac532e11f81a`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0bc4e6e6bc21814066b9ec7467ea608909aead56aaf7d7f6972cc89eefea9f`  
		Last Modified: Wed, 14 Jul 2021 00:48:44 GMT  
		Size: 252.4 MB (252361492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767e94dd377ecd0bbcfb7093ad56d12b9939dcd7e13e05dd7670d173f21a2c5`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:8d1f2ef5fb434a44d42cb351057d60051a5189ee8f004e2b908b315c1efef3d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:b86dd45c91810f1d3fcd3e71cae037cd4d7b72259c12fcb2b01c61b56ef3f9be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339171352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c75e892305ef5ab58d4577cb13433537d2630cc6e50f2a6afb1ffb72941ba22`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:06:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 02:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:09:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 02:09:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:09:25 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:10:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:10:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fc149e3ee734eaa227c577708e79be620b1cfbdc44eba44feb059be8d49971`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c2a7ad34c303dcb8348811e3ee140f0bb94723bdea38c27e3cfa94c838602`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa62a799c06ad3c3011c26d06d55762eb5765bd81835e8989d55c8c7fc04806`  
		Last Modified: Wed, 14 Jul 2021 02:32:50 GMT  
		Size: 176.7 MB (176700701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360166355a7d9f55f98c1058cee3cef1c4ab76332ab13cf582f2993c8a40e881`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6360a9085b12f4ed8ac487d8b34824d7238d62178791afce5c3528eff7846b`  
		Last Modified: Wed, 14 Jul 2021 02:33:10 GMT  
		Size: 47.3 MB (47259111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f6269c2be5c26ee8b44ee2f34dfd7425a57f8a93678ac249222838d0dda7e2`  
		Last Modified: Wed, 14 Jul 2021 02:33:01 GMT  
		Size: 311.4 KB (311426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535103c95d968dd78f20089095f78c0ae8f47704a8680927b3e321c01564d6b`  
		Last Modified: Wed, 14 Jul 2021 02:33:16 GMT  
		Size: 79.6 MB (79602525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:2dbc144c61e66565df67f78119ac4df1e3749f96de5241a33c90ff8ea91a71b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284614576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be03030d2d7ac22b0b649b073098992cb8a07700ce0beae38e470b30420a8e65`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:00:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:00:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:00:40 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:00:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:00:42 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 01:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:02:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:02:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:02:59 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:03:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:03:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:04:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ef2a91707578a7aa5e67bde1b1ee25c43d3e2005c3514859d532dabeeba08`  
		Last Modified: Wed, 14 Jul 2021 01:19:08 GMT  
		Size: 1.2 MB (1183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f09bd680e7527c5536e3230907946a5aa58e56eb96ad044ecdea7e8de6f17ae`  
		Last Modified: Wed, 14 Jul 2021 01:19:07 GMT  
		Size: 4.7 MB (4676456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0314c569a7bfdae2ebb0dcb70368ff20da4a4641f48f7eb29871f5616511a011`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60830c62be41d8614c4359151a1187cb0f2341edefe989e8854fdf7da34765b`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cb8d0e16826782c8658ccc6b607e60dccc7a6671377b04b9ed908e42c5300`  
		Last Modified: Wed, 14 Jul 2021 01:21:18 GMT  
		Size: 157.2 MB (157205836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8c442e11344f7e8c76f4beaff7faf0c960a0067648aa8da2da8fa44fc3ed03`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879dc1c1cf3f6722a9a613abfa5e2dc0d952c41aaaa0643a79a7287f61b7eca5`  
		Last Modified: Wed, 14 Jul 2021 01:21:52 GMT  
		Size: 36.7 MB (36691143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec4f202fb03053e9739c7176bcf25a69aba7c750bb93e09640c0378cd4e547`  
		Last Modified: Wed, 14 Jul 2021 01:21:32 GMT  
		Size: 311.4 KB (311429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2883f187e8c7f1f285a7d98023e857d0c52b4914a15b2184adecc907c0795b`  
		Last Modified: Wed, 14 Jul 2021 01:22:15 GMT  
		Size: 60.5 MB (60481826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:48165af6bf6d4cb2c1ce596596e90b230ab4693f4ba1261966e12703a9f9cb3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.8 MB (318814411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8691163736865a3a200a68c03a86b48f07aee1fb8a305e1e8107fbb1b44beced`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:31:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 00:32:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:32:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:32:21 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:32:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:33:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c16bac23518e4abf60d1c392e081256894df83fb7cddae089cfaf7131e2101`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db12b2dd1b010b5d533dcf3aafc411ceaf8c995dc98159511b4cb32f94c27c8`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f940dbd5b4415e8d2641c3154a2ae919cdc2b9fde7c70677e48453e3f349b29`  
		Last Modified: Wed, 14 Jul 2021 00:51:46 GMT  
		Size: 171.1 MB (171141545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59698e949a60aa162ddd3ef9bf411fcd75f8055472fe660a8191034d8525c5`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a8eff17984ce9b4d02bbb30b90dd2f14b922d2c80af7394b157c0d136aa766`  
		Last Modified: Wed, 14 Jul 2021 00:52:06 GMT  
		Size: 41.5 MB (41520897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4174f757f3653a6b2fde53f1fc1b10284fec87f13eaeb286475643d600b9d743`  
		Last Modified: Wed, 14 Jul 2021 00:51:59 GMT  
		Size: 311.4 KB (311365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84169b7479a191b9f2919dbc47e7f6a10d328878886100eba2a445d8533c2261`  
		Last Modified: Wed, 14 Jul 2021 00:52:11 GMT  
		Size: 72.0 MB (71972680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:788abbdd16f2717b6c6c1235bc32627ccbb4a9cbeb925b41eb09042bbec77bb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:4f854c0fe7f05228e5ebcdb1da76dbc98d5b9d9a3947c2f28c14b49c8d30ebf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **838.2 MB (838184607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28ba90d41392b3639e70ea49f0c999c2c8a1f7dc241c774894430ba49043e8ba`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:06:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 02:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:09:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 02:09:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:09:25 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:10:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:10:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fc149e3ee734eaa227c577708e79be620b1cfbdc44eba44feb059be8d49971`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c2a7ad34c303dcb8348811e3ee140f0bb94723bdea38c27e3cfa94c838602`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa62a799c06ad3c3011c26d06d55762eb5765bd81835e8989d55c8c7fc04806`  
		Last Modified: Wed, 14 Jul 2021 02:32:50 GMT  
		Size: 176.7 MB (176700701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360166355a7d9f55f98c1058cee3cef1c4ab76332ab13cf582f2993c8a40e881`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6360a9085b12f4ed8ac487d8b34824d7238d62178791afce5c3528eff7846b`  
		Last Modified: Wed, 14 Jul 2021 02:33:10 GMT  
		Size: 47.3 MB (47259111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f6269c2be5c26ee8b44ee2f34dfd7425a57f8a93678ac249222838d0dda7e2`  
		Last Modified: Wed, 14 Jul 2021 02:33:01 GMT  
		Size: 311.4 KB (311426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535103c95d968dd78f20089095f78c0ae8f47704a8680927b3e321c01564d6b`  
		Last Modified: Wed, 14 Jul 2021 02:33:16 GMT  
		Size: 79.6 MB (79602525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62871fd2842b89c20a23780f9f5164c3c87d753e64a4f976b0a20ffb1ef8b48`  
		Last Modified: Wed, 14 Jul 2021 02:35:11 GMT  
		Size: 499.0 MB (499013255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:e1580f4c020e90d3746c2d356e42db84ae88d46665fab12d8e92013f537a37a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **727.9 MB (727857525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d085d8d4ac489f1fdeeacdef7b094f25b1c8eadf4bfc1644feeda1dacf02c15b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:00:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:00:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:00:40 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:00:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:00:42 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 01:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:02:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:02:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:02:59 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:03:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:03:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:04:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:09:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ef2a91707578a7aa5e67bde1b1ee25c43d3e2005c3514859d532dabeeba08`  
		Last Modified: Wed, 14 Jul 2021 01:19:08 GMT  
		Size: 1.2 MB (1183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f09bd680e7527c5536e3230907946a5aa58e56eb96ad044ecdea7e8de6f17ae`  
		Last Modified: Wed, 14 Jul 2021 01:19:07 GMT  
		Size: 4.7 MB (4676456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0314c569a7bfdae2ebb0dcb70368ff20da4a4641f48f7eb29871f5616511a011`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60830c62be41d8614c4359151a1187cb0f2341edefe989e8854fdf7da34765b`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cb8d0e16826782c8658ccc6b607e60dccc7a6671377b04b9ed908e42c5300`  
		Last Modified: Wed, 14 Jul 2021 01:21:18 GMT  
		Size: 157.2 MB (157205836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8c442e11344f7e8c76f4beaff7faf0c960a0067648aa8da2da8fa44fc3ed03`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879dc1c1cf3f6722a9a613abfa5e2dc0d952c41aaaa0643a79a7287f61b7eca5`  
		Last Modified: Wed, 14 Jul 2021 01:21:52 GMT  
		Size: 36.7 MB (36691143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec4f202fb03053e9739c7176bcf25a69aba7c750bb93e09640c0378cd4e547`  
		Last Modified: Wed, 14 Jul 2021 01:21:32 GMT  
		Size: 311.4 KB (311429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2883f187e8c7f1f285a7d98023e857d0c52b4914a15b2184adecc907c0795b`  
		Last Modified: Wed, 14 Jul 2021 01:22:15 GMT  
		Size: 60.5 MB (60481826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9358db55b8bc624945da369b5ac9da2083940f66af836c0940439c5d213e9006`  
		Last Modified: Wed, 14 Jul 2021 01:27:41 GMT  
		Size: 443.2 MB (443242949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:97eb2b87592fb74fb146057b956a707cb2857167dc72450ed1a869e9f48fc5d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.1 MB (787113112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cdc5fb795e596fba14ac06ca8fbdfb9f59f26da50b75a7a2d7c14483dfb9496`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:31:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 00:32:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:32:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:32:21 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:32:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:33:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:35:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c16bac23518e4abf60d1c392e081256894df83fb7cddae089cfaf7131e2101`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db12b2dd1b010b5d533dcf3aafc411ceaf8c995dc98159511b4cb32f94c27c8`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f940dbd5b4415e8d2641c3154a2ae919cdc2b9fde7c70677e48453e3f349b29`  
		Last Modified: Wed, 14 Jul 2021 00:51:46 GMT  
		Size: 171.1 MB (171141545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59698e949a60aa162ddd3ef9bf411fcd75f8055472fe660a8191034d8525c5`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a8eff17984ce9b4d02bbb30b90dd2f14b922d2c80af7394b157c0d136aa766`  
		Last Modified: Wed, 14 Jul 2021 00:52:06 GMT  
		Size: 41.5 MB (41520897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4174f757f3653a6b2fde53f1fc1b10284fec87f13eaeb286475643d600b9d743`  
		Last Modified: Wed, 14 Jul 2021 00:51:59 GMT  
		Size: 311.4 KB (311365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84169b7479a191b9f2919dbc47e7f6a10d328878886100eba2a445d8533c2261`  
		Last Modified: Wed, 14 Jul 2021 00:52:11 GMT  
		Size: 72.0 MB (71972680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eeda9cec8d9f57856b200d3de8e4ecb7273230ef351cde599f88b64fe29c2bf`  
		Last Modified: Wed, 14 Jul 2021 00:54:11 GMT  
		Size: 468.3 MB (468298701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:c8e0c09b861b15b539e34c9ac02f0c9d054f8917856fdf04756fb388056b6e9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:95171ed138733e8b903a5f871af1e7b7660f9cee6385d0a0623785c5ee74b0c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **968.0 MB (967996808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5264f5838f360835a3c06415bc5885f6580b675109102ed7f8e152394b99932`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:54:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:54:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 23 Jun 2021 16:54:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 23 Jun 2021 16:54:07 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 16:54:07 GMT
ENV LC_ALL=C.UTF-8
# Wed, 23 Jun 2021 16:54:07 GMT
ENV ROS_DISTRO=noetic
# Wed, 23 Jun 2021 16:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:55:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 23 Jun 2021 16:55:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 23 Jun 2021 16:55:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:55:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:55:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 23 Jun 2021 16:56:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:59:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368710b5d60bd3571596105db24587dc7641662961cd8565f0ab308ea71c8716`  
		Last Modified: Wed, 23 Jun 2021 17:00:59 GMT  
		Size: 10.9 MB (10891785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c851fa0b21cd231e582f810f8c19cefe3e82acfd0b381ee63df5ad2ea6d405`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d911fa207ab982f2d18b595a9cbd025da0e7d7b99a38329c00d496ae74e5c57`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf3cb86fc6e74480b1bed2f10d298288eaef33b5c4a44e36c5723bed2d7d603`  
		Last Modified: Wed, 23 Jun 2021 17:01:36 GMT  
		Size: 239.0 MB (239043542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6807ff55dd30ea5a41adf5345578639e51e44f6cac1d76453af573795d8367d9`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda640c7cc970da7dc489bbd348f6d10ca8aadea00bb348b143454fef3f798f1`  
		Last Modified: Wed, 23 Jun 2021 17:01:59 GMT  
		Size: 86.6 MB (86566646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6b8e0c86f409efb0b6383db70437892d4daca00797115f65c9c22a2ed27322`  
		Last Modified: Wed, 23 Jun 2021 17:01:45 GMT  
		Size: 302.4 KB (302359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aeca0ec3c658ebff801eb589b5d7083dafb559be63ecbf3a4f0ed4cb127398`  
		Last Modified: Wed, 23 Jun 2021 17:02:00 GMT  
		Size: 76.0 MB (75974809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdb9b3d78aef77e80ec1947e18fe26e59fcbab970732b81d76d3c7cf980209b`  
		Last Modified: Wed, 23 Jun 2021 17:03:43 GMT  
		Size: 504.8 MB (504779638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0cea16968607f7d0018a950bd28631977542a0cd563a19972fb990aeb699cf76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **884.8 MB (884774266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee770b0841c380ee388cc22de354bef2754788aa80a63f2acb201b36d064bfa9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:34:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:34:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 23 Jun 2021 12:34:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 23 Jun 2021 12:34:36 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 12:34:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 23 Jun 2021 12:34:36 GMT
ENV ROS_DISTRO=noetic
# Wed, 23 Jun 2021 12:35:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:35:36 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 23 Jun 2021 12:35:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 23 Jun 2021 12:35:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:35:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:36:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 23 Jun 2021 12:36:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:39:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a6d0fd3d166254b7e229d1f59f216a508567a9850665d123014684e30eeb4c`  
		Last Modified: Wed, 23 Jun 2021 12:42:27 GMT  
		Size: 10.9 MB (10883414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a054e7e8c0b332fb66dc5088973cbcb57d8a1ce5e8249443fef3856a708478`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee9c05970568fc6fe659f9305867a4b6425bed7f4237de3516cf3dc553f0238`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df81d3dac71b04be5d0a51a53296f7f7dd6d0aa6d6387c7229191cb57889b58`  
		Last Modified: Wed, 23 Jun 2021 12:43:01 GMT  
		Size: 184.2 MB (184226666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce9ec19f2ee8191d40e2ceea8d6bd89e9e0f8133c049808b0548557b9b71f65`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b320ffadbb584163174053ad9da711044b8679fc2a8de068ee4732f53449edec`  
		Last Modified: Wed, 23 Jun 2021 12:43:23 GMT  
		Size: 84.4 MB (84357037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9607df761ad999a479ca2c254d645b6cc0426d0805ed9e5106482e2eb75b334`  
		Last Modified: Wed, 23 Jun 2021 12:43:10 GMT  
		Size: 302.1 KB (302127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6589ea28fd69f1bbfdce955f0e3598a503017bc915334e4405b7373d17320b8`  
		Last Modified: Wed, 23 Jun 2021 12:43:21 GMT  
		Size: 74.1 MB (74088042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755fdb7bedf30fa92d7a8dc3fd1bba014066a11c857139006e3e3098e3712543`  
		Last Modified: Wed, 23 Jun 2021 12:45:02 GMT  
		Size: 481.7 MB (481692577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:788abbdd16f2717b6c6c1235bc32627ccbb4a9cbeb925b41eb09042bbec77bb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:4f854c0fe7f05228e5ebcdb1da76dbc98d5b9d9a3947c2f28c14b49c8d30ebf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **838.2 MB (838184607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28ba90d41392b3639e70ea49f0c999c2c8a1f7dc241c774894430ba49043e8ba`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:06:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 02:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:09:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 02:09:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:09:25 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:10:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:10:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fc149e3ee734eaa227c577708e79be620b1cfbdc44eba44feb059be8d49971`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c2a7ad34c303dcb8348811e3ee140f0bb94723bdea38c27e3cfa94c838602`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa62a799c06ad3c3011c26d06d55762eb5765bd81835e8989d55c8c7fc04806`  
		Last Modified: Wed, 14 Jul 2021 02:32:50 GMT  
		Size: 176.7 MB (176700701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360166355a7d9f55f98c1058cee3cef1c4ab76332ab13cf582f2993c8a40e881`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6360a9085b12f4ed8ac487d8b34824d7238d62178791afce5c3528eff7846b`  
		Last Modified: Wed, 14 Jul 2021 02:33:10 GMT  
		Size: 47.3 MB (47259111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f6269c2be5c26ee8b44ee2f34dfd7425a57f8a93678ac249222838d0dda7e2`  
		Last Modified: Wed, 14 Jul 2021 02:33:01 GMT  
		Size: 311.4 KB (311426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535103c95d968dd78f20089095f78c0ae8f47704a8680927b3e321c01564d6b`  
		Last Modified: Wed, 14 Jul 2021 02:33:16 GMT  
		Size: 79.6 MB (79602525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62871fd2842b89c20a23780f9f5164c3c87d753e64a4f976b0a20ffb1ef8b48`  
		Last Modified: Wed, 14 Jul 2021 02:35:11 GMT  
		Size: 499.0 MB (499013255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:e1580f4c020e90d3746c2d356e42db84ae88d46665fab12d8e92013f537a37a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **727.9 MB (727857525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d085d8d4ac489f1fdeeacdef7b094f25b1c8eadf4bfc1644feeda1dacf02c15b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:00:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:00:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:00:40 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:00:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:00:42 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 01:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:02:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:02:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:02:59 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:03:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:03:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:04:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:09:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ef2a91707578a7aa5e67bde1b1ee25c43d3e2005c3514859d532dabeeba08`  
		Last Modified: Wed, 14 Jul 2021 01:19:08 GMT  
		Size: 1.2 MB (1183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f09bd680e7527c5536e3230907946a5aa58e56eb96ad044ecdea7e8de6f17ae`  
		Last Modified: Wed, 14 Jul 2021 01:19:07 GMT  
		Size: 4.7 MB (4676456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0314c569a7bfdae2ebb0dcb70368ff20da4a4641f48f7eb29871f5616511a011`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60830c62be41d8614c4359151a1187cb0f2341edefe989e8854fdf7da34765b`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cb8d0e16826782c8658ccc6b607e60dccc7a6671377b04b9ed908e42c5300`  
		Last Modified: Wed, 14 Jul 2021 01:21:18 GMT  
		Size: 157.2 MB (157205836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8c442e11344f7e8c76f4beaff7faf0c960a0067648aa8da2da8fa44fc3ed03`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879dc1c1cf3f6722a9a613abfa5e2dc0d952c41aaaa0643a79a7287f61b7eca5`  
		Last Modified: Wed, 14 Jul 2021 01:21:52 GMT  
		Size: 36.7 MB (36691143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec4f202fb03053e9739c7176bcf25a69aba7c750bb93e09640c0378cd4e547`  
		Last Modified: Wed, 14 Jul 2021 01:21:32 GMT  
		Size: 311.4 KB (311429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2883f187e8c7f1f285a7d98023e857d0c52b4914a15b2184adecc907c0795b`  
		Last Modified: Wed, 14 Jul 2021 01:22:15 GMT  
		Size: 60.5 MB (60481826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9358db55b8bc624945da369b5ac9da2083940f66af836c0940439c5d213e9006`  
		Last Modified: Wed, 14 Jul 2021 01:27:41 GMT  
		Size: 443.2 MB (443242949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:97eb2b87592fb74fb146057b956a707cb2857167dc72450ed1a869e9f48fc5d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.1 MB (787113112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cdc5fb795e596fba14ac06ca8fbdfb9f59f26da50b75a7a2d7c14483dfb9496`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:31:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 00:32:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:32:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:32:21 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:32:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:33:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:35:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c16bac23518e4abf60d1c392e081256894df83fb7cddae089cfaf7131e2101`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db12b2dd1b010b5d533dcf3aafc411ceaf8c995dc98159511b4cb32f94c27c8`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f940dbd5b4415e8d2641c3154a2ae919cdc2b9fde7c70677e48453e3f349b29`  
		Last Modified: Wed, 14 Jul 2021 00:51:46 GMT  
		Size: 171.1 MB (171141545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59698e949a60aa162ddd3ef9bf411fcd75f8055472fe660a8191034d8525c5`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a8eff17984ce9b4d02bbb30b90dd2f14b922d2c80af7394b157c0d136aa766`  
		Last Modified: Wed, 14 Jul 2021 00:52:06 GMT  
		Size: 41.5 MB (41520897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4174f757f3653a6b2fde53f1fc1b10284fec87f13eaeb286475643d600b9d743`  
		Last Modified: Wed, 14 Jul 2021 00:51:59 GMT  
		Size: 311.4 KB (311365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84169b7479a191b9f2919dbc47e7f6a10d328878886100eba2a445d8533c2261`  
		Last Modified: Wed, 14 Jul 2021 00:52:11 GMT  
		Size: 72.0 MB (71972680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eeda9cec8d9f57856b200d3de8e4ecb7273230ef351cde599f88b64fe29c2bf`  
		Last Modified: Wed, 14 Jul 2021 00:54:11 GMT  
		Size: 468.3 MB (468298701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:cac7431a907c43e4bb3bd022d806bff1f7c2370d481168407c10e795a00c8ffc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:adea3cc00b209b6593981d24148705d0359e181f6c6858e92ce16d6ca06a93fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.9 MB (354908217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84870c73cac7e080a24ef027e5e15a8f787e57f2d863ef675db254f80ded325`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:06:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 02:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:09:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 02:09:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:09:25 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:10:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:10:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fc149e3ee734eaa227c577708e79be620b1cfbdc44eba44feb059be8d49971`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c2a7ad34c303dcb8348811e3ee140f0bb94723bdea38c27e3cfa94c838602`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa62a799c06ad3c3011c26d06d55762eb5765bd81835e8989d55c8c7fc04806`  
		Last Modified: Wed, 14 Jul 2021 02:32:50 GMT  
		Size: 176.7 MB (176700701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360166355a7d9f55f98c1058cee3cef1c4ab76332ab13cf582f2993c8a40e881`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6360a9085b12f4ed8ac487d8b34824d7238d62178791afce5c3528eff7846b`  
		Last Modified: Wed, 14 Jul 2021 02:33:10 GMT  
		Size: 47.3 MB (47259111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f6269c2be5c26ee8b44ee2f34dfd7425a57f8a93678ac249222838d0dda7e2`  
		Last Modified: Wed, 14 Jul 2021 02:33:01 GMT  
		Size: 311.4 KB (311426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535103c95d968dd78f20089095f78c0ae8f47704a8680927b3e321c01564d6b`  
		Last Modified: Wed, 14 Jul 2021 02:33:16 GMT  
		Size: 79.6 MB (79602525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e76fea2ad07f5de223daeb1b7ba4b90eceea87f143acb5a234ba9b0b9ed3dc`  
		Last Modified: Wed, 14 Jul 2021 02:33:32 GMT  
		Size: 15.7 MB (15736865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:60637874699daa2683541796ac4718fe8342902c616a98e3457ccca8a6cfdb4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298574628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e985262ef637bc5ae04d487a6dac768c5e674470613025d23c0428876754e9c4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:00:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:00:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:00:40 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:00:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:00:42 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 01:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:02:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:02:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:02:59 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:03:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:03:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:04:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:05:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ef2a91707578a7aa5e67bde1b1ee25c43d3e2005c3514859d532dabeeba08`  
		Last Modified: Wed, 14 Jul 2021 01:19:08 GMT  
		Size: 1.2 MB (1183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f09bd680e7527c5536e3230907946a5aa58e56eb96ad044ecdea7e8de6f17ae`  
		Last Modified: Wed, 14 Jul 2021 01:19:07 GMT  
		Size: 4.7 MB (4676456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0314c569a7bfdae2ebb0dcb70368ff20da4a4641f48f7eb29871f5616511a011`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60830c62be41d8614c4359151a1187cb0f2341edefe989e8854fdf7da34765b`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cb8d0e16826782c8658ccc6b607e60dccc7a6671377b04b9ed908e42c5300`  
		Last Modified: Wed, 14 Jul 2021 01:21:18 GMT  
		Size: 157.2 MB (157205836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8c442e11344f7e8c76f4beaff7faf0c960a0067648aa8da2da8fa44fc3ed03`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879dc1c1cf3f6722a9a613abfa5e2dc0d952c41aaaa0643a79a7287f61b7eca5`  
		Last Modified: Wed, 14 Jul 2021 01:21:52 GMT  
		Size: 36.7 MB (36691143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec4f202fb03053e9739c7176bcf25a69aba7c750bb93e09640c0378cd4e547`  
		Last Modified: Wed, 14 Jul 2021 01:21:32 GMT  
		Size: 311.4 KB (311429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2883f187e8c7f1f285a7d98023e857d0c52b4914a15b2184adecc907c0795b`  
		Last Modified: Wed, 14 Jul 2021 01:22:15 GMT  
		Size: 60.5 MB (60481826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2d2e1516fd3ed66de5e7409b55f60dc3063b6a8cf213ee9e9ed34782703bd6`  
		Last Modified: Wed, 14 Jul 2021 01:22:42 GMT  
		Size: 14.0 MB (13960052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a305257d71a2d242cf088acda5b112f391dcf652eea4a79a45a2d9d6510d19bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334165507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40781401db230b03e4d695ed840b6e8f715a7737ac0e721d33efb20ffc8e5ebf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:31:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 00:32:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:32:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:32:21 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:32:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:33:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c16bac23518e4abf60d1c392e081256894df83fb7cddae089cfaf7131e2101`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db12b2dd1b010b5d533dcf3aafc411ceaf8c995dc98159511b4cb32f94c27c8`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f940dbd5b4415e8d2641c3154a2ae919cdc2b9fde7c70677e48453e3f349b29`  
		Last Modified: Wed, 14 Jul 2021 00:51:46 GMT  
		Size: 171.1 MB (171141545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59698e949a60aa162ddd3ef9bf411fcd75f8055472fe660a8191034d8525c5`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a8eff17984ce9b4d02bbb30b90dd2f14b922d2c80af7394b157c0d136aa766`  
		Last Modified: Wed, 14 Jul 2021 00:52:06 GMT  
		Size: 41.5 MB (41520897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4174f757f3653a6b2fde53f1fc1b10284fec87f13eaeb286475643d600b9d743`  
		Last Modified: Wed, 14 Jul 2021 00:51:59 GMT  
		Size: 311.4 KB (311365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84169b7479a191b9f2919dbc47e7f6a10d328878886100eba2a445d8533c2261`  
		Last Modified: Wed, 14 Jul 2021 00:52:11 GMT  
		Size: 72.0 MB (71972680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44ec7b7f6e0363e1b00715552ee9caaf2ea50968c6e8e1ba02f0b2f1f951531`  
		Last Modified: Wed, 14 Jul 2021 00:52:31 GMT  
		Size: 15.4 MB (15351096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:d3c2c83940885aa9fc2d2f1f477022dfb06d7b3b8982a22f5bef51d78432c076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:ffcbf02b129bfb3faa964d9f10e97f1cc501435a4c1fd3747a5bf0378e438498
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.4 MB (484437125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d30dabe6f695c3c478711677f35aeb261300c2420b136bb31d816d2378d2720`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:54:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:54:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 23 Jun 2021 16:54:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 23 Jun 2021 16:54:07 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 16:54:07 GMT
ENV LC_ALL=C.UTF-8
# Wed, 23 Jun 2021 16:54:07 GMT
ENV ROS_DISTRO=noetic
# Wed, 23 Jun 2021 16:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:55:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 23 Jun 2021 16:55:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 23 Jun 2021 16:55:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:55:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:55:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 23 Jun 2021 16:56:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:56:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368710b5d60bd3571596105db24587dc7641662961cd8565f0ab308ea71c8716`  
		Last Modified: Wed, 23 Jun 2021 17:00:59 GMT  
		Size: 10.9 MB (10891785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c851fa0b21cd231e582f810f8c19cefe3e82acfd0b381ee63df5ad2ea6d405`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d911fa207ab982f2d18b595a9cbd025da0e7d7b99a38329c00d496ae74e5c57`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf3cb86fc6e74480b1bed2f10d298288eaef33b5c4a44e36c5723bed2d7d603`  
		Last Modified: Wed, 23 Jun 2021 17:01:36 GMT  
		Size: 239.0 MB (239043542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6807ff55dd30ea5a41adf5345578639e51e44f6cac1d76453af573795d8367d9`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda640c7cc970da7dc489bbd348f6d10ca8aadea00bb348b143454fef3f798f1`  
		Last Modified: Wed, 23 Jun 2021 17:01:59 GMT  
		Size: 86.6 MB (86566646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6b8e0c86f409efb0b6383db70437892d4daca00797115f65c9c22a2ed27322`  
		Last Modified: Wed, 23 Jun 2021 17:01:45 GMT  
		Size: 302.4 KB (302359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aeca0ec3c658ebff801eb589b5d7083dafb559be63ecbf3a4f0ed4cb127398`  
		Last Modified: Wed, 23 Jun 2021 17:02:00 GMT  
		Size: 76.0 MB (75974809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228c8ed43e25be90ca823b4c143449a5b504b22c238a1ddc117569532f373d5`  
		Last Modified: Wed, 23 Jun 2021 17:02:11 GMT  
		Size: 21.2 MB (21219955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f3a211482cd13444032d6e0fd52b1ed4cda50d89bedb91082fa3dc0ed773415a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.0 MB (423977337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5c76dcf42f26e71f7f4551754bed4945433dfa588ec12a4065360e0454d8eb8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:34:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:34:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 23 Jun 2021 12:34:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 23 Jun 2021 12:34:36 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 12:34:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 23 Jun 2021 12:34:36 GMT
ENV ROS_DISTRO=noetic
# Wed, 23 Jun 2021 12:35:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:35:36 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 23 Jun 2021 12:35:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 23 Jun 2021 12:35:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:35:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:36:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 23 Jun 2021 12:36:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:36:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a6d0fd3d166254b7e229d1f59f216a508567a9850665d123014684e30eeb4c`  
		Last Modified: Wed, 23 Jun 2021 12:42:27 GMT  
		Size: 10.9 MB (10883414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a054e7e8c0b332fb66dc5088973cbcb57d8a1ce5e8249443fef3856a708478`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee9c05970568fc6fe659f9305867a4b6425bed7f4237de3516cf3dc553f0238`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df81d3dac71b04be5d0a51a53296f7f7dd6d0aa6d6387c7229191cb57889b58`  
		Last Modified: Wed, 23 Jun 2021 12:43:01 GMT  
		Size: 184.2 MB (184226666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce9ec19f2ee8191d40e2ceea8d6bd89e9e0f8133c049808b0548557b9b71f65`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b320ffadbb584163174053ad9da711044b8679fc2a8de068ee4732f53449edec`  
		Last Modified: Wed, 23 Jun 2021 12:43:23 GMT  
		Size: 84.4 MB (84357037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9607df761ad999a479ca2c254d645b6cc0426d0805ed9e5106482e2eb75b334`  
		Last Modified: Wed, 23 Jun 2021 12:43:10 GMT  
		Size: 302.1 KB (302127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6589ea28fd69f1bbfdce955f0e3598a503017bc915334e4405b7373d17320b8`  
		Last Modified: Wed, 23 Jun 2021 12:43:21 GMT  
		Size: 74.1 MB (74088042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d77fdf0e185059de6a2bcdc1db66a1eecaab06ef847415856f281d4b94575`  
		Last Modified: Wed, 23 Jun 2021 12:43:34 GMT  
		Size: 20.9 MB (20895648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:cac7431a907c43e4bb3bd022d806bff1f7c2370d481168407c10e795a00c8ffc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:adea3cc00b209b6593981d24148705d0359e181f6c6858e92ce16d6ca06a93fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.9 MB (354908217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84870c73cac7e080a24ef027e5e15a8f787e57f2d863ef675db254f80ded325`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:06:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 02:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:09:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 02:09:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:09:25 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:10:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:10:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fc149e3ee734eaa227c577708e79be620b1cfbdc44eba44feb059be8d49971`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c2a7ad34c303dcb8348811e3ee140f0bb94723bdea38c27e3cfa94c838602`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa62a799c06ad3c3011c26d06d55762eb5765bd81835e8989d55c8c7fc04806`  
		Last Modified: Wed, 14 Jul 2021 02:32:50 GMT  
		Size: 176.7 MB (176700701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360166355a7d9f55f98c1058cee3cef1c4ab76332ab13cf582f2993c8a40e881`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6360a9085b12f4ed8ac487d8b34824d7238d62178791afce5c3528eff7846b`  
		Last Modified: Wed, 14 Jul 2021 02:33:10 GMT  
		Size: 47.3 MB (47259111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f6269c2be5c26ee8b44ee2f34dfd7425a57f8a93678ac249222838d0dda7e2`  
		Last Modified: Wed, 14 Jul 2021 02:33:01 GMT  
		Size: 311.4 KB (311426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535103c95d968dd78f20089095f78c0ae8f47704a8680927b3e321c01564d6b`  
		Last Modified: Wed, 14 Jul 2021 02:33:16 GMT  
		Size: 79.6 MB (79602525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e76fea2ad07f5de223daeb1b7ba4b90eceea87f143acb5a234ba9b0b9ed3dc`  
		Last Modified: Wed, 14 Jul 2021 02:33:32 GMT  
		Size: 15.7 MB (15736865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:60637874699daa2683541796ac4718fe8342902c616a98e3457ccca8a6cfdb4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298574628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e985262ef637bc5ae04d487a6dac768c5e674470613025d23c0428876754e9c4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:00:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:00:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:00:40 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:00:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:00:42 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 01:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:02:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:02:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:02:59 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:03:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:03:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:04:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:05:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ef2a91707578a7aa5e67bde1b1ee25c43d3e2005c3514859d532dabeeba08`  
		Last Modified: Wed, 14 Jul 2021 01:19:08 GMT  
		Size: 1.2 MB (1183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f09bd680e7527c5536e3230907946a5aa58e56eb96ad044ecdea7e8de6f17ae`  
		Last Modified: Wed, 14 Jul 2021 01:19:07 GMT  
		Size: 4.7 MB (4676456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0314c569a7bfdae2ebb0dcb70368ff20da4a4641f48f7eb29871f5616511a011`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60830c62be41d8614c4359151a1187cb0f2341edefe989e8854fdf7da34765b`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cb8d0e16826782c8658ccc6b607e60dccc7a6671377b04b9ed908e42c5300`  
		Last Modified: Wed, 14 Jul 2021 01:21:18 GMT  
		Size: 157.2 MB (157205836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8c442e11344f7e8c76f4beaff7faf0c960a0067648aa8da2da8fa44fc3ed03`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879dc1c1cf3f6722a9a613abfa5e2dc0d952c41aaaa0643a79a7287f61b7eca5`  
		Last Modified: Wed, 14 Jul 2021 01:21:52 GMT  
		Size: 36.7 MB (36691143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec4f202fb03053e9739c7176bcf25a69aba7c750bb93e09640c0378cd4e547`  
		Last Modified: Wed, 14 Jul 2021 01:21:32 GMT  
		Size: 311.4 KB (311429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2883f187e8c7f1f285a7d98023e857d0c52b4914a15b2184adecc907c0795b`  
		Last Modified: Wed, 14 Jul 2021 01:22:15 GMT  
		Size: 60.5 MB (60481826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2d2e1516fd3ed66de5e7409b55f60dc3063b6a8cf213ee9e9ed34782703bd6`  
		Last Modified: Wed, 14 Jul 2021 01:22:42 GMT  
		Size: 14.0 MB (13960052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a305257d71a2d242cf088acda5b112f391dcf652eea4a79a45a2d9d6510d19bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334165507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40781401db230b03e4d695ed840b6e8f715a7737ac0e721d33efb20ffc8e5ebf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:31:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 00:32:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:32:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:32:21 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:32:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:33:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c16bac23518e4abf60d1c392e081256894df83fb7cddae089cfaf7131e2101`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db12b2dd1b010b5d533dcf3aafc411ceaf8c995dc98159511b4cb32f94c27c8`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f940dbd5b4415e8d2641c3154a2ae919cdc2b9fde7c70677e48453e3f349b29`  
		Last Modified: Wed, 14 Jul 2021 00:51:46 GMT  
		Size: 171.1 MB (171141545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59698e949a60aa162ddd3ef9bf411fcd75f8055472fe660a8191034d8525c5`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a8eff17984ce9b4d02bbb30b90dd2f14b922d2c80af7394b157c0d136aa766`  
		Last Modified: Wed, 14 Jul 2021 00:52:06 GMT  
		Size: 41.5 MB (41520897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4174f757f3653a6b2fde53f1fc1b10284fec87f13eaeb286475643d600b9d743`  
		Last Modified: Wed, 14 Jul 2021 00:51:59 GMT  
		Size: 311.4 KB (311365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84169b7479a191b9f2919dbc47e7f6a10d328878886100eba2a445d8533c2261`  
		Last Modified: Wed, 14 Jul 2021 00:52:11 GMT  
		Size: 72.0 MB (71972680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44ec7b7f6e0363e1b00715552ee9caaf2ea50968c6e8e1ba02f0b2f1f951531`  
		Last Modified: Wed, 14 Jul 2021 00:52:31 GMT  
		Size: 15.4 MB (15351096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:8d1f2ef5fb434a44d42cb351057d60051a5189ee8f004e2b908b315c1efef3d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:b86dd45c91810f1d3fcd3e71cae037cd4d7b72259c12fcb2b01c61b56ef3f9be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339171352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c75e892305ef5ab58d4577cb13433537d2630cc6e50f2a6afb1ffb72941ba22`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:06:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 02:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:09:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 02:09:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:09:25 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:10:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:10:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fc149e3ee734eaa227c577708e79be620b1cfbdc44eba44feb059be8d49971`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c2a7ad34c303dcb8348811e3ee140f0bb94723bdea38c27e3cfa94c838602`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa62a799c06ad3c3011c26d06d55762eb5765bd81835e8989d55c8c7fc04806`  
		Last Modified: Wed, 14 Jul 2021 02:32:50 GMT  
		Size: 176.7 MB (176700701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360166355a7d9f55f98c1058cee3cef1c4ab76332ab13cf582f2993c8a40e881`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6360a9085b12f4ed8ac487d8b34824d7238d62178791afce5c3528eff7846b`  
		Last Modified: Wed, 14 Jul 2021 02:33:10 GMT  
		Size: 47.3 MB (47259111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f6269c2be5c26ee8b44ee2f34dfd7425a57f8a93678ac249222838d0dda7e2`  
		Last Modified: Wed, 14 Jul 2021 02:33:01 GMT  
		Size: 311.4 KB (311426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535103c95d968dd78f20089095f78c0ae8f47704a8680927b3e321c01564d6b`  
		Last Modified: Wed, 14 Jul 2021 02:33:16 GMT  
		Size: 79.6 MB (79602525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:2dbc144c61e66565df67f78119ac4df1e3749f96de5241a33c90ff8ea91a71b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284614576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be03030d2d7ac22b0b649b073098992cb8a07700ce0beae38e470b30420a8e65`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:00:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:00:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:00:40 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:00:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:00:42 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 01:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:02:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:02:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:02:59 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:03:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:03:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:04:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ef2a91707578a7aa5e67bde1b1ee25c43d3e2005c3514859d532dabeeba08`  
		Last Modified: Wed, 14 Jul 2021 01:19:08 GMT  
		Size: 1.2 MB (1183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f09bd680e7527c5536e3230907946a5aa58e56eb96ad044ecdea7e8de6f17ae`  
		Last Modified: Wed, 14 Jul 2021 01:19:07 GMT  
		Size: 4.7 MB (4676456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0314c569a7bfdae2ebb0dcb70368ff20da4a4641f48f7eb29871f5616511a011`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60830c62be41d8614c4359151a1187cb0f2341edefe989e8854fdf7da34765b`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cb8d0e16826782c8658ccc6b607e60dccc7a6671377b04b9ed908e42c5300`  
		Last Modified: Wed, 14 Jul 2021 01:21:18 GMT  
		Size: 157.2 MB (157205836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8c442e11344f7e8c76f4beaff7faf0c960a0067648aa8da2da8fa44fc3ed03`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879dc1c1cf3f6722a9a613abfa5e2dc0d952c41aaaa0643a79a7287f61b7eca5`  
		Last Modified: Wed, 14 Jul 2021 01:21:52 GMT  
		Size: 36.7 MB (36691143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec4f202fb03053e9739c7176bcf25a69aba7c750bb93e09640c0378cd4e547`  
		Last Modified: Wed, 14 Jul 2021 01:21:32 GMT  
		Size: 311.4 KB (311429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2883f187e8c7f1f285a7d98023e857d0c52b4914a15b2184adecc907c0795b`  
		Last Modified: Wed, 14 Jul 2021 01:22:15 GMT  
		Size: 60.5 MB (60481826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:48165af6bf6d4cb2c1ce596596e90b230ab4693f4ba1261966e12703a9f9cb3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.8 MB (318814411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8691163736865a3a200a68c03a86b48f07aee1fb8a305e1e8107fbb1b44beced`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:31:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 00:32:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:32:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:32:21 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:32:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:33:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c16bac23518e4abf60d1c392e081256894df83fb7cddae089cfaf7131e2101`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db12b2dd1b010b5d533dcf3aafc411ceaf8c995dc98159511b4cb32f94c27c8`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f940dbd5b4415e8d2641c3154a2ae919cdc2b9fde7c70677e48453e3f349b29`  
		Last Modified: Wed, 14 Jul 2021 00:51:46 GMT  
		Size: 171.1 MB (171141545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59698e949a60aa162ddd3ef9bf411fcd75f8055472fe660a8191034d8525c5`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a8eff17984ce9b4d02bbb30b90dd2f14b922d2c80af7394b157c0d136aa766`  
		Last Modified: Wed, 14 Jul 2021 00:52:06 GMT  
		Size: 41.5 MB (41520897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4174f757f3653a6b2fde53f1fc1b10284fec87f13eaeb286475643d600b9d743`  
		Last Modified: Wed, 14 Jul 2021 00:51:59 GMT  
		Size: 311.4 KB (311365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84169b7479a191b9f2919dbc47e7f6a10d328878886100eba2a445d8533c2261`  
		Last Modified: Wed, 14 Jul 2021 00:52:11 GMT  
		Size: 72.0 MB (71972680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:d0f6a74157d324cc40669a97a06cbda8d13c79ab135fe3b7b61ccb557d67103f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:6aea7247bac4cb0aeb1792cb141ab3008ac272e24c56eab3ddebc1bf8dc1539d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.2 MB (463217170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c7863284678344dc36f900367d88af5fc116dfd0332fcf3ec755da65843afca`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:54:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:54:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 23 Jun 2021 16:54:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 23 Jun 2021 16:54:07 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 16:54:07 GMT
ENV LC_ALL=C.UTF-8
# Wed, 23 Jun 2021 16:54:07 GMT
ENV ROS_DISTRO=noetic
# Wed, 23 Jun 2021 16:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:55:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 23 Jun 2021 16:55:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 23 Jun 2021 16:55:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:55:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:55:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 23 Jun 2021 16:56:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368710b5d60bd3571596105db24587dc7641662961cd8565f0ab308ea71c8716`  
		Last Modified: Wed, 23 Jun 2021 17:00:59 GMT  
		Size: 10.9 MB (10891785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c851fa0b21cd231e582f810f8c19cefe3e82acfd0b381ee63df5ad2ea6d405`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d911fa207ab982f2d18b595a9cbd025da0e7d7b99a38329c00d496ae74e5c57`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf3cb86fc6e74480b1bed2f10d298288eaef33b5c4a44e36c5723bed2d7d603`  
		Last Modified: Wed, 23 Jun 2021 17:01:36 GMT  
		Size: 239.0 MB (239043542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6807ff55dd30ea5a41adf5345578639e51e44f6cac1d76453af573795d8367d9`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda640c7cc970da7dc489bbd348f6d10ca8aadea00bb348b143454fef3f798f1`  
		Last Modified: Wed, 23 Jun 2021 17:01:59 GMT  
		Size: 86.6 MB (86566646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6b8e0c86f409efb0b6383db70437892d4daca00797115f65c9c22a2ed27322`  
		Last Modified: Wed, 23 Jun 2021 17:01:45 GMT  
		Size: 302.4 KB (302359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aeca0ec3c658ebff801eb589b5d7083dafb559be63ecbf3a4f0ed4cb127398`  
		Last Modified: Wed, 23 Jun 2021 17:02:00 GMT  
		Size: 76.0 MB (75974809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b1ada5d4ae138bb9487fb775b2eb196bc064a26f59ab67da8b80abe62c7d1daa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.1 MB (403081689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10d0974add5e11f7b44c5e5e6e5a2b3c62a80867d1aa149625064403f5c088d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:34:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:34:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 23 Jun 2021 12:34:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 23 Jun 2021 12:34:36 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 12:34:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 23 Jun 2021 12:34:36 GMT
ENV ROS_DISTRO=noetic
# Wed, 23 Jun 2021 12:35:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:35:36 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 23 Jun 2021 12:35:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 23 Jun 2021 12:35:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:35:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:36:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 23 Jun 2021 12:36:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a6d0fd3d166254b7e229d1f59f216a508567a9850665d123014684e30eeb4c`  
		Last Modified: Wed, 23 Jun 2021 12:42:27 GMT  
		Size: 10.9 MB (10883414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a054e7e8c0b332fb66dc5088973cbcb57d8a1ce5e8249443fef3856a708478`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee9c05970568fc6fe659f9305867a4b6425bed7f4237de3516cf3dc553f0238`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df81d3dac71b04be5d0a51a53296f7f7dd6d0aa6d6387c7229191cb57889b58`  
		Last Modified: Wed, 23 Jun 2021 12:43:01 GMT  
		Size: 184.2 MB (184226666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce9ec19f2ee8191d40e2ceea8d6bd89e9e0f8133c049808b0548557b9b71f65`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b320ffadbb584163174053ad9da711044b8679fc2a8de068ee4732f53449edec`  
		Last Modified: Wed, 23 Jun 2021 12:43:23 GMT  
		Size: 84.4 MB (84357037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9607df761ad999a479ca2c254d645b6cc0426d0805ed9e5106482e2eb75b334`  
		Last Modified: Wed, 23 Jun 2021 12:43:10 GMT  
		Size: 302.1 KB (302127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6589ea28fd69f1bbfdce955f0e3598a503017bc915334e4405b7373d17320b8`  
		Last Modified: Wed, 23 Jun 2021 12:43:21 GMT  
		Size: 74.1 MB (74088042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:8d1f2ef5fb434a44d42cb351057d60051a5189ee8f004e2b908b315c1efef3d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:b86dd45c91810f1d3fcd3e71cae037cd4d7b72259c12fcb2b01c61b56ef3f9be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339171352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c75e892305ef5ab58d4577cb13433537d2630cc6e50f2a6afb1ffb72941ba22`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:06:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 02:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:09:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 02:09:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:09:25 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:10:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:10:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fc149e3ee734eaa227c577708e79be620b1cfbdc44eba44feb059be8d49971`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c2a7ad34c303dcb8348811e3ee140f0bb94723bdea38c27e3cfa94c838602`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa62a799c06ad3c3011c26d06d55762eb5765bd81835e8989d55c8c7fc04806`  
		Last Modified: Wed, 14 Jul 2021 02:32:50 GMT  
		Size: 176.7 MB (176700701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360166355a7d9f55f98c1058cee3cef1c4ab76332ab13cf582f2993c8a40e881`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6360a9085b12f4ed8ac487d8b34824d7238d62178791afce5c3528eff7846b`  
		Last Modified: Wed, 14 Jul 2021 02:33:10 GMT  
		Size: 47.3 MB (47259111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f6269c2be5c26ee8b44ee2f34dfd7425a57f8a93678ac249222838d0dda7e2`  
		Last Modified: Wed, 14 Jul 2021 02:33:01 GMT  
		Size: 311.4 KB (311426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535103c95d968dd78f20089095f78c0ae8f47704a8680927b3e321c01564d6b`  
		Last Modified: Wed, 14 Jul 2021 02:33:16 GMT  
		Size: 79.6 MB (79602525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:2dbc144c61e66565df67f78119ac4df1e3749f96de5241a33c90ff8ea91a71b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284614576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be03030d2d7ac22b0b649b073098992cb8a07700ce0beae38e470b30420a8e65`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:00:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:00:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:00:40 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:00:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:00:42 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 01:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:02:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:02:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:02:59 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:03:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:03:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:04:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ef2a91707578a7aa5e67bde1b1ee25c43d3e2005c3514859d532dabeeba08`  
		Last Modified: Wed, 14 Jul 2021 01:19:08 GMT  
		Size: 1.2 MB (1183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f09bd680e7527c5536e3230907946a5aa58e56eb96ad044ecdea7e8de6f17ae`  
		Last Modified: Wed, 14 Jul 2021 01:19:07 GMT  
		Size: 4.7 MB (4676456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0314c569a7bfdae2ebb0dcb70368ff20da4a4641f48f7eb29871f5616511a011`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60830c62be41d8614c4359151a1187cb0f2341edefe989e8854fdf7da34765b`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cb8d0e16826782c8658ccc6b607e60dccc7a6671377b04b9ed908e42c5300`  
		Last Modified: Wed, 14 Jul 2021 01:21:18 GMT  
		Size: 157.2 MB (157205836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8c442e11344f7e8c76f4beaff7faf0c960a0067648aa8da2da8fa44fc3ed03`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879dc1c1cf3f6722a9a613abfa5e2dc0d952c41aaaa0643a79a7287f61b7eca5`  
		Last Modified: Wed, 14 Jul 2021 01:21:52 GMT  
		Size: 36.7 MB (36691143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec4f202fb03053e9739c7176bcf25a69aba7c750bb93e09640c0378cd4e547`  
		Last Modified: Wed, 14 Jul 2021 01:21:32 GMT  
		Size: 311.4 KB (311429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2883f187e8c7f1f285a7d98023e857d0c52b4914a15b2184adecc907c0795b`  
		Last Modified: Wed, 14 Jul 2021 01:22:15 GMT  
		Size: 60.5 MB (60481826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:48165af6bf6d4cb2c1ce596596e90b230ab4693f4ba1261966e12703a9f9cb3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.8 MB (318814411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8691163736865a3a200a68c03a86b48f07aee1fb8a305e1e8107fbb1b44beced`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:31:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 00:32:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:32:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:32:21 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:32:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:33:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c16bac23518e4abf60d1c392e081256894df83fb7cddae089cfaf7131e2101`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db12b2dd1b010b5d533dcf3aafc411ceaf8c995dc98159511b4cb32f94c27c8`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f940dbd5b4415e8d2641c3154a2ae919cdc2b9fde7c70677e48453e3f349b29`  
		Last Modified: Wed, 14 Jul 2021 00:51:46 GMT  
		Size: 171.1 MB (171141545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59698e949a60aa162ddd3ef9bf411fcd75f8055472fe660a8191034d8525c5`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a8eff17984ce9b4d02bbb30b90dd2f14b922d2c80af7394b157c0d136aa766`  
		Last Modified: Wed, 14 Jul 2021 00:52:06 GMT  
		Size: 41.5 MB (41520897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4174f757f3653a6b2fde53f1fc1b10284fec87f13eaeb286475643d600b9d743`  
		Last Modified: Wed, 14 Jul 2021 00:51:59 GMT  
		Size: 311.4 KB (311365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84169b7479a191b9f2919dbc47e7f6a10d328878886100eba2a445d8533c2261`  
		Last Modified: Wed, 14 Jul 2021 00:52:11 GMT  
		Size: 72.0 MB (71972680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:6dabfd41cbea71d5a6951eedf23310c0066d8daea8e45eb150695fb8a54e8151
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:08b3a54d83699b1e50781e268e72ee769b1a433471e9157d5ea6a97f4bf77407
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (211998290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cac1ddb34ffd140fc52d682cb23466d1a7b69607a01a8cd233c3bab218e1cbc3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:06:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 02:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:09:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 02:09:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:09:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fc149e3ee734eaa227c577708e79be620b1cfbdc44eba44feb059be8d49971`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c2a7ad34c303dcb8348811e3ee140f0bb94723bdea38c27e3cfa94c838602`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa62a799c06ad3c3011c26d06d55762eb5765bd81835e8989d55c8c7fc04806`  
		Last Modified: Wed, 14 Jul 2021 02:32:50 GMT  
		Size: 176.7 MB (176700701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360166355a7d9f55f98c1058cee3cef1c4ab76332ab13cf582f2993c8a40e881`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:7110444de2301ea1901c1ec74777622d9999cd69527b83f16a7008a6b87fdb79
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187130178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75bc418e1ee0bff250528706626838b7aaf22bad859e91690b878b05c6eaad1a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:00:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:00:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:00:40 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:00:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:00:42 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 01:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:02:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:02:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:02:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ef2a91707578a7aa5e67bde1b1ee25c43d3e2005c3514859d532dabeeba08`  
		Last Modified: Wed, 14 Jul 2021 01:19:08 GMT  
		Size: 1.2 MB (1183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f09bd680e7527c5536e3230907946a5aa58e56eb96ad044ecdea7e8de6f17ae`  
		Last Modified: Wed, 14 Jul 2021 01:19:07 GMT  
		Size: 4.7 MB (4676456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0314c569a7bfdae2ebb0dcb70368ff20da4a4641f48f7eb29871f5616511a011`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60830c62be41d8614c4359151a1187cb0f2341edefe989e8854fdf7da34765b`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cb8d0e16826782c8658ccc6b607e60dccc7a6671377b04b9ed908e42c5300`  
		Last Modified: Wed, 14 Jul 2021 01:21:18 GMT  
		Size: 157.2 MB (157205836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8c442e11344f7e8c76f4beaff7faf0c960a0067648aa8da2da8fa44fc3ed03`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ad84bf1f4e24e924f529ce7ead29e4210e854a93febf4725a03662d978f7e696
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205009469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3319402086a4cde3f31db9a1423410b471c080d950246db7c92a388ba819ef5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:31:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 00:32:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:32:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:32:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c16bac23518e4abf60d1c392e081256894df83fb7cddae089cfaf7131e2101`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db12b2dd1b010b5d533dcf3aafc411ceaf8c995dc98159511b4cb32f94c27c8`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f940dbd5b4415e8d2641c3154a2ae919cdc2b9fde7c70677e48453e3f349b29`  
		Last Modified: Wed, 14 Jul 2021 00:51:46 GMT  
		Size: 171.1 MB (171141545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59698e949a60aa162ddd3ef9bf411fcd75f8055472fe660a8191034d8525c5`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:70f91bf81345452f6b045854b5dbacbc216ecfc9ec964fd6183b45ec39fb85e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:ba50632be1e7f85d68e1750783502c98aeb356878cc19ec375cc222e4e57e293
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300373356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ae679bd6a0c56288695dcf805c53dfc358da268737f120526eef15a7c90c3d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:54:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:54:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 23 Jun 2021 16:54:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 23 Jun 2021 16:54:07 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 16:54:07 GMT
ENV LC_ALL=C.UTF-8
# Wed, 23 Jun 2021 16:54:07 GMT
ENV ROS_DISTRO=noetic
# Wed, 23 Jun 2021 16:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:55:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 23 Jun 2021 16:55:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 23 Jun 2021 16:55:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368710b5d60bd3571596105db24587dc7641662961cd8565f0ab308ea71c8716`  
		Last Modified: Wed, 23 Jun 2021 17:00:59 GMT  
		Size: 10.9 MB (10891785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c851fa0b21cd231e582f810f8c19cefe3e82acfd0b381ee63df5ad2ea6d405`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d911fa207ab982f2d18b595a9cbd025da0e7d7b99a38329c00d496ae74e5c57`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf3cb86fc6e74480b1bed2f10d298288eaef33b5c4a44e36c5723bed2d7d603`  
		Last Modified: Wed, 23 Jun 2021 17:01:36 GMT  
		Size: 239.0 MB (239043542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6807ff55dd30ea5a41adf5345578639e51e44f6cac1d76453af573795d8367d9`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:12d2b8eb9ef000ea4ebee26ba7d5f1708def8cdf5c8e0587feb025fbed15a0c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244334483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fc1d3642319b3dd8ab3d8191544cbf0055c09e3b13e18933986409213904c79`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:34:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:34:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 23 Jun 2021 12:34:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 23 Jun 2021 12:34:36 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 12:34:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 23 Jun 2021 12:34:36 GMT
ENV ROS_DISTRO=noetic
# Wed, 23 Jun 2021 12:35:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:35:36 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 23 Jun 2021 12:35:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 23 Jun 2021 12:35:37 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a6d0fd3d166254b7e229d1f59f216a508567a9850665d123014684e30eeb4c`  
		Last Modified: Wed, 23 Jun 2021 12:42:27 GMT  
		Size: 10.9 MB (10883414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a054e7e8c0b332fb66dc5088973cbcb57d8a1ce5e8249443fef3856a708478`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee9c05970568fc6fe659f9305867a4b6425bed7f4237de3516cf3dc553f0238`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df81d3dac71b04be5d0a51a53296f7f7dd6d0aa6d6387c7229191cb57889b58`  
		Last Modified: Wed, 23 Jun 2021 12:43:01 GMT  
		Size: 184.2 MB (184226666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce9ec19f2ee8191d40e2ceea8d6bd89e9e0f8133c049808b0548557b9b71f65`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:6dabfd41cbea71d5a6951eedf23310c0066d8daea8e45eb150695fb8a54e8151
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:08b3a54d83699b1e50781e268e72ee769b1a433471e9157d5ea6a97f4bf77407
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (211998290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cac1ddb34ffd140fc52d682cb23466d1a7b69607a01a8cd233c3bab218e1cbc3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:06:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 02:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:09:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 02:09:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:09:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fc149e3ee734eaa227c577708e79be620b1cfbdc44eba44feb059be8d49971`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c2a7ad34c303dcb8348811e3ee140f0bb94723bdea38c27e3cfa94c838602`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa62a799c06ad3c3011c26d06d55762eb5765bd81835e8989d55c8c7fc04806`  
		Last Modified: Wed, 14 Jul 2021 02:32:50 GMT  
		Size: 176.7 MB (176700701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360166355a7d9f55f98c1058cee3cef1c4ab76332ab13cf582f2993c8a40e881`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:7110444de2301ea1901c1ec74777622d9999cd69527b83f16a7008a6b87fdb79
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187130178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75bc418e1ee0bff250528706626838b7aaf22bad859e91690b878b05c6eaad1a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:00:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:00:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:00:40 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:00:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:00:42 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 01:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:02:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:02:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:02:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ef2a91707578a7aa5e67bde1b1ee25c43d3e2005c3514859d532dabeeba08`  
		Last Modified: Wed, 14 Jul 2021 01:19:08 GMT  
		Size: 1.2 MB (1183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f09bd680e7527c5536e3230907946a5aa58e56eb96ad044ecdea7e8de6f17ae`  
		Last Modified: Wed, 14 Jul 2021 01:19:07 GMT  
		Size: 4.7 MB (4676456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0314c569a7bfdae2ebb0dcb70368ff20da4a4641f48f7eb29871f5616511a011`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60830c62be41d8614c4359151a1187cb0f2341edefe989e8854fdf7da34765b`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cb8d0e16826782c8658ccc6b607e60dccc7a6671377b04b9ed908e42c5300`  
		Last Modified: Wed, 14 Jul 2021 01:21:18 GMT  
		Size: 157.2 MB (157205836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8c442e11344f7e8c76f4beaff7faf0c960a0067648aa8da2da8fa44fc3ed03`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ad84bf1f4e24e924f529ce7ead29e4210e854a93febf4725a03662d978f7e696
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205009469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3319402086a4cde3f31db9a1423410b471c080d950246db7c92a388ba819ef5f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:31:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 00:32:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:32:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:32:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c16bac23518e4abf60d1c392e081256894df83fb7cddae089cfaf7131e2101`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db12b2dd1b010b5d533dcf3aafc411ceaf8c995dc98159511b4cb32f94c27c8`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f940dbd5b4415e8d2641c3154a2ae919cdc2b9fde7c70677e48453e3f349b29`  
		Last Modified: Wed, 14 Jul 2021 00:51:46 GMT  
		Size: 171.1 MB (171141545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59698e949a60aa162ddd3ef9bf411fcd75f8055472fe660a8191034d8525c5`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:58425c1b41f2292db91065236cf60785a1f6e30049292e966ba14b9590d9e48c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:2a59ea0be0266569aad467e34390165f4dbc36f566e43091cc9f25e27922c685
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.5 MB (232540777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd67dccbdfe5d95843c4ad1553f2b21d19d3b59ac1a56e359223af4d7edadae2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:26:09 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 02:26:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:26:51 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:27:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:27:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:27:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:27:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591dc9793842ffc9a42cf5ec22fb4989ae835edf2bdbb8149cedfcce0d6a1b5f`  
		Last Modified: Wed, 14 Jul 2021 02:39:14 GMT  
		Size: 104.0 MB (104041692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3ddb7d6e9c3ed48fa4a97e3f0d14587fd3fe8d6dfb6cda319a563a033d14a1`  
		Last Modified: Wed, 14 Jul 2021 02:38:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e18c965f24291e45d1a63af72591fe112b32ca55c67d28e01d9028ed2ee633c`  
		Last Modified: Wed, 14 Jul 2021 02:39:44 GMT  
		Size: 70.8 MB (70796766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd11c5e8bf5476993b5e5db2880634369156fdc6d4dd54570b76ab74aa0de09a`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 238.6 KB (238614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4578383d135282389ec968781336ef5339ceeaeb77fedad4244339447a262e`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585de5ef0121eab1bca194101deba13a59c5dd66731a7988ef18cff8066ab4ca`  
		Last Modified: Wed, 14 Jul 2021 02:39:33 GMT  
		Size: 22.2 MB (22164073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7643d34396ecaeaa9bf95bb0ba0d2b86c90b5909d9db960a1495d903e2709090
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.2 MB (221190595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c67d571630c4ed995384a018dc5a1c905b439fefd28ed0b010420b52d6e63d3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:42:24 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 00:43:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:43:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:43:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:43:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:43:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:44:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6302a5a127c89f8f76e78480594108a0d7d06b60a89b4975526ee82304c333`  
		Last Modified: Wed, 14 Jul 2021 00:58:27 GMT  
		Size: 100.4 MB (100442443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed4eb300f9d62b4200883336a06c4e4a8c4d890096139e40a7433f0eb19c1b`  
		Last Modified: Wed, 14 Jul 2021 00:58:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402bfc647e1fd1ab9a4847f84273249517aaf1a4a26e8d4f53875340bffe0261`  
		Last Modified: Wed, 14 Jul 2021 00:58:51 GMT  
		Size: 65.1 MB (65137606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a24ecc4e22c8d052eab52f50488f5f3332fa2d2aac910ac6eaeb03ad3ff169`  
		Last Modified: Wed, 14 Jul 2021 00:58:40 GMT  
		Size: 238.6 KB (238602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d4894c659864a52419078687aa61e414bf7cf3621963bf4fa0b9f72c0665bc`  
		Last Modified: Wed, 14 Jul 2021 00:58:39 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518623f7b6c1c97adb1004f148e808e506f9dd89c4d4e14a08e22f66e18aaf1`  
		Last Modified: Wed, 14 Jul 2021 00:58:44 GMT  
		Size: 21.5 MB (21501974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:58425c1b41f2292db91065236cf60785a1f6e30049292e966ba14b9590d9e48c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:2a59ea0be0266569aad467e34390165f4dbc36f566e43091cc9f25e27922c685
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.5 MB (232540777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd67dccbdfe5d95843c4ad1553f2b21d19d3b59ac1a56e359223af4d7edadae2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:26:09 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 02:26:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:26:51 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:27:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:27:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:27:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:27:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591dc9793842ffc9a42cf5ec22fb4989ae835edf2bdbb8149cedfcce0d6a1b5f`  
		Last Modified: Wed, 14 Jul 2021 02:39:14 GMT  
		Size: 104.0 MB (104041692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3ddb7d6e9c3ed48fa4a97e3f0d14587fd3fe8d6dfb6cda319a563a033d14a1`  
		Last Modified: Wed, 14 Jul 2021 02:38:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e18c965f24291e45d1a63af72591fe112b32ca55c67d28e01d9028ed2ee633c`  
		Last Modified: Wed, 14 Jul 2021 02:39:44 GMT  
		Size: 70.8 MB (70796766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd11c5e8bf5476993b5e5db2880634369156fdc6d4dd54570b76ab74aa0de09a`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 238.6 KB (238614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4578383d135282389ec968781336ef5339ceeaeb77fedad4244339447a262e`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585de5ef0121eab1bca194101deba13a59c5dd66731a7988ef18cff8066ab4ca`  
		Last Modified: Wed, 14 Jul 2021 02:39:33 GMT  
		Size: 22.2 MB (22164073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7643d34396ecaeaa9bf95bb0ba0d2b86c90b5909d9db960a1495d903e2709090
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.2 MB (221190595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c67d571630c4ed995384a018dc5a1c905b439fefd28ed0b010420b52d6e63d3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:42:24 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 00:43:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:43:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:43:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:43:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:43:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:44:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6302a5a127c89f8f76e78480594108a0d7d06b60a89b4975526ee82304c333`  
		Last Modified: Wed, 14 Jul 2021 00:58:27 GMT  
		Size: 100.4 MB (100442443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed4eb300f9d62b4200883336a06c4e4a8c4d890096139e40a7433f0eb19c1b`  
		Last Modified: Wed, 14 Jul 2021 00:58:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402bfc647e1fd1ab9a4847f84273249517aaf1a4a26e8d4f53875340bffe0261`  
		Last Modified: Wed, 14 Jul 2021 00:58:51 GMT  
		Size: 65.1 MB (65137606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a24ecc4e22c8d052eab52f50488f5f3332fa2d2aac910ac6eaeb03ad3ff169`  
		Last Modified: Wed, 14 Jul 2021 00:58:40 GMT  
		Size: 238.6 KB (238602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d4894c659864a52419078687aa61e414bf7cf3621963bf4fa0b9f72c0665bc`  
		Last Modified: Wed, 14 Jul 2021 00:58:39 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518623f7b6c1c97adb1004f148e808e506f9dd89c4d4e14a08e22f66e18aaf1`  
		Last Modified: Wed, 14 Jul 2021 00:58:44 GMT  
		Size: 21.5 MB (21501974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-focal`

```console
$ docker pull ros@sha256:58425c1b41f2292db91065236cf60785a1f6e30049292e966ba14b9590d9e48c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:2a59ea0be0266569aad467e34390165f4dbc36f566e43091cc9f25e27922c685
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.5 MB (232540777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd67dccbdfe5d95843c4ad1553f2b21d19d3b59ac1a56e359223af4d7edadae2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:26:09 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 02:26:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:26:51 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:27:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:27:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:27:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:27:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591dc9793842ffc9a42cf5ec22fb4989ae835edf2bdbb8149cedfcce0d6a1b5f`  
		Last Modified: Wed, 14 Jul 2021 02:39:14 GMT  
		Size: 104.0 MB (104041692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3ddb7d6e9c3ed48fa4a97e3f0d14587fd3fe8d6dfb6cda319a563a033d14a1`  
		Last Modified: Wed, 14 Jul 2021 02:38:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e18c965f24291e45d1a63af72591fe112b32ca55c67d28e01d9028ed2ee633c`  
		Last Modified: Wed, 14 Jul 2021 02:39:44 GMT  
		Size: 70.8 MB (70796766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd11c5e8bf5476993b5e5db2880634369156fdc6d4dd54570b76ab74aa0de09a`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 238.6 KB (238614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4578383d135282389ec968781336ef5339ceeaeb77fedad4244339447a262e`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585de5ef0121eab1bca194101deba13a59c5dd66731a7988ef18cff8066ab4ca`  
		Last Modified: Wed, 14 Jul 2021 02:39:33 GMT  
		Size: 22.2 MB (22164073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7643d34396ecaeaa9bf95bb0ba0d2b86c90b5909d9db960a1495d903e2709090
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.2 MB (221190595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c67d571630c4ed995384a018dc5a1c905b439fefd28ed0b010420b52d6e63d3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:42:24 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 00:43:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:43:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:43:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:43:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:43:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:44:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6302a5a127c89f8f76e78480594108a0d7d06b60a89b4975526ee82304c333`  
		Last Modified: Wed, 14 Jul 2021 00:58:27 GMT  
		Size: 100.4 MB (100442443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed4eb300f9d62b4200883336a06c4e4a8c4d890096139e40a7433f0eb19c1b`  
		Last Modified: Wed, 14 Jul 2021 00:58:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402bfc647e1fd1ab9a4847f84273249517aaf1a4a26e8d4f53875340bffe0261`  
		Last Modified: Wed, 14 Jul 2021 00:58:51 GMT  
		Size: 65.1 MB (65137606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a24ecc4e22c8d052eab52f50488f5f3332fa2d2aac910ac6eaeb03ad3ff169`  
		Last Modified: Wed, 14 Jul 2021 00:58:40 GMT  
		Size: 238.6 KB (238602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d4894c659864a52419078687aa61e414bf7cf3621963bf4fa0b9f72c0665bc`  
		Last Modified: Wed, 14 Jul 2021 00:58:39 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518623f7b6c1c97adb1004f148e808e506f9dd89c4d4e14a08e22f66e18aaf1`  
		Last Modified: Wed, 14 Jul 2021 00:58:44 GMT  
		Size: 21.5 MB (21501974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:f0c7c935efbd93d3e72608306bb03154426cfc5e2dce4c07564c0ad3c19ddc14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:8dada15f6d14b5e0d4f02926d6919ff011c3e1cb2ebc709b876e14d57c2702b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139339284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e0516d53f61be13d8d8911826bb7f419313284d1c9daedc3a3427153dd53309`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:26:09 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 02:26:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:26:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591dc9793842ffc9a42cf5ec22fb4989ae835edf2bdbb8149cedfcce0d6a1b5f`  
		Last Modified: Wed, 14 Jul 2021 02:39:14 GMT  
		Size: 104.0 MB (104041692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3ddb7d6e9c3ed48fa4a97e3f0d14587fd3fe8d6dfb6cda319a563a033d14a1`  
		Last Modified: Wed, 14 Jul 2021 02:38:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3cb472c196c23bf6368689c9384da05236970737c8a602a96a485b2be50eae3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134310371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9ff02d56352ada016070d9a30054e928d52109b8441ba69fb62fb646d2687f9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:42:24 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 00:43:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:43:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:43:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6302a5a127c89f8f76e78480594108a0d7d06b60a89b4975526ee82304c333`  
		Last Modified: Wed, 14 Jul 2021 00:58:27 GMT  
		Size: 100.4 MB (100442443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed4eb300f9d62b4200883336a06c4e4a8c4d890096139e40a7433f0eb19c1b`  
		Last Modified: Wed, 14 Jul 2021 00:58:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-focal`

```console
$ docker pull ros@sha256:f0c7c935efbd93d3e72608306bb03154426cfc5e2dce4c07564c0ad3c19ddc14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:8dada15f6d14b5e0d4f02926d6919ff011c3e1cb2ebc709b876e14d57c2702b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139339284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e0516d53f61be13d8d8911826bb7f419313284d1c9daedc3a3427153dd53309`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:26:09 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 02:26:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:26:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591dc9793842ffc9a42cf5ec22fb4989ae835edf2bdbb8149cedfcce0d6a1b5f`  
		Last Modified: Wed, 14 Jul 2021 02:39:14 GMT  
		Size: 104.0 MB (104041692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3ddb7d6e9c3ed48fa4a97e3f0d14587fd3fe8d6dfb6cda319a563a033d14a1`  
		Last Modified: Wed, 14 Jul 2021 02:38:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3cb472c196c23bf6368689c9384da05236970737c8a602a96a485b2be50eae3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134310371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9ff02d56352ada016070d9a30054e928d52109b8441ba69fb62fb646d2687f9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:42:24 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 00:43:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:43:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:43:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6302a5a127c89f8f76e78480594108a0d7d06b60a89b4975526ee82304c333`  
		Last Modified: Wed, 14 Jul 2021 00:58:27 GMT  
		Size: 100.4 MB (100442443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed4eb300f9d62b4200883336a06c4e4a8c4d890096139e40a7433f0eb19c1b`  
		Last Modified: Wed, 14 Jul 2021 00:58:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge`

```console
$ docker pull ros@sha256:a73660a19c505bac69598046e111fac3f1f3e894b0c71209e3c4deadaf5145a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:33b2f9b3e471b0ea56c31408b4b1c95caa53eb50bacf104a1d3e3bd3a983caa2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.1 MB (326070148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3afcb5e3b74687cc7db1964d5017088653d2732b251405a7dfcc8f3ade7e092c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:26:09 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 02:26:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:26:51 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:27:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:27:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:27:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:27:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:27:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:27:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:27:53 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 02:27:53 GMT
ENV ROS2_DISTRO=rolling
# Wed, 14 Jul 2021 02:28:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:28:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.15.0-1*     ros-rolling-demo-nodes-py=0.15.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:28:28 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591dc9793842ffc9a42cf5ec22fb4989ae835edf2bdbb8149cedfcce0d6a1b5f`  
		Last Modified: Wed, 14 Jul 2021 02:39:14 GMT  
		Size: 104.0 MB (104041692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3ddb7d6e9c3ed48fa4a97e3f0d14587fd3fe8d6dfb6cda319a563a033d14a1`  
		Last Modified: Wed, 14 Jul 2021 02:38:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e18c965f24291e45d1a63af72591fe112b32ca55c67d28e01d9028ed2ee633c`  
		Last Modified: Wed, 14 Jul 2021 02:39:44 GMT  
		Size: 70.8 MB (70796766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd11c5e8bf5476993b5e5db2880634369156fdc6d4dd54570b76ab74aa0de09a`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 238.6 KB (238614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4578383d135282389ec968781336ef5339ceeaeb77fedad4244339447a262e`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585de5ef0121eab1bca194101deba13a59c5dd66731a7988ef18cff8066ab4ca`  
		Last Modified: Wed, 14 Jul 2021 02:39:33 GMT  
		Size: 22.2 MB (22164073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ca207bc28bc4a2702953d1346b80bf440a07b92c7e49fd2f6e39e7a929194a`  
		Last Modified: Wed, 14 Jul 2021 02:40:00 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e93a1a7456f0f6e1e2c23a0cc99414af06de1c6618c7a64d0786ca956619447`  
		Last Modified: Wed, 14 Jul 2021 02:40:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c356e4605f910a3bc60492169b3be00ba438f35a692b4c6b57ec30dc2cb0a8a`  
		Last Modified: Wed, 14 Jul 2021 02:40:26 GMT  
		Size: 78.4 MB (78410524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3f154ee1eb8d4cc86d088eb732212fc9fb8f136d404fe347b1e9b3c54f85b1`  
		Last Modified: Wed, 14 Jul 2021 02:40:05 GMT  
		Size: 15.1 MB (15118220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8779ce298b1686d380aba75c2298fa0e5198c2cbbdd04e531676a6d2de8bbcaf`  
		Last Modified: Wed, 14 Jul 2021 02:40:00 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:786ff3e5163b3bb01033afe89c5e0aed3bd53ad0f8057656ea7d0bc26c39119d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.2 MB (314248897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:083b1429a71d23c5a8a6e3942eaae79dd8ac26c42a6a39afbdccd0613b5ae3ea`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:42:24 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 00:43:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:43:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:43:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:43:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:43:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:44:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:44:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:44:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:44:35 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 00:44:36 GMT
ENV ROS2_DISTRO=rolling
# Wed, 14 Jul 2021 00:45:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.15.0-1*     ros-rolling-demo-nodes-py=0.15.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:45:16 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6302a5a127c89f8f76e78480594108a0d7d06b60a89b4975526ee82304c333`  
		Last Modified: Wed, 14 Jul 2021 00:58:27 GMT  
		Size: 100.4 MB (100442443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed4eb300f9d62b4200883336a06c4e4a8c4d890096139e40a7433f0eb19c1b`  
		Last Modified: Wed, 14 Jul 2021 00:58:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402bfc647e1fd1ab9a4847f84273249517aaf1a4a26e8d4f53875340bffe0261`  
		Last Modified: Wed, 14 Jul 2021 00:58:51 GMT  
		Size: 65.1 MB (65137606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a24ecc4e22c8d052eab52f50488f5f3332fa2d2aac910ac6eaeb03ad3ff169`  
		Last Modified: Wed, 14 Jul 2021 00:58:40 GMT  
		Size: 238.6 KB (238602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d4894c659864a52419078687aa61e414bf7cf3621963bf4fa0b9f72c0665bc`  
		Last Modified: Wed, 14 Jul 2021 00:58:39 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518623f7b6c1c97adb1004f148e808e506f9dd89c4d4e14a08e22f66e18aaf1`  
		Last Modified: Wed, 14 Jul 2021 00:58:44 GMT  
		Size: 21.5 MB (21501974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c17da46a946095cb6849fcf8f00b1e3835bb882210a10dc68dea9d6a3ca18`  
		Last Modified: Wed, 14 Jul 2021 00:59:08 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7528e2fb4b27c1a655e92955236db88c2ec0559c097a69f9913d73c316744dc9`  
		Last Modified: Wed, 14 Jul 2021 00:59:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246b6d215f41693fe4ca808d52845fb47fcb6767e4a7ca5725711201e139e70e`  
		Last Modified: Wed, 14 Jul 2021 00:59:30 GMT  
		Size: 78.4 MB (78368573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d34b6430634cc1c8675eac653879df8852fe7b420161817670430f406f878b6`  
		Last Modified: Wed, 14 Jul 2021 00:59:12 GMT  
		Size: 14.7 MB (14689100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea34dba74831a1eec880bed8016892b3f9b0c33aa941aec0d28f1b53acaebc4`  
		Last Modified: Wed, 14 Jul 2021 00:59:08 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:a73660a19c505bac69598046e111fac3f1f3e894b0c71209e3c4deadaf5145a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:33b2f9b3e471b0ea56c31408b4b1c95caa53eb50bacf104a1d3e3bd3a983caa2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.1 MB (326070148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3afcb5e3b74687cc7db1964d5017088653d2732b251405a7dfcc8f3ade7e092c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:20:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 02:20:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:20:57 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:26:09 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 02:26:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:26:51 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 02:26:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:26:51 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:27:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:27:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:27:25 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 02:27:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:27:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:27:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:27:53 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 02:27:53 GMT
ENV ROS2_DISTRO=rolling
# Wed, 14 Jul 2021 02:28:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:28:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.15.0-1*     ros-rolling-demo-nodes-py=0.15.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:28:28 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d676980256dd20ca6ed635363f49c12e88be724caee04c13498ed0ecd3c3f47`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01449172621b1fa36d313c8e5b24657ab3f888a603e03af6bfc6559474a64855`  
		Last Modified: Wed, 14 Jul 2021 02:35:31 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591dc9793842ffc9a42cf5ec22fb4989ae835edf2bdbb8149cedfcce0d6a1b5f`  
		Last Modified: Wed, 14 Jul 2021 02:39:14 GMT  
		Size: 104.0 MB (104041692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3ddb7d6e9c3ed48fa4a97e3f0d14587fd3fe8d6dfb6cda319a563a033d14a1`  
		Last Modified: Wed, 14 Jul 2021 02:38:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e18c965f24291e45d1a63af72591fe112b32ca55c67d28e01d9028ed2ee633c`  
		Last Modified: Wed, 14 Jul 2021 02:39:44 GMT  
		Size: 70.8 MB (70796766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd11c5e8bf5476993b5e5db2880634369156fdc6d4dd54570b76ab74aa0de09a`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 238.6 KB (238614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4578383d135282389ec968781336ef5339ceeaeb77fedad4244339447a262e`  
		Last Modified: Wed, 14 Jul 2021 02:39:26 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585de5ef0121eab1bca194101deba13a59c5dd66731a7988ef18cff8066ab4ca`  
		Last Modified: Wed, 14 Jul 2021 02:39:33 GMT  
		Size: 22.2 MB (22164073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ca207bc28bc4a2702953d1346b80bf440a07b92c7e49fd2f6e39e7a929194a`  
		Last Modified: Wed, 14 Jul 2021 02:40:00 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e93a1a7456f0f6e1e2c23a0cc99414af06de1c6618c7a64d0786ca956619447`  
		Last Modified: Wed, 14 Jul 2021 02:40:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c356e4605f910a3bc60492169b3be00ba438f35a692b4c6b57ec30dc2cb0a8a`  
		Last Modified: Wed, 14 Jul 2021 02:40:26 GMT  
		Size: 78.4 MB (78410524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3f154ee1eb8d4cc86d088eb732212fc9fb8f136d404fe347b1e9b3c54f85b1`  
		Last Modified: Wed, 14 Jul 2021 02:40:05 GMT  
		Size: 15.1 MB (15118220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8779ce298b1686d380aba75c2298fa0e5198c2cbbdd04e531676a6d2de8bbcaf`  
		Last Modified: Wed, 14 Jul 2021 02:40:00 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:786ff3e5163b3bb01033afe89c5e0aed3bd53ad0f8057656ea7d0bc26c39119d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.2 MB (314248897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:083b1429a71d23c5a8a6e3942eaae79dd8ac26c42a6a39afbdccd0613b5ae3ea`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:36:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 14 Jul 2021 00:36:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:36:22 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:42:24 GMT
ENV ROS_DISTRO=rolling
# Wed, 14 Jul 2021 00:43:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 14 Jul 2021 00:43:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:43:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:43:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:43:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 14 Jul 2021 00:44:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:44:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:44:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:44:35 GMT
ENV ROS1_DISTRO=noetic
# Wed, 14 Jul 2021 00:44:36 GMT
ENV ROS2_DISTRO=rolling
# Wed, 14 Jul 2021 00:45:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.15.0-1*     ros-rolling-demo-nodes-py=0.15.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:45:16 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d200847aab4cc08dfb33a00c48cc6ff6aeee0645c2697c3d902fe3bab395f`  
		Last Modified: Wed, 14 Jul 2021 00:54:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5373175d6166cd421fd345702c02d89c9e184d55f419779a336b6c3dc49b934c`  
		Last Modified: Wed, 14 Jul 2021 00:54:31 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6302a5a127c89f8f76e78480594108a0d7d06b60a89b4975526ee82304c333`  
		Last Modified: Wed, 14 Jul 2021 00:58:27 GMT  
		Size: 100.4 MB (100442443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed4eb300f9d62b4200883336a06c4e4a8c4d890096139e40a7433f0eb19c1b`  
		Last Modified: Wed, 14 Jul 2021 00:58:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402bfc647e1fd1ab9a4847f84273249517aaf1a4a26e8d4f53875340bffe0261`  
		Last Modified: Wed, 14 Jul 2021 00:58:51 GMT  
		Size: 65.1 MB (65137606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a24ecc4e22c8d052eab52f50488f5f3332fa2d2aac910ac6eaeb03ad3ff169`  
		Last Modified: Wed, 14 Jul 2021 00:58:40 GMT  
		Size: 238.6 KB (238602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d4894c659864a52419078687aa61e414bf7cf3621963bf4fa0b9f72c0665bc`  
		Last Modified: Wed, 14 Jul 2021 00:58:39 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f518623f7b6c1c97adb1004f148e808e506f9dd89c4d4e14a08e22f66e18aaf1`  
		Last Modified: Wed, 14 Jul 2021 00:58:44 GMT  
		Size: 21.5 MB (21501974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c17da46a946095cb6849fcf8f00b1e3835bb882210a10dc68dea9d6a3ca18`  
		Last Modified: Wed, 14 Jul 2021 00:59:08 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7528e2fb4b27c1a655e92955236db88c2ec0559c097a69f9913d73c316744dc9`  
		Last Modified: Wed, 14 Jul 2021 00:59:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246b6d215f41693fe4ca808d52845fb47fcb6767e4a7ca5725711201e139e70e`  
		Last Modified: Wed, 14 Jul 2021 00:59:30 GMT  
		Size: 78.4 MB (78368573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d34b6430634cc1c8675eac653879df8852fe7b420161817670430f406f878b6`  
		Last Modified: Wed, 14 Jul 2021 00:59:12 GMT  
		Size: 14.7 MB (14689100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea34dba74831a1eec880bed8016892b3f9b0c33aa941aec0d28f1b53acaebc4`  
		Last Modified: Wed, 14 Jul 2021 00:59:08 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
