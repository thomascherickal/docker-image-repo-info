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
$ docker pull ros@sha256:ca2804388f4fbefdb4a26839ff52fe065d9a13ea8e9e2607b35790e5f7a9dd6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:a77609596d61673ef5b0712997ca252e169f58afe885f64d09bd4f9aecb1c8db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250946161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31fc1039988517fcee66a388d650df9f7d668cdae592b4a3baeffd5fae89fc7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:40:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:40:54 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 07:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:41:51 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:41:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:41:51 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:42:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:42:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:42:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:42:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0027cc618944892ad1b86538d6217fe6fd67802a203835f21e23b9092c7803e`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dfaab9c9705644ca3f79857ab252921550c6a180e296e7b92b6a977ac6d474`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceb646c34ee3d4ee7f4fd7180dc9e6e3c92623e1604211cce753f1dbe7d3adb`  
		Last Modified: Thu, 02 Mar 2023 08:06:26 GMT  
		Size: 120.4 MB (120372660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf7e1f206c0b544fde7fa6dfaadb2b5693a54add75c9796cb61bc298d020b41`  
		Last Modified: Thu, 02 Mar 2023 08:06:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1742aee23639ba227fee287e7ee707bb4e0b5722782641f35fb848535e224bdf`  
		Last Modified: Thu, 02 Mar 2023 08:06:45 GMT  
		Size: 73.3 MB (73340778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ff9b438a1df4250cc0e74a1bfadbeeb8cd5cd6caf37b5c574332d0ef6166b0`  
		Last Modified: Thu, 02 Mar 2023 08:06:35 GMT  
		Size: 279.2 KB (279215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4eccc0b2110a03254d4a7f7b8738f09cf3b5a8ce912a7708357240deece496`  
		Last Modified: Thu, 02 Mar 2023 08:06:35 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51fbf933cbf116bd938a654be9c565b3aa20bb2242a9021fa2559e3cf0339ee`  
		Last Modified: Thu, 02 Mar 2023 08:06:38 GMT  
		Size: 21.7 MB (21662384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:934c9283e3d48098dadf95c77a79a88ea4c5e9a0f271bede8e7fc154b93f9e97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226802496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797fdf269cafa9a646733093d1d3d343908984b5908fe293f93ad246f522f787`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:36 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:43:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 03:44:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:44:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:44:31 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:44:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:45:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1659f1c90f60434c50265969a97cd41a22913c2037483ff3bd9792717987`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a73223e5ee62173a4b294378545321fee65e69698550366cccd744cdda7fa2`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd7e465b25c7c0b51fa71a0769a0d8ee12c963a8760da60297aaaf481d33d8`  
		Last Modified: Thu, 02 Mar 2023 04:09:07 GMT  
		Size: 104.6 MB (104569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bd83378013cccd76320c75fb5937199f996eb144292044c9dfcb1419089d8d`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0208396681856b3ee322e06ae0454a98f416931c3b6e27c348fe4923edeefefd`  
		Last Modified: Thu, 02 Mar 2023 04:09:23 GMT  
		Size: 67.7 MB (67683638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd600f7c98c5fbacb990bfb6221305e0b939a4a8850b0681d70ce3b97870e8e`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 279.2 KB (279217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea21264705160c5780c3c14d6050afbc00c6b2de0b190944cbe9c6bad84ec3a`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 2.4 KB (2413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f1e1e57ea67c116aa79df7407e788e1060cedbd46bd14461fa7c06a434bd2b`  
		Last Modified: Thu, 02 Mar 2023 04:09:18 GMT  
		Size: 20.4 MB (20384821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:ca2804388f4fbefdb4a26839ff52fe065d9a13ea8e9e2607b35790e5f7a9dd6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:a77609596d61673ef5b0712997ca252e169f58afe885f64d09bd4f9aecb1c8db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250946161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31fc1039988517fcee66a388d650df9f7d668cdae592b4a3baeffd5fae89fc7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:40:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:40:54 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 07:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:41:51 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:41:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:41:51 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:42:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:42:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:42:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:42:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0027cc618944892ad1b86538d6217fe6fd67802a203835f21e23b9092c7803e`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dfaab9c9705644ca3f79857ab252921550c6a180e296e7b92b6a977ac6d474`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceb646c34ee3d4ee7f4fd7180dc9e6e3c92623e1604211cce753f1dbe7d3adb`  
		Last Modified: Thu, 02 Mar 2023 08:06:26 GMT  
		Size: 120.4 MB (120372660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf7e1f206c0b544fde7fa6dfaadb2b5693a54add75c9796cb61bc298d020b41`  
		Last Modified: Thu, 02 Mar 2023 08:06:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1742aee23639ba227fee287e7ee707bb4e0b5722782641f35fb848535e224bdf`  
		Last Modified: Thu, 02 Mar 2023 08:06:45 GMT  
		Size: 73.3 MB (73340778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ff9b438a1df4250cc0e74a1bfadbeeb8cd5cd6caf37b5c574332d0ef6166b0`  
		Last Modified: Thu, 02 Mar 2023 08:06:35 GMT  
		Size: 279.2 KB (279215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4eccc0b2110a03254d4a7f7b8738f09cf3b5a8ce912a7708357240deece496`  
		Last Modified: Thu, 02 Mar 2023 08:06:35 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51fbf933cbf116bd938a654be9c565b3aa20bb2242a9021fa2559e3cf0339ee`  
		Last Modified: Thu, 02 Mar 2023 08:06:38 GMT  
		Size: 21.7 MB (21662384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:934c9283e3d48098dadf95c77a79a88ea4c5e9a0f271bede8e7fc154b93f9e97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226802496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797fdf269cafa9a646733093d1d3d343908984b5908fe293f93ad246f522f787`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:36 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:43:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 03:44:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:44:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:44:31 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:44:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:45:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1659f1c90f60434c50265969a97cd41a22913c2037483ff3bd9792717987`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a73223e5ee62173a4b294378545321fee65e69698550366cccd744cdda7fa2`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd7e465b25c7c0b51fa71a0769a0d8ee12c963a8760da60297aaaf481d33d8`  
		Last Modified: Thu, 02 Mar 2023 04:09:07 GMT  
		Size: 104.6 MB (104569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bd83378013cccd76320c75fb5937199f996eb144292044c9dfcb1419089d8d`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0208396681856b3ee322e06ae0454a98f416931c3b6e27c348fe4923edeefefd`  
		Last Modified: Thu, 02 Mar 2023 04:09:23 GMT  
		Size: 67.7 MB (67683638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd600f7c98c5fbacb990bfb6221305e0b939a4a8850b0681d70ce3b97870e8e`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 279.2 KB (279217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea21264705160c5780c3c14d6050afbc00c6b2de0b190944cbe9c6bad84ec3a`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 2.4 KB (2413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f1e1e57ea67c116aa79df7407e788e1060cedbd46bd14461fa7c06a434bd2b`  
		Last Modified: Thu, 02 Mar 2023 04:09:18 GMT  
		Size: 20.4 MB (20384821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:ca2804388f4fbefdb4a26839ff52fe065d9a13ea8e9e2607b35790e5f7a9dd6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:a77609596d61673ef5b0712997ca252e169f58afe885f64d09bd4f9aecb1c8db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250946161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31fc1039988517fcee66a388d650df9f7d668cdae592b4a3baeffd5fae89fc7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:40:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:40:54 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 07:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:41:51 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:41:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:41:51 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:42:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:42:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:42:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:42:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0027cc618944892ad1b86538d6217fe6fd67802a203835f21e23b9092c7803e`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dfaab9c9705644ca3f79857ab252921550c6a180e296e7b92b6a977ac6d474`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceb646c34ee3d4ee7f4fd7180dc9e6e3c92623e1604211cce753f1dbe7d3adb`  
		Last Modified: Thu, 02 Mar 2023 08:06:26 GMT  
		Size: 120.4 MB (120372660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf7e1f206c0b544fde7fa6dfaadb2b5693a54add75c9796cb61bc298d020b41`  
		Last Modified: Thu, 02 Mar 2023 08:06:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1742aee23639ba227fee287e7ee707bb4e0b5722782641f35fb848535e224bdf`  
		Last Modified: Thu, 02 Mar 2023 08:06:45 GMT  
		Size: 73.3 MB (73340778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ff9b438a1df4250cc0e74a1bfadbeeb8cd5cd6caf37b5c574332d0ef6166b0`  
		Last Modified: Thu, 02 Mar 2023 08:06:35 GMT  
		Size: 279.2 KB (279215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4eccc0b2110a03254d4a7f7b8738f09cf3b5a8ce912a7708357240deece496`  
		Last Modified: Thu, 02 Mar 2023 08:06:35 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51fbf933cbf116bd938a654be9c565b3aa20bb2242a9021fa2559e3cf0339ee`  
		Last Modified: Thu, 02 Mar 2023 08:06:38 GMT  
		Size: 21.7 MB (21662384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:934c9283e3d48098dadf95c77a79a88ea4c5e9a0f271bede8e7fc154b93f9e97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226802496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797fdf269cafa9a646733093d1d3d343908984b5908fe293f93ad246f522f787`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:36 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:43:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 03:44:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:44:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:44:31 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:44:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:45:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1659f1c90f60434c50265969a97cd41a22913c2037483ff3bd9792717987`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a73223e5ee62173a4b294378545321fee65e69698550366cccd744cdda7fa2`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd7e465b25c7c0b51fa71a0769a0d8ee12c963a8760da60297aaaf481d33d8`  
		Last Modified: Thu, 02 Mar 2023 04:09:07 GMT  
		Size: 104.6 MB (104569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bd83378013cccd76320c75fb5937199f996eb144292044c9dfcb1419089d8d`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0208396681856b3ee322e06ae0454a98f416931c3b6e27c348fe4923edeefefd`  
		Last Modified: Thu, 02 Mar 2023 04:09:23 GMT  
		Size: 67.7 MB (67683638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd600f7c98c5fbacb990bfb6221305e0b939a4a8850b0681d70ce3b97870e8e`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 279.2 KB (279217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea21264705160c5780c3c14d6050afbc00c6b2de0b190944cbe9c6bad84ec3a`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 2.4 KB (2413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f1e1e57ea67c116aa79df7407e788e1060cedbd46bd14461fa7c06a434bd2b`  
		Last Modified: Thu, 02 Mar 2023 04:09:18 GMT  
		Size: 20.4 MB (20384821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:c565a6cfc3fb4c17f46467f635f4e6b14503aaf00f5a134085581ad5b614e7b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:0d155b837971fcc3ec33137d6e77fa50f313457b582e6522c74537e1128166db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155661329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05856e295eb67aa7f69987002ab98c9e9078b92233a00fa6d6ecfb811a2592bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:40:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:40:54 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 07:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:41:51 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:41:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:41:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0027cc618944892ad1b86538d6217fe6fd67802a203835f21e23b9092c7803e`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dfaab9c9705644ca3f79857ab252921550c6a180e296e7b92b6a977ac6d474`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceb646c34ee3d4ee7f4fd7180dc9e6e3c92623e1604211cce753f1dbe7d3adb`  
		Last Modified: Thu, 02 Mar 2023 08:06:26 GMT  
		Size: 120.4 MB (120372660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf7e1f206c0b544fde7fa6dfaadb2b5693a54add75c9796cb61bc298d020b41`  
		Last Modified: Thu, 02 Mar 2023 08:06:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:955bc30eb2c680250bd8228deb1d56f9ab150841bde76c9bec6f82b956b207f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138452407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92204f583031272e939c4449b13fb5cab2c4aad4c3a6242fd34ccdaa8a150b8c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:36 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:43:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 03:44:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:44:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:44:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1659f1c90f60434c50265969a97cd41a22913c2037483ff3bd9792717987`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a73223e5ee62173a4b294378545321fee65e69698550366cccd744cdda7fa2`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd7e465b25c7c0b51fa71a0769a0d8ee12c963a8760da60297aaaf481d33d8`  
		Last Modified: Thu, 02 Mar 2023 04:09:07 GMT  
		Size: 104.6 MB (104569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bd83378013cccd76320c75fb5937199f996eb144292044c9dfcb1419089d8d`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:c565a6cfc3fb4c17f46467f635f4e6b14503aaf00f5a134085581ad5b614e7b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:0d155b837971fcc3ec33137d6e77fa50f313457b582e6522c74537e1128166db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155661329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05856e295eb67aa7f69987002ab98c9e9078b92233a00fa6d6ecfb811a2592bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:40:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:40:54 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 07:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:41:51 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:41:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:41:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0027cc618944892ad1b86538d6217fe6fd67802a203835f21e23b9092c7803e`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dfaab9c9705644ca3f79857ab252921550c6a180e296e7b92b6a977ac6d474`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceb646c34ee3d4ee7f4fd7180dc9e6e3c92623e1604211cce753f1dbe7d3adb`  
		Last Modified: Thu, 02 Mar 2023 08:06:26 GMT  
		Size: 120.4 MB (120372660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf7e1f206c0b544fde7fa6dfaadb2b5693a54add75c9796cb61bc298d020b41`  
		Last Modified: Thu, 02 Mar 2023 08:06:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:955bc30eb2c680250bd8228deb1d56f9ab150841bde76c9bec6f82b956b207f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138452407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92204f583031272e939c4449b13fb5cab2c4aad4c3a6242fd34ccdaa8a150b8c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:36 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:43:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 03:44:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:44:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:44:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1659f1c90f60434c50265969a97cd41a22913c2037483ff3bd9792717987`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a73223e5ee62173a4b294378545321fee65e69698550366cccd744cdda7fa2`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd7e465b25c7c0b51fa71a0769a0d8ee12c963a8760da60297aaaf481d33d8`  
		Last Modified: Thu, 02 Mar 2023 04:09:07 GMT  
		Size: 104.6 MB (104569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bd83378013cccd76320c75fb5937199f996eb144292044c9dfcb1419089d8d`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:70944e35f4079772eb56af0c2a45fa348ff79b23b863c22f3a24818e3c48c2dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:c7b69ca43d8d2d172cbd3f295c59035c83c48b4cb0ecde31da73bf0bb1d45a4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349046072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f015a97a62f6b75c53211592d1d89a0cfcc2cbf061b5094501ff039328d9a77e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:40:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:40:54 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 07:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:41:51 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:41:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:41:51 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:42:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:42:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:42:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:42:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:43:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:43:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:43:01 GMT
ENV ROS1_DISTRO=noetic
# Thu, 02 Mar 2023 07:43:01 GMT
ENV ROS2_DISTRO=foxy
# Thu, 02 Mar 2023 07:43:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:43:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:43:38 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0027cc618944892ad1b86538d6217fe6fd67802a203835f21e23b9092c7803e`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dfaab9c9705644ca3f79857ab252921550c6a180e296e7b92b6a977ac6d474`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceb646c34ee3d4ee7f4fd7180dc9e6e3c92623e1604211cce753f1dbe7d3adb`  
		Last Modified: Thu, 02 Mar 2023 08:06:26 GMT  
		Size: 120.4 MB (120372660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf7e1f206c0b544fde7fa6dfaadb2b5693a54add75c9796cb61bc298d020b41`  
		Last Modified: Thu, 02 Mar 2023 08:06:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1742aee23639ba227fee287e7ee707bb4e0b5722782641f35fb848535e224bdf`  
		Last Modified: Thu, 02 Mar 2023 08:06:45 GMT  
		Size: 73.3 MB (73340778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ff9b438a1df4250cc0e74a1bfadbeeb8cd5cd6caf37b5c574332d0ef6166b0`  
		Last Modified: Thu, 02 Mar 2023 08:06:35 GMT  
		Size: 279.2 KB (279215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4eccc0b2110a03254d4a7f7b8738f09cf3b5a8ce912a7708357240deece496`  
		Last Modified: Thu, 02 Mar 2023 08:06:35 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51fbf933cbf116bd938a654be9c565b3aa20bb2242a9021fa2559e3cf0339ee`  
		Last Modified: Thu, 02 Mar 2023 08:06:38 GMT  
		Size: 21.7 MB (21662384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331a0470f9e7c5d0b905332f9c4072e3b61cd04f36a30e64cc9444fdcd6ce8e9`  
		Last Modified: Thu, 02 Mar 2023 08:06:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe170dcb2ffce6f44324cb8b4d9dcd3bead2dcd3957c19cdf8d1564f0553d6d`  
		Last Modified: Thu, 02 Mar 2023 08:06:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55074ecf6ca2398559430a777604ae1f601fa2f21e10a063a85a9d8e8dc72205`  
		Last Modified: Thu, 02 Mar 2023 08:07:09 GMT  
		Size: 76.4 MB (76425017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0feb856e3881e5ab4ed604e5bca5312112f2583f01bf9ec1eaebcd40cd6a7ee7`  
		Last Modified: Thu, 02 Mar 2023 08:07:00 GMT  
		Size: 21.7 MB (21674267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5f7d6d793f766b61ed78f21a56ebb89136f0cef296bb6be1fd3eb31be025c3`  
		Last Modified: Thu, 02 Mar 2023 08:06:56 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a0b3325105eac515d5465568286afdbf4bb402bc1ee5bc35a01dba6131fd441
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317620039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40fec20d33a0e5320521134c4dd19ad08b2c7c9cafc4779108e04e28f8604277`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:36 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:43:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 03:44:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:44:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:44:31 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:44:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:45:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:45:23 GMT
ENV ROS1_DISTRO=noetic
# Thu, 02 Mar 2023 03:45:23 GMT
ENV ROS2_DISTRO=foxy
# Thu, 02 Mar 2023 03:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:53 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1659f1c90f60434c50265969a97cd41a22913c2037483ff3bd9792717987`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a73223e5ee62173a4b294378545321fee65e69698550366cccd744cdda7fa2`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd7e465b25c7c0b51fa71a0769a0d8ee12c963a8760da60297aaaf481d33d8`  
		Last Modified: Thu, 02 Mar 2023 04:09:07 GMT  
		Size: 104.6 MB (104569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bd83378013cccd76320c75fb5937199f996eb144292044c9dfcb1419089d8d`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0208396681856b3ee322e06ae0454a98f416931c3b6e27c348fe4923edeefefd`  
		Last Modified: Thu, 02 Mar 2023 04:09:23 GMT  
		Size: 67.7 MB (67683638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd600f7c98c5fbacb990bfb6221305e0b939a4a8850b0681d70ce3b97870e8e`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 279.2 KB (279217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea21264705160c5780c3c14d6050afbc00c6b2de0b190944cbe9c6bad84ec3a`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 2.4 KB (2413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f1e1e57ea67c116aa79df7407e788e1060cedbd46bd14461fa7c06a434bd2b`  
		Last Modified: Thu, 02 Mar 2023 04:09:18 GMT  
		Size: 20.4 MB (20384821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57336bd1f5b659fca7d2c15f05835498bece96470d7126cb8c6994cc661da08`  
		Last Modified: Thu, 02 Mar 2023 04:09:35 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d551c2118ed584d3c3117d35f5f86852fb5428cf57422b5cdfaad1a12377f5`  
		Last Modified: Thu, 02 Mar 2023 04:09:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d997e889567155d577278109c067af17322ca8eb3c71a7488070d6a4948495c`  
		Last Modified: Thu, 02 Mar 2023 04:09:47 GMT  
		Size: 76.5 MB (76491880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82b2ada8d839cd2b72c7f974a2d7323f582f2cf836821c1678dacf155bb5ac`  
		Last Modified: Thu, 02 Mar 2023 04:09:38 GMT  
		Size: 14.3 MB (14325041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e355150cb1e9732212022cc89c7a129d8d79a62013c5570671e3a2166ad888`  
		Last Modified: Thu, 02 Mar 2023 04:09:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:70944e35f4079772eb56af0c2a45fa348ff79b23b863c22f3a24818e3c48c2dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:c7b69ca43d8d2d172cbd3f295c59035c83c48b4cb0ecde31da73bf0bb1d45a4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349046072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f015a97a62f6b75c53211592d1d89a0cfcc2cbf061b5094501ff039328d9a77e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:40:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:40:53 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:40:54 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 07:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:41:51 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:41:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:41:51 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:42:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:42:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:42:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:42:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:43:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:43:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:43:01 GMT
ENV ROS1_DISTRO=noetic
# Thu, 02 Mar 2023 07:43:01 GMT
ENV ROS2_DISTRO=foxy
# Thu, 02 Mar 2023 07:43:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:43:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:43:38 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0027cc618944892ad1b86538d6217fe6fd67802a203835f21e23b9092c7803e`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dfaab9c9705644ca3f79857ab252921550c6a180e296e7b92b6a977ac6d474`  
		Last Modified: Thu, 02 Mar 2023 08:06:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceb646c34ee3d4ee7f4fd7180dc9e6e3c92623e1604211cce753f1dbe7d3adb`  
		Last Modified: Thu, 02 Mar 2023 08:06:26 GMT  
		Size: 120.4 MB (120372660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf7e1f206c0b544fde7fa6dfaadb2b5693a54add75c9796cb61bc298d020b41`  
		Last Modified: Thu, 02 Mar 2023 08:06:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1742aee23639ba227fee287e7ee707bb4e0b5722782641f35fb848535e224bdf`  
		Last Modified: Thu, 02 Mar 2023 08:06:45 GMT  
		Size: 73.3 MB (73340778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ff9b438a1df4250cc0e74a1bfadbeeb8cd5cd6caf37b5c574332d0ef6166b0`  
		Last Modified: Thu, 02 Mar 2023 08:06:35 GMT  
		Size: 279.2 KB (279215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4eccc0b2110a03254d4a7f7b8738f09cf3b5a8ce912a7708357240deece496`  
		Last Modified: Thu, 02 Mar 2023 08:06:35 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51fbf933cbf116bd938a654be9c565b3aa20bb2242a9021fa2559e3cf0339ee`  
		Last Modified: Thu, 02 Mar 2023 08:06:38 GMT  
		Size: 21.7 MB (21662384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331a0470f9e7c5d0b905332f9c4072e3b61cd04f36a30e64cc9444fdcd6ce8e9`  
		Last Modified: Thu, 02 Mar 2023 08:06:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe170dcb2ffce6f44324cb8b4d9dcd3bead2dcd3957c19cdf8d1564f0553d6d`  
		Last Modified: Thu, 02 Mar 2023 08:06:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55074ecf6ca2398559430a777604ae1f601fa2f21e10a063a85a9d8e8dc72205`  
		Last Modified: Thu, 02 Mar 2023 08:07:09 GMT  
		Size: 76.4 MB (76425017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0feb856e3881e5ab4ed604e5bca5312112f2583f01bf9ec1eaebcd40cd6a7ee7`  
		Last Modified: Thu, 02 Mar 2023 08:07:00 GMT  
		Size: 21.7 MB (21674267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5f7d6d793f766b61ed78f21a56ebb89136f0cef296bb6be1fd3eb31be025c3`  
		Last Modified: Thu, 02 Mar 2023 08:06:56 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6a0b3325105eac515d5465568286afdbf4bb402bc1ee5bc35a01dba6131fd441
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317620039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40fec20d33a0e5320521134c4dd19ad08b2c7c9cafc4779108e04e28f8604277`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:36 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:43:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 03:44:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:44:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:44:31 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:44:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:45:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:45:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:45:23 GMT
ENV ROS1_DISTRO=noetic
# Thu, 02 Mar 2023 03:45:23 GMT
ENV ROS2_DISTRO=foxy
# Thu, 02 Mar 2023 03:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:45:53 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1659f1c90f60434c50265969a97cd41a22913c2037483ff3bd9792717987`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a73223e5ee62173a4b294378545321fee65e69698550366cccd744cdda7fa2`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd7e465b25c7c0b51fa71a0769a0d8ee12c963a8760da60297aaaf481d33d8`  
		Last Modified: Thu, 02 Mar 2023 04:09:07 GMT  
		Size: 104.6 MB (104569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bd83378013cccd76320c75fb5937199f996eb144292044c9dfcb1419089d8d`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0208396681856b3ee322e06ae0454a98f416931c3b6e27c348fe4923edeefefd`  
		Last Modified: Thu, 02 Mar 2023 04:09:23 GMT  
		Size: 67.7 MB (67683638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd600f7c98c5fbacb990bfb6221305e0b939a4a8850b0681d70ce3b97870e8e`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 279.2 KB (279217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea21264705160c5780c3c14d6050afbc00c6b2de0b190944cbe9c6bad84ec3a`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 2.4 KB (2413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f1e1e57ea67c116aa79df7407e788e1060cedbd46bd14461fa7c06a434bd2b`  
		Last Modified: Thu, 02 Mar 2023 04:09:18 GMT  
		Size: 20.4 MB (20384821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57336bd1f5b659fca7d2c15f05835498bece96470d7126cb8c6994cc661da08`  
		Last Modified: Thu, 02 Mar 2023 04:09:35 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d551c2118ed584d3c3117d35f5f86852fb5428cf57422b5cdfaad1a12377f5`  
		Last Modified: Thu, 02 Mar 2023 04:09:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d997e889567155d577278109c067af17322ca8eb3c71a7488070d6a4948495c`  
		Last Modified: Thu, 02 Mar 2023 04:09:47 GMT  
		Size: 76.5 MB (76491880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82b2ada8d839cd2b72c7f974a2d7323f582f2cf836821c1678dacf155bb5ac`  
		Last Modified: Thu, 02 Mar 2023 04:09:38 GMT  
		Size: 14.3 MB (14325041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e355150cb1e9732212022cc89c7a129d8d79a62013c5570671e3a2166ad888`  
		Last Modified: Thu, 02 Mar 2023 04:09:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble`

```console
$ docker pull ros@sha256:3b0e8f2d2ff998c17b521adf0ae2300669cd29ec48b179771a83a2495be72045
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:b12e8e25576ae0b41400a53968806e1c8a861e35381073b3baef45a83cafb5f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263048436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf3502690f913bb0793628e39a93e479a6310aebbee6e65e9d1cb1598267dd01`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 07:45:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:45:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:45:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:45:52 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:46:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:46:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:46:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:47:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f2be4669bf5e0d981bd25dce9fc1cf7b12acd140fc4c22c8d7775f5f0d8dca`  
		Last Modified: Thu, 02 Mar 2023 08:07:35 GMT  
		Size: 106.3 MB (106343240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216ea0d3b5795e8929e583b997a5548be75d03e2a29c115d9f56a944ed84ef0c`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a2aa4beb52be76c6dcd46fc6d1847a75b9ae29c6ebcedc86c9d7f47e4b7165`  
		Last Modified: Thu, 02 Mar 2023 08:07:57 GMT  
		Size: 97.9 MB (97887836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680641f18bb2dd24d14e77d0c3c76ee534de308a8b9d4bd0e587ef1e7b1eb7f8`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 313.2 KB (313170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bef39aad161da9cfed034f35d026bd853ef6023d95711bfc15adb24433f0727`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb484450c9c02df2f1231534b50c85b959723c443ff405fa836795d75227868e`  
		Last Modified: Thu, 02 Mar 2023 08:07:47 GMT  
		Size: 23.1 MB (23071319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c2d497729f6aee71e99bcdd9e454ad5eb1dd3468ae4d4effbf6d4f0ba96c689f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255709503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af910ab58e75966664e169632c6f9accf125c72c2c695d2fa000e4570f4eb25c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 03:48:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:48:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:48:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:48:35 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:49:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:49:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:49:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:50:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13cc6d4ba7a8ad400f19bd92e8cb2286caeca1d46ce132719b2b1987256c21f`  
		Last Modified: Thu, 02 Mar 2023 04:10:13 GMT  
		Size: 104.1 MB (104057998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396dec5942a2fa6aff8e013fe4ebdcfabe51979982de742c3c3a1f04b10a63d5`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617a68eb8bb8b1ab93ca9de116c7d22adcb04072699fcb1ad23a5f18e1ac0305`  
		Last Modified: Thu, 02 Mar 2023 04:10:33 GMT  
		Size: 95.5 MB (95477602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aea5ab66a030d09edeb6bd52a5d2d8c7ee9d2f179e47f3769d797ea1cec2eaa`  
		Last Modified: Thu, 02 Mar 2023 04:10:23 GMT  
		Size: 313.2 KB (313171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83267e4907f639f28f19da252316e35ac2d9754f0b1c072254ccbbae8c95aea2`  
		Last Modified: Thu, 02 Mar 2023 04:10:22 GMT  
		Size: 2.4 KB (2403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b408f45a9652713b3956f2c893ddb6bf2c327cde2e347d0ccd449062384917`  
		Last Modified: Thu, 02 Mar 2023 04:10:26 GMT  
		Size: 22.5 MB (22497086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception`

```console
$ docker pull ros@sha256:ead61725ee89c33ed7e0996e53be4aee71ce8ac66e7c81ae8b4ecb11050db31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception` - linux; amd64

```console
$ docker pull ros@sha256:93cab6530351292e9491bcce9971077bb900cac2cd4b819e24efb4f499b78e36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1092096613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:929c5deab8e5bc0b45fdab8b88eba427d306aa3d2ed44d56c5eabcb57a9c8e86`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 07:45:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:45:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:45:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:45:52 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:46:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:46:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:46:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:47:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:55:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f2be4669bf5e0d981bd25dce9fc1cf7b12acd140fc4c22c8d7775f5f0d8dca`  
		Last Modified: Thu, 02 Mar 2023 08:07:35 GMT  
		Size: 106.3 MB (106343240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216ea0d3b5795e8929e583b997a5548be75d03e2a29c115d9f56a944ed84ef0c`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a2aa4beb52be76c6dcd46fc6d1847a75b9ae29c6ebcedc86c9d7f47e4b7165`  
		Last Modified: Thu, 02 Mar 2023 08:07:57 GMT  
		Size: 97.9 MB (97887836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680641f18bb2dd24d14e77d0c3c76ee534de308a8b9d4bd0e587ef1e7b1eb7f8`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 313.2 KB (313170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bef39aad161da9cfed034f35d026bd853ef6023d95711bfc15adb24433f0727`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb484450c9c02df2f1231534b50c85b959723c443ff405fa836795d75227868e`  
		Last Modified: Thu, 02 Mar 2023 08:07:47 GMT  
		Size: 23.1 MB (23071319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc404e49e56c36e9670cbdd387127b0a1fbd8fe39be0fb1d4083903bd346999`  
		Last Modified: Thu, 02 Mar 2023 08:09:42 GMT  
		Size: 829.0 MB (829048177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c8bab57a8f2c50eb07bffdfac36b588b2e1a41478bd1d280e49278e65af6c13b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1043601969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db03ca1342359fa204959a5f325ab0e7e86fefd577d18ae2df2210d11326200`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 03:48:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:48:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:48:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:48:35 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:49:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:49:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:49:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:50:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:00:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13cc6d4ba7a8ad400f19bd92e8cb2286caeca1d46ce132719b2b1987256c21f`  
		Last Modified: Thu, 02 Mar 2023 04:10:13 GMT  
		Size: 104.1 MB (104057998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396dec5942a2fa6aff8e013fe4ebdcfabe51979982de742c3c3a1f04b10a63d5`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617a68eb8bb8b1ab93ca9de116c7d22adcb04072699fcb1ad23a5f18e1ac0305`  
		Last Modified: Thu, 02 Mar 2023 04:10:33 GMT  
		Size: 95.5 MB (95477602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aea5ab66a030d09edeb6bd52a5d2d8c7ee9d2f179e47f3769d797ea1cec2eaa`  
		Last Modified: Thu, 02 Mar 2023 04:10:23 GMT  
		Size: 313.2 KB (313171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83267e4907f639f28f19da252316e35ac2d9754f0b1c072254ccbbae8c95aea2`  
		Last Modified: Thu, 02 Mar 2023 04:10:22 GMT  
		Size: 2.4 KB (2403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b408f45a9652713b3956f2c893ddb6bf2c327cde2e347d0ccd449062384917`  
		Last Modified: Thu, 02 Mar 2023 04:10:26 GMT  
		Size: 22.5 MB (22497086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d341d48b444deadedb8e2239abd96f5742dca7e6193142b50410f887680e8e`  
		Last Modified: Thu, 02 Mar 2023 04:12:04 GMT  
		Size: 787.9 MB (787892466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-perception-jammy`

```console
$ docker pull ros@sha256:ead61725ee89c33ed7e0996e53be4aee71ce8ac66e7c81ae8b4ecb11050db31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:93cab6530351292e9491bcce9971077bb900cac2cd4b819e24efb4f499b78e36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1092096613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:929c5deab8e5bc0b45fdab8b88eba427d306aa3d2ed44d56c5eabcb57a9c8e86`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 07:45:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:45:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:45:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:45:52 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:46:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:46:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:46:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:47:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:55:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f2be4669bf5e0d981bd25dce9fc1cf7b12acd140fc4c22c8d7775f5f0d8dca`  
		Last Modified: Thu, 02 Mar 2023 08:07:35 GMT  
		Size: 106.3 MB (106343240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216ea0d3b5795e8929e583b997a5548be75d03e2a29c115d9f56a944ed84ef0c`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a2aa4beb52be76c6dcd46fc6d1847a75b9ae29c6ebcedc86c9d7f47e4b7165`  
		Last Modified: Thu, 02 Mar 2023 08:07:57 GMT  
		Size: 97.9 MB (97887836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680641f18bb2dd24d14e77d0c3c76ee534de308a8b9d4bd0e587ef1e7b1eb7f8`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 313.2 KB (313170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bef39aad161da9cfed034f35d026bd853ef6023d95711bfc15adb24433f0727`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb484450c9c02df2f1231534b50c85b959723c443ff405fa836795d75227868e`  
		Last Modified: Thu, 02 Mar 2023 08:07:47 GMT  
		Size: 23.1 MB (23071319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc404e49e56c36e9670cbdd387127b0a1fbd8fe39be0fb1d4083903bd346999`  
		Last Modified: Thu, 02 Mar 2023 08:09:42 GMT  
		Size: 829.0 MB (829048177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c8bab57a8f2c50eb07bffdfac36b588b2e1a41478bd1d280e49278e65af6c13b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1043601969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db03ca1342359fa204959a5f325ab0e7e86fefd577d18ae2df2210d11326200`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 03:48:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:48:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:48:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:48:35 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:49:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:49:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:49:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:50:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:00:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13cc6d4ba7a8ad400f19bd92e8cb2286caeca1d46ce132719b2b1987256c21f`  
		Last Modified: Thu, 02 Mar 2023 04:10:13 GMT  
		Size: 104.1 MB (104057998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396dec5942a2fa6aff8e013fe4ebdcfabe51979982de742c3c3a1f04b10a63d5`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617a68eb8bb8b1ab93ca9de116c7d22adcb04072699fcb1ad23a5f18e1ac0305`  
		Last Modified: Thu, 02 Mar 2023 04:10:33 GMT  
		Size: 95.5 MB (95477602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aea5ab66a030d09edeb6bd52a5d2d8c7ee9d2f179e47f3769d797ea1cec2eaa`  
		Last Modified: Thu, 02 Mar 2023 04:10:23 GMT  
		Size: 313.2 KB (313171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83267e4907f639f28f19da252316e35ac2d9754f0b1c072254ccbbae8c95aea2`  
		Last Modified: Thu, 02 Mar 2023 04:10:22 GMT  
		Size: 2.4 KB (2403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b408f45a9652713b3956f2c893ddb6bf2c327cde2e347d0ccd449062384917`  
		Last Modified: Thu, 02 Mar 2023 04:10:26 GMT  
		Size: 22.5 MB (22497086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d341d48b444deadedb8e2239abd96f5742dca7e6193142b50410f887680e8e`  
		Last Modified: Thu, 02 Mar 2023 04:12:04 GMT  
		Size: 787.9 MB (787892466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base`

```console
$ docker pull ros@sha256:3b0e8f2d2ff998c17b521adf0ae2300669cd29ec48b179771a83a2495be72045
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:b12e8e25576ae0b41400a53968806e1c8a861e35381073b3baef45a83cafb5f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263048436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf3502690f913bb0793628e39a93e479a6310aebbee6e65e9d1cb1598267dd01`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 07:45:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:45:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:45:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:45:52 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:46:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:46:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:46:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:47:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f2be4669bf5e0d981bd25dce9fc1cf7b12acd140fc4c22c8d7775f5f0d8dca`  
		Last Modified: Thu, 02 Mar 2023 08:07:35 GMT  
		Size: 106.3 MB (106343240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216ea0d3b5795e8929e583b997a5548be75d03e2a29c115d9f56a944ed84ef0c`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a2aa4beb52be76c6dcd46fc6d1847a75b9ae29c6ebcedc86c9d7f47e4b7165`  
		Last Modified: Thu, 02 Mar 2023 08:07:57 GMT  
		Size: 97.9 MB (97887836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680641f18bb2dd24d14e77d0c3c76ee534de308a8b9d4bd0e587ef1e7b1eb7f8`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 313.2 KB (313170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bef39aad161da9cfed034f35d026bd853ef6023d95711bfc15adb24433f0727`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb484450c9c02df2f1231534b50c85b959723c443ff405fa836795d75227868e`  
		Last Modified: Thu, 02 Mar 2023 08:07:47 GMT  
		Size: 23.1 MB (23071319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c2d497729f6aee71e99bcdd9e454ad5eb1dd3468ae4d4effbf6d4f0ba96c689f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255709503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af910ab58e75966664e169632c6f9accf125c72c2c695d2fa000e4570f4eb25c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 03:48:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:48:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:48:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:48:35 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:49:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:49:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:49:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:50:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13cc6d4ba7a8ad400f19bd92e8cb2286caeca1d46ce132719b2b1987256c21f`  
		Last Modified: Thu, 02 Mar 2023 04:10:13 GMT  
		Size: 104.1 MB (104057998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396dec5942a2fa6aff8e013fe4ebdcfabe51979982de742c3c3a1f04b10a63d5`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617a68eb8bb8b1ab93ca9de116c7d22adcb04072699fcb1ad23a5f18e1ac0305`  
		Last Modified: Thu, 02 Mar 2023 04:10:33 GMT  
		Size: 95.5 MB (95477602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aea5ab66a030d09edeb6bd52a5d2d8c7ee9d2f179e47f3769d797ea1cec2eaa`  
		Last Modified: Thu, 02 Mar 2023 04:10:23 GMT  
		Size: 313.2 KB (313171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83267e4907f639f28f19da252316e35ac2d9754f0b1c072254ccbbae8c95aea2`  
		Last Modified: Thu, 02 Mar 2023 04:10:22 GMT  
		Size: 2.4 KB (2403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b408f45a9652713b3956f2c893ddb6bf2c327cde2e347d0ccd449062384917`  
		Last Modified: Thu, 02 Mar 2023 04:10:26 GMT  
		Size: 22.5 MB (22497086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:3b0e8f2d2ff998c17b521adf0ae2300669cd29ec48b179771a83a2495be72045
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:b12e8e25576ae0b41400a53968806e1c8a861e35381073b3baef45a83cafb5f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263048436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf3502690f913bb0793628e39a93e479a6310aebbee6e65e9d1cb1598267dd01`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 07:45:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:45:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:45:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:45:52 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:46:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:46:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:46:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:47:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f2be4669bf5e0d981bd25dce9fc1cf7b12acd140fc4c22c8d7775f5f0d8dca`  
		Last Modified: Thu, 02 Mar 2023 08:07:35 GMT  
		Size: 106.3 MB (106343240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216ea0d3b5795e8929e583b997a5548be75d03e2a29c115d9f56a944ed84ef0c`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a2aa4beb52be76c6dcd46fc6d1847a75b9ae29c6ebcedc86c9d7f47e4b7165`  
		Last Modified: Thu, 02 Mar 2023 08:07:57 GMT  
		Size: 97.9 MB (97887836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680641f18bb2dd24d14e77d0c3c76ee534de308a8b9d4bd0e587ef1e7b1eb7f8`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 313.2 KB (313170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bef39aad161da9cfed034f35d026bd853ef6023d95711bfc15adb24433f0727`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb484450c9c02df2f1231534b50c85b959723c443ff405fa836795d75227868e`  
		Last Modified: Thu, 02 Mar 2023 08:07:47 GMT  
		Size: 23.1 MB (23071319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c2d497729f6aee71e99bcdd9e454ad5eb1dd3468ae4d4effbf6d4f0ba96c689f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255709503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af910ab58e75966664e169632c6f9accf125c72c2c695d2fa000e4570f4eb25c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 03:48:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:48:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:48:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:48:35 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:49:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:49:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:49:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:50:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13cc6d4ba7a8ad400f19bd92e8cb2286caeca1d46ce132719b2b1987256c21f`  
		Last Modified: Thu, 02 Mar 2023 04:10:13 GMT  
		Size: 104.1 MB (104057998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396dec5942a2fa6aff8e013fe4ebdcfabe51979982de742c3c3a1f04b10a63d5`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617a68eb8bb8b1ab93ca9de116c7d22adcb04072699fcb1ad23a5f18e1ac0305`  
		Last Modified: Thu, 02 Mar 2023 04:10:33 GMT  
		Size: 95.5 MB (95477602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aea5ab66a030d09edeb6bd52a5d2d8c7ee9d2f179e47f3769d797ea1cec2eaa`  
		Last Modified: Thu, 02 Mar 2023 04:10:23 GMT  
		Size: 313.2 KB (313171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83267e4907f639f28f19da252316e35ac2d9754f0b1c072254ccbbae8c95aea2`  
		Last Modified: Thu, 02 Mar 2023 04:10:22 GMT  
		Size: 2.4 KB (2403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b408f45a9652713b3956f2c893ddb6bf2c327cde2e347d0ccd449062384917`  
		Last Modified: Thu, 02 Mar 2023 04:10:26 GMT  
		Size: 22.5 MB (22497086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core`

```console
$ docker pull ros@sha256:ab00ff93592c87a1ddb9dcaf05152e223fc3c3a60d78dddc76e8319489b03c72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:2a5627af3d69d32824e3c3d201b41934befece891ade561b99b02e84c7c6e48c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141773684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25650769e50a84d1a0d79b8c74c1c0ed0bcb65349bd6f46aac17cbb4a241d8fa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 07:45:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:45:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:45:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:45:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f2be4669bf5e0d981bd25dce9fc1cf7b12acd140fc4c22c8d7775f5f0d8dca`  
		Last Modified: Thu, 02 Mar 2023 08:07:35 GMT  
		Size: 106.3 MB (106343240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216ea0d3b5795e8929e583b997a5548be75d03e2a29c115d9f56a944ed84ef0c`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6c32d57535d278d669da801345b8c68ca9fffd201351e066935e67b48ea2d0bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137419241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:317653c9b23895eb55566f681320ede95f2996c4e2d0a159e716fb763d3db6e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 03:48:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:48:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:48:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:48:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13cc6d4ba7a8ad400f19bd92e8cb2286caeca1d46ce132719b2b1987256c21f`  
		Last Modified: Thu, 02 Mar 2023 04:10:13 GMT  
		Size: 104.1 MB (104057998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396dec5942a2fa6aff8e013fe4ebdcfabe51979982de742c3c3a1f04b10a63d5`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:humble-ros-core-jammy`

```console
$ docker pull ros@sha256:ab00ff93592c87a1ddb9dcaf05152e223fc3c3a60d78dddc76e8319489b03c72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:2a5627af3d69d32824e3c3d201b41934befece891ade561b99b02e84c7c6e48c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141773684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25650769e50a84d1a0d79b8c74c1c0ed0bcb65349bd6f46aac17cbb4a241d8fa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 07:45:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:45:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:45:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:45:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f2be4669bf5e0d981bd25dce9fc1cf7b12acd140fc4c22c8d7775f5f0d8dca`  
		Last Modified: Thu, 02 Mar 2023 08:07:35 GMT  
		Size: 106.3 MB (106343240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216ea0d3b5795e8929e583b997a5548be75d03e2a29c115d9f56a944ed84ef0c`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6c32d57535d278d669da801345b8c68ca9fffd201351e066935e67b48ea2d0bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137419241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:317653c9b23895eb55566f681320ede95f2996c4e2d0a159e716fb763d3db6e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 03:48:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:48:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:48:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:48:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13cc6d4ba7a8ad400f19bd92e8cb2286caeca1d46ce132719b2b1987256c21f`  
		Last Modified: Thu, 02 Mar 2023 04:10:13 GMT  
		Size: 104.1 MB (104057998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396dec5942a2fa6aff8e013fe4ebdcfabe51979982de742c3c3a1f04b10a63d5`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:3b0e8f2d2ff998c17b521adf0ae2300669cd29ec48b179771a83a2495be72045
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:b12e8e25576ae0b41400a53968806e1c8a861e35381073b3baef45a83cafb5f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263048436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf3502690f913bb0793628e39a93e479a6310aebbee6e65e9d1cb1598267dd01`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 07:45:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:45:52 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:45:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:45:52 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:46:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:46:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:46:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:47:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f2be4669bf5e0d981bd25dce9fc1cf7b12acd140fc4c22c8d7775f5f0d8dca`  
		Last Modified: Thu, 02 Mar 2023 08:07:35 GMT  
		Size: 106.3 MB (106343240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216ea0d3b5795e8929e583b997a5548be75d03e2a29c115d9f56a944ed84ef0c`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a2aa4beb52be76c6dcd46fc6d1847a75b9ae29c6ebcedc86c9d7f47e4b7165`  
		Last Modified: Thu, 02 Mar 2023 08:07:57 GMT  
		Size: 97.9 MB (97887836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680641f18bb2dd24d14e77d0c3c76ee534de308a8b9d4bd0e587ef1e7b1eb7f8`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 313.2 KB (313170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bef39aad161da9cfed034f35d026bd853ef6023d95711bfc15adb24433f0727`  
		Last Modified: Thu, 02 Mar 2023 08:07:43 GMT  
		Size: 2.4 KB (2427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb484450c9c02df2f1231534b50c85b959723c443ff405fa836795d75227868e`  
		Last Modified: Thu, 02 Mar 2023 08:07:47 GMT  
		Size: 23.1 MB (23071319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c2d497729f6aee71e99bcdd9e454ad5eb1dd3468ae4d4effbf6d4f0ba96c689f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255709503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af910ab58e75966664e169632c6f9accf125c72c2c695d2fa000e4570f4eb25c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 03:48:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:48:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:48:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:48:35 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:49:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:49:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:49:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:50:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13cc6d4ba7a8ad400f19bd92e8cb2286caeca1d46ce132719b2b1987256c21f`  
		Last Modified: Thu, 02 Mar 2023 04:10:13 GMT  
		Size: 104.1 MB (104057998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396dec5942a2fa6aff8e013fe4ebdcfabe51979982de742c3c3a1f04b10a63d5`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617a68eb8bb8b1ab93ca9de116c7d22adcb04072699fcb1ad23a5f18e1ac0305`  
		Last Modified: Thu, 02 Mar 2023 04:10:33 GMT  
		Size: 95.5 MB (95477602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aea5ab66a030d09edeb6bd52a5d2d8c7ee9d2f179e47f3769d797ea1cec2eaa`  
		Last Modified: Thu, 02 Mar 2023 04:10:23 GMT  
		Size: 313.2 KB (313171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83267e4907f639f28f19da252316e35ac2d9754f0b1c072254ccbbae8c95aea2`  
		Last Modified: Thu, 02 Mar 2023 04:10:22 GMT  
		Size: 2.4 KB (2403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b408f45a9652713b3956f2c893ddb6bf2c327cde2e347d0ccd449062384917`  
		Last Modified: Thu, 02 Mar 2023 04:10:26 GMT  
		Size: 22.5 MB (22497086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:2b3882e1f5797d6595a18e66f892fc51d274bdfb938189f5d36b01d82bcf01a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:93ff17f047b26c4000ff1e18878fa6b7a9382144a3c7da9a35ba6a91daa48f13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.6 MB (437556445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d941256e42ae81c23437fb91cad81c68d0add57857c039dd828856052add40e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:17:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 07:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:09 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:21:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:21:10 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:21:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778654c0b435df260fd94e3a713e5ac0391d850b1dd50fc06d28724d697fd461`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 819.0 KB (819000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d3083a206086f721888a54dea32baf21c2cbc9155b39a9bac8631b20fede9`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 4.9 MB (4878631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3996b56577fbab1f217c1223e4ebab884c63ce1386b54be8a894044ad014a1d2`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff9d7fdf49d225218831b48c5847ebec87cb5bf3ea8cf9ab3eea0d1ef0e50a3`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e996788e40044c1f9c625c87249f7c8e303e5b8ed46020cad2d20e09982229d`  
		Last Modified: Thu, 02 Mar 2023 08:02:00 GMT  
		Size: 259.6 MB (259580317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9e9a8cb8917a1575d0a91f4e93b6a1d90ce64013c9d9648ad09eb9ef72e24`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360c9e013d6493daea567582a2a448f49a706cf4fded3acfd62c562004627daf`  
		Last Modified: Thu, 02 Mar 2023 08:02:18 GMT  
		Size: 70.3 MB (70267262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11487da93620b5bdb7d2f78eaf417d53227fed9b51f79df5cbbbdde4cd0da6`  
		Last Modified: Thu, 02 Mar 2023 08:02:09 GMT  
		Size: 297.5 KB (297495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c5f20223785c1f0757781aa7972ae767a9cbe64b3311b544ee8051d7e6a4c1`  
		Last Modified: Thu, 02 Mar 2023 08:02:20 GMT  
		Size: 75.0 MB (75000741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:e44ed680e0f8a8017636396ffdd9014c8c8942aee80f5aca1a37be4933236ba2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386040880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a9ff6e7934d64730587cd2da4d4ff2af00304d1805a1dc514b9be9dec6fd9a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:59:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 11:59:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 12:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:02:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:02:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:02:56 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:03:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:03:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b0874a47238c32833a1eb83551fa898735b969e33ba525c389d76a5973f18f`  
		Last Modified: Thu, 02 Mar 2023 12:27:23 GMT  
		Size: 819.1 KB (819062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca96c8d5fedefbf017ce0e41cecd02d40bb2d5b9093183b5889473daeda03`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 4.1 MB (4089642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c69e7b7b6ea014cc49dc25e4e3ad18bcc240bc2e96cd077a9618bfab8816e`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a769aaaa6a5a307f498af8c8bc3c3992f64f37b6d9f716dc2c0eddf7a13c2`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39727381991a44c63174e1b8193e9cc4386b91a936cca3b942c67cb58012e6d7`  
		Last Modified: Thu, 02 Mar 2023 12:27:54 GMT  
		Size: 239.0 MB (239045530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134249505ec9b290e4986fd60e7b3bf9da3ea895cf2609ef3b8a4f9ced66eead`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f49c73b5c2e574db7cbb840ea3132a051626d8ea7f869ead59ebd1b8448f601`  
		Last Modified: Thu, 02 Mar 2023 12:28:12 GMT  
		Size: 54.7 MB (54733714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3a64e4ebd696ce4cef7a0e94e6fa5022a1d218ed4f1ec9fcc479ccb03dfb26`  
		Last Modified: Thu, 02 Mar 2023 12:28:04 GMT  
		Size: 297.6 KB (297553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce032e347c9e1d2bbe0065495e4253363c1c7d7f8bf6a27570b03729f482058f`  
		Last Modified: Thu, 02 Mar 2023 12:28:15 GMT  
		Size: 64.7 MB (64749464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e270a7432c93f738fb6cb42ae04726c84dee53c855f2cb43c9fae71d373a7a6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412192920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afc8882704f4a7b5cd865f8bffa9416bc6ddb23ffdf7cbf0d0a81e4be623b99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:16:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 03:20:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:20:16 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:21:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:22:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcb6c39567ec9b2c7ea7bca3bf033f2f41f3a4c07d089b9de2d8a14bab3292`  
		Last Modified: Thu, 02 Mar 2023 04:04:42 GMT  
		Size: 818.9 KB (818853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c5391c267d74199876bc0f614d5b80ad1e03948938fecf4d80e0ab49f7c90`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 4.5 MB (4461697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65a69abc68e01cb3f3e8e00001fc0ff966cd84b753e82111e495e9d319ee03d`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151a1078cd0202754dec71f67746b6c116798ceaaec93e1fd31ae3fd305b501`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2b2ae19293c39a9abe7ed81542deaf9824db2f84b81e2cbe87c4b55e01fb8`  
		Last Modified: Thu, 02 Mar 2023 04:05:13 GMT  
		Size: 252.5 MB (252548696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae119db2c7c4ffba52e20aea0bf61b6e9bb6a81bb69236b7177610e3d8d3faf`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf304e76035eea24e63c6f8df3b3226e6af34ae05635d41819e5084f1ad6717c`  
		Last Modified: Thu, 02 Mar 2023 04:05:28 GMT  
		Size: 63.1 MB (63096257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce94d2b7b5f6ce75418a3f1a7754706762dc89fb5ac7ae79de0c100223e5b594`  
		Last Modified: Thu, 02 Mar 2023 04:05:22 GMT  
		Size: 297.5 KB (297502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75def227e2b8440db3d1998106b192c98342ceab881d620f4a43be96b5876616`  
		Last Modified: Thu, 02 Mar 2023 04:05:32 GMT  
		Size: 67.2 MB (67234530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:65d6bfbb791c088bd1383975711eabcec4473ca07a751663d74150c9148cfb02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:79e816817c0c62c8b4ac5896bb86de9b81aa812811d28e98a8093dd6a75a4611
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742921991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef6d842f5887469b3de34491b750bdc06bf9b3fb2db1ae8f5483aee71b2e54e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:17:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 07:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:09 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:21:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:21:10 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:21:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778654c0b435df260fd94e3a713e5ac0391d850b1dd50fc06d28724d697fd461`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 819.0 KB (819000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d3083a206086f721888a54dea32baf21c2cbc9155b39a9bac8631b20fede9`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 4.9 MB (4878631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3996b56577fbab1f217c1223e4ebab884c63ce1386b54be8a894044ad014a1d2`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff9d7fdf49d225218831b48c5847ebec87cb5bf3ea8cf9ab3eea0d1ef0e50a3`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e996788e40044c1f9c625c87249f7c8e303e5b8ed46020cad2d20e09982229d`  
		Last Modified: Thu, 02 Mar 2023 08:02:00 GMT  
		Size: 259.6 MB (259580317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9e9a8cb8917a1575d0a91f4e93b6a1d90ce64013c9d9648ad09eb9ef72e24`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360c9e013d6493daea567582a2a448f49a706cf4fded3acfd62c562004627daf`  
		Last Modified: Thu, 02 Mar 2023 08:02:18 GMT  
		Size: 70.3 MB (70267262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11487da93620b5bdb7d2f78eaf417d53227fed9b51f79df5cbbbdde4cd0da6`  
		Last Modified: Thu, 02 Mar 2023 08:02:09 GMT  
		Size: 297.5 KB (297495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c5f20223785c1f0757781aa7972ae767a9cbe64b3311b544ee8051d7e6a4c1`  
		Last Modified: Thu, 02 Mar 2023 08:02:20 GMT  
		Size: 75.0 MB (75000741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8388fa8a2bcbb7a302dce3d0f8131726b593f5bc8d26fdbc97aef5cd9f4f22fb`  
		Last Modified: Thu, 02 Mar 2023 08:03:26 GMT  
		Size: 305.4 MB (305365546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:c6f6e67d683733d2f335bdd9e1775e8691b9845e71d385b387c1fdb71f4c1b0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.1 MB (646074287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:655d63d2d4ed7e4a0fb56cb73f683f654195b400000c3442172f2bb317ac2645`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:59:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 11:59:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 12:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:02:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:02:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:02:56 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:03:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:03:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b0874a47238c32833a1eb83551fa898735b969e33ba525c389d76a5973f18f`  
		Last Modified: Thu, 02 Mar 2023 12:27:23 GMT  
		Size: 819.1 KB (819062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca96c8d5fedefbf017ce0e41cecd02d40bb2d5b9093183b5889473daeda03`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 4.1 MB (4089642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c69e7b7b6ea014cc49dc25e4e3ad18bcc240bc2e96cd077a9618bfab8816e`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a769aaaa6a5a307f498af8c8bc3c3992f64f37b6d9f716dc2c0eddf7a13c2`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39727381991a44c63174e1b8193e9cc4386b91a936cca3b942c67cb58012e6d7`  
		Last Modified: Thu, 02 Mar 2023 12:27:54 GMT  
		Size: 239.0 MB (239045530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134249505ec9b290e4986fd60e7b3bf9da3ea895cf2609ef3b8a4f9ced66eead`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f49c73b5c2e574db7cbb840ea3132a051626d8ea7f869ead59ebd1b8448f601`  
		Last Modified: Thu, 02 Mar 2023 12:28:12 GMT  
		Size: 54.7 MB (54733714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3a64e4ebd696ce4cef7a0e94e6fa5022a1d218ed4f1ec9fcc479ccb03dfb26`  
		Last Modified: Thu, 02 Mar 2023 12:28:04 GMT  
		Size: 297.6 KB (297553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce032e347c9e1d2bbe0065495e4253363c1c7d7f8bf6a27570b03729f482058f`  
		Last Modified: Thu, 02 Mar 2023 12:28:15 GMT  
		Size: 64.7 MB (64749464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc25ed8a81e7808a52790e3188dd72a806b9ea001987c1887368ba166c2e7478`  
		Last Modified: Thu, 02 Mar 2023 12:29:17 GMT  
		Size: 260.0 MB (260033407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e1b941abdebf9b35eafaa66c7af8798b68e64bb5ce0a5607375f724bf2c8f186
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.9 MB (703878978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0ec9eedc67be1a5d55da359fa18c644604f55f12b54940a188575117252326`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:16:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 03:20:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:20:16 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:21:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:22:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcb6c39567ec9b2c7ea7bca3bf033f2f41f3a4c07d089b9de2d8a14bab3292`  
		Last Modified: Thu, 02 Mar 2023 04:04:42 GMT  
		Size: 818.9 KB (818853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c5391c267d74199876bc0f614d5b80ad1e03948938fecf4d80e0ab49f7c90`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 4.5 MB (4461697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65a69abc68e01cb3f3e8e00001fc0ff966cd84b753e82111e495e9d319ee03d`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151a1078cd0202754dec71f67746b6c116798ceaaec93e1fd31ae3fd305b501`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2b2ae19293c39a9abe7ed81542deaf9824db2f84b81e2cbe87c4b55e01fb8`  
		Last Modified: Thu, 02 Mar 2023 04:05:13 GMT  
		Size: 252.5 MB (252548696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae119db2c7c4ffba52e20aea0bf61b6e9bb6a81bb69236b7177610e3d8d3faf`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf304e76035eea24e63c6f8df3b3226e6af34ae05635d41819e5084f1ad6717c`  
		Last Modified: Thu, 02 Mar 2023 04:05:28 GMT  
		Size: 63.1 MB (63096257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce94d2b7b5f6ce75418a3f1a7754706762dc89fb5ac7ae79de0c100223e5b594`  
		Last Modified: Thu, 02 Mar 2023 04:05:22 GMT  
		Size: 297.5 KB (297502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75def227e2b8440db3d1998106b192c98342ceab881d620f4a43be96b5876616`  
		Last Modified: Thu, 02 Mar 2023 04:05:32 GMT  
		Size: 67.2 MB (67234530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7183d8ea19dba367749ba2ab4d0f9ac2c0e9bcb402f872cde6996cb72acb1a1`  
		Last Modified: Thu, 02 Mar 2023 04:06:31 GMT  
		Size: 291.7 MB (291686058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:65d6bfbb791c088bd1383975711eabcec4473ca07a751663d74150c9148cfb02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:79e816817c0c62c8b4ac5896bb86de9b81aa812811d28e98a8093dd6a75a4611
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.9 MB (742921991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef6d842f5887469b3de34491b750bdc06bf9b3fb2db1ae8f5483aee71b2e54e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:17:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 07:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:09 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:21:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:21:10 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:21:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778654c0b435df260fd94e3a713e5ac0391d850b1dd50fc06d28724d697fd461`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 819.0 KB (819000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d3083a206086f721888a54dea32baf21c2cbc9155b39a9bac8631b20fede9`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 4.9 MB (4878631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3996b56577fbab1f217c1223e4ebab884c63ce1386b54be8a894044ad014a1d2`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff9d7fdf49d225218831b48c5847ebec87cb5bf3ea8cf9ab3eea0d1ef0e50a3`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e996788e40044c1f9c625c87249f7c8e303e5b8ed46020cad2d20e09982229d`  
		Last Modified: Thu, 02 Mar 2023 08:02:00 GMT  
		Size: 259.6 MB (259580317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9e9a8cb8917a1575d0a91f4e93b6a1d90ce64013c9d9648ad09eb9ef72e24`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360c9e013d6493daea567582a2a448f49a706cf4fded3acfd62c562004627daf`  
		Last Modified: Thu, 02 Mar 2023 08:02:18 GMT  
		Size: 70.3 MB (70267262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11487da93620b5bdb7d2f78eaf417d53227fed9b51f79df5cbbbdde4cd0da6`  
		Last Modified: Thu, 02 Mar 2023 08:02:09 GMT  
		Size: 297.5 KB (297495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c5f20223785c1f0757781aa7972ae767a9cbe64b3311b544ee8051d7e6a4c1`  
		Last Modified: Thu, 02 Mar 2023 08:02:20 GMT  
		Size: 75.0 MB (75000741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8388fa8a2bcbb7a302dce3d0f8131726b593f5bc8d26fdbc97aef5cd9f4f22fb`  
		Last Modified: Thu, 02 Mar 2023 08:03:26 GMT  
		Size: 305.4 MB (305365546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:c6f6e67d683733d2f335bdd9e1775e8691b9845e71d385b387c1fdb71f4c1b0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.1 MB (646074287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:655d63d2d4ed7e4a0fb56cb73f683f654195b400000c3442172f2bb317ac2645`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:59:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 11:59:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 12:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:02:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:02:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:02:56 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:03:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:03:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b0874a47238c32833a1eb83551fa898735b969e33ba525c389d76a5973f18f`  
		Last Modified: Thu, 02 Mar 2023 12:27:23 GMT  
		Size: 819.1 KB (819062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca96c8d5fedefbf017ce0e41cecd02d40bb2d5b9093183b5889473daeda03`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 4.1 MB (4089642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c69e7b7b6ea014cc49dc25e4e3ad18bcc240bc2e96cd077a9618bfab8816e`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a769aaaa6a5a307f498af8c8bc3c3992f64f37b6d9f716dc2c0eddf7a13c2`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39727381991a44c63174e1b8193e9cc4386b91a936cca3b942c67cb58012e6d7`  
		Last Modified: Thu, 02 Mar 2023 12:27:54 GMT  
		Size: 239.0 MB (239045530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134249505ec9b290e4986fd60e7b3bf9da3ea895cf2609ef3b8a4f9ced66eead`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f49c73b5c2e574db7cbb840ea3132a051626d8ea7f869ead59ebd1b8448f601`  
		Last Modified: Thu, 02 Mar 2023 12:28:12 GMT  
		Size: 54.7 MB (54733714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3a64e4ebd696ce4cef7a0e94e6fa5022a1d218ed4f1ec9fcc479ccb03dfb26`  
		Last Modified: Thu, 02 Mar 2023 12:28:04 GMT  
		Size: 297.6 KB (297553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce032e347c9e1d2bbe0065495e4253363c1c7d7f8bf6a27570b03729f482058f`  
		Last Modified: Thu, 02 Mar 2023 12:28:15 GMT  
		Size: 64.7 MB (64749464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc25ed8a81e7808a52790e3188dd72a806b9ea001987c1887368ba166c2e7478`  
		Last Modified: Thu, 02 Mar 2023 12:29:17 GMT  
		Size: 260.0 MB (260033407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e1b941abdebf9b35eafaa66c7af8798b68e64bb5ce0a5607375f724bf2c8f186
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.9 MB (703878978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0ec9eedc67be1a5d55da359fa18c644604f55f12b54940a188575117252326`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:16:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 03:20:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:20:16 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:21:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:22:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcb6c39567ec9b2c7ea7bca3bf033f2f41f3a4c07d089b9de2d8a14bab3292`  
		Last Modified: Thu, 02 Mar 2023 04:04:42 GMT  
		Size: 818.9 KB (818853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c5391c267d74199876bc0f614d5b80ad1e03948938fecf4d80e0ab49f7c90`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 4.5 MB (4461697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65a69abc68e01cb3f3e8e00001fc0ff966cd84b753e82111e495e9d319ee03d`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151a1078cd0202754dec71f67746b6c116798ceaaec93e1fd31ae3fd305b501`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2b2ae19293c39a9abe7ed81542deaf9824db2f84b81e2cbe87c4b55e01fb8`  
		Last Modified: Thu, 02 Mar 2023 04:05:13 GMT  
		Size: 252.5 MB (252548696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae119db2c7c4ffba52e20aea0bf61b6e9bb6a81bb69236b7177610e3d8d3faf`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf304e76035eea24e63c6f8df3b3226e6af34ae05635d41819e5084f1ad6717c`  
		Last Modified: Thu, 02 Mar 2023 04:05:28 GMT  
		Size: 63.1 MB (63096257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce94d2b7b5f6ce75418a3f1a7754706762dc89fb5ac7ae79de0c100223e5b594`  
		Last Modified: Thu, 02 Mar 2023 04:05:22 GMT  
		Size: 297.5 KB (297502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75def227e2b8440db3d1998106b192c98342ceab881d620f4a43be96b5876616`  
		Last Modified: Thu, 02 Mar 2023 04:05:32 GMT  
		Size: 67.2 MB (67234530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7183d8ea19dba367749ba2ab4d0f9ac2c0e9bcb402f872cde6996cb72acb1a1`  
		Last Modified: Thu, 02 Mar 2023 04:06:31 GMT  
		Size: 291.7 MB (291686058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:44e4815d30da6d8a20aaf856852a82f793914a04a5c984268635a5ab987847f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:596994f0ab152e085ccaf24836fa91630720e42d14984ab0f6a12765025bd3a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448643015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:893eb20a1d3a4654663ef556113da4b034044bac012b2fe0f80419a66f54a71d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:17:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 07:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:09 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:21:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:21:10 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:21:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778654c0b435df260fd94e3a713e5ac0391d850b1dd50fc06d28724d697fd461`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 819.0 KB (819000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d3083a206086f721888a54dea32baf21c2cbc9155b39a9bac8631b20fede9`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 4.9 MB (4878631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3996b56577fbab1f217c1223e4ebab884c63ce1386b54be8a894044ad014a1d2`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff9d7fdf49d225218831b48c5847ebec87cb5bf3ea8cf9ab3eea0d1ef0e50a3`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e996788e40044c1f9c625c87249f7c8e303e5b8ed46020cad2d20e09982229d`  
		Last Modified: Thu, 02 Mar 2023 08:02:00 GMT  
		Size: 259.6 MB (259580317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9e9a8cb8917a1575d0a91f4e93b6a1d90ce64013c9d9648ad09eb9ef72e24`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360c9e013d6493daea567582a2a448f49a706cf4fded3acfd62c562004627daf`  
		Last Modified: Thu, 02 Mar 2023 08:02:18 GMT  
		Size: 70.3 MB (70267262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11487da93620b5bdb7d2f78eaf417d53227fed9b51f79df5cbbbdde4cd0da6`  
		Last Modified: Thu, 02 Mar 2023 08:02:09 GMT  
		Size: 297.5 KB (297495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c5f20223785c1f0757781aa7972ae767a9cbe64b3311b544ee8051d7e6a4c1`  
		Last Modified: Thu, 02 Mar 2023 08:02:20 GMT  
		Size: 75.0 MB (75000741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b95716061af8748ea49196507a8909434771576d47cbf3b683ed37797181a43`  
		Last Modified: Thu, 02 Mar 2023 08:02:33 GMT  
		Size: 11.1 MB (11086570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:28db3ae460cf4176b01cebe1c7a7001dd769664852b3582fa08716d6840d5988
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396163059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c220745b4f574d4dad949748606cdefb8b7158488125ebe70cd48d1b3b8629be`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:59:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 11:59:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 12:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:02:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:02:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:02:56 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:03:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:03:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:05:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b0874a47238c32833a1eb83551fa898735b969e33ba525c389d76a5973f18f`  
		Last Modified: Thu, 02 Mar 2023 12:27:23 GMT  
		Size: 819.1 KB (819062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca96c8d5fedefbf017ce0e41cecd02d40bb2d5b9093183b5889473daeda03`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 4.1 MB (4089642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c69e7b7b6ea014cc49dc25e4e3ad18bcc240bc2e96cd077a9618bfab8816e`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a769aaaa6a5a307f498af8c8bc3c3992f64f37b6d9f716dc2c0eddf7a13c2`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39727381991a44c63174e1b8193e9cc4386b91a936cca3b942c67cb58012e6d7`  
		Last Modified: Thu, 02 Mar 2023 12:27:54 GMT  
		Size: 239.0 MB (239045530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134249505ec9b290e4986fd60e7b3bf9da3ea895cf2609ef3b8a4f9ced66eead`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f49c73b5c2e574db7cbb840ea3132a051626d8ea7f869ead59ebd1b8448f601`  
		Last Modified: Thu, 02 Mar 2023 12:28:12 GMT  
		Size: 54.7 MB (54733714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3a64e4ebd696ce4cef7a0e94e6fa5022a1d218ed4f1ec9fcc479ccb03dfb26`  
		Last Modified: Thu, 02 Mar 2023 12:28:04 GMT  
		Size: 297.6 KB (297553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce032e347c9e1d2bbe0065495e4253363c1c7d7f8bf6a27570b03729f482058f`  
		Last Modified: Thu, 02 Mar 2023 12:28:15 GMT  
		Size: 64.7 MB (64749464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f39080fa0b454b326c79d9cc1508f0d297bc9a2cd939700b29c2c2b68ac3ef`  
		Last Modified: Thu, 02 Mar 2023 12:28:30 GMT  
		Size: 10.1 MB (10122179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6288af56a458618c741df9cab3be4072895bce454b48f0073addf0f6da952616
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422932923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402dcb9e4c4c82f607da7e660dd32ab52a4682e7ce6343de3ef78d0e8bc24ca8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:16:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 03:20:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:20:16 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:21:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:22:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:23:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcb6c39567ec9b2c7ea7bca3bf033f2f41f3a4c07d089b9de2d8a14bab3292`  
		Last Modified: Thu, 02 Mar 2023 04:04:42 GMT  
		Size: 818.9 KB (818853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c5391c267d74199876bc0f614d5b80ad1e03948938fecf4d80e0ab49f7c90`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 4.5 MB (4461697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65a69abc68e01cb3f3e8e00001fc0ff966cd84b753e82111e495e9d319ee03d`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151a1078cd0202754dec71f67746b6c116798ceaaec93e1fd31ae3fd305b501`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2b2ae19293c39a9abe7ed81542deaf9824db2f84b81e2cbe87c4b55e01fb8`  
		Last Modified: Thu, 02 Mar 2023 04:05:13 GMT  
		Size: 252.5 MB (252548696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae119db2c7c4ffba52e20aea0bf61b6e9bb6a81bb69236b7177610e3d8d3faf`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf304e76035eea24e63c6f8df3b3226e6af34ae05635d41819e5084f1ad6717c`  
		Last Modified: Thu, 02 Mar 2023 04:05:28 GMT  
		Size: 63.1 MB (63096257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce94d2b7b5f6ce75418a3f1a7754706762dc89fb5ac7ae79de0c100223e5b594`  
		Last Modified: Thu, 02 Mar 2023 04:05:22 GMT  
		Size: 297.5 KB (297502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75def227e2b8440db3d1998106b192c98342ceab881d620f4a43be96b5876616`  
		Last Modified: Thu, 02 Mar 2023 04:05:32 GMT  
		Size: 67.2 MB (67234530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccaf24f26bfdcbe1f5d03582710621430bc9c5e2a7c5d27c2a38b824fe85e3be`  
		Last Modified: Thu, 02 Mar 2023 04:05:45 GMT  
		Size: 10.7 MB (10740003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:44e4815d30da6d8a20aaf856852a82f793914a04a5c984268635a5ab987847f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:596994f0ab152e085ccaf24836fa91630720e42d14984ab0f6a12765025bd3a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448643015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:893eb20a1d3a4654663ef556113da4b034044bac012b2fe0f80419a66f54a71d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:17:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 07:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:09 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:21:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:21:10 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:21:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778654c0b435df260fd94e3a713e5ac0391d850b1dd50fc06d28724d697fd461`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 819.0 KB (819000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d3083a206086f721888a54dea32baf21c2cbc9155b39a9bac8631b20fede9`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 4.9 MB (4878631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3996b56577fbab1f217c1223e4ebab884c63ce1386b54be8a894044ad014a1d2`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff9d7fdf49d225218831b48c5847ebec87cb5bf3ea8cf9ab3eea0d1ef0e50a3`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e996788e40044c1f9c625c87249f7c8e303e5b8ed46020cad2d20e09982229d`  
		Last Modified: Thu, 02 Mar 2023 08:02:00 GMT  
		Size: 259.6 MB (259580317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9e9a8cb8917a1575d0a91f4e93b6a1d90ce64013c9d9648ad09eb9ef72e24`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360c9e013d6493daea567582a2a448f49a706cf4fded3acfd62c562004627daf`  
		Last Modified: Thu, 02 Mar 2023 08:02:18 GMT  
		Size: 70.3 MB (70267262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11487da93620b5bdb7d2f78eaf417d53227fed9b51f79df5cbbbdde4cd0da6`  
		Last Modified: Thu, 02 Mar 2023 08:02:09 GMT  
		Size: 297.5 KB (297495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c5f20223785c1f0757781aa7972ae767a9cbe64b3311b544ee8051d7e6a4c1`  
		Last Modified: Thu, 02 Mar 2023 08:02:20 GMT  
		Size: 75.0 MB (75000741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b95716061af8748ea49196507a8909434771576d47cbf3b683ed37797181a43`  
		Last Modified: Thu, 02 Mar 2023 08:02:33 GMT  
		Size: 11.1 MB (11086570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:28db3ae460cf4176b01cebe1c7a7001dd769664852b3582fa08716d6840d5988
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396163059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c220745b4f574d4dad949748606cdefb8b7158488125ebe70cd48d1b3b8629be`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:59:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 11:59:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 12:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:02:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:02:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:02:56 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:03:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:03:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:05:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b0874a47238c32833a1eb83551fa898735b969e33ba525c389d76a5973f18f`  
		Last Modified: Thu, 02 Mar 2023 12:27:23 GMT  
		Size: 819.1 KB (819062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca96c8d5fedefbf017ce0e41cecd02d40bb2d5b9093183b5889473daeda03`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 4.1 MB (4089642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c69e7b7b6ea014cc49dc25e4e3ad18bcc240bc2e96cd077a9618bfab8816e`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a769aaaa6a5a307f498af8c8bc3c3992f64f37b6d9f716dc2c0eddf7a13c2`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39727381991a44c63174e1b8193e9cc4386b91a936cca3b942c67cb58012e6d7`  
		Last Modified: Thu, 02 Mar 2023 12:27:54 GMT  
		Size: 239.0 MB (239045530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134249505ec9b290e4986fd60e7b3bf9da3ea895cf2609ef3b8a4f9ced66eead`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f49c73b5c2e574db7cbb840ea3132a051626d8ea7f869ead59ebd1b8448f601`  
		Last Modified: Thu, 02 Mar 2023 12:28:12 GMT  
		Size: 54.7 MB (54733714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3a64e4ebd696ce4cef7a0e94e6fa5022a1d218ed4f1ec9fcc479ccb03dfb26`  
		Last Modified: Thu, 02 Mar 2023 12:28:04 GMT  
		Size: 297.6 KB (297553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce032e347c9e1d2bbe0065495e4253363c1c7d7f8bf6a27570b03729f482058f`  
		Last Modified: Thu, 02 Mar 2023 12:28:15 GMT  
		Size: 64.7 MB (64749464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f39080fa0b454b326c79d9cc1508f0d297bc9a2cd939700b29c2c2b68ac3ef`  
		Last Modified: Thu, 02 Mar 2023 12:28:30 GMT  
		Size: 10.1 MB (10122179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6288af56a458618c741df9cab3be4072895bce454b48f0073addf0f6da952616
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422932923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402dcb9e4c4c82f607da7e660dd32ab52a4682e7ce6343de3ef78d0e8bc24ca8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:16:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 03:20:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:20:16 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:21:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:22:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:23:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcb6c39567ec9b2c7ea7bca3bf033f2f41f3a4c07d089b9de2d8a14bab3292`  
		Last Modified: Thu, 02 Mar 2023 04:04:42 GMT  
		Size: 818.9 KB (818853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c5391c267d74199876bc0f614d5b80ad1e03948938fecf4d80e0ab49f7c90`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 4.5 MB (4461697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65a69abc68e01cb3f3e8e00001fc0ff966cd84b753e82111e495e9d319ee03d`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151a1078cd0202754dec71f67746b6c116798ceaaec93e1fd31ae3fd305b501`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2b2ae19293c39a9abe7ed81542deaf9824db2f84b81e2cbe87c4b55e01fb8`  
		Last Modified: Thu, 02 Mar 2023 04:05:13 GMT  
		Size: 252.5 MB (252548696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae119db2c7c4ffba52e20aea0bf61b6e9bb6a81bb69236b7177610e3d8d3faf`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf304e76035eea24e63c6f8df3b3226e6af34ae05635d41819e5084f1ad6717c`  
		Last Modified: Thu, 02 Mar 2023 04:05:28 GMT  
		Size: 63.1 MB (63096257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce94d2b7b5f6ce75418a3f1a7754706762dc89fb5ac7ae79de0c100223e5b594`  
		Last Modified: Thu, 02 Mar 2023 04:05:22 GMT  
		Size: 297.5 KB (297502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75def227e2b8440db3d1998106b192c98342ceab881d620f4a43be96b5876616`  
		Last Modified: Thu, 02 Mar 2023 04:05:32 GMT  
		Size: 67.2 MB (67234530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccaf24f26bfdcbe1f5d03582710621430bc9c5e2a7c5d27c2a38b824fe85e3be`  
		Last Modified: Thu, 02 Mar 2023 04:05:45 GMT  
		Size: 10.7 MB (10740003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:2b3882e1f5797d6595a18e66f892fc51d274bdfb938189f5d36b01d82bcf01a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:93ff17f047b26c4000ff1e18878fa6b7a9382144a3c7da9a35ba6a91daa48f13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.6 MB (437556445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d941256e42ae81c23437fb91cad81c68d0add57857c039dd828856052add40e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:17:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 07:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:09 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:21:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:21:10 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:21:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778654c0b435df260fd94e3a713e5ac0391d850b1dd50fc06d28724d697fd461`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 819.0 KB (819000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d3083a206086f721888a54dea32baf21c2cbc9155b39a9bac8631b20fede9`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 4.9 MB (4878631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3996b56577fbab1f217c1223e4ebab884c63ce1386b54be8a894044ad014a1d2`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff9d7fdf49d225218831b48c5847ebec87cb5bf3ea8cf9ab3eea0d1ef0e50a3`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e996788e40044c1f9c625c87249f7c8e303e5b8ed46020cad2d20e09982229d`  
		Last Modified: Thu, 02 Mar 2023 08:02:00 GMT  
		Size: 259.6 MB (259580317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9e9a8cb8917a1575d0a91f4e93b6a1d90ce64013c9d9648ad09eb9ef72e24`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360c9e013d6493daea567582a2a448f49a706cf4fded3acfd62c562004627daf`  
		Last Modified: Thu, 02 Mar 2023 08:02:18 GMT  
		Size: 70.3 MB (70267262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11487da93620b5bdb7d2f78eaf417d53227fed9b51f79df5cbbbdde4cd0da6`  
		Last Modified: Thu, 02 Mar 2023 08:02:09 GMT  
		Size: 297.5 KB (297495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c5f20223785c1f0757781aa7972ae767a9cbe64b3311b544ee8051d7e6a4c1`  
		Last Modified: Thu, 02 Mar 2023 08:02:20 GMT  
		Size: 75.0 MB (75000741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:e44ed680e0f8a8017636396ffdd9014c8c8942aee80f5aca1a37be4933236ba2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386040880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a9ff6e7934d64730587cd2da4d4ff2af00304d1805a1dc514b9be9dec6fd9a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:59:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 11:59:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 12:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:02:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:02:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:02:56 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:03:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:03:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b0874a47238c32833a1eb83551fa898735b969e33ba525c389d76a5973f18f`  
		Last Modified: Thu, 02 Mar 2023 12:27:23 GMT  
		Size: 819.1 KB (819062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca96c8d5fedefbf017ce0e41cecd02d40bb2d5b9093183b5889473daeda03`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 4.1 MB (4089642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c69e7b7b6ea014cc49dc25e4e3ad18bcc240bc2e96cd077a9618bfab8816e`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a769aaaa6a5a307f498af8c8bc3c3992f64f37b6d9f716dc2c0eddf7a13c2`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39727381991a44c63174e1b8193e9cc4386b91a936cca3b942c67cb58012e6d7`  
		Last Modified: Thu, 02 Mar 2023 12:27:54 GMT  
		Size: 239.0 MB (239045530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134249505ec9b290e4986fd60e7b3bf9da3ea895cf2609ef3b8a4f9ced66eead`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f49c73b5c2e574db7cbb840ea3132a051626d8ea7f869ead59ebd1b8448f601`  
		Last Modified: Thu, 02 Mar 2023 12:28:12 GMT  
		Size: 54.7 MB (54733714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3a64e4ebd696ce4cef7a0e94e6fa5022a1d218ed4f1ec9fcc479ccb03dfb26`  
		Last Modified: Thu, 02 Mar 2023 12:28:04 GMT  
		Size: 297.6 KB (297553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce032e347c9e1d2bbe0065495e4253363c1c7d7f8bf6a27570b03729f482058f`  
		Last Modified: Thu, 02 Mar 2023 12:28:15 GMT  
		Size: 64.7 MB (64749464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e270a7432c93f738fb6cb42ae04726c84dee53c855f2cb43c9fae71d373a7a6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412192920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afc8882704f4a7b5cd865f8bffa9416bc6ddb23ffdf7cbf0d0a81e4be623b99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:16:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 03:20:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:20:16 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:21:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:22:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcb6c39567ec9b2c7ea7bca3bf033f2f41f3a4c07d089b9de2d8a14bab3292`  
		Last Modified: Thu, 02 Mar 2023 04:04:42 GMT  
		Size: 818.9 KB (818853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c5391c267d74199876bc0f614d5b80ad1e03948938fecf4d80e0ab49f7c90`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 4.5 MB (4461697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65a69abc68e01cb3f3e8e00001fc0ff966cd84b753e82111e495e9d319ee03d`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151a1078cd0202754dec71f67746b6c116798ceaaec93e1fd31ae3fd305b501`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2b2ae19293c39a9abe7ed81542deaf9824db2f84b81e2cbe87c4b55e01fb8`  
		Last Modified: Thu, 02 Mar 2023 04:05:13 GMT  
		Size: 252.5 MB (252548696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae119db2c7c4ffba52e20aea0bf61b6e9bb6a81bb69236b7177610e3d8d3faf`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf304e76035eea24e63c6f8df3b3226e6af34ae05635d41819e5084f1ad6717c`  
		Last Modified: Thu, 02 Mar 2023 04:05:28 GMT  
		Size: 63.1 MB (63096257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce94d2b7b5f6ce75418a3f1a7754706762dc89fb5ac7ae79de0c100223e5b594`  
		Last Modified: Thu, 02 Mar 2023 04:05:22 GMT  
		Size: 297.5 KB (297502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75def227e2b8440db3d1998106b192c98342ceab881d620f4a43be96b5876616`  
		Last Modified: Thu, 02 Mar 2023 04:05:32 GMT  
		Size: 67.2 MB (67234530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:2b3882e1f5797d6595a18e66f892fc51d274bdfb938189f5d36b01d82bcf01a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:93ff17f047b26c4000ff1e18878fa6b7a9382144a3c7da9a35ba6a91daa48f13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.6 MB (437556445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d941256e42ae81c23437fb91cad81c68d0add57857c039dd828856052add40e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:17:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 07:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:09 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:21:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:21:10 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:21:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778654c0b435df260fd94e3a713e5ac0391d850b1dd50fc06d28724d697fd461`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 819.0 KB (819000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d3083a206086f721888a54dea32baf21c2cbc9155b39a9bac8631b20fede9`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 4.9 MB (4878631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3996b56577fbab1f217c1223e4ebab884c63ce1386b54be8a894044ad014a1d2`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff9d7fdf49d225218831b48c5847ebec87cb5bf3ea8cf9ab3eea0d1ef0e50a3`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e996788e40044c1f9c625c87249f7c8e303e5b8ed46020cad2d20e09982229d`  
		Last Modified: Thu, 02 Mar 2023 08:02:00 GMT  
		Size: 259.6 MB (259580317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9e9a8cb8917a1575d0a91f4e93b6a1d90ce64013c9d9648ad09eb9ef72e24`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360c9e013d6493daea567582a2a448f49a706cf4fded3acfd62c562004627daf`  
		Last Modified: Thu, 02 Mar 2023 08:02:18 GMT  
		Size: 70.3 MB (70267262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11487da93620b5bdb7d2f78eaf417d53227fed9b51f79df5cbbbdde4cd0da6`  
		Last Modified: Thu, 02 Mar 2023 08:02:09 GMT  
		Size: 297.5 KB (297495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c5f20223785c1f0757781aa7972ae767a9cbe64b3311b544ee8051d7e6a4c1`  
		Last Modified: Thu, 02 Mar 2023 08:02:20 GMT  
		Size: 75.0 MB (75000741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:e44ed680e0f8a8017636396ffdd9014c8c8942aee80f5aca1a37be4933236ba2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386040880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a9ff6e7934d64730587cd2da4d4ff2af00304d1805a1dc514b9be9dec6fd9a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:59:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 11:59:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 12:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:02:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:02:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:02:56 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:03:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:03:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b0874a47238c32833a1eb83551fa898735b969e33ba525c389d76a5973f18f`  
		Last Modified: Thu, 02 Mar 2023 12:27:23 GMT  
		Size: 819.1 KB (819062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca96c8d5fedefbf017ce0e41cecd02d40bb2d5b9093183b5889473daeda03`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 4.1 MB (4089642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c69e7b7b6ea014cc49dc25e4e3ad18bcc240bc2e96cd077a9618bfab8816e`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a769aaaa6a5a307f498af8c8bc3c3992f64f37b6d9f716dc2c0eddf7a13c2`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39727381991a44c63174e1b8193e9cc4386b91a936cca3b942c67cb58012e6d7`  
		Last Modified: Thu, 02 Mar 2023 12:27:54 GMT  
		Size: 239.0 MB (239045530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134249505ec9b290e4986fd60e7b3bf9da3ea895cf2609ef3b8a4f9ced66eead`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f49c73b5c2e574db7cbb840ea3132a051626d8ea7f869ead59ebd1b8448f601`  
		Last Modified: Thu, 02 Mar 2023 12:28:12 GMT  
		Size: 54.7 MB (54733714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3a64e4ebd696ce4cef7a0e94e6fa5022a1d218ed4f1ec9fcc479ccb03dfb26`  
		Last Modified: Thu, 02 Mar 2023 12:28:04 GMT  
		Size: 297.6 KB (297553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce032e347c9e1d2bbe0065495e4253363c1c7d7f8bf6a27570b03729f482058f`  
		Last Modified: Thu, 02 Mar 2023 12:28:15 GMT  
		Size: 64.7 MB (64749464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e270a7432c93f738fb6cb42ae04726c84dee53c855f2cb43c9fae71d373a7a6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412192920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afc8882704f4a7b5cd865f8bffa9416bc6ddb23ffdf7cbf0d0a81e4be623b99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:16:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 03:20:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:20:16 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:21:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:22:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcb6c39567ec9b2c7ea7bca3bf033f2f41f3a4c07d089b9de2d8a14bab3292`  
		Last Modified: Thu, 02 Mar 2023 04:04:42 GMT  
		Size: 818.9 KB (818853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c5391c267d74199876bc0f614d5b80ad1e03948938fecf4d80e0ab49f7c90`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 4.5 MB (4461697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65a69abc68e01cb3f3e8e00001fc0ff966cd84b753e82111e495e9d319ee03d`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151a1078cd0202754dec71f67746b6c116798ceaaec93e1fd31ae3fd305b501`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2b2ae19293c39a9abe7ed81542deaf9824db2f84b81e2cbe87c4b55e01fb8`  
		Last Modified: Thu, 02 Mar 2023 04:05:13 GMT  
		Size: 252.5 MB (252548696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae119db2c7c4ffba52e20aea0bf61b6e9bb6a81bb69236b7177610e3d8d3faf`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf304e76035eea24e63c6f8df3b3226e6af34ae05635d41819e5084f1ad6717c`  
		Last Modified: Thu, 02 Mar 2023 04:05:28 GMT  
		Size: 63.1 MB (63096257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce94d2b7b5f6ce75418a3f1a7754706762dc89fb5ac7ae79de0c100223e5b594`  
		Last Modified: Thu, 02 Mar 2023 04:05:22 GMT  
		Size: 297.5 KB (297502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75def227e2b8440db3d1998106b192c98342ceab881d620f4a43be96b5876616`  
		Last Modified: Thu, 02 Mar 2023 04:05:32 GMT  
		Size: 67.2 MB (67234530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:26ab3d4f0c179600d532cddb3e7a302bc078b8832c5326b005f23d90ec294ab0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:9c5263688f810644ca2b574aaea20528a8854a7824aded3f8bcac45e4bb1cfff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291990947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5895e7229f09cdc6495dce8551b0f865b3a8512108c62c987bc4149b0409143`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:17:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 07:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:09 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:21:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:21:10 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778654c0b435df260fd94e3a713e5ac0391d850b1dd50fc06d28724d697fd461`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 819.0 KB (819000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d3083a206086f721888a54dea32baf21c2cbc9155b39a9bac8631b20fede9`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 4.9 MB (4878631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3996b56577fbab1f217c1223e4ebab884c63ce1386b54be8a894044ad014a1d2`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff9d7fdf49d225218831b48c5847ebec87cb5bf3ea8cf9ab3eea0d1ef0e50a3`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e996788e40044c1f9c625c87249f7c8e303e5b8ed46020cad2d20e09982229d`  
		Last Modified: Thu, 02 Mar 2023 08:02:00 GMT  
		Size: 259.6 MB (259580317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9e9a8cb8917a1575d0a91f4e93b6a1d90ce64013c9d9648ad09eb9ef72e24`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:5f3987ab48ccd606364b53d6c197c52dc936598e195011659206011bbb722bc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266260149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e51dfcdecf577d494317e257a7779e5f06d3e8a3afec9f43f4847d650c7f0297`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:59:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 11:59:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 12:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:02:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:02:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:02:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b0874a47238c32833a1eb83551fa898735b969e33ba525c389d76a5973f18f`  
		Last Modified: Thu, 02 Mar 2023 12:27:23 GMT  
		Size: 819.1 KB (819062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca96c8d5fedefbf017ce0e41cecd02d40bb2d5b9093183b5889473daeda03`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 4.1 MB (4089642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c69e7b7b6ea014cc49dc25e4e3ad18bcc240bc2e96cd077a9618bfab8816e`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a769aaaa6a5a307f498af8c8bc3c3992f64f37b6d9f716dc2c0eddf7a13c2`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39727381991a44c63174e1b8193e9cc4386b91a936cca3b942c67cb58012e6d7`  
		Last Modified: Thu, 02 Mar 2023 12:27:54 GMT  
		Size: 239.0 MB (239045530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134249505ec9b290e4986fd60e7b3bf9da3ea895cf2609ef3b8a4f9ced66eead`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f4fdb424228f37cd137ffadf7b95bd312186d5f425c4d1ae7631c8acab304086
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281564631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:748356f92137700ffc2e8451c39d156388a6474e6e4aafe39f6a49c3c69a2cfe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:16:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 03:20:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:20:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcb6c39567ec9b2c7ea7bca3bf033f2f41f3a4c07d089b9de2d8a14bab3292`  
		Last Modified: Thu, 02 Mar 2023 04:04:42 GMT  
		Size: 818.9 KB (818853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c5391c267d74199876bc0f614d5b80ad1e03948938fecf4d80e0ab49f7c90`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 4.5 MB (4461697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65a69abc68e01cb3f3e8e00001fc0ff966cd84b753e82111e495e9d319ee03d`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151a1078cd0202754dec71f67746b6c116798ceaaec93e1fd31ae3fd305b501`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2b2ae19293c39a9abe7ed81542deaf9824db2f84b81e2cbe87c4b55e01fb8`  
		Last Modified: Thu, 02 Mar 2023 04:05:13 GMT  
		Size: 252.5 MB (252548696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae119db2c7c4ffba52e20aea0bf61b6e9bb6a81bb69236b7177610e3d8d3faf`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:26ab3d4f0c179600d532cddb3e7a302bc078b8832c5326b005f23d90ec294ab0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:9c5263688f810644ca2b574aaea20528a8854a7824aded3f8bcac45e4bb1cfff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291990947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5895e7229f09cdc6495dce8551b0f865b3a8512108c62c987bc4149b0409143`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:17:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 07:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:09 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:21:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:21:10 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778654c0b435df260fd94e3a713e5ac0391d850b1dd50fc06d28724d697fd461`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 819.0 KB (819000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d3083a206086f721888a54dea32baf21c2cbc9155b39a9bac8631b20fede9`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 4.9 MB (4878631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3996b56577fbab1f217c1223e4ebab884c63ce1386b54be8a894044ad014a1d2`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff9d7fdf49d225218831b48c5847ebec87cb5bf3ea8cf9ab3eea0d1ef0e50a3`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e996788e40044c1f9c625c87249f7c8e303e5b8ed46020cad2d20e09982229d`  
		Last Modified: Thu, 02 Mar 2023 08:02:00 GMT  
		Size: 259.6 MB (259580317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9e9a8cb8917a1575d0a91f4e93b6a1d90ce64013c9d9648ad09eb9ef72e24`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:5f3987ab48ccd606364b53d6c197c52dc936598e195011659206011bbb722bc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266260149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e51dfcdecf577d494317e257a7779e5f06d3e8a3afec9f43f4847d650c7f0297`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:59:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 11:59:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 12:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:02:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:02:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:02:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b0874a47238c32833a1eb83551fa898735b969e33ba525c389d76a5973f18f`  
		Last Modified: Thu, 02 Mar 2023 12:27:23 GMT  
		Size: 819.1 KB (819062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca96c8d5fedefbf017ce0e41cecd02d40bb2d5b9093183b5889473daeda03`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 4.1 MB (4089642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c69e7b7b6ea014cc49dc25e4e3ad18bcc240bc2e96cd077a9618bfab8816e`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a769aaaa6a5a307f498af8c8bc3c3992f64f37b6d9f716dc2c0eddf7a13c2`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39727381991a44c63174e1b8193e9cc4386b91a936cca3b942c67cb58012e6d7`  
		Last Modified: Thu, 02 Mar 2023 12:27:54 GMT  
		Size: 239.0 MB (239045530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134249505ec9b290e4986fd60e7b3bf9da3ea895cf2609ef3b8a4f9ced66eead`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f4fdb424228f37cd137ffadf7b95bd312186d5f425c4d1ae7631c8acab304086
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281564631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:748356f92137700ffc2e8451c39d156388a6474e6e4aafe39f6a49c3c69a2cfe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:16:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 03:20:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:20:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcb6c39567ec9b2c7ea7bca3bf033f2f41f3a4c07d089b9de2d8a14bab3292`  
		Last Modified: Thu, 02 Mar 2023 04:04:42 GMT  
		Size: 818.9 KB (818853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c5391c267d74199876bc0f614d5b80ad1e03948938fecf4d80e0ab49f7c90`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 4.5 MB (4461697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65a69abc68e01cb3f3e8e00001fc0ff966cd84b753e82111e495e9d319ee03d`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151a1078cd0202754dec71f67746b6c116798ceaaec93e1fd31ae3fd305b501`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2b2ae19293c39a9abe7ed81542deaf9824db2f84b81e2cbe87c4b55e01fb8`  
		Last Modified: Thu, 02 Mar 2023 04:05:13 GMT  
		Size: 252.5 MB (252548696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae119db2c7c4ffba52e20aea0bf61b6e9bb6a81bb69236b7177610e3d8d3faf`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:6544ba22bf4108def2c59cdb4666a2c4078185797809ba439bfda18151da7e31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:5985d5e9f4c663f2b91f620a71a93e68b6d6c7dd51099b8b64cb0ef8ac91c0b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343196661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87393749fffce7e59df69409d29e8d9c359bc11cbec3c4ae74a70fd90ee49b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 07:31:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:31:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:31:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:31:54 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:32:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:32:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752ff12fc1879563f6c3a37566aa1d63df61d32a482e1122678d06111c6c704`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb64a2fb206ee95fea7407d2fa098f13262e2dec6bd6acfc406eb3c7f3ee1e5`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2059687f395790fbfedafba19c2e4f73dd81bccae9ec7df3c7861b1df6886ca`  
		Last Modified: Thu, 02 Mar 2023 08:04:04 GMT  
		Size: 177.0 MB (177016208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1445ae9867c355c105face7eed407747aa39c1481c7133429c4c53f35088f16a`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d980596d1b73b63dea8c555dad924aed845b5cb90d0c7a4efcac51afe9a2f9a`  
		Last Modified: Thu, 02 Mar 2023 08:04:20 GMT  
		Size: 50.9 MB (50940124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a47bd281f5ba44bd21eda0d09fb13887e4d6c4fda7c69a3178992a9c83f88`  
		Last Modified: Thu, 02 Mar 2023 08:04:12 GMT  
		Size: 344.7 KB (344699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9ca0b3eec34631f459c101dd52259cac12e5132e1706dd716cef22ac1fe5ad`  
		Last Modified: Thu, 02 Mar 2023 08:04:24 GMT  
		Size: 79.6 MB (79606966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:14c689a399bcd7fe8f06113ee14d54d4b57157b7f4f7e0972d05be2b8f1424c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289275564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ab4552eb387f1971a6586c16ad9138a357b938f788b802f0a7839880707b63`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 12:12:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 12:12:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 12:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:15:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:15:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:15:45 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:16:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:16:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:18:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ea6bac35a1ab81469aabdf6a1f6f860ce1c9ed7e82625c53a6f8b1a64e823c`  
		Last Modified: Thu, 02 Mar 2023 12:29:30 GMT  
		Size: 1.2 MB (1154650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14af9ed8fe780bf6b1681423e06ab17566673bef9750c0b5591b03a7e12484`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 4.7 MB (4679133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4bc1671aa822702e1cd36abac0e9193c7a18d0ee42c398e454c47b02f193d`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b751eaf15e5904ee56e930eb3d87c9cc4ea0e10a3ae4f87ff3282b2c170f018`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a025315ed3938804103cdb57fc646fce4f4deeb9fbad47a00f203886109060e8`  
		Last Modified: Thu, 02 Mar 2023 12:29:56 GMT  
		Size: 157.5 MB (157509036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f6dbad8263386860670ffb777d531e98c9c6fe16503702f9d54f3e12f90e59`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d249e5b32be6ff0d611151ae4d2b63c966cef66818158da38c4091987a90409f`  
		Last Modified: Thu, 02 Mar 2023 12:30:15 GMT  
		Size: 40.5 MB (40502552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca015739736a2bd72291f44fcdb02fad7bb42e0f3d175dadec86956b6db0ac4`  
		Last Modified: Thu, 02 Mar 2023 12:30:09 GMT  
		Size: 344.7 KB (344697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30691ce4ba2eb6faf749bce8089a569dcb2925e478daff5e14a6824e0de2d8e3`  
		Last Modified: Thu, 02 Mar 2023 12:30:19 GMT  
		Size: 60.5 MB (60496631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:506e8db703e314af69b14807ebe528e947a5b1eb73889198f02ee54ec0da4c51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322891261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4212faa5635bbf446cfdd3501171661f3315d25db534b9067aff29deca32b14f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:29:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 03:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:32:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:32:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:32:40 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:33:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:33:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:35:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13947cb4d4fb29ac4bbd3748e79ab20da65033b2563147127613ccba352ba358`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a630cbcf281c994586155784a2c5c8a5c02f75715b54f9ec0fdd406eed859bf`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72441278ae08e882e2a05bfd9029475e9242e17a2f6b6d22859299db3b3e7f`  
		Last Modified: Thu, 02 Mar 2023 04:07:06 GMT  
		Size: 171.5 MB (171486823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee1963dd3f45dd61f69960595462707cd1dbabe500bcd3fa2b7cbd8ca6d63`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e5d1a2bcf7618178b56d1446e6c04fb2115af48f4fa2867c6789f1e58fca9e`  
		Last Modified: Thu, 02 Mar 2023 04:07:21 GMT  
		Size: 45.2 MB (45202848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fd00223ed309f05c64722f2df17f2327b9ee0ba7dad3204a61b8d28f08af6`  
		Last Modified: Thu, 02 Mar 2023 04:07:15 GMT  
		Size: 344.7 KB (344683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c981817b61382e14bd0208b60a2a288ac8ae59fc2941e85d8179eaffda1a938`  
		Last Modified: Thu, 02 Mar 2023 04:07:25 GMT  
		Size: 72.0 MB (71973530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:e0f2175cf9be5a46691b862fd29a2e0beffec1439df08c60b05f6e83c8bb9300
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:1125d4c624347752ce3fcf3e0556fbbf8c56fc4663e983fd67ff76129a50436d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835169484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768b4f8635c79f42cc5ee59f765f2d66c485156547018c19fe160247d9b45c20`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 07:31:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:31:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:31:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:31:54 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:32:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:32:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:40:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752ff12fc1879563f6c3a37566aa1d63df61d32a482e1122678d06111c6c704`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb64a2fb206ee95fea7407d2fa098f13262e2dec6bd6acfc406eb3c7f3ee1e5`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2059687f395790fbfedafba19c2e4f73dd81bccae9ec7df3c7861b1df6886ca`  
		Last Modified: Thu, 02 Mar 2023 08:04:04 GMT  
		Size: 177.0 MB (177016208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1445ae9867c355c105face7eed407747aa39c1481c7133429c4c53f35088f16a`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d980596d1b73b63dea8c555dad924aed845b5cb90d0c7a4efcac51afe9a2f9a`  
		Last Modified: Thu, 02 Mar 2023 08:04:20 GMT  
		Size: 50.9 MB (50940124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a47bd281f5ba44bd21eda0d09fb13887e4d6c4fda7c69a3178992a9c83f88`  
		Last Modified: Thu, 02 Mar 2023 08:04:12 GMT  
		Size: 344.7 KB (344699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9ca0b3eec34631f459c101dd52259cac12e5132e1706dd716cef22ac1fe5ad`  
		Last Modified: Thu, 02 Mar 2023 08:04:24 GMT  
		Size: 79.6 MB (79606966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc947c6624bf33d024b55571718244719b9a5edd2cca1c27afa1a4b480423782`  
		Last Modified: Thu, 02 Mar 2023 08:05:56 GMT  
		Size: 492.0 MB (491972823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:93e63c8844f4360dde7f320e76167dea05ee8f18a1bb7216fab4cccf901f4383
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726200713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d00b6305eebbad3d0fab34023a1646dc566a9bdf217beef3b18b78bcf440064e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 12:12:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 12:12:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 12:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:15:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:15:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:15:45 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:16:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:16:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:18:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:26:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ea6bac35a1ab81469aabdf6a1f6f860ce1c9ed7e82625c53a6f8b1a64e823c`  
		Last Modified: Thu, 02 Mar 2023 12:29:30 GMT  
		Size: 1.2 MB (1154650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14af9ed8fe780bf6b1681423e06ab17566673bef9750c0b5591b03a7e12484`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 4.7 MB (4679133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4bc1671aa822702e1cd36abac0e9193c7a18d0ee42c398e454c47b02f193d`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b751eaf15e5904ee56e930eb3d87c9cc4ea0e10a3ae4f87ff3282b2c170f018`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a025315ed3938804103cdb57fc646fce4f4deeb9fbad47a00f203886109060e8`  
		Last Modified: Thu, 02 Mar 2023 12:29:56 GMT  
		Size: 157.5 MB (157509036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f6dbad8263386860670ffb777d531e98c9c6fe16503702f9d54f3e12f90e59`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d249e5b32be6ff0d611151ae4d2b63c966cef66818158da38c4091987a90409f`  
		Last Modified: Thu, 02 Mar 2023 12:30:15 GMT  
		Size: 40.5 MB (40502552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca015739736a2bd72291f44fcdb02fad7bb42e0f3d175dadec86956b6db0ac4`  
		Last Modified: Thu, 02 Mar 2023 12:30:09 GMT  
		Size: 344.7 KB (344697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30691ce4ba2eb6faf749bce8089a569dcb2925e478daff5e14a6824e0de2d8e3`  
		Last Modified: Thu, 02 Mar 2023 12:30:19 GMT  
		Size: 60.5 MB (60496631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7b459fcfdca04b978505b7554f91d5d445a8883b151efd6443e40960489415`  
		Last Modified: Thu, 02 Mar 2023 12:31:45 GMT  
		Size: 436.9 MB (436925149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4826891ed564df798ff1b4aa5407feac941f6a54dc98a853ec9036856f9463cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.5 MB (785456931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9848de65ec4cfa6ab50210233a2530b2cc55a0f9ab478501b85b976c1e923dfb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:29:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 03:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:32:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:32:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:32:40 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:33:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:33:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:35:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13947cb4d4fb29ac4bbd3748e79ab20da65033b2563147127613ccba352ba358`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a630cbcf281c994586155784a2c5c8a5c02f75715b54f9ec0fdd406eed859bf`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72441278ae08e882e2a05bfd9029475e9242e17a2f6b6d22859299db3b3e7f`  
		Last Modified: Thu, 02 Mar 2023 04:07:06 GMT  
		Size: 171.5 MB (171486823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee1963dd3f45dd61f69960595462707cd1dbabe500bcd3fa2b7cbd8ca6d63`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e5d1a2bcf7618178b56d1446e6c04fb2115af48f4fa2867c6789f1e58fca9e`  
		Last Modified: Thu, 02 Mar 2023 04:07:21 GMT  
		Size: 45.2 MB (45202848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fd00223ed309f05c64722f2df17f2327b9ee0ba7dad3204a61b8d28f08af6`  
		Last Modified: Thu, 02 Mar 2023 04:07:15 GMT  
		Size: 344.7 KB (344683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c981817b61382e14bd0208b60a2a288ac8ae59fc2941e85d8179eaffda1a938`  
		Last Modified: Thu, 02 Mar 2023 04:07:25 GMT  
		Size: 72.0 MB (71973530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7950975947accb838c9965d22e2f50224d5b91a7bde53b6d7e48b00e18469ecb`  
		Last Modified: Thu, 02 Mar 2023 04:08:43 GMT  
		Size: 462.6 MB (462565670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:1688370b222e678fad42b09007a1a56a71cf197bf613bff44cae80512d1d607a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:ee2a4590ecf54b0be03ac546c5fc4dab8c7c6fcb46c4fa40a3b03ce7c3d6587d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.4 MB (951369401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a167e3e0e9034fc6638cde7fb25189f680ef793e507dc734e937154f50ad9af`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:09 GMT
ADD file:9ea7d74fdfdb29946ab72e1aea5810331debe27db7e50a0fc4e0d5a192ab6166 in / 
# Wed, 01 Mar 2023 04:10:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:01:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:01:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Mar 2023 17:01:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Mar 2023 17:01:13 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 17:01:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Mar 2023 17:01:13 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Mar 2023 17:02:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:02:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Mar 2023 17:02:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Mar 2023 17:02:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:03:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:03:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Mar 2023 17:03:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:07:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8a6bce2a40cb0c3e3cc6646bfeccfb2ac5b303c39ea70d67e30406d270f2009`  
		Last Modified: Wed, 01 Mar 2023 04:14:42 GMT  
		Size: 50.4 MB (50449101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a1ffc835f48ecec7c683701866277b285e39a42777bb6819d705ba54c9b7ee`  
		Last Modified: Wed, 01 Mar 2023 17:09:08 GMT  
		Size: 10.9 MB (10896984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ab4ec3b1ff1518ff16c31e9e4f4b239089fdad9819bb1b0806733d42d30b73`  
		Last Modified: Wed, 01 Mar 2023 17:09:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9841b85e22a255629ec6b026e828d764cdc3c990de2d2c70eef2cfa655083074`  
		Last Modified: Wed, 01 Mar 2023 17:09:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fcea5877730e4a516a82878a4f5f98da043bd4cc6f242e907c49f88c966f58`  
		Last Modified: Wed, 01 Mar 2023 17:09:38 GMT  
		Size: 239.2 MB (239240139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e461f854cd1f5763471d57c32aadc9f1bf067ff5b25408ead48199dee31c5f5`  
		Last Modified: Wed, 01 Mar 2023 17:09:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2b0f357d817701e8f5aa5dcd9f07b1ac984f80f3c9a9524a119394f9f67e49`  
		Last Modified: Wed, 01 Mar 2023 17:09:56 GMT  
		Size: 86.6 MB (86623675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e25a2a9e7feaf23a3d2bf9cef272554c05d1f79eb0dfb7cd0de7dc9c8eb0d42`  
		Last Modified: Wed, 01 Mar 2023 17:09:44 GMT  
		Size: 339.1 KB (339063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983285871d052c66975bf9eb2cbe185a844c7f586fd82d3003a0d5e980f6f61d`  
		Last Modified: Wed, 01 Mar 2023 17:09:54 GMT  
		Size: 76.0 MB (75978363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4324e50905e6727619201ae83db24d74ed4401fd0a768604a565d5401f04b9`  
		Last Modified: Wed, 01 Mar 2023 17:11:22 GMT  
		Size: 487.8 MB (487839664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:dd2c75dae72c51d1ffe2cbb71446d3378a08d78e4fefd4c0f95e67bd07b9283d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **868.2 MB (868161188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adf9fa79d061e4f865b9f453be54cf2de7d18307617d23374ba1238ce4404fb0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:46 GMT
ADD file:bf5b2f8cbddd98de6093dde190b043c3e2b58a5063d1acec0aba091e7d203dbd in / 
# Wed, 01 Mar 2023 02:20:47 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 12:29:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:29:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Mar 2023 12:29:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Mar 2023 12:29:13 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 12:29:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Mar 2023 12:29:13 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Mar 2023 12:30:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:30:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Mar 2023 12:30:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Mar 2023 12:30:41 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 12:31:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:31:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Mar 2023 12:31:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:35:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06cfbde07ccb39d53563bd87f3c2b50f04ddd0c8f6cd52be3c7089a3413688e1`  
		Last Modified: Wed, 01 Mar 2023 02:24:34 GMT  
		Size: 49.2 MB (49240002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a788fbcf95c26646fbabe7bb6f29416ca2663c0cfd87e1ccac361a7459568915`  
		Last Modified: Wed, 01 Mar 2023 12:37:20 GMT  
		Size: 10.9 MB (10902711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46d425485295faa6248cc3b6ce203089f5c51e6d6bd9ec2c65a3724f0986ba0`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de7b8f0c8434b3ef1c87e53a130007029f5fd37ea81634299d1e8226d10b4d5`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6b26d79f53cceae9c1d805e9d806a04c531a4290ef45b9f07bdc82202a1edd`  
		Last Modified: Wed, 01 Mar 2023 12:37:41 GMT  
		Size: 184.4 MB (184426336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e132bc958bc874cc517925ada16c2f3e782550fa85b319f3c4d921c3056fa77`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684edd9821b7de6b481112fbe45042cad36413aa11363fb633886c635a8f9671`  
		Last Modified: Wed, 01 Mar 2023 12:37:56 GMT  
		Size: 84.4 MB (84394773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca3197ee040ba7fb24fa4bd78b4b5706f52ca48e0aa05792b4d71282bf02b8c`  
		Last Modified: Wed, 01 Mar 2023 12:37:48 GMT  
		Size: 339.1 KB (339066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e66c8397888300bf62815d64b821ce057d0870bdde305763d3b14c7c7531f8c`  
		Last Modified: Wed, 01 Mar 2023 12:37:55 GMT  
		Size: 74.1 MB (74090620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7576684435d637fe5e0224e62bfeebb1d57a9bb4c8658ba6277c31eafb028042`  
		Last Modified: Wed, 01 Mar 2023 12:38:59 GMT  
		Size: 464.8 MB (464765268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:e0f2175cf9be5a46691b862fd29a2e0beffec1439df08c60b05f6e83c8bb9300
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:1125d4c624347752ce3fcf3e0556fbbf8c56fc4663e983fd67ff76129a50436d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835169484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768b4f8635c79f42cc5ee59f765f2d66c485156547018c19fe160247d9b45c20`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 07:31:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:31:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:31:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:31:54 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:32:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:32:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:40:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752ff12fc1879563f6c3a37566aa1d63df61d32a482e1122678d06111c6c704`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb64a2fb206ee95fea7407d2fa098f13262e2dec6bd6acfc406eb3c7f3ee1e5`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2059687f395790fbfedafba19c2e4f73dd81bccae9ec7df3c7861b1df6886ca`  
		Last Modified: Thu, 02 Mar 2023 08:04:04 GMT  
		Size: 177.0 MB (177016208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1445ae9867c355c105face7eed407747aa39c1481c7133429c4c53f35088f16a`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d980596d1b73b63dea8c555dad924aed845b5cb90d0c7a4efcac51afe9a2f9a`  
		Last Modified: Thu, 02 Mar 2023 08:04:20 GMT  
		Size: 50.9 MB (50940124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a47bd281f5ba44bd21eda0d09fb13887e4d6c4fda7c69a3178992a9c83f88`  
		Last Modified: Thu, 02 Mar 2023 08:04:12 GMT  
		Size: 344.7 KB (344699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9ca0b3eec34631f459c101dd52259cac12e5132e1706dd716cef22ac1fe5ad`  
		Last Modified: Thu, 02 Mar 2023 08:04:24 GMT  
		Size: 79.6 MB (79606966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc947c6624bf33d024b55571718244719b9a5edd2cca1c27afa1a4b480423782`  
		Last Modified: Thu, 02 Mar 2023 08:05:56 GMT  
		Size: 492.0 MB (491972823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:93e63c8844f4360dde7f320e76167dea05ee8f18a1bb7216fab4cccf901f4383
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726200713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d00b6305eebbad3d0fab34023a1646dc566a9bdf217beef3b18b78bcf440064e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 12:12:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 12:12:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 12:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:15:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:15:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:15:45 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:16:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:16:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:18:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:26:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ea6bac35a1ab81469aabdf6a1f6f860ce1c9ed7e82625c53a6f8b1a64e823c`  
		Last Modified: Thu, 02 Mar 2023 12:29:30 GMT  
		Size: 1.2 MB (1154650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14af9ed8fe780bf6b1681423e06ab17566673bef9750c0b5591b03a7e12484`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 4.7 MB (4679133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4bc1671aa822702e1cd36abac0e9193c7a18d0ee42c398e454c47b02f193d`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b751eaf15e5904ee56e930eb3d87c9cc4ea0e10a3ae4f87ff3282b2c170f018`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a025315ed3938804103cdb57fc646fce4f4deeb9fbad47a00f203886109060e8`  
		Last Modified: Thu, 02 Mar 2023 12:29:56 GMT  
		Size: 157.5 MB (157509036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f6dbad8263386860670ffb777d531e98c9c6fe16503702f9d54f3e12f90e59`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d249e5b32be6ff0d611151ae4d2b63c966cef66818158da38c4091987a90409f`  
		Last Modified: Thu, 02 Mar 2023 12:30:15 GMT  
		Size: 40.5 MB (40502552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca015739736a2bd72291f44fcdb02fad7bb42e0f3d175dadec86956b6db0ac4`  
		Last Modified: Thu, 02 Mar 2023 12:30:09 GMT  
		Size: 344.7 KB (344697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30691ce4ba2eb6faf749bce8089a569dcb2925e478daff5e14a6824e0de2d8e3`  
		Last Modified: Thu, 02 Mar 2023 12:30:19 GMT  
		Size: 60.5 MB (60496631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7b459fcfdca04b978505b7554f91d5d445a8883b151efd6443e40960489415`  
		Last Modified: Thu, 02 Mar 2023 12:31:45 GMT  
		Size: 436.9 MB (436925149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4826891ed564df798ff1b4aa5407feac941f6a54dc98a853ec9036856f9463cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.5 MB (785456931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9848de65ec4cfa6ab50210233a2530b2cc55a0f9ab478501b85b976c1e923dfb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:29:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 03:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:32:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:32:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:32:40 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:33:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:33:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:35:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13947cb4d4fb29ac4bbd3748e79ab20da65033b2563147127613ccba352ba358`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a630cbcf281c994586155784a2c5c8a5c02f75715b54f9ec0fdd406eed859bf`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72441278ae08e882e2a05bfd9029475e9242e17a2f6b6d22859299db3b3e7f`  
		Last Modified: Thu, 02 Mar 2023 04:07:06 GMT  
		Size: 171.5 MB (171486823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee1963dd3f45dd61f69960595462707cd1dbabe500bcd3fa2b7cbd8ca6d63`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e5d1a2bcf7618178b56d1446e6c04fb2115af48f4fa2867c6789f1e58fca9e`  
		Last Modified: Thu, 02 Mar 2023 04:07:21 GMT  
		Size: 45.2 MB (45202848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fd00223ed309f05c64722f2df17f2327b9ee0ba7dad3204a61b8d28f08af6`  
		Last Modified: Thu, 02 Mar 2023 04:07:15 GMT  
		Size: 344.7 KB (344683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c981817b61382e14bd0208b60a2a288ac8ae59fc2941e85d8179eaffda1a938`  
		Last Modified: Thu, 02 Mar 2023 04:07:25 GMT  
		Size: 72.0 MB (71973530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7950975947accb838c9965d22e2f50224d5b91a7bde53b6d7e48b00e18469ecb`  
		Last Modified: Thu, 02 Mar 2023 04:08:43 GMT  
		Size: 462.6 MB (462565670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:82d5bf035fe3b5c42e8688debe3e078b713540843cf505cceb88038e7d0273ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:a8d9060891e856521591f9715b2683979a0be65fd2089a8952747f53d9a46f38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359058260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624cf37ca7919de992e1c61d617325a34de7c33317fcf47334fd69a115f479f5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 07:31:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:31:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:31:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:31:54 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:32:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:32:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:34:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752ff12fc1879563f6c3a37566aa1d63df61d32a482e1122678d06111c6c704`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb64a2fb206ee95fea7407d2fa098f13262e2dec6bd6acfc406eb3c7f3ee1e5`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2059687f395790fbfedafba19c2e4f73dd81bccae9ec7df3c7861b1df6886ca`  
		Last Modified: Thu, 02 Mar 2023 08:04:04 GMT  
		Size: 177.0 MB (177016208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1445ae9867c355c105face7eed407747aa39c1481c7133429c4c53f35088f16a`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d980596d1b73b63dea8c555dad924aed845b5cb90d0c7a4efcac51afe9a2f9a`  
		Last Modified: Thu, 02 Mar 2023 08:04:20 GMT  
		Size: 50.9 MB (50940124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a47bd281f5ba44bd21eda0d09fb13887e4d6c4fda7c69a3178992a9c83f88`  
		Last Modified: Thu, 02 Mar 2023 08:04:12 GMT  
		Size: 344.7 KB (344699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9ca0b3eec34631f459c101dd52259cac12e5132e1706dd716cef22ac1fe5ad`  
		Last Modified: Thu, 02 Mar 2023 08:04:24 GMT  
		Size: 79.6 MB (79606966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f798b4c9c20b8496ae911b3d6bb2271e57fe9be07c5881b9793d305dd5d4d714`  
		Last Modified: Thu, 02 Mar 2023 08:04:37 GMT  
		Size: 15.9 MB (15861599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:d89461b84e435b7fa403ba650b692a892fcc9060b1b1afe2c0fa17e6325cc329
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303342434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452cd9a62c22e328d62d626f7e459e8092629e9a6558305320a5d56a83a8af1c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 12:12:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 12:12:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 12:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:15:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:15:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:15:45 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:16:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:16:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:18:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:19:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ea6bac35a1ab81469aabdf6a1f6f860ce1c9ed7e82625c53a6f8b1a64e823c`  
		Last Modified: Thu, 02 Mar 2023 12:29:30 GMT  
		Size: 1.2 MB (1154650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14af9ed8fe780bf6b1681423e06ab17566673bef9750c0b5591b03a7e12484`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 4.7 MB (4679133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4bc1671aa822702e1cd36abac0e9193c7a18d0ee42c398e454c47b02f193d`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b751eaf15e5904ee56e930eb3d87c9cc4ea0e10a3ae4f87ff3282b2c170f018`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a025315ed3938804103cdb57fc646fce4f4deeb9fbad47a00f203886109060e8`  
		Last Modified: Thu, 02 Mar 2023 12:29:56 GMT  
		Size: 157.5 MB (157509036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f6dbad8263386860670ffb777d531e98c9c6fe16503702f9d54f3e12f90e59`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d249e5b32be6ff0d611151ae4d2b63c966cef66818158da38c4091987a90409f`  
		Last Modified: Thu, 02 Mar 2023 12:30:15 GMT  
		Size: 40.5 MB (40502552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca015739736a2bd72291f44fcdb02fad7bb42e0f3d175dadec86956b6db0ac4`  
		Last Modified: Thu, 02 Mar 2023 12:30:09 GMT  
		Size: 344.7 KB (344697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30691ce4ba2eb6faf749bce8089a569dcb2925e478daff5e14a6824e0de2d8e3`  
		Last Modified: Thu, 02 Mar 2023 12:30:19 GMT  
		Size: 60.5 MB (60496631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831678b0bf51f05cef0d09fb3452cc39d4ec3dc03c82feb283d6aa582e341a6f`  
		Last Modified: Thu, 02 Mar 2023 12:30:35 GMT  
		Size: 14.1 MB (14066870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:caaa0e825225cd40f175539b5ea209f98a87b00cca33db4dbfe656be51020dcc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338348326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b6a6e82b6c81ade07153b89a59f6c7e63e63075a98fdd8429a3ac34671a77ea`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:29:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 03:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:32:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:32:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:32:40 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:33:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:33:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:35:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:35:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13947cb4d4fb29ac4bbd3748e79ab20da65033b2563147127613ccba352ba358`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a630cbcf281c994586155784a2c5c8a5c02f75715b54f9ec0fdd406eed859bf`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72441278ae08e882e2a05bfd9029475e9242e17a2f6b6d22859299db3b3e7f`  
		Last Modified: Thu, 02 Mar 2023 04:07:06 GMT  
		Size: 171.5 MB (171486823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee1963dd3f45dd61f69960595462707cd1dbabe500bcd3fa2b7cbd8ca6d63`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e5d1a2bcf7618178b56d1446e6c04fb2115af48f4fa2867c6789f1e58fca9e`  
		Last Modified: Thu, 02 Mar 2023 04:07:21 GMT  
		Size: 45.2 MB (45202848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fd00223ed309f05c64722f2df17f2327b9ee0ba7dad3204a61b8d28f08af6`  
		Last Modified: Thu, 02 Mar 2023 04:07:15 GMT  
		Size: 344.7 KB (344683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c981817b61382e14bd0208b60a2a288ac8ae59fc2941e85d8179eaffda1a938`  
		Last Modified: Thu, 02 Mar 2023 04:07:25 GMT  
		Size: 72.0 MB (71973530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52f52cb51404f8e7e25b700451b7ccbc7fb4e559f57a9759625ee461c2fa934`  
		Last Modified: Thu, 02 Mar 2023 04:07:39 GMT  
		Size: 15.5 MB (15457065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:4ac19fe814f4fcc14484aaa2ceeed2006a0295f052ecf31bcf7aac4cff0f4c77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:bf0fba36da1ab60d2a1f54479ac9827729238660a3d33139ec57f51b46fe317f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.7 MB (484685923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30da8c8d1452a1dcd694f99f784dc52e0a117c88a7a55e4b9cffa8ae146aaf1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:09 GMT
ADD file:9ea7d74fdfdb29946ab72e1aea5810331debe27db7e50a0fc4e0d5a192ab6166 in / 
# Wed, 01 Mar 2023 04:10:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:01:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:01:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Mar 2023 17:01:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Mar 2023 17:01:13 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 17:01:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Mar 2023 17:01:13 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Mar 2023 17:02:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:02:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Mar 2023 17:02:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Mar 2023 17:02:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:03:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:03:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Mar 2023 17:03:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:04:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8a6bce2a40cb0c3e3cc6646bfeccfb2ac5b303c39ea70d67e30406d270f2009`  
		Last Modified: Wed, 01 Mar 2023 04:14:42 GMT  
		Size: 50.4 MB (50449101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a1ffc835f48ecec7c683701866277b285e39a42777bb6819d705ba54c9b7ee`  
		Last Modified: Wed, 01 Mar 2023 17:09:08 GMT  
		Size: 10.9 MB (10896984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ab4ec3b1ff1518ff16c31e9e4f4b239089fdad9819bb1b0806733d42d30b73`  
		Last Modified: Wed, 01 Mar 2023 17:09:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9841b85e22a255629ec6b026e828d764cdc3c990de2d2c70eef2cfa655083074`  
		Last Modified: Wed, 01 Mar 2023 17:09:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fcea5877730e4a516a82878a4f5f98da043bd4cc6f242e907c49f88c966f58`  
		Last Modified: Wed, 01 Mar 2023 17:09:38 GMT  
		Size: 239.2 MB (239240139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e461f854cd1f5763471d57c32aadc9f1bf067ff5b25408ead48199dee31c5f5`  
		Last Modified: Wed, 01 Mar 2023 17:09:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2b0f357d817701e8f5aa5dcd9f07b1ac984f80f3c9a9524a119394f9f67e49`  
		Last Modified: Wed, 01 Mar 2023 17:09:56 GMT  
		Size: 86.6 MB (86623675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e25a2a9e7feaf23a3d2bf9cef272554c05d1f79eb0dfb7cd0de7dc9c8eb0d42`  
		Last Modified: Wed, 01 Mar 2023 17:09:44 GMT  
		Size: 339.1 KB (339063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983285871d052c66975bf9eb2cbe185a844c7f586fd82d3003a0d5e980f6f61d`  
		Last Modified: Wed, 01 Mar 2023 17:09:54 GMT  
		Size: 76.0 MB (75978363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc393ef17f1c6bf4420e3ff6a2c30422a37cbb1f13df86c8d971e33dca19fe4`  
		Last Modified: Wed, 01 Mar 2023 17:10:05 GMT  
		Size: 21.2 MB (21156186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5f60b45ccb6ab1271ed9cc7efb6f11e9c0ca8b891e82b4f9881db630ae240030
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.2 MB (424215617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e48551368ac4ebee90f1cd089e2569e2739814ed992ab7a6fa66da36d51881a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:46 GMT
ADD file:bf5b2f8cbddd98de6093dde190b043c3e2b58a5063d1acec0aba091e7d203dbd in / 
# Wed, 01 Mar 2023 02:20:47 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 12:29:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:29:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Mar 2023 12:29:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Mar 2023 12:29:13 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 12:29:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Mar 2023 12:29:13 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Mar 2023 12:30:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:30:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Mar 2023 12:30:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Mar 2023 12:30:41 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 12:31:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:31:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Mar 2023 12:31:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:32:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06cfbde07ccb39d53563bd87f3c2b50f04ddd0c8f6cd52be3c7089a3413688e1`  
		Last Modified: Wed, 01 Mar 2023 02:24:34 GMT  
		Size: 49.2 MB (49240002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a788fbcf95c26646fbabe7bb6f29416ca2663c0cfd87e1ccac361a7459568915`  
		Last Modified: Wed, 01 Mar 2023 12:37:20 GMT  
		Size: 10.9 MB (10902711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46d425485295faa6248cc3b6ce203089f5c51e6d6bd9ec2c65a3724f0986ba0`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de7b8f0c8434b3ef1c87e53a130007029f5fd37ea81634299d1e8226d10b4d5`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6b26d79f53cceae9c1d805e9d806a04c531a4290ef45b9f07bdc82202a1edd`  
		Last Modified: Wed, 01 Mar 2023 12:37:41 GMT  
		Size: 184.4 MB (184426336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e132bc958bc874cc517925ada16c2f3e782550fa85b319f3c4d921c3056fa77`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684edd9821b7de6b481112fbe45042cad36413aa11363fb633886c635a8f9671`  
		Last Modified: Wed, 01 Mar 2023 12:37:56 GMT  
		Size: 84.4 MB (84394773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca3197ee040ba7fb24fa4bd78b4b5706f52ca48e0aa05792b4d71282bf02b8c`  
		Last Modified: Wed, 01 Mar 2023 12:37:48 GMT  
		Size: 339.1 KB (339066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e66c8397888300bf62815d64b821ce057d0870bdde305763d3b14c7c7531f8c`  
		Last Modified: Wed, 01 Mar 2023 12:37:55 GMT  
		Size: 74.1 MB (74090620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb6cb0f9628a2810ae12f64de2ed0d14b86dab3b639e2568dd649b652a664ea`  
		Last Modified: Wed, 01 Mar 2023 12:38:04 GMT  
		Size: 20.8 MB (20819697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:82d5bf035fe3b5c42e8688debe3e078b713540843cf505cceb88038e7d0273ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:a8d9060891e856521591f9715b2683979a0be65fd2089a8952747f53d9a46f38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.1 MB (359058260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624cf37ca7919de992e1c61d617325a34de7c33317fcf47334fd69a115f479f5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 07:31:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:31:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:31:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:31:54 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:32:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:32:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:34:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752ff12fc1879563f6c3a37566aa1d63df61d32a482e1122678d06111c6c704`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb64a2fb206ee95fea7407d2fa098f13262e2dec6bd6acfc406eb3c7f3ee1e5`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2059687f395790fbfedafba19c2e4f73dd81bccae9ec7df3c7861b1df6886ca`  
		Last Modified: Thu, 02 Mar 2023 08:04:04 GMT  
		Size: 177.0 MB (177016208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1445ae9867c355c105face7eed407747aa39c1481c7133429c4c53f35088f16a`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d980596d1b73b63dea8c555dad924aed845b5cb90d0c7a4efcac51afe9a2f9a`  
		Last Modified: Thu, 02 Mar 2023 08:04:20 GMT  
		Size: 50.9 MB (50940124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a47bd281f5ba44bd21eda0d09fb13887e4d6c4fda7c69a3178992a9c83f88`  
		Last Modified: Thu, 02 Mar 2023 08:04:12 GMT  
		Size: 344.7 KB (344699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9ca0b3eec34631f459c101dd52259cac12e5132e1706dd716cef22ac1fe5ad`  
		Last Modified: Thu, 02 Mar 2023 08:04:24 GMT  
		Size: 79.6 MB (79606966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f798b4c9c20b8496ae911b3d6bb2271e57fe9be07c5881b9793d305dd5d4d714`  
		Last Modified: Thu, 02 Mar 2023 08:04:37 GMT  
		Size: 15.9 MB (15861599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:d89461b84e435b7fa403ba650b692a892fcc9060b1b1afe2c0fa17e6325cc329
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303342434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452cd9a62c22e328d62d626f7e459e8092629e9a6558305320a5d56a83a8af1c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 12:12:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 12:12:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 12:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:15:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:15:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:15:45 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:16:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:16:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:18:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:19:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ea6bac35a1ab81469aabdf6a1f6f860ce1c9ed7e82625c53a6f8b1a64e823c`  
		Last Modified: Thu, 02 Mar 2023 12:29:30 GMT  
		Size: 1.2 MB (1154650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14af9ed8fe780bf6b1681423e06ab17566673bef9750c0b5591b03a7e12484`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 4.7 MB (4679133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4bc1671aa822702e1cd36abac0e9193c7a18d0ee42c398e454c47b02f193d`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b751eaf15e5904ee56e930eb3d87c9cc4ea0e10a3ae4f87ff3282b2c170f018`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a025315ed3938804103cdb57fc646fce4f4deeb9fbad47a00f203886109060e8`  
		Last Modified: Thu, 02 Mar 2023 12:29:56 GMT  
		Size: 157.5 MB (157509036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f6dbad8263386860670ffb777d531e98c9c6fe16503702f9d54f3e12f90e59`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d249e5b32be6ff0d611151ae4d2b63c966cef66818158da38c4091987a90409f`  
		Last Modified: Thu, 02 Mar 2023 12:30:15 GMT  
		Size: 40.5 MB (40502552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca015739736a2bd72291f44fcdb02fad7bb42e0f3d175dadec86956b6db0ac4`  
		Last Modified: Thu, 02 Mar 2023 12:30:09 GMT  
		Size: 344.7 KB (344697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30691ce4ba2eb6faf749bce8089a569dcb2925e478daff5e14a6824e0de2d8e3`  
		Last Modified: Thu, 02 Mar 2023 12:30:19 GMT  
		Size: 60.5 MB (60496631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831678b0bf51f05cef0d09fb3452cc39d4ec3dc03c82feb283d6aa582e341a6f`  
		Last Modified: Thu, 02 Mar 2023 12:30:35 GMT  
		Size: 14.1 MB (14066870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:caaa0e825225cd40f175539b5ea209f98a87b00cca33db4dbfe656be51020dcc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338348326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b6a6e82b6c81ade07153b89a59f6c7e63e63075a98fdd8429a3ac34671a77ea`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:29:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 03:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:32:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:32:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:32:40 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:33:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:33:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:35:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:35:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13947cb4d4fb29ac4bbd3748e79ab20da65033b2563147127613ccba352ba358`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a630cbcf281c994586155784a2c5c8a5c02f75715b54f9ec0fdd406eed859bf`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72441278ae08e882e2a05bfd9029475e9242e17a2f6b6d22859299db3b3e7f`  
		Last Modified: Thu, 02 Mar 2023 04:07:06 GMT  
		Size: 171.5 MB (171486823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee1963dd3f45dd61f69960595462707cd1dbabe500bcd3fa2b7cbd8ca6d63`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e5d1a2bcf7618178b56d1446e6c04fb2115af48f4fa2867c6789f1e58fca9e`  
		Last Modified: Thu, 02 Mar 2023 04:07:21 GMT  
		Size: 45.2 MB (45202848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fd00223ed309f05c64722f2df17f2327b9ee0ba7dad3204a61b8d28f08af6`  
		Last Modified: Thu, 02 Mar 2023 04:07:15 GMT  
		Size: 344.7 KB (344683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c981817b61382e14bd0208b60a2a288ac8ae59fc2941e85d8179eaffda1a938`  
		Last Modified: Thu, 02 Mar 2023 04:07:25 GMT  
		Size: 72.0 MB (71973530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52f52cb51404f8e7e25b700451b7ccbc7fb4e559f57a9759625ee461c2fa934`  
		Last Modified: Thu, 02 Mar 2023 04:07:39 GMT  
		Size: 15.5 MB (15457065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:6544ba22bf4108def2c59cdb4666a2c4078185797809ba439bfda18151da7e31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:5985d5e9f4c663f2b91f620a71a93e68b6d6c7dd51099b8b64cb0ef8ac91c0b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343196661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87393749fffce7e59df69409d29e8d9c359bc11cbec3c4ae74a70fd90ee49b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 07:31:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:31:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:31:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:31:54 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:32:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:32:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752ff12fc1879563f6c3a37566aa1d63df61d32a482e1122678d06111c6c704`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb64a2fb206ee95fea7407d2fa098f13262e2dec6bd6acfc406eb3c7f3ee1e5`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2059687f395790fbfedafba19c2e4f73dd81bccae9ec7df3c7861b1df6886ca`  
		Last Modified: Thu, 02 Mar 2023 08:04:04 GMT  
		Size: 177.0 MB (177016208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1445ae9867c355c105face7eed407747aa39c1481c7133429c4c53f35088f16a`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d980596d1b73b63dea8c555dad924aed845b5cb90d0c7a4efcac51afe9a2f9a`  
		Last Modified: Thu, 02 Mar 2023 08:04:20 GMT  
		Size: 50.9 MB (50940124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a47bd281f5ba44bd21eda0d09fb13887e4d6c4fda7c69a3178992a9c83f88`  
		Last Modified: Thu, 02 Mar 2023 08:04:12 GMT  
		Size: 344.7 KB (344699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9ca0b3eec34631f459c101dd52259cac12e5132e1706dd716cef22ac1fe5ad`  
		Last Modified: Thu, 02 Mar 2023 08:04:24 GMT  
		Size: 79.6 MB (79606966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:14c689a399bcd7fe8f06113ee14d54d4b57157b7f4f7e0972d05be2b8f1424c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289275564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ab4552eb387f1971a6586c16ad9138a357b938f788b802f0a7839880707b63`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 12:12:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 12:12:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 12:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:15:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:15:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:15:45 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:16:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:16:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:18:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ea6bac35a1ab81469aabdf6a1f6f860ce1c9ed7e82625c53a6f8b1a64e823c`  
		Last Modified: Thu, 02 Mar 2023 12:29:30 GMT  
		Size: 1.2 MB (1154650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14af9ed8fe780bf6b1681423e06ab17566673bef9750c0b5591b03a7e12484`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 4.7 MB (4679133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4bc1671aa822702e1cd36abac0e9193c7a18d0ee42c398e454c47b02f193d`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b751eaf15e5904ee56e930eb3d87c9cc4ea0e10a3ae4f87ff3282b2c170f018`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a025315ed3938804103cdb57fc646fce4f4deeb9fbad47a00f203886109060e8`  
		Last Modified: Thu, 02 Mar 2023 12:29:56 GMT  
		Size: 157.5 MB (157509036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f6dbad8263386860670ffb777d531e98c9c6fe16503702f9d54f3e12f90e59`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d249e5b32be6ff0d611151ae4d2b63c966cef66818158da38c4091987a90409f`  
		Last Modified: Thu, 02 Mar 2023 12:30:15 GMT  
		Size: 40.5 MB (40502552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca015739736a2bd72291f44fcdb02fad7bb42e0f3d175dadec86956b6db0ac4`  
		Last Modified: Thu, 02 Mar 2023 12:30:09 GMT  
		Size: 344.7 KB (344697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30691ce4ba2eb6faf749bce8089a569dcb2925e478daff5e14a6824e0de2d8e3`  
		Last Modified: Thu, 02 Mar 2023 12:30:19 GMT  
		Size: 60.5 MB (60496631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:506e8db703e314af69b14807ebe528e947a5b1eb73889198f02ee54ec0da4c51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322891261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4212faa5635bbf446cfdd3501171661f3315d25db534b9067aff29deca32b14f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:29:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 03:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:32:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:32:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:32:40 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:33:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:33:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:35:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13947cb4d4fb29ac4bbd3748e79ab20da65033b2563147127613ccba352ba358`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a630cbcf281c994586155784a2c5c8a5c02f75715b54f9ec0fdd406eed859bf`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72441278ae08e882e2a05bfd9029475e9242e17a2f6b6d22859299db3b3e7f`  
		Last Modified: Thu, 02 Mar 2023 04:07:06 GMT  
		Size: 171.5 MB (171486823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee1963dd3f45dd61f69960595462707cd1dbabe500bcd3fa2b7cbd8ca6d63`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e5d1a2bcf7618178b56d1446e6c04fb2115af48f4fa2867c6789f1e58fca9e`  
		Last Modified: Thu, 02 Mar 2023 04:07:21 GMT  
		Size: 45.2 MB (45202848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fd00223ed309f05c64722f2df17f2327b9ee0ba7dad3204a61b8d28f08af6`  
		Last Modified: Thu, 02 Mar 2023 04:07:15 GMT  
		Size: 344.7 KB (344683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c981817b61382e14bd0208b60a2a288ac8ae59fc2941e85d8179eaffda1a938`  
		Last Modified: Thu, 02 Mar 2023 04:07:25 GMT  
		Size: 72.0 MB (71973530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:62de5f69aa6d7742900b02ef2ba5344489317640e60df7309b67661e0985bfc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:ba18990ef69c0cab2f459b1f9572031be815cce209686a01ff338760cf35e199
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.5 MB (463529737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:420cddd5ca50a0c5d8bee50528173e8043d16732a804927de44090359dc60de8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:09 GMT
ADD file:9ea7d74fdfdb29946ab72e1aea5810331debe27db7e50a0fc4e0d5a192ab6166 in / 
# Wed, 01 Mar 2023 04:10:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:01:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:01:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Mar 2023 17:01:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Mar 2023 17:01:13 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 17:01:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Mar 2023 17:01:13 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Mar 2023 17:02:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:02:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Mar 2023 17:02:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Mar 2023 17:02:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:03:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:03:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Mar 2023 17:03:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8a6bce2a40cb0c3e3cc6646bfeccfb2ac5b303c39ea70d67e30406d270f2009`  
		Last Modified: Wed, 01 Mar 2023 04:14:42 GMT  
		Size: 50.4 MB (50449101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a1ffc835f48ecec7c683701866277b285e39a42777bb6819d705ba54c9b7ee`  
		Last Modified: Wed, 01 Mar 2023 17:09:08 GMT  
		Size: 10.9 MB (10896984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ab4ec3b1ff1518ff16c31e9e4f4b239089fdad9819bb1b0806733d42d30b73`  
		Last Modified: Wed, 01 Mar 2023 17:09:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9841b85e22a255629ec6b026e828d764cdc3c990de2d2c70eef2cfa655083074`  
		Last Modified: Wed, 01 Mar 2023 17:09:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fcea5877730e4a516a82878a4f5f98da043bd4cc6f242e907c49f88c966f58`  
		Last Modified: Wed, 01 Mar 2023 17:09:38 GMT  
		Size: 239.2 MB (239240139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e461f854cd1f5763471d57c32aadc9f1bf067ff5b25408ead48199dee31c5f5`  
		Last Modified: Wed, 01 Mar 2023 17:09:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2b0f357d817701e8f5aa5dcd9f07b1ac984f80f3c9a9524a119394f9f67e49`  
		Last Modified: Wed, 01 Mar 2023 17:09:56 GMT  
		Size: 86.6 MB (86623675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e25a2a9e7feaf23a3d2bf9cef272554c05d1f79eb0dfb7cd0de7dc9c8eb0d42`  
		Last Modified: Wed, 01 Mar 2023 17:09:44 GMT  
		Size: 339.1 KB (339063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983285871d052c66975bf9eb2cbe185a844c7f586fd82d3003a0d5e980f6f61d`  
		Last Modified: Wed, 01 Mar 2023 17:09:54 GMT  
		Size: 76.0 MB (75978363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c9fe16a6c88247f34d045e5545958241a43f85a4af090abfff2c6073cf9268b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.4 MB (403395920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1eb289d9a5acd82cc16eef02ad24f244b129bf50816fefd2f8492160493ed60`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:46 GMT
ADD file:bf5b2f8cbddd98de6093dde190b043c3e2b58a5063d1acec0aba091e7d203dbd in / 
# Wed, 01 Mar 2023 02:20:47 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 12:29:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:29:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Mar 2023 12:29:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Mar 2023 12:29:13 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 12:29:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Mar 2023 12:29:13 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Mar 2023 12:30:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:30:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Mar 2023 12:30:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Mar 2023 12:30:41 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 12:31:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:31:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Mar 2023 12:31:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06cfbde07ccb39d53563bd87f3c2b50f04ddd0c8f6cd52be3c7089a3413688e1`  
		Last Modified: Wed, 01 Mar 2023 02:24:34 GMT  
		Size: 49.2 MB (49240002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a788fbcf95c26646fbabe7bb6f29416ca2663c0cfd87e1ccac361a7459568915`  
		Last Modified: Wed, 01 Mar 2023 12:37:20 GMT  
		Size: 10.9 MB (10902711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46d425485295faa6248cc3b6ce203089f5c51e6d6bd9ec2c65a3724f0986ba0`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de7b8f0c8434b3ef1c87e53a130007029f5fd37ea81634299d1e8226d10b4d5`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6b26d79f53cceae9c1d805e9d806a04c531a4290ef45b9f07bdc82202a1edd`  
		Last Modified: Wed, 01 Mar 2023 12:37:41 GMT  
		Size: 184.4 MB (184426336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e132bc958bc874cc517925ada16c2f3e782550fa85b319f3c4d921c3056fa77`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684edd9821b7de6b481112fbe45042cad36413aa11363fb633886c635a8f9671`  
		Last Modified: Wed, 01 Mar 2023 12:37:56 GMT  
		Size: 84.4 MB (84394773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca3197ee040ba7fb24fa4bd78b4b5706f52ca48e0aa05792b4d71282bf02b8c`  
		Last Modified: Wed, 01 Mar 2023 12:37:48 GMT  
		Size: 339.1 KB (339066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e66c8397888300bf62815d64b821ce057d0870bdde305763d3b14c7c7531f8c`  
		Last Modified: Wed, 01 Mar 2023 12:37:55 GMT  
		Size: 74.1 MB (74090620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:6544ba22bf4108def2c59cdb4666a2c4078185797809ba439bfda18151da7e31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:5985d5e9f4c663f2b91f620a71a93e68b6d6c7dd51099b8b64cb0ef8ac91c0b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343196661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87393749fffce7e59df69409d29e8d9c359bc11cbec3c4ae74a70fd90ee49b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 07:31:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:31:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:31:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:31:54 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:32:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:32:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752ff12fc1879563f6c3a37566aa1d63df61d32a482e1122678d06111c6c704`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb64a2fb206ee95fea7407d2fa098f13262e2dec6bd6acfc406eb3c7f3ee1e5`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2059687f395790fbfedafba19c2e4f73dd81bccae9ec7df3c7861b1df6886ca`  
		Last Modified: Thu, 02 Mar 2023 08:04:04 GMT  
		Size: 177.0 MB (177016208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1445ae9867c355c105face7eed407747aa39c1481c7133429c4c53f35088f16a`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d980596d1b73b63dea8c555dad924aed845b5cb90d0c7a4efcac51afe9a2f9a`  
		Last Modified: Thu, 02 Mar 2023 08:04:20 GMT  
		Size: 50.9 MB (50940124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a47bd281f5ba44bd21eda0d09fb13887e4d6c4fda7c69a3178992a9c83f88`  
		Last Modified: Thu, 02 Mar 2023 08:04:12 GMT  
		Size: 344.7 KB (344699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9ca0b3eec34631f459c101dd52259cac12e5132e1706dd716cef22ac1fe5ad`  
		Last Modified: Thu, 02 Mar 2023 08:04:24 GMT  
		Size: 79.6 MB (79606966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:14c689a399bcd7fe8f06113ee14d54d4b57157b7f4f7e0972d05be2b8f1424c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289275564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ab4552eb387f1971a6586c16ad9138a357b938f788b802f0a7839880707b63`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 12:12:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 12:12:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 12:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:15:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:15:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:15:45 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:16:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:16:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:18:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ea6bac35a1ab81469aabdf6a1f6f860ce1c9ed7e82625c53a6f8b1a64e823c`  
		Last Modified: Thu, 02 Mar 2023 12:29:30 GMT  
		Size: 1.2 MB (1154650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14af9ed8fe780bf6b1681423e06ab17566673bef9750c0b5591b03a7e12484`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 4.7 MB (4679133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4bc1671aa822702e1cd36abac0e9193c7a18d0ee42c398e454c47b02f193d`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b751eaf15e5904ee56e930eb3d87c9cc4ea0e10a3ae4f87ff3282b2c170f018`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a025315ed3938804103cdb57fc646fce4f4deeb9fbad47a00f203886109060e8`  
		Last Modified: Thu, 02 Mar 2023 12:29:56 GMT  
		Size: 157.5 MB (157509036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f6dbad8263386860670ffb777d531e98c9c6fe16503702f9d54f3e12f90e59`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d249e5b32be6ff0d611151ae4d2b63c966cef66818158da38c4091987a90409f`  
		Last Modified: Thu, 02 Mar 2023 12:30:15 GMT  
		Size: 40.5 MB (40502552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca015739736a2bd72291f44fcdb02fad7bb42e0f3d175dadec86956b6db0ac4`  
		Last Modified: Thu, 02 Mar 2023 12:30:09 GMT  
		Size: 344.7 KB (344697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30691ce4ba2eb6faf749bce8089a569dcb2925e478daff5e14a6824e0de2d8e3`  
		Last Modified: Thu, 02 Mar 2023 12:30:19 GMT  
		Size: 60.5 MB (60496631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:506e8db703e314af69b14807ebe528e947a5b1eb73889198f02ee54ec0da4c51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322891261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4212faa5635bbf446cfdd3501171661f3315d25db534b9067aff29deca32b14f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:29:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 03:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:32:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:32:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:32:40 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:33:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:33:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:35:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13947cb4d4fb29ac4bbd3748e79ab20da65033b2563147127613ccba352ba358`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a630cbcf281c994586155784a2c5c8a5c02f75715b54f9ec0fdd406eed859bf`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72441278ae08e882e2a05bfd9029475e9242e17a2f6b6d22859299db3b3e7f`  
		Last Modified: Thu, 02 Mar 2023 04:07:06 GMT  
		Size: 171.5 MB (171486823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee1963dd3f45dd61f69960595462707cd1dbabe500bcd3fa2b7cbd8ca6d63`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e5d1a2bcf7618178b56d1446e6c04fb2115af48f4fa2867c6789f1e58fca9e`  
		Last Modified: Thu, 02 Mar 2023 04:07:21 GMT  
		Size: 45.2 MB (45202848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fd00223ed309f05c64722f2df17f2327b9ee0ba7dad3204a61b8d28f08af6`  
		Last Modified: Thu, 02 Mar 2023 04:07:15 GMT  
		Size: 344.7 KB (344683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c981817b61382e14bd0208b60a2a288ac8ae59fc2941e85d8179eaffda1a938`  
		Last Modified: Thu, 02 Mar 2023 04:07:25 GMT  
		Size: 72.0 MB (71973530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:99d7682251e5c2cddc908d3f2f2fa804311a0e6b668ffa238cde939e5e602255
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:5699cc68b1831fc92aa7d1a4c63f7a732f1ee3ce027e805c907cd6cdf88955c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212304872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60534a72b997b5dcce45b1a81e2c3715e7c9b7629c7c6e2ff5371fe385b1bbad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 07:31:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:31:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:31:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:31:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752ff12fc1879563f6c3a37566aa1d63df61d32a482e1122678d06111c6c704`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb64a2fb206ee95fea7407d2fa098f13262e2dec6bd6acfc406eb3c7f3ee1e5`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2059687f395790fbfedafba19c2e4f73dd81bccae9ec7df3c7861b1df6886ca`  
		Last Modified: Thu, 02 Mar 2023 08:04:04 GMT  
		Size: 177.0 MB (177016208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1445ae9867c355c105face7eed407747aa39c1481c7133429c4c53f35088f16a`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:93dc53559685aecb2fda770e70acc564d4f877c3fbaf90b42aa5c70781140820
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187931684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365ea3d85c1c823fa8304fd7d8118343f4c9d55375236d7c9d6072da3ba8d815`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 12:12:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 12:12:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 12:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:15:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:15:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:15:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ea6bac35a1ab81469aabdf6a1f6f860ce1c9ed7e82625c53a6f8b1a64e823c`  
		Last Modified: Thu, 02 Mar 2023 12:29:30 GMT  
		Size: 1.2 MB (1154650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14af9ed8fe780bf6b1681423e06ab17566673bef9750c0b5591b03a7e12484`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 4.7 MB (4679133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4bc1671aa822702e1cd36abac0e9193c7a18d0ee42c398e454c47b02f193d`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b751eaf15e5904ee56e930eb3d87c9cc4ea0e10a3ae4f87ff3282b2c170f018`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a025315ed3938804103cdb57fc646fce4f4deeb9fbad47a00f203886109060e8`  
		Last Modified: Thu, 02 Mar 2023 12:29:56 GMT  
		Size: 157.5 MB (157509036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f6dbad8263386860670ffb777d531e98c9c6fe16503702f9d54f3e12f90e59`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:75b39f2eb13e7db3653d56e63728799a3e25c6bf7868c6b02318922fbe17e7d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205370200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31ae095b06299fee387b279f3f2e0ed1f4eabe255a73826905e51bd7b9aa1575`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:29:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 03:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:32:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:32:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:32:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13947cb4d4fb29ac4bbd3748e79ab20da65033b2563147127613ccba352ba358`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a630cbcf281c994586155784a2c5c8a5c02f75715b54f9ec0fdd406eed859bf`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72441278ae08e882e2a05bfd9029475e9242e17a2f6b6d22859299db3b3e7f`  
		Last Modified: Thu, 02 Mar 2023 04:07:06 GMT  
		Size: 171.5 MB (171486823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee1963dd3f45dd61f69960595462707cd1dbabe500bcd3fa2b7cbd8ca6d63`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:bad4044bc668cd6eed1fcc56f771c626a9038dbe8725ed2395ffc2841f1f4c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:7785269a093c90620b0dd7d1f33e681c451d7533ccf299ec651e41a0031b80bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300588636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1146a51e430cec8a22d8d8ad7332fc4e618b36b40ab651202f07f910aa0b4fa5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:09 GMT
ADD file:9ea7d74fdfdb29946ab72e1aea5810331debe27db7e50a0fc4e0d5a192ab6166 in / 
# Wed, 01 Mar 2023 04:10:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:01:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:01:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Mar 2023 17:01:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Mar 2023 17:01:13 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 17:01:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Mar 2023 17:01:13 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Mar 2023 17:02:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:02:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Mar 2023 17:02:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Mar 2023 17:02:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d8a6bce2a40cb0c3e3cc6646bfeccfb2ac5b303c39ea70d67e30406d270f2009`  
		Last Modified: Wed, 01 Mar 2023 04:14:42 GMT  
		Size: 50.4 MB (50449101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a1ffc835f48ecec7c683701866277b285e39a42777bb6819d705ba54c9b7ee`  
		Last Modified: Wed, 01 Mar 2023 17:09:08 GMT  
		Size: 10.9 MB (10896984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ab4ec3b1ff1518ff16c31e9e4f4b239089fdad9819bb1b0806733d42d30b73`  
		Last Modified: Wed, 01 Mar 2023 17:09:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9841b85e22a255629ec6b026e828d764cdc3c990de2d2c70eef2cfa655083074`  
		Last Modified: Wed, 01 Mar 2023 17:09:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fcea5877730e4a516a82878a4f5f98da043bd4cc6f242e907c49f88c966f58`  
		Last Modified: Wed, 01 Mar 2023 17:09:38 GMT  
		Size: 239.2 MB (239240139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e461f854cd1f5763471d57c32aadc9f1bf067ff5b25408ead48199dee31c5f5`  
		Last Modified: Wed, 01 Mar 2023 17:09:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:55aed9d35e66b740bdf5d6a7ec786f7b1ccc2b86f82a298a18d07c98335a87a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244571461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aa8fae09c5ca8a3e3ee00729f90344c724e58db573c46921dde685023ce1f8e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:46 GMT
ADD file:bf5b2f8cbddd98de6093dde190b043c3e2b58a5063d1acec0aba091e7d203dbd in / 
# Wed, 01 Mar 2023 02:20:47 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 12:29:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:29:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Mar 2023 12:29:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Mar 2023 12:29:13 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 12:29:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Mar 2023 12:29:13 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Mar 2023 12:30:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:30:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Mar 2023 12:30:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Mar 2023 12:30:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:06cfbde07ccb39d53563bd87f3c2b50f04ddd0c8f6cd52be3c7089a3413688e1`  
		Last Modified: Wed, 01 Mar 2023 02:24:34 GMT  
		Size: 49.2 MB (49240002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a788fbcf95c26646fbabe7bb6f29416ca2663c0cfd87e1ccac361a7459568915`  
		Last Modified: Wed, 01 Mar 2023 12:37:20 GMT  
		Size: 10.9 MB (10902711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46d425485295faa6248cc3b6ce203089f5c51e6d6bd9ec2c65a3724f0986ba0`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de7b8f0c8434b3ef1c87e53a130007029f5fd37ea81634299d1e8226d10b4d5`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6b26d79f53cceae9c1d805e9d806a04c531a4290ef45b9f07bdc82202a1edd`  
		Last Modified: Wed, 01 Mar 2023 12:37:41 GMT  
		Size: 184.4 MB (184426336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e132bc958bc874cc517925ada16c2f3e782550fa85b319f3c4d921c3056fa77`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:99d7682251e5c2cddc908d3f2f2fa804311a0e6b668ffa238cde939e5e602255
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:5699cc68b1831fc92aa7d1a4c63f7a732f1ee3ce027e805c907cd6cdf88955c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212304872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60534a72b997b5dcce45b1a81e2c3715e7c9b7629c7c6e2ff5371fe385b1bbad`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 07:31:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:31:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:31:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:31:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752ff12fc1879563f6c3a37566aa1d63df61d32a482e1122678d06111c6c704`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb64a2fb206ee95fea7407d2fa098f13262e2dec6bd6acfc406eb3c7f3ee1e5`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2059687f395790fbfedafba19c2e4f73dd81bccae9ec7df3c7861b1df6886ca`  
		Last Modified: Thu, 02 Mar 2023 08:04:04 GMT  
		Size: 177.0 MB (177016208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1445ae9867c355c105face7eed407747aa39c1481c7133429c4c53f35088f16a`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:93dc53559685aecb2fda770e70acc564d4f877c3fbaf90b42aa5c70781140820
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187931684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365ea3d85c1c823fa8304fd7d8118343f4c9d55375236d7c9d6072da3ba8d815`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 12:12:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 12:12:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 12:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:15:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:15:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:15:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ea6bac35a1ab81469aabdf6a1f6f860ce1c9ed7e82625c53a6f8b1a64e823c`  
		Last Modified: Thu, 02 Mar 2023 12:29:30 GMT  
		Size: 1.2 MB (1154650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14af9ed8fe780bf6b1681423e06ab17566673bef9750c0b5591b03a7e12484`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 4.7 MB (4679133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4bc1671aa822702e1cd36abac0e9193c7a18d0ee42c398e454c47b02f193d`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b751eaf15e5904ee56e930eb3d87c9cc4ea0e10a3ae4f87ff3282b2c170f018`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a025315ed3938804103cdb57fc646fce4f4deeb9fbad47a00f203886109060e8`  
		Last Modified: Thu, 02 Mar 2023 12:29:56 GMT  
		Size: 157.5 MB (157509036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f6dbad8263386860670ffb777d531e98c9c6fe16503702f9d54f3e12f90e59`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:75b39f2eb13e7db3653d56e63728799a3e25c6bf7868c6b02318922fbe17e7d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205370200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31ae095b06299fee387b279f3f2e0ed1f4eabe255a73826905e51bd7b9aa1575`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:29:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 03:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:32:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:32:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:32:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13947cb4d4fb29ac4bbd3748e79ab20da65033b2563147127613ccba352ba358`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a630cbcf281c994586155784a2c5c8a5c02f75715b54f9ec0fdd406eed859bf`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72441278ae08e882e2a05bfd9029475e9242e17a2f6b6d22859299db3b3e7f`  
		Last Modified: Thu, 02 Mar 2023 04:07:06 GMT  
		Size: 171.5 MB (171486823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee1963dd3f45dd61f69960595462707cd1dbabe500bcd3fa2b7cbd8ca6d63`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:725cc7354a11ceb61d160dcf303c293d7d3beaba7d95d079340690eb6aefc05e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:646814923496be2e5ca94801df9b8484b9a6a231ccda48f455936065ada30ee9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263486470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a3a68e0f2d27db20548f648f494f5beca8f40438d4b96c2756780c57659cc0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:56:06 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 07:56:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:56:58 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:56:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:56:58 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:57:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:57:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:57:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:58:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597269e3fad2d81e51094a0db14d3edd235aa622fe24d229adad86fbd007619f`  
		Last Modified: Thu, 02 Mar 2023 08:10:10 GMT  
		Size: 119.6 MB (119586788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47883564c7696a74c435a12bfb19a30f1406dce6103413d70bb5b387b0f9fff8`  
		Last Modified: Thu, 02 Mar 2023 08:09:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554ebe02a40db0cc480713d00599341ed78d5b7b52018de4645d0620fdfb1f0`  
		Last Modified: Thu, 02 Mar 2023 08:10:30 GMT  
		Size: 84.9 MB (84915796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47000bc1f53d442d3e7d498c3b9ed78e4634be95e66176fb60fbb242ff78461`  
		Last Modified: Thu, 02 Mar 2023 08:10:18 GMT  
		Size: 300.7 KB (300743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f57c3714d255a98ac80781bc3f96d20f647d871cb731e59de767a82b8140f4`  
		Last Modified: Thu, 02 Mar 2023 08:10:18 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867e5da436da7aec642c099ff3b3e895e78cf98c22fb1d94c8ab5e9ffe742ffe`  
		Last Modified: Thu, 02 Mar 2023 08:10:22 GMT  
		Size: 23.3 MB (23250279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f2826ba3c870ae4ddb1e82dd37a6f89a8c89846628c65bd7184a0cf41b09db0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256116645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2dd48b3834ba4c4459cab11b489a03d8e8ca71fba3fbf16b12a986b01486b5e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 04:00:41 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 04:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 04:01:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 04:01:17 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 04:01:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 04:01:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 04:01:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1512e661fd644a0a4900ade6cc3896f1af3864cb271b92c768460df153fe80`  
		Last Modified: Thu, 02 Mar 2023 04:12:30 GMT  
		Size: 117.2 MB (117162162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a0c490f5c253510c383ddd657e6887f0bb539a113c0a0435d523ba56efd749`  
		Last Modified: Thu, 02 Mar 2023 04:12:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25f9d6b96f8c0438546063d06191220803549e5b0ff9459d3e87bbe78c5824b`  
		Last Modified: Thu, 02 Mar 2023 04:12:47 GMT  
		Size: 82.6 MB (82628848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cefc12879615a02e1af0dfc5696868758fe87d9adc59064496024233964af4`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 300.7 KB (300740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8ddc9b5c11c2319392bec026c322582406cf8a604872d0758472866c56950b`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d224cc5443868b83b2ee7dd1eda419b6b2c07247b45b1a59f7cb938bb27f0c6`  
		Last Modified: Thu, 02 Mar 2023 04:12:42 GMT  
		Size: 22.7 MB (22661232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception`

```console
$ docker pull ros@sha256:7af145274ef70ba405c5258445c53c665a88c5595adebc262fdc39f1bf597185
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception` - linux; amd64

```console
$ docker pull ros@sha256:5da797d46254f7000a450850190ffbde2242371d2746eba47847dc647c336225
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1092988843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0177765e9963758738146c448bcafce9a04f7f650b489010d3877426ed755d8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:56:06 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 07:56:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:56:58 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:56:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:56:58 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:57:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:57:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:57:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:58:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 08:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597269e3fad2d81e51094a0db14d3edd235aa622fe24d229adad86fbd007619f`  
		Last Modified: Thu, 02 Mar 2023 08:10:10 GMT  
		Size: 119.6 MB (119586788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47883564c7696a74c435a12bfb19a30f1406dce6103413d70bb5b387b0f9fff8`  
		Last Modified: Thu, 02 Mar 2023 08:09:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554ebe02a40db0cc480713d00599341ed78d5b7b52018de4645d0620fdfb1f0`  
		Last Modified: Thu, 02 Mar 2023 08:10:30 GMT  
		Size: 84.9 MB (84915796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47000bc1f53d442d3e7d498c3b9ed78e4634be95e66176fb60fbb242ff78461`  
		Last Modified: Thu, 02 Mar 2023 08:10:18 GMT  
		Size: 300.7 KB (300743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f57c3714d255a98ac80781bc3f96d20f647d871cb731e59de767a82b8140f4`  
		Last Modified: Thu, 02 Mar 2023 08:10:18 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867e5da436da7aec642c099ff3b3e895e78cf98c22fb1d94c8ab5e9ffe742ffe`  
		Last Modified: Thu, 02 Mar 2023 08:10:22 GMT  
		Size: 23.3 MB (23250279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ef9ecd2e6a632aa2876ba5b53e605201af16985524d0da918bef5974916b58`  
		Last Modified: Thu, 02 Mar 2023 08:12:14 GMT  
		Size: 829.5 MB (829502373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e9a41ac2d42695ef32f115f22f30fed4369173b0b4c38c2e4a4d261258844ab4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1044419009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63166cb5a2eb8163c53a2d6765c7be7d10ae18157967d5bdd7417d909c9c4cd5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 04:00:41 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 04:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 04:01:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 04:01:17 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 04:01:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 04:01:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 04:01:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1512e661fd644a0a4900ade6cc3896f1af3864cb271b92c768460df153fe80`  
		Last Modified: Thu, 02 Mar 2023 04:12:30 GMT  
		Size: 117.2 MB (117162162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a0c490f5c253510c383ddd657e6887f0bb539a113c0a0435d523ba56efd749`  
		Last Modified: Thu, 02 Mar 2023 04:12:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25f9d6b96f8c0438546063d06191220803549e5b0ff9459d3e87bbe78c5824b`  
		Last Modified: Thu, 02 Mar 2023 04:12:47 GMT  
		Size: 82.6 MB (82628848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cefc12879615a02e1af0dfc5696868758fe87d9adc59064496024233964af4`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 300.7 KB (300740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8ddc9b5c11c2319392bec026c322582406cf8a604872d0758472866c56950b`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d224cc5443868b83b2ee7dd1eda419b6b2c07247b45b1a59f7cb938bb27f0c6`  
		Last Modified: Thu, 02 Mar 2023 04:12:42 GMT  
		Size: 22.7 MB (22661232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de08b1d5bd8091e93b55d94969cbb7a4abf43136e5722c937ba1409a7dfce1f`  
		Last Modified: Thu, 02 Mar 2023 04:14:11 GMT  
		Size: 788.3 MB (788302364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:7af145274ef70ba405c5258445c53c665a88c5595adebc262fdc39f1bf597185
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:5da797d46254f7000a450850190ffbde2242371d2746eba47847dc647c336225
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.1 GB (1092988843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0177765e9963758738146c448bcafce9a04f7f650b489010d3877426ed755d8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:56:06 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 07:56:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:56:58 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:56:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:56:58 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:57:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:57:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:57:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:58:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 08:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597269e3fad2d81e51094a0db14d3edd235aa622fe24d229adad86fbd007619f`  
		Last Modified: Thu, 02 Mar 2023 08:10:10 GMT  
		Size: 119.6 MB (119586788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47883564c7696a74c435a12bfb19a30f1406dce6103413d70bb5b387b0f9fff8`  
		Last Modified: Thu, 02 Mar 2023 08:09:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554ebe02a40db0cc480713d00599341ed78d5b7b52018de4645d0620fdfb1f0`  
		Last Modified: Thu, 02 Mar 2023 08:10:30 GMT  
		Size: 84.9 MB (84915796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47000bc1f53d442d3e7d498c3b9ed78e4634be95e66176fb60fbb242ff78461`  
		Last Modified: Thu, 02 Mar 2023 08:10:18 GMT  
		Size: 300.7 KB (300743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f57c3714d255a98ac80781bc3f96d20f647d871cb731e59de767a82b8140f4`  
		Last Modified: Thu, 02 Mar 2023 08:10:18 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867e5da436da7aec642c099ff3b3e895e78cf98c22fb1d94c8ab5e9ffe742ffe`  
		Last Modified: Thu, 02 Mar 2023 08:10:22 GMT  
		Size: 23.3 MB (23250279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ef9ecd2e6a632aa2876ba5b53e605201af16985524d0da918bef5974916b58`  
		Last Modified: Thu, 02 Mar 2023 08:12:14 GMT  
		Size: 829.5 MB (829502373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e9a41ac2d42695ef32f115f22f30fed4369173b0b4c38c2e4a4d261258844ab4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1044419009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63166cb5a2eb8163c53a2d6765c7be7d10ae18157967d5bdd7417d909c9c4cd5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 04:00:41 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 04:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 04:01:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 04:01:17 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 04:01:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 04:01:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 04:01:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1512e661fd644a0a4900ade6cc3896f1af3864cb271b92c768460df153fe80`  
		Last Modified: Thu, 02 Mar 2023 04:12:30 GMT  
		Size: 117.2 MB (117162162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a0c490f5c253510c383ddd657e6887f0bb539a113c0a0435d523ba56efd749`  
		Last Modified: Thu, 02 Mar 2023 04:12:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25f9d6b96f8c0438546063d06191220803549e5b0ff9459d3e87bbe78c5824b`  
		Last Modified: Thu, 02 Mar 2023 04:12:47 GMT  
		Size: 82.6 MB (82628848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cefc12879615a02e1af0dfc5696868758fe87d9adc59064496024233964af4`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 300.7 KB (300740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8ddc9b5c11c2319392bec026c322582406cf8a604872d0758472866c56950b`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d224cc5443868b83b2ee7dd1eda419b6b2c07247b45b1a59f7cb938bb27f0c6`  
		Last Modified: Thu, 02 Mar 2023 04:12:42 GMT  
		Size: 22.7 MB (22661232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de08b1d5bd8091e93b55d94969cbb7a4abf43136e5722c937ba1409a7dfce1f`  
		Last Modified: Thu, 02 Mar 2023 04:14:11 GMT  
		Size: 788.3 MB (788302364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:725cc7354a11ceb61d160dcf303c293d7d3beaba7d95d079340690eb6aefc05e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:646814923496be2e5ca94801df9b8484b9a6a231ccda48f455936065ada30ee9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263486470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a3a68e0f2d27db20548f648f494f5beca8f40438d4b96c2756780c57659cc0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:56:06 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 07:56:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:56:58 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:56:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:56:58 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:57:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:57:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:57:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:58:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597269e3fad2d81e51094a0db14d3edd235aa622fe24d229adad86fbd007619f`  
		Last Modified: Thu, 02 Mar 2023 08:10:10 GMT  
		Size: 119.6 MB (119586788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47883564c7696a74c435a12bfb19a30f1406dce6103413d70bb5b387b0f9fff8`  
		Last Modified: Thu, 02 Mar 2023 08:09:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554ebe02a40db0cc480713d00599341ed78d5b7b52018de4645d0620fdfb1f0`  
		Last Modified: Thu, 02 Mar 2023 08:10:30 GMT  
		Size: 84.9 MB (84915796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47000bc1f53d442d3e7d498c3b9ed78e4634be95e66176fb60fbb242ff78461`  
		Last Modified: Thu, 02 Mar 2023 08:10:18 GMT  
		Size: 300.7 KB (300743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f57c3714d255a98ac80781bc3f96d20f647d871cb731e59de767a82b8140f4`  
		Last Modified: Thu, 02 Mar 2023 08:10:18 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867e5da436da7aec642c099ff3b3e895e78cf98c22fb1d94c8ab5e9ffe742ffe`  
		Last Modified: Thu, 02 Mar 2023 08:10:22 GMT  
		Size: 23.3 MB (23250279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f2826ba3c870ae4ddb1e82dd37a6f89a8c89846628c65bd7184a0cf41b09db0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256116645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2dd48b3834ba4c4459cab11b489a03d8e8ca71fba3fbf16b12a986b01486b5e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 04:00:41 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 04:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 04:01:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 04:01:17 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 04:01:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 04:01:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 04:01:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1512e661fd644a0a4900ade6cc3896f1af3864cb271b92c768460df153fe80`  
		Last Modified: Thu, 02 Mar 2023 04:12:30 GMT  
		Size: 117.2 MB (117162162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a0c490f5c253510c383ddd657e6887f0bb539a113c0a0435d523ba56efd749`  
		Last Modified: Thu, 02 Mar 2023 04:12:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25f9d6b96f8c0438546063d06191220803549e5b0ff9459d3e87bbe78c5824b`  
		Last Modified: Thu, 02 Mar 2023 04:12:47 GMT  
		Size: 82.6 MB (82628848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cefc12879615a02e1af0dfc5696868758fe87d9adc59064496024233964af4`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 300.7 KB (300740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8ddc9b5c11c2319392bec026c322582406cf8a604872d0758472866c56950b`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d224cc5443868b83b2ee7dd1eda419b6b2c07247b45b1a59f7cb938bb27f0c6`  
		Last Modified: Thu, 02 Mar 2023 04:12:42 GMT  
		Size: 22.7 MB (22661232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-jammy`

```console
$ docker pull ros@sha256:725cc7354a11ceb61d160dcf303c293d7d3beaba7d95d079340690eb6aefc05e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:646814923496be2e5ca94801df9b8484b9a6a231ccda48f455936065ada30ee9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263486470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a3a68e0f2d27db20548f648f494f5beca8f40438d4b96c2756780c57659cc0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:56:06 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 07:56:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:56:58 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:56:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:56:58 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:57:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:57:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:57:40 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 07:58:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597269e3fad2d81e51094a0db14d3edd235aa622fe24d229adad86fbd007619f`  
		Last Modified: Thu, 02 Mar 2023 08:10:10 GMT  
		Size: 119.6 MB (119586788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47883564c7696a74c435a12bfb19a30f1406dce6103413d70bb5b387b0f9fff8`  
		Last Modified: Thu, 02 Mar 2023 08:09:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554ebe02a40db0cc480713d00599341ed78d5b7b52018de4645d0620fdfb1f0`  
		Last Modified: Thu, 02 Mar 2023 08:10:30 GMT  
		Size: 84.9 MB (84915796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47000bc1f53d442d3e7d498c3b9ed78e4634be95e66176fb60fbb242ff78461`  
		Last Modified: Thu, 02 Mar 2023 08:10:18 GMT  
		Size: 300.7 KB (300743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f57c3714d255a98ac80781bc3f96d20f647d871cb731e59de767a82b8140f4`  
		Last Modified: Thu, 02 Mar 2023 08:10:18 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867e5da436da7aec642c099ff3b3e895e78cf98c22fb1d94c8ab5e9ffe742ffe`  
		Last Modified: Thu, 02 Mar 2023 08:10:22 GMT  
		Size: 23.3 MB (23250279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f2826ba3c870ae4ddb1e82dd37a6f89a8c89846628c65bd7184a0cf41b09db0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256116645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2dd48b3834ba4c4459cab11b489a03d8e8ca71fba3fbf16b12a986b01486b5e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 04:00:41 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 04:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 04:01:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 04:01:17 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 04:01:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 04:01:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 04:01:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1512e661fd644a0a4900ade6cc3896f1af3864cb271b92c768460df153fe80`  
		Last Modified: Thu, 02 Mar 2023 04:12:30 GMT  
		Size: 117.2 MB (117162162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a0c490f5c253510c383ddd657e6887f0bb539a113c0a0435d523ba56efd749`  
		Last Modified: Thu, 02 Mar 2023 04:12:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25f9d6b96f8c0438546063d06191220803549e5b0ff9459d3e87bbe78c5824b`  
		Last Modified: Thu, 02 Mar 2023 04:12:47 GMT  
		Size: 82.6 MB (82628848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cefc12879615a02e1af0dfc5696868758fe87d9adc59064496024233964af4`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 300.7 KB (300740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8ddc9b5c11c2319392bec026c322582406cf8a604872d0758472866c56950b`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d224cc5443868b83b2ee7dd1eda419b6b2c07247b45b1a59f7cb938bb27f0c6`  
		Last Modified: Thu, 02 Mar 2023 04:12:42 GMT  
		Size: 22.7 MB (22661232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:43519fc688be77eea9fbff958c3b9716d5080713b2038fa31400e0717f1239f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:683b8eea2e4131fdf2d527f3bdfbf71d4fb71549496d943707625c28d7a12954
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155017230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb30b6c74a0bb21c315d5aae7b23a7c42193c0fee72704a9e8805d3f9dcb39f7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:56:06 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 07:56:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:56:58 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:56:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:56:58 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597269e3fad2d81e51094a0db14d3edd235aa622fe24d229adad86fbd007619f`  
		Last Modified: Thu, 02 Mar 2023 08:10:10 GMT  
		Size: 119.6 MB (119586788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47883564c7696a74c435a12bfb19a30f1406dce6103413d70bb5b387b0f9fff8`  
		Last Modified: Thu, 02 Mar 2023 08:09:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e394f41765f530ad2770ed87db90f1f573193f39bc49a07bfc7fa77c74126be6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150523404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5936a6233f7abbc6bcd6e5513f9083391b6511f6468b87d529828d8243968d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 04:00:41 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 04:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 04:01:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 04:01:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1512e661fd644a0a4900ade6cc3896f1af3864cb271b92c768460df153fe80`  
		Last Modified: Thu, 02 Mar 2023 04:12:30 GMT  
		Size: 117.2 MB (117162162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a0c490f5c253510c383ddd657e6887f0bb539a113c0a0435d523ba56efd749`  
		Last Modified: Thu, 02 Mar 2023 04:12:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:43519fc688be77eea9fbff958c3b9716d5080713b2038fa31400e0717f1239f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:683b8eea2e4131fdf2d527f3bdfbf71d4fb71549496d943707625c28d7a12954
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155017230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb30b6c74a0bb21c315d5aae7b23a7c42193c0fee72704a9e8805d3f9dcb39f7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 07:43:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:44:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 07:44:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:44:14 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:44:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:56:06 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 07:56:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:56:58 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 07:56:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:56:58 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f8c551927da9bf0e6183ca57144eb52c4cfba7077e5cad6b6ba8cc924dfdf8`  
		Last Modified: Thu, 02 Mar 2023 08:07:21 GMT  
		Size: 1.2 MB (1169624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92556ded650c06629c372b95a6fc958e129547cec3d2b44dbd493ec01e6a0269`  
		Last Modified: Thu, 02 Mar 2023 08:07:19 GMT  
		Size: 3.8 MB (3828401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2fa7334b1384d0dd1db04563b249d6ba14dba379e1bc922faf207237a97f16`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712ecf776b1c8f9d3a6e14b360d9f7c3f54e30ace3709ca57909b05d00c991c`  
		Last Modified: Thu, 02 Mar 2023 08:07:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597269e3fad2d81e51094a0db14d3edd235aa622fe24d229adad86fbd007619f`  
		Last Modified: Thu, 02 Mar 2023 08:10:10 GMT  
		Size: 119.6 MB (119586788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47883564c7696a74c435a12bfb19a30f1406dce6103413d70bb5b387b0f9fff8`  
		Last Modified: Thu, 02 Mar 2023 08:09:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e394f41765f530ad2770ed87db90f1f573193f39bc49a07bfc7fa77c74126be6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150523404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5936a6233f7abbc6bcd6e5513f9083391b6511f6468b87d529828d8243968d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 04:00:41 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 04:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 04:01:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 04:01:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1512e661fd644a0a4900ade6cc3896f1af3864cb271b92c768460df153fe80`  
		Last Modified: Thu, 02 Mar 2023 04:12:30 GMT  
		Size: 117.2 MB (117162162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a0c490f5c253510c383ddd657e6887f0bb539a113c0a0435d523ba56efd749`  
		Last Modified: Thu, 02 Mar 2023 04:12:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
