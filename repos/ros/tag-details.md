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
$ docker pull ros@sha256:c0b3b66cae3741dca25ed73a9263544a168dc66c6836ec84e3b33eaee3d6f0af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:96012077f6cd64756b7f1339ecaff8c6276cffdc2cb3d60dca783a6d28b65731
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.7 MB (236669874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ee1d4d17a982b8409772f9906b8116b0e8356cf69576df29080473e2f6d047`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 03:38:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:38:52 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:38:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:38:52 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:39:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:39:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:39:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:39:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ceb427087b3041b32a2be8c73788330f9675008ba201372eac0b4efc2cc18`  
		Last Modified: Sat, 16 Oct 2021 03:49:49 GMT  
		Size: 120.0 MB (119985810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e7b97e74c6f685d0d0a9362a5cf4a8769e1696bbf995293763867daaba3d19`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7748c6e4eab99c248c57227d0705c45d1b5c16a2a61bc6e2b4390c76f5346b70`  
		Last Modified: Sat, 16 Oct 2021 03:50:09 GMT  
		Size: 70.8 MB (70844958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204e3cb07dc82bf75a08f0e4498123299d9e74ab8013405bfcf2d7c06b149b00`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 244.9 KB (244893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbf530a707a11219db69d544ff5edbf747a4541147f82d4c0a9072da290fe8f`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d0f031d5ee8d2a1754ef8291702f1ddc0a60f24fe9e0f529f7d6bbefa59828`  
		Last Modified: Sat, 16 Oct 2021 03:50:01 GMT  
		Size: 10.3 MB (10288974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4ec429ad8b1abecd8f150d381a44427a1d4501f91e4b83d2ebb765e77628cf65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.1 MB (212140824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67520d943e5f44778958f5a52344b173ae86cee024afaf866bd4b6310bb56d34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:30:43 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 02:31:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:31:37 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:31:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:31:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:32:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:32:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:32:22 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:32:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149fc655748fb600fd752cb6805c8a4ca22cb195276c6222f500719d598fb59c`  
		Last Modified: Sat, 16 Oct 2021 02:49:26 GMT  
		Size: 104.2 MB (104159054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa569375e41dce495d90956baf65112208fd3655215fd4563bd0dd5a665da217`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b885237a11c3c3a5e31b49a568d28e2f32c00c1cde49be15ef946313a54218c`  
		Last Modified: Sat, 16 Oct 2021 02:49:47 GMT  
		Size: 65.0 MB (64966810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0695bf566d5652b3dd582cbc3fabac21343dc6476601a5fae98304412675a`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 244.8 KB (244842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8067ff73af3c358526193f7ea6d83e770f689e4b23865209c2b5f56b3d9d56`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 2.0 KB (1980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85d6588bac0c377f420f223ef5eff321027f991a1cbf69f707bf743e3248758`  
		Last Modified: Sat, 16 Oct 2021 02:49:39 GMT  
		Size: 9.1 MB (9085686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:c0b3b66cae3741dca25ed73a9263544a168dc66c6836ec84e3b33eaee3d6f0af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:96012077f6cd64756b7f1339ecaff8c6276cffdc2cb3d60dca783a6d28b65731
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.7 MB (236669874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ee1d4d17a982b8409772f9906b8116b0e8356cf69576df29080473e2f6d047`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 03:38:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:38:52 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:38:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:38:52 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:39:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:39:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:39:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:39:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ceb427087b3041b32a2be8c73788330f9675008ba201372eac0b4efc2cc18`  
		Last Modified: Sat, 16 Oct 2021 03:49:49 GMT  
		Size: 120.0 MB (119985810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e7b97e74c6f685d0d0a9362a5cf4a8769e1696bbf995293763867daaba3d19`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7748c6e4eab99c248c57227d0705c45d1b5c16a2a61bc6e2b4390c76f5346b70`  
		Last Modified: Sat, 16 Oct 2021 03:50:09 GMT  
		Size: 70.8 MB (70844958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204e3cb07dc82bf75a08f0e4498123299d9e74ab8013405bfcf2d7c06b149b00`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 244.9 KB (244893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbf530a707a11219db69d544ff5edbf747a4541147f82d4c0a9072da290fe8f`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d0f031d5ee8d2a1754ef8291702f1ddc0a60f24fe9e0f529f7d6bbefa59828`  
		Last Modified: Sat, 16 Oct 2021 03:50:01 GMT  
		Size: 10.3 MB (10288974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4ec429ad8b1abecd8f150d381a44427a1d4501f91e4b83d2ebb765e77628cf65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.1 MB (212140824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67520d943e5f44778958f5a52344b173ae86cee024afaf866bd4b6310bb56d34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:30:43 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 02:31:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:31:37 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:31:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:31:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:32:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:32:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:32:22 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:32:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149fc655748fb600fd752cb6805c8a4ca22cb195276c6222f500719d598fb59c`  
		Last Modified: Sat, 16 Oct 2021 02:49:26 GMT  
		Size: 104.2 MB (104159054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa569375e41dce495d90956baf65112208fd3655215fd4563bd0dd5a665da217`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b885237a11c3c3a5e31b49a568d28e2f32c00c1cde49be15ef946313a54218c`  
		Last Modified: Sat, 16 Oct 2021 02:49:47 GMT  
		Size: 65.0 MB (64966810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0695bf566d5652b3dd582cbc3fabac21343dc6476601a5fae98304412675a`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 244.8 KB (244842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8067ff73af3c358526193f7ea6d83e770f689e4b23865209c2b5f56b3d9d56`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 2.0 KB (1980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85d6588bac0c377f420f223ef5eff321027f991a1cbf69f707bf743e3248758`  
		Last Modified: Sat, 16 Oct 2021 02:49:39 GMT  
		Size: 9.1 MB (9085686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:c0b3b66cae3741dca25ed73a9263544a168dc66c6836ec84e3b33eaee3d6f0af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:96012077f6cd64756b7f1339ecaff8c6276cffdc2cb3d60dca783a6d28b65731
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.7 MB (236669874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ee1d4d17a982b8409772f9906b8116b0e8356cf69576df29080473e2f6d047`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 03:38:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:38:52 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:38:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:38:52 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:39:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:39:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:39:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:39:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ceb427087b3041b32a2be8c73788330f9675008ba201372eac0b4efc2cc18`  
		Last Modified: Sat, 16 Oct 2021 03:49:49 GMT  
		Size: 120.0 MB (119985810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e7b97e74c6f685d0d0a9362a5cf4a8769e1696bbf995293763867daaba3d19`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7748c6e4eab99c248c57227d0705c45d1b5c16a2a61bc6e2b4390c76f5346b70`  
		Last Modified: Sat, 16 Oct 2021 03:50:09 GMT  
		Size: 70.8 MB (70844958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204e3cb07dc82bf75a08f0e4498123299d9e74ab8013405bfcf2d7c06b149b00`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 244.9 KB (244893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbf530a707a11219db69d544ff5edbf747a4541147f82d4c0a9072da290fe8f`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d0f031d5ee8d2a1754ef8291702f1ddc0a60f24fe9e0f529f7d6bbefa59828`  
		Last Modified: Sat, 16 Oct 2021 03:50:01 GMT  
		Size: 10.3 MB (10288974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4ec429ad8b1abecd8f150d381a44427a1d4501f91e4b83d2ebb765e77628cf65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.1 MB (212140824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67520d943e5f44778958f5a52344b173ae86cee024afaf866bd4b6310bb56d34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:30:43 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 02:31:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:31:37 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:31:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:31:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:32:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:32:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:32:22 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:32:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149fc655748fb600fd752cb6805c8a4ca22cb195276c6222f500719d598fb59c`  
		Last Modified: Sat, 16 Oct 2021 02:49:26 GMT  
		Size: 104.2 MB (104159054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa569375e41dce495d90956baf65112208fd3655215fd4563bd0dd5a665da217`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b885237a11c3c3a5e31b49a568d28e2f32c00c1cde49be15ef946313a54218c`  
		Last Modified: Sat, 16 Oct 2021 02:49:47 GMT  
		Size: 65.0 MB (64966810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0695bf566d5652b3dd582cbc3fabac21343dc6476601a5fae98304412675a`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 244.8 KB (244842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8067ff73af3c358526193f7ea6d83e770f689e4b23865209c2b5f56b3d9d56`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 2.0 KB (1980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85d6588bac0c377f420f223ef5eff321027f991a1cbf69f707bf743e3248758`  
		Last Modified: Sat, 16 Oct 2021 02:49:39 GMT  
		Size: 9.1 MB (9085686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:b7f0b8bfb8da54ae099a2328db3cab7d1870d757c40a644f31cd2c147a4e8629
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:6d9fdee9adef13401b84394d6b6dbb2818b0110c5f9fa39d750c7fdd361d5dc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155288997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d993fe89aa9539880d85717791f229e3f140a86b50a00f604123cf4837268c9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 03:38:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:38:52 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:38:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:38:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ceb427087b3041b32a2be8c73788330f9675008ba201372eac0b4efc2cc18`  
		Last Modified: Sat, 16 Oct 2021 03:49:49 GMT  
		Size: 120.0 MB (119985810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e7b97e74c6f685d0d0a9362a5cf4a8769e1696bbf995293763867daaba3d19`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6489b14e3318e9cb9a06dffe3884041b0a1f4941d4327bf87600bebe7363214e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137841506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4811d37e65f4ee397c3849cd90324b690d1cf0d3b19e7197e28f230e645d9a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:30:43 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 02:31:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:31:37 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:31:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:31:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149fc655748fb600fd752cb6805c8a4ca22cb195276c6222f500719d598fb59c`  
		Last Modified: Sat, 16 Oct 2021 02:49:26 GMT  
		Size: 104.2 MB (104159054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa569375e41dce495d90956baf65112208fd3655215fd4563bd0dd5a665da217`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:b7f0b8bfb8da54ae099a2328db3cab7d1870d757c40a644f31cd2c147a4e8629
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:6d9fdee9adef13401b84394d6b6dbb2818b0110c5f9fa39d750c7fdd361d5dc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155288997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d993fe89aa9539880d85717791f229e3f140a86b50a00f604123cf4837268c9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 03:38:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:38:52 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:38:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:38:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ceb427087b3041b32a2be8c73788330f9675008ba201372eac0b4efc2cc18`  
		Last Modified: Sat, 16 Oct 2021 03:49:49 GMT  
		Size: 120.0 MB (119985810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e7b97e74c6f685d0d0a9362a5cf4a8769e1696bbf995293763867daaba3d19`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6489b14e3318e9cb9a06dffe3884041b0a1f4941d4327bf87600bebe7363214e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137841506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4811d37e65f4ee397c3849cd90324b690d1cf0d3b19e7197e28f230e645d9a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:30:43 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 02:31:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:31:37 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:31:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:31:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149fc655748fb600fd752cb6805c8a4ca22cb195276c6222f500719d598fb59c`  
		Last Modified: Sat, 16 Oct 2021 02:49:26 GMT  
		Size: 104.2 MB (104159054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa569375e41dce495d90956baf65112208fd3655215fd4563bd0dd5a665da217`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:99f1c176a39d64a79a3cb84cb375b0bc012286f2d345bd479e43758e5bb9c15b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:d6a691738fa31cf6f356ae929c63fa9c3cee10fa2a11b85aaeddea89cdc6bf21
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.6 MB (345574883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03ee3a802313ea6d94c4ea06dcf0a4ea7d519713184674747a57bd5e0705497`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 03:38:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:38:52 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:38:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:38:52 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:39:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:39:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:39:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:39:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:40:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:40:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:40:10 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 03:40:10 GMT
ENV ROS2_DISTRO=foxy
# Sat, 16 Oct 2021 03:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:40:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:40:54 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ceb427087b3041b32a2be8c73788330f9675008ba201372eac0b4efc2cc18`  
		Last Modified: Sat, 16 Oct 2021 03:49:49 GMT  
		Size: 120.0 MB (119985810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e7b97e74c6f685d0d0a9362a5cf4a8769e1696bbf995293763867daaba3d19`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7748c6e4eab99c248c57227d0705c45d1b5c16a2a61bc6e2b4390c76f5346b70`  
		Last Modified: Sat, 16 Oct 2021 03:50:09 GMT  
		Size: 70.8 MB (70844958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204e3cb07dc82bf75a08f0e4498123299d9e74ab8013405bfcf2d7c06b149b00`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 244.9 KB (244893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbf530a707a11219db69d544ff5edbf747a4541147f82d4c0a9072da290fe8f`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d0f031d5ee8d2a1754ef8291702f1ddc0a60f24fe9e0f529f7d6bbefa59828`  
		Last Modified: Sat, 16 Oct 2021 03:50:01 GMT  
		Size: 10.3 MB (10288974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3266ccdb42b1bec97ebd06d1c3eaa4d779d288eb37ae26849976749b79c80ae3`  
		Last Modified: Sat, 16 Oct 2021 03:50:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bef8c1f330d77992b360d005a576e48ec3d99fd46b1987a0ea1b1040582c021`  
		Last Modified: Sat, 16 Oct 2021 03:50:25 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb3ee012879069e106e17763a6e2d3e49c73191dd093ef747c5b2e3169bc98e`  
		Last Modified: Sat, 16 Oct 2021 03:50:40 GMT  
		Size: 76.1 MB (76133715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f37efb0fea05d9d8bcc998f6107f9c748ff4392c0b21867cf7932632b57f3`  
		Last Modified: Sat, 16 Oct 2021 03:50:32 GMT  
		Size: 32.8 MB (32770666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99793e32227b0d56e1de7b3a51a55c90f798adef85c7e29bf5612a90f185ecbb`  
		Last Modified: Sat, 16 Oct 2021 03:50:25 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ee4e073ea4611160dbbfc6de7e157c317c5e33164af06dc142b4d41c884682e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.2 MB (313238986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c3d34c3c3c4bc62fbf29383cca6753f61c1310a64555bbd09b26b322e39c6c2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:30:43 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 02:31:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:31:37 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:31:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:31:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:32:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:32:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:32:22 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:32:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:32:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:32:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:32:47 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 02:32:48 GMT
ENV ROS2_DISTRO=foxy
# Sat, 16 Oct 2021 02:33:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:33:46 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149fc655748fb600fd752cb6805c8a4ca22cb195276c6222f500719d598fb59c`  
		Last Modified: Sat, 16 Oct 2021 02:49:26 GMT  
		Size: 104.2 MB (104159054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa569375e41dce495d90956baf65112208fd3655215fd4563bd0dd5a665da217`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b885237a11c3c3a5e31b49a568d28e2f32c00c1cde49be15ef946313a54218c`  
		Last Modified: Sat, 16 Oct 2021 02:49:47 GMT  
		Size: 65.0 MB (64966810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0695bf566d5652b3dd582cbc3fabac21343dc6476601a5fae98304412675a`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 244.8 KB (244842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8067ff73af3c358526193f7ea6d83e770f689e4b23865209c2b5f56b3d9d56`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 2.0 KB (1980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85d6588bac0c377f420f223ef5eff321027f991a1cbf69f707bf743e3248758`  
		Last Modified: Sat, 16 Oct 2021 02:49:39 GMT  
		Size: 9.1 MB (9085686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8b3f8b242de8613b5d45b654f5bf5568fd17f9a92cbd928b34797b63391423`  
		Last Modified: Sat, 16 Oct 2021 02:50:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a8a5380e7abb39261fa5400a00576025d4eb11caeeb986aaaf2c8568bf5f8d`  
		Last Modified: Sat, 16 Oct 2021 02:50:20 GMT  
		Size: 76.0 MB (75965631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed331b81210890b615cf836e0ee15a88c272727bd3297ae76a759d75a13e876`  
		Last Modified: Sat, 16 Oct 2021 02:50:09 GMT  
		Size: 25.1 MB (25132062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93afdda0273b3dcaa4f74bf774af1ab186012afe83faac4c6fb6a1b09af2e2`  
		Last Modified: Sat, 16 Oct 2021 02:50:05 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:99f1c176a39d64a79a3cb84cb375b0bc012286f2d345bd479e43758e5bb9c15b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:d6a691738fa31cf6f356ae929c63fa9c3cee10fa2a11b85aaeddea89cdc6bf21
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.6 MB (345574883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03ee3a802313ea6d94c4ea06dcf0a4ea7d519713184674747a57bd5e0705497`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 03:38:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:38:52 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:38:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:38:52 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:39:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:39:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:39:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:39:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:40:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:40:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:40:10 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 03:40:10 GMT
ENV ROS2_DISTRO=foxy
# Sat, 16 Oct 2021 03:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:40:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:40:54 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ceb427087b3041b32a2be8c73788330f9675008ba201372eac0b4efc2cc18`  
		Last Modified: Sat, 16 Oct 2021 03:49:49 GMT  
		Size: 120.0 MB (119985810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e7b97e74c6f685d0d0a9362a5cf4a8769e1696bbf995293763867daaba3d19`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7748c6e4eab99c248c57227d0705c45d1b5c16a2a61bc6e2b4390c76f5346b70`  
		Last Modified: Sat, 16 Oct 2021 03:50:09 GMT  
		Size: 70.8 MB (70844958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204e3cb07dc82bf75a08f0e4498123299d9e74ab8013405bfcf2d7c06b149b00`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 244.9 KB (244893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbf530a707a11219db69d544ff5edbf747a4541147f82d4c0a9072da290fe8f`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d0f031d5ee8d2a1754ef8291702f1ddc0a60f24fe9e0f529f7d6bbefa59828`  
		Last Modified: Sat, 16 Oct 2021 03:50:01 GMT  
		Size: 10.3 MB (10288974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3266ccdb42b1bec97ebd06d1c3eaa4d779d288eb37ae26849976749b79c80ae3`  
		Last Modified: Sat, 16 Oct 2021 03:50:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bef8c1f330d77992b360d005a576e48ec3d99fd46b1987a0ea1b1040582c021`  
		Last Modified: Sat, 16 Oct 2021 03:50:25 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb3ee012879069e106e17763a6e2d3e49c73191dd093ef747c5b2e3169bc98e`  
		Last Modified: Sat, 16 Oct 2021 03:50:40 GMT  
		Size: 76.1 MB (76133715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f37efb0fea05d9d8bcc998f6107f9c748ff4392c0b21867cf7932632b57f3`  
		Last Modified: Sat, 16 Oct 2021 03:50:32 GMT  
		Size: 32.8 MB (32770666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99793e32227b0d56e1de7b3a51a55c90f798adef85c7e29bf5612a90f185ecbb`  
		Last Modified: Sat, 16 Oct 2021 03:50:25 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ee4e073ea4611160dbbfc6de7e157c317c5e33164af06dc142b4d41c884682e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.2 MB (313238986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c3d34c3c3c4bc62fbf29383cca6753f61c1310a64555bbd09b26b322e39c6c2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:30:43 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 02:31:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:31:37 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:31:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:31:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:32:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:32:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:32:22 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:32:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:32:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:32:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:32:47 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 02:32:48 GMT
ENV ROS2_DISTRO=foxy
# Sat, 16 Oct 2021 02:33:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:33:46 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149fc655748fb600fd752cb6805c8a4ca22cb195276c6222f500719d598fb59c`  
		Last Modified: Sat, 16 Oct 2021 02:49:26 GMT  
		Size: 104.2 MB (104159054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa569375e41dce495d90956baf65112208fd3655215fd4563bd0dd5a665da217`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b885237a11c3c3a5e31b49a568d28e2f32c00c1cde49be15ef946313a54218c`  
		Last Modified: Sat, 16 Oct 2021 02:49:47 GMT  
		Size: 65.0 MB (64966810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0695bf566d5652b3dd582cbc3fabac21343dc6476601a5fae98304412675a`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 244.8 KB (244842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8067ff73af3c358526193f7ea6d83e770f689e4b23865209c2b5f56b3d9d56`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 2.0 KB (1980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85d6588bac0c377f420f223ef5eff321027f991a1cbf69f707bf743e3248758`  
		Last Modified: Sat, 16 Oct 2021 02:49:39 GMT  
		Size: 9.1 MB (9085686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8b3f8b242de8613b5d45b654f5bf5568fd17f9a92cbd928b34797b63391423`  
		Last Modified: Sat, 16 Oct 2021 02:50:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a8a5380e7abb39261fa5400a00576025d4eb11caeeb986aaaf2c8568bf5f8d`  
		Last Modified: Sat, 16 Oct 2021 02:50:20 GMT  
		Size: 76.0 MB (75965631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed331b81210890b615cf836e0ee15a88c272727bd3297ae76a759d75a13e876`  
		Last Modified: Sat, 16 Oct 2021 02:50:09 GMT  
		Size: 25.1 MB (25132062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93afdda0273b3dcaa4f74bf774af1ab186012afe83faac4c6fb6a1b09af2e2`  
		Last Modified: Sat, 16 Oct 2021 02:50:05 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic`

```console
$ docker pull ros@sha256:65beaaee344167f62b4ff87373d84faa27e1ea73b5de15f1a59646bea87de4d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic` - linux; amd64

```console
$ docker pull ros@sha256:23cfd590c135a42606747f60b888595a2ae00810f439dc4b78f4d4d2e04df476
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232089648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e88918e911975edd2d2ae88c1078561146665fdb1a836d044b132913f1a7cbf7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:41:01 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 03:41:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:41:44 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:41:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:41:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:42:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:42:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:42:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:42:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667bbaa58b18042bba7f627e73f63afc769ef1ba6dd8d02db26a97639896068`  
		Last Modified: Sat, 16 Oct 2021 03:51:07 GMT  
		Size: 103.6 MB (103626785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a680ad47ebc112dc93a40e8bd9e894aaf9519f94d0682ddd3fd48b7397cf56`  
		Last Modified: Sat, 16 Oct 2021 03:50:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99485d848bd2d8d3e44bc608ce7b5ded397a3875cd31a870b9204f6cf034156`  
		Last Modified: Sat, 16 Oct 2021 03:51:28 GMT  
		Size: 70.8 MB (70797181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0eba6427f6ee57b80c5edcf96532a72d18d44acf2723fcb86619039bbcfd4e`  
		Last Modified: Sat, 16 Oct 2021 03:51:18 GMT  
		Size: 250.9 KB (250902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec01b9342ad47c2d894dd5445179b44b59795f39844beddfe6e4ff69fcd8f8`  
		Last Modified: Sat, 16 Oct 2021 03:51:18 GMT  
		Size: 2.0 KB (2015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa73989292d31559372cc09b8599aba98531656e025666399df977d646028b`  
		Last Modified: Sat, 16 Oct 2021 03:51:21 GMT  
		Size: 22.1 MB (22109577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cad2d4c2bba24c8d1bc99484270c7187550f8478caba71e670ad4018db70f19f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.3 MB (220295241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1dc7d553defc3476d6d036001a2ebef1c69198b71864342ba12919988328c4a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:33:55 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 02:34:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:34:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:34:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:34:41 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:35:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:35:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:35:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3549f1d260e60d8924c9b7e02611c65b2136c4991bbccee64e068f45993511`  
		Last Modified: Sat, 16 Oct 2021 02:50:49 GMT  
		Size: 100.0 MB (100010821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c03abd5daa700ddf866335aef47153c602aab661fc4e8a8cd6b920a3b78c6d9`  
		Last Modified: Sat, 16 Oct 2021 02:50:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bee7cb9969d594ee7bc764af007e4c0e9dbdd159efb7f78cd99599fe5d24227`  
		Last Modified: Sat, 16 Oct 2021 02:51:09 GMT  
		Size: 64.9 MB (64922456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d5fa4cfb7df399ade2516372c36c4997dd6b036fcf0fed2519961a0cc9cfca`  
		Last Modified: Sat, 16 Oct 2021 02:51:00 GMT  
		Size: 250.8 KB (250842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e07cbc601974d308056bc5dd837d1e5cf3f31275052df2573bbe28b172562`  
		Last Modified: Sat, 16 Oct 2021 02:50:59 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0000799c6000c28c01d2cfe4f94f943eea059b940290cb2bbeda007a003af9e`  
		Last Modified: Sat, 16 Oct 2021 02:51:02 GMT  
		Size: 21.4 MB (21426708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base`

```console
$ docker pull ros@sha256:65beaaee344167f62b4ff87373d84faa27e1ea73b5de15f1a59646bea87de4d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:23cfd590c135a42606747f60b888595a2ae00810f439dc4b78f4d4d2e04df476
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232089648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e88918e911975edd2d2ae88c1078561146665fdb1a836d044b132913f1a7cbf7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:41:01 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 03:41:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:41:44 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:41:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:41:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:42:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:42:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:42:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:42:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667bbaa58b18042bba7f627e73f63afc769ef1ba6dd8d02db26a97639896068`  
		Last Modified: Sat, 16 Oct 2021 03:51:07 GMT  
		Size: 103.6 MB (103626785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a680ad47ebc112dc93a40e8bd9e894aaf9519f94d0682ddd3fd48b7397cf56`  
		Last Modified: Sat, 16 Oct 2021 03:50:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99485d848bd2d8d3e44bc608ce7b5ded397a3875cd31a870b9204f6cf034156`  
		Last Modified: Sat, 16 Oct 2021 03:51:28 GMT  
		Size: 70.8 MB (70797181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0eba6427f6ee57b80c5edcf96532a72d18d44acf2723fcb86619039bbcfd4e`  
		Last Modified: Sat, 16 Oct 2021 03:51:18 GMT  
		Size: 250.9 KB (250902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec01b9342ad47c2d894dd5445179b44b59795f39844beddfe6e4ff69fcd8f8`  
		Last Modified: Sat, 16 Oct 2021 03:51:18 GMT  
		Size: 2.0 KB (2015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa73989292d31559372cc09b8599aba98531656e025666399df977d646028b`  
		Last Modified: Sat, 16 Oct 2021 03:51:21 GMT  
		Size: 22.1 MB (22109577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cad2d4c2bba24c8d1bc99484270c7187550f8478caba71e670ad4018db70f19f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.3 MB (220295241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1dc7d553defc3476d6d036001a2ebef1c69198b71864342ba12919988328c4a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:33:55 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 02:34:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:34:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:34:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:34:41 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:35:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:35:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:35:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3549f1d260e60d8924c9b7e02611c65b2136c4991bbccee64e068f45993511`  
		Last Modified: Sat, 16 Oct 2021 02:50:49 GMT  
		Size: 100.0 MB (100010821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c03abd5daa700ddf866335aef47153c602aab661fc4e8a8cd6b920a3b78c6d9`  
		Last Modified: Sat, 16 Oct 2021 02:50:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bee7cb9969d594ee7bc764af007e4c0e9dbdd159efb7f78cd99599fe5d24227`  
		Last Modified: Sat, 16 Oct 2021 02:51:09 GMT  
		Size: 64.9 MB (64922456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d5fa4cfb7df399ade2516372c36c4997dd6b036fcf0fed2519961a0cc9cfca`  
		Last Modified: Sat, 16 Oct 2021 02:51:00 GMT  
		Size: 250.8 KB (250842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e07cbc601974d308056bc5dd837d1e5cf3f31275052df2573bbe28b172562`  
		Last Modified: Sat, 16 Oct 2021 02:50:59 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0000799c6000c28c01d2cfe4f94f943eea059b940290cb2bbeda007a003af9e`  
		Last Modified: Sat, 16 Oct 2021 02:51:02 GMT  
		Size: 21.4 MB (21426708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-base-focal`

```console
$ docker pull ros@sha256:65beaaee344167f62b4ff87373d84faa27e1ea73b5de15f1a59646bea87de4d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:23cfd590c135a42606747f60b888595a2ae00810f439dc4b78f4d4d2e04df476
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232089648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e88918e911975edd2d2ae88c1078561146665fdb1a836d044b132913f1a7cbf7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:41:01 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 03:41:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:41:44 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:41:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:41:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:42:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:42:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:42:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:42:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667bbaa58b18042bba7f627e73f63afc769ef1ba6dd8d02db26a97639896068`  
		Last Modified: Sat, 16 Oct 2021 03:51:07 GMT  
		Size: 103.6 MB (103626785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a680ad47ebc112dc93a40e8bd9e894aaf9519f94d0682ddd3fd48b7397cf56`  
		Last Modified: Sat, 16 Oct 2021 03:50:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99485d848bd2d8d3e44bc608ce7b5ded397a3875cd31a870b9204f6cf034156`  
		Last Modified: Sat, 16 Oct 2021 03:51:28 GMT  
		Size: 70.8 MB (70797181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0eba6427f6ee57b80c5edcf96532a72d18d44acf2723fcb86619039bbcfd4e`  
		Last Modified: Sat, 16 Oct 2021 03:51:18 GMT  
		Size: 250.9 KB (250902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec01b9342ad47c2d894dd5445179b44b59795f39844beddfe6e4ff69fcd8f8`  
		Last Modified: Sat, 16 Oct 2021 03:51:18 GMT  
		Size: 2.0 KB (2015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa73989292d31559372cc09b8599aba98531656e025666399df977d646028b`  
		Last Modified: Sat, 16 Oct 2021 03:51:21 GMT  
		Size: 22.1 MB (22109577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cad2d4c2bba24c8d1bc99484270c7187550f8478caba71e670ad4018db70f19f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.3 MB (220295241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1dc7d553defc3476d6d036001a2ebef1c69198b71864342ba12919988328c4a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:33:55 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 02:34:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:34:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:34:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:34:41 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:35:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:35:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:35:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3549f1d260e60d8924c9b7e02611c65b2136c4991bbccee64e068f45993511`  
		Last Modified: Sat, 16 Oct 2021 02:50:49 GMT  
		Size: 100.0 MB (100010821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c03abd5daa700ddf866335aef47153c602aab661fc4e8a8cd6b920a3b78c6d9`  
		Last Modified: Sat, 16 Oct 2021 02:50:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bee7cb9969d594ee7bc764af007e4c0e9dbdd159efb7f78cd99599fe5d24227`  
		Last Modified: Sat, 16 Oct 2021 02:51:09 GMT  
		Size: 64.9 MB (64922456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d5fa4cfb7df399ade2516372c36c4997dd6b036fcf0fed2519961a0cc9cfca`  
		Last Modified: Sat, 16 Oct 2021 02:51:00 GMT  
		Size: 250.8 KB (250842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e07cbc601974d308056bc5dd837d1e5cf3f31275052df2573bbe28b172562`  
		Last Modified: Sat, 16 Oct 2021 02:50:59 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0000799c6000c28c01d2cfe4f94f943eea059b940290cb2bbeda007a003af9e`  
		Last Modified: Sat, 16 Oct 2021 02:51:02 GMT  
		Size: 21.4 MB (21426708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:33dfbf45b6bdfe348ec3f49d87472240d5e298b198151ba67c0e7be6ab31ea07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:2db466601f573478dff37d6e9468aae47c56e0b70040b591e3d4bf6161cb928b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138929973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74de063e642332c68d62547ffa2d35b3ed568176b276221416ec38a3a57193ac`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:41:01 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 03:41:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:41:44 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:41:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:41:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667bbaa58b18042bba7f627e73f63afc769ef1ba6dd8d02db26a97639896068`  
		Last Modified: Sat, 16 Oct 2021 03:51:07 GMT  
		Size: 103.6 MB (103626785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a680ad47ebc112dc93a40e8bd9e894aaf9519f94d0682ddd3fd48b7397cf56`  
		Last Modified: Sat, 16 Oct 2021 03:50:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f8b7b03fa299fddd95769265d965960f04b1f19951e402ee747b3cf9b71d5dbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133693274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ccb605a13d195379dbf5f02e41aec3ad47029ac2387dfbda4ea2b70f868eb51`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:33:55 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 02:34:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:34:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:34:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:34:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3549f1d260e60d8924c9b7e02611c65b2136c4991bbccee64e068f45993511`  
		Last Modified: Sat, 16 Oct 2021 02:50:49 GMT  
		Size: 100.0 MB (100010821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c03abd5daa700ddf866335aef47153c602aab661fc4e8a8cd6b920a3b78c6d9`  
		Last Modified: Sat, 16 Oct 2021 02:50:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:33dfbf45b6bdfe348ec3f49d87472240d5e298b198151ba67c0e7be6ab31ea07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:2db466601f573478dff37d6e9468aae47c56e0b70040b591e3d4bf6161cb928b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138929973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74de063e642332c68d62547ffa2d35b3ed568176b276221416ec38a3a57193ac`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:41:01 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 03:41:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:41:44 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:41:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:41:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667bbaa58b18042bba7f627e73f63afc769ef1ba6dd8d02db26a97639896068`  
		Last Modified: Sat, 16 Oct 2021 03:51:07 GMT  
		Size: 103.6 MB (103626785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a680ad47ebc112dc93a40e8bd9e894aaf9519f94d0682ddd3fd48b7397cf56`  
		Last Modified: Sat, 16 Oct 2021 03:50:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f8b7b03fa299fddd95769265d965960f04b1f19951e402ee747b3cf9b71d5dbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133693274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ccb605a13d195379dbf5f02e41aec3ad47029ac2387dfbda4ea2b70f868eb51`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:33:55 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 02:34:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:34:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:34:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:34:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3549f1d260e60d8924c9b7e02611c65b2136c4991bbccee64e068f45993511`  
		Last Modified: Sat, 16 Oct 2021 02:50:49 GMT  
		Size: 100.0 MB (100010821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c03abd5daa700ddf866335aef47153c602aab661fc4e8a8cd6b920a3b78c6d9`  
		Last Modified: Sat, 16 Oct 2021 02:50:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:2460c7566039843af23a4225886759e22c4baed07b7614868be17609eab3edef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:c6dd40e51f57c2ec7e1b8738e8c26a6c475a648dd84e0a4deb9a28ce4ef28fd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326882035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f301a02130abaf6bbb58b78735b412ab18b95ba7732b267e56c41d0042546e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:41:01 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 03:41:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:41:44 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:41:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:41:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:42:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:42:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:42:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:42:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:42:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:42:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:42:43 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 03:42:43 GMT
ENV ROS2_DISTRO=galactic
# Sat, 16 Oct 2021 03:43:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:43:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:43:21 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667bbaa58b18042bba7f627e73f63afc769ef1ba6dd8d02db26a97639896068`  
		Last Modified: Sat, 16 Oct 2021 03:51:07 GMT  
		Size: 103.6 MB (103626785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a680ad47ebc112dc93a40e8bd9e894aaf9519f94d0682ddd3fd48b7397cf56`  
		Last Modified: Sat, 16 Oct 2021 03:50:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99485d848bd2d8d3e44bc608ce7b5ded397a3875cd31a870b9204f6cf034156`  
		Last Modified: Sat, 16 Oct 2021 03:51:28 GMT  
		Size: 70.8 MB (70797181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0eba6427f6ee57b80c5edcf96532a72d18d44acf2723fcb86619039bbcfd4e`  
		Last Modified: Sat, 16 Oct 2021 03:51:18 GMT  
		Size: 250.9 KB (250902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec01b9342ad47c2d894dd5445179b44b59795f39844beddfe6e4ff69fcd8f8`  
		Last Modified: Sat, 16 Oct 2021 03:51:18 GMT  
		Size: 2.0 KB (2015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa73989292d31559372cc09b8599aba98531656e025666399df977d646028b`  
		Last Modified: Sat, 16 Oct 2021 03:51:21 GMT  
		Size: 22.1 MB (22109577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6ab392dd7f78d2056a4c25f10f651ca439c1864d9cd6a1fbb27fc2935cb775`  
		Last Modified: Sat, 16 Oct 2021 03:51:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94ca8cbc799d108c3749d14472e55fd288c0e598eaa1b9edc53f0cf025cbac3`  
		Last Modified: Sat, 16 Oct 2021 03:51:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3af756f97cfe386dea5b1db3e1b5fe1f35ea544431b7291a007b670e582f862`  
		Last Modified: Sat, 16 Oct 2021 03:51:55 GMT  
		Size: 78.4 MB (78428180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe76e0e0d2ca464b408860b8e23a18a43452e301954cfe7bbc93d2c0a2278d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:44 GMT  
		Size: 16.4 MB (16363582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb2b71889a46b806951a881fb9dd19ab87702574bab162ec2564946c94b4248`  
		Last Modified: Sat, 16 Oct 2021 03:51:41 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:611804205cea57f17c89440b48101650ce1d61515b496d43a3f28b9e4b5b4523
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.1 MB (314114501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7738fa2f2e57d4f0ea940e4301ac4ddc546c31a474be7d02185684e9919a4eb5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:33:55 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 02:34:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:34:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:34:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:34:41 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:35:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:35:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:35:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:35:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:35:52 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 02:35:54 GMT
ENV ROS2_DISTRO=galactic
# Sat, 16 Oct 2021 02:36:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:36:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:36:50 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3549f1d260e60d8924c9b7e02611c65b2136c4991bbccee64e068f45993511`  
		Last Modified: Sat, 16 Oct 2021 02:50:49 GMT  
		Size: 100.0 MB (100010821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c03abd5daa700ddf866335aef47153c602aab661fc4e8a8cd6b920a3b78c6d9`  
		Last Modified: Sat, 16 Oct 2021 02:50:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bee7cb9969d594ee7bc764af007e4c0e9dbdd159efb7f78cd99599fe5d24227`  
		Last Modified: Sat, 16 Oct 2021 02:51:09 GMT  
		Size: 64.9 MB (64922456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d5fa4cfb7df399ade2516372c36c4997dd6b036fcf0fed2519961a0cc9cfca`  
		Last Modified: Sat, 16 Oct 2021 02:51:00 GMT  
		Size: 250.8 KB (250842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e07cbc601974d308056bc5dd837d1e5cf3f31275052df2573bbe28b172562`  
		Last Modified: Sat, 16 Oct 2021 02:50:59 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0000799c6000c28c01d2cfe4f94f943eea059b940290cb2bbeda007a003af9e`  
		Last Modified: Sat, 16 Oct 2021 02:51:02 GMT  
		Size: 21.4 MB (21426708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2851f2a6e5262082b1f79d371bd1027a38174d9acfc54c904de4322dd8a3a9`  
		Last Modified: Sat, 16 Oct 2021 02:51:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d940b7e8be291f71cd4fccbd8a9d1a3605e2afc316fe0b0a585842ddb079e93`  
		Last Modified: Sat, 16 Oct 2021 02:51:38 GMT  
		Size: 78.2 MB (78154188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fd20dbaace6c0249bf97438631a252e94c1375061c252235c665d890e6684c`  
		Last Modified: Sat, 16 Oct 2021 02:51:26 GMT  
		Size: 15.7 MB (15664601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5459c33b271053f26001f47c2a62cea83cea63737804c92278fb38390dbc233b`  
		Last Modified: Sat, 16 Oct 2021 02:51:23 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:galactic-ros1-bridge-focal`

```console
$ docker pull ros@sha256:2460c7566039843af23a4225886759e22c4baed07b7614868be17609eab3edef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:c6dd40e51f57c2ec7e1b8738e8c26a6c475a648dd84e0a4deb9a28ce4ef28fd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326882035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f301a02130abaf6bbb58b78735b412ab18b95ba7732b267e56c41d0042546e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:41:01 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 03:41:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:41:44 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:41:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:41:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:42:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:42:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:42:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:42:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:42:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:42:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:42:43 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 03:42:43 GMT
ENV ROS2_DISTRO=galactic
# Sat, 16 Oct 2021 03:43:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:43:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:43:21 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667bbaa58b18042bba7f627e73f63afc769ef1ba6dd8d02db26a97639896068`  
		Last Modified: Sat, 16 Oct 2021 03:51:07 GMT  
		Size: 103.6 MB (103626785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a680ad47ebc112dc93a40e8bd9e894aaf9519f94d0682ddd3fd48b7397cf56`  
		Last Modified: Sat, 16 Oct 2021 03:50:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99485d848bd2d8d3e44bc608ce7b5ded397a3875cd31a870b9204f6cf034156`  
		Last Modified: Sat, 16 Oct 2021 03:51:28 GMT  
		Size: 70.8 MB (70797181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0eba6427f6ee57b80c5edcf96532a72d18d44acf2723fcb86619039bbcfd4e`  
		Last Modified: Sat, 16 Oct 2021 03:51:18 GMT  
		Size: 250.9 KB (250902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec01b9342ad47c2d894dd5445179b44b59795f39844beddfe6e4ff69fcd8f8`  
		Last Modified: Sat, 16 Oct 2021 03:51:18 GMT  
		Size: 2.0 KB (2015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa73989292d31559372cc09b8599aba98531656e025666399df977d646028b`  
		Last Modified: Sat, 16 Oct 2021 03:51:21 GMT  
		Size: 22.1 MB (22109577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6ab392dd7f78d2056a4c25f10f651ca439c1864d9cd6a1fbb27fc2935cb775`  
		Last Modified: Sat, 16 Oct 2021 03:51:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94ca8cbc799d108c3749d14472e55fd288c0e598eaa1b9edc53f0cf025cbac3`  
		Last Modified: Sat, 16 Oct 2021 03:51:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3af756f97cfe386dea5b1db3e1b5fe1f35ea544431b7291a007b670e582f862`  
		Last Modified: Sat, 16 Oct 2021 03:51:55 GMT  
		Size: 78.4 MB (78428180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe76e0e0d2ca464b408860b8e23a18a43452e301954cfe7bbc93d2c0a2278d1`  
		Last Modified: Sat, 16 Oct 2021 03:51:44 GMT  
		Size: 16.4 MB (16363582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb2b71889a46b806951a881fb9dd19ab87702574bab162ec2564946c94b4248`  
		Last Modified: Sat, 16 Oct 2021 03:51:41 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:611804205cea57f17c89440b48101650ce1d61515b496d43a3f28b9e4b5b4523
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.1 MB (314114501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7738fa2f2e57d4f0ea940e4301ac4ddc546c31a474be7d02185684e9919a4eb5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:33:55 GMT
ENV ROS_DISTRO=galactic
# Sat, 16 Oct 2021 02:34:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:34:40 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:34:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:34:41 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:35:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:35:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:35:14 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:35:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:35:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:35:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:35:52 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 02:35:54 GMT
ENV ROS2_DISTRO=galactic
# Sat, 16 Oct 2021 02:36:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:36:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:36:50 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3549f1d260e60d8924c9b7e02611c65b2136c4991bbccee64e068f45993511`  
		Last Modified: Sat, 16 Oct 2021 02:50:49 GMT  
		Size: 100.0 MB (100010821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c03abd5daa700ddf866335aef47153c602aab661fc4e8a8cd6b920a3b78c6d9`  
		Last Modified: Sat, 16 Oct 2021 02:50:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bee7cb9969d594ee7bc764af007e4c0e9dbdd159efb7f78cd99599fe5d24227`  
		Last Modified: Sat, 16 Oct 2021 02:51:09 GMT  
		Size: 64.9 MB (64922456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d5fa4cfb7df399ade2516372c36c4997dd6b036fcf0fed2519961a0cc9cfca`  
		Last Modified: Sat, 16 Oct 2021 02:51:00 GMT  
		Size: 250.8 KB (250842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e07cbc601974d308056bc5dd837d1e5cf3f31275052df2573bbe28b172562`  
		Last Modified: Sat, 16 Oct 2021 02:50:59 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0000799c6000c28c01d2cfe4f94f943eea059b940290cb2bbeda007a003af9e`  
		Last Modified: Sat, 16 Oct 2021 02:51:02 GMT  
		Size: 21.4 MB (21426708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2851f2a6e5262082b1f79d371bd1027a38174d9acfc54c904de4322dd8a3a9`  
		Last Modified: Sat, 16 Oct 2021 02:51:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d940b7e8be291f71cd4fccbd8a9d1a3605e2afc316fe0b0a585842ddb079e93`  
		Last Modified: Sat, 16 Oct 2021 02:51:38 GMT  
		Size: 78.2 MB (78154188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fd20dbaace6c0249bf97438631a252e94c1375061c252235c665d890e6684c`  
		Last Modified: Sat, 16 Oct 2021 02:51:26 GMT  
		Size: 15.7 MB (15664601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5459c33b271053f26001f47c2a62cea83cea63737804c92278fb38390dbc233b`  
		Last Modified: Sat, 16 Oct 2021 02:51:23 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:c0b3b66cae3741dca25ed73a9263544a168dc66c6836ec84e3b33eaee3d6f0af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:96012077f6cd64756b7f1339ecaff8c6276cffdc2cb3d60dca783a6d28b65731
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.7 MB (236669874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ee1d4d17a982b8409772f9906b8116b0e8356cf69576df29080473e2f6d047`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 03:38:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:38:52 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:38:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:38:52 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:39:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:39:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:39:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:39:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ceb427087b3041b32a2be8c73788330f9675008ba201372eac0b4efc2cc18`  
		Last Modified: Sat, 16 Oct 2021 03:49:49 GMT  
		Size: 120.0 MB (119985810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e7b97e74c6f685d0d0a9362a5cf4a8769e1696bbf995293763867daaba3d19`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7748c6e4eab99c248c57227d0705c45d1b5c16a2a61bc6e2b4390c76f5346b70`  
		Last Modified: Sat, 16 Oct 2021 03:50:09 GMT  
		Size: 70.8 MB (70844958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204e3cb07dc82bf75a08f0e4498123299d9e74ab8013405bfcf2d7c06b149b00`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 244.9 KB (244893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbf530a707a11219db69d544ff5edbf747a4541147f82d4c0a9072da290fe8f`  
		Last Modified: Sat, 16 Oct 2021 03:49:59 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d0f031d5ee8d2a1754ef8291702f1ddc0a60f24fe9e0f529f7d6bbefa59828`  
		Last Modified: Sat, 16 Oct 2021 03:50:01 GMT  
		Size: 10.3 MB (10288974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4ec429ad8b1abecd8f150d381a44427a1d4501f91e4b83d2ebb765e77628cf65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.1 MB (212140824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67520d943e5f44778958f5a52344b173ae86cee024afaf866bd4b6310bb56d34`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:30:43 GMT
ENV ROS_DISTRO=foxy
# Sat, 16 Oct 2021 02:31:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:31:37 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:31:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:31:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:32:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:32:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:32:22 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:32:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149fc655748fb600fd752cb6805c8a4ca22cb195276c6222f500719d598fb59c`  
		Last Modified: Sat, 16 Oct 2021 02:49:26 GMT  
		Size: 104.2 MB (104159054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa569375e41dce495d90956baf65112208fd3655215fd4563bd0dd5a665da217`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b885237a11c3c3a5e31b49a568d28e2f32c00c1cde49be15ef946313a54218c`  
		Last Modified: Sat, 16 Oct 2021 02:49:47 GMT  
		Size: 65.0 MB (64966810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0695bf566d5652b3dd582cbc3fabac21343dc6476601a5fae98304412675a`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 244.8 KB (244842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8067ff73af3c358526193f7ea6d83e770f689e4b23865209c2b5f56b3d9d56`  
		Last Modified: Sat, 16 Oct 2021 02:49:38 GMT  
		Size: 2.0 KB (1980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85d6588bac0c377f420f223ef5eff321027f991a1cbf69f707bf743e3248758`  
		Last Modified: Sat, 16 Oct 2021 02:49:39 GMT  
		Size: 9.1 MB (9085686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:be382da2ecd6a236e02fe06da683760bf54c8e4363affb24f6abf0c8bfb1b557
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:6c99c80a97d9a6af8b830bd34c028e9a80d42138ab0d4ab9bfa78998c70c0954
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437374863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38caaa68c7ca79c4d362762f7247e2c807a9fd5f853a02aaae4e98b234c997e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:04acecfb9b8911a037727ca2a78502c80b888e42d6da628a42c2de4e56822718
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385882280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85fa2e457ee8085812f72b9b8e69931c8ea51bcd49d758276bc6f71b07d2bf8e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:47:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Oct 2021 22:48:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Oct 2021 22:48:19 GMT
ENV ROS_DISTRO=melodic
# Sat, 02 Oct 2021 22:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:51:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 02 Oct 2021 22:51:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Oct 2021 22:51:34 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:52:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:52:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Oct 2021 22:53:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c4e1c45e7370c0a89001ce3f27b8cb29dda1a3045cd21b5feb45b86814cc7`  
		Last Modified: Sat, 02 Oct 2021 23:10:35 GMT  
		Size: 841.6 KB (841600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761ddc01c5cd4707b222831b5c898c4b7c72dedbdf08c7c034c52e27d8fb48df`  
		Last Modified: Sat, 02 Oct 2021 23:10:34 GMT  
		Size: 4.1 MB (4085877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb81f09de324d7eafb7dc79196a2d1a0aaaaeff8cf5ac7d677a48cca9b9c11`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348110f0ae217262ab74d39bdb78bc24d293b05a66c566e992e393aa8636729f`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cea75c843f202719e12d6c0b65b06a1a2743414d67560aa090dfab89f781a`  
		Last Modified: Sat, 02 Oct 2021 23:13:03 GMT  
		Size: 238.9 MB (238932373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4a908a0a89a54ec468746bc176e64be9430edab2bf39917df6e1f5bebad7d8`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ef458d73013d5c9b799742848a41a1f9cbd78cbde326a39b803252e573e99d`  
		Last Modified: Sat, 02 Oct 2021 23:13:45 GMT  
		Size: 54.7 MB (54696354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bca198f4909aba3f932611e3d650c626d3d048ef94761ee6c32858e7e4b54e`  
		Last Modified: Sat, 02 Oct 2021 23:13:15 GMT  
		Size: 273.0 KB (273025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61086c7dd1564bcc465f85db1b7f2909f76c12955724943f3cc231f86fb8d123`  
		Last Modified: Sat, 02 Oct 2021 23:13:59 GMT  
		Size: 64.7 MB (64746332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e5239162ec4996a68f747d8b752f963e54c05186a59dc6a76dda4f6f8e0b23c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.5 MB (411534466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f31317abc163751ef8ad62ce84b944d92c3a1fa33a19bf4b00d33e99b244ec4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:13:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:14:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:14:19 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:14:20 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:14:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 Oct 2021 02:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:15:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:15:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:15:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:16:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:16:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b375d18c489948026f16ab6561023b9683664146a16727ea0d507f3212d10c88`  
		Last Modified: Sat, 16 Oct 2021 02:41:41 GMT  
		Size: 841.5 KB (841522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ee8d4939a8e2553ea047e48055e411b82560a018db242d498108e70b60627`  
		Last Modified: Sat, 16 Oct 2021 02:41:40 GMT  
		Size: 4.3 MB (4264000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862199e119a42d1ded50dd77acbe2078a38f8e1e7d178aa1132f95d77fc039d`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14963566c87e352863745e6c6c88f5e7dce6d77061d5c8585ba2f302da70ab7e`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4813509a2fdd51eb3e888f1b92d34fbeef04e05d071344ffb92fb8d5317a1a13`  
		Last Modified: Sat, 16 Oct 2021 02:42:15 GMT  
		Size: 252.4 MB (252356358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9e7629c2e32c08e9d73766f92d20e6568336a56f47e9a3452bef255c562a66`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cabbc72c38b3bd93fa364c1bf2771868db54d3addb7c6b38e4001f8bfe14a87`  
		Last Modified: Sat, 16 Oct 2021 02:42:35 GMT  
		Size: 63.1 MB (63067322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbeab3a7555411aa1fc5cc2196f41ba0abcd0974b1ddd8243eb0f81c05ac175`  
		Last Modified: Sat, 16 Oct 2021 02:42:27 GMT  
		Size: 273.4 KB (273368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feff670c1aa58b1e11ed8b369126064e9ced4f8439ff7696e3ce2bdfaca85df7`  
		Last Modified: Sat, 16 Oct 2021 02:42:38 GMT  
		Size: 67.0 MB (67002048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:e605e7f2b3c7d9bf763a549bdf04074d476cd65ccb750d062c1cf01772087a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:073274ee3ed4b8853373529777dc094d60f8a7690085cd8789f67e16608e3762
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742504012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eb9859ebf79cd993bb8f61e0a64932761983cf954bb32eb0dfb1220002a0958`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:01:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d2455ea11a3f51289e515125af2fd29538c49291c3d9de5bf605c367fd146c`  
		Last Modified: Fri, 01 Oct 2021 06:24:17 GMT  
		Size: 305.1 MB (305129149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:18983de90a8231f4772cbb4bd48f42d91307993c015347f3fd066acf16977f38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.7 MB (645744934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a57a275ef59016aa164b8013b4711ca65473bd2a171b44db6e165f690075900a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:47:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Oct 2021 22:48:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Oct 2021 22:48:19 GMT
ENV ROS_DISTRO=melodic
# Sat, 02 Oct 2021 22:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:51:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 02 Oct 2021 22:51:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Oct 2021 22:51:34 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:52:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:52:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Oct 2021 22:53:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c4e1c45e7370c0a89001ce3f27b8cb29dda1a3045cd21b5feb45b86814cc7`  
		Last Modified: Sat, 02 Oct 2021 23:10:35 GMT  
		Size: 841.6 KB (841600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761ddc01c5cd4707b222831b5c898c4b7c72dedbdf08c7c034c52e27d8fb48df`  
		Last Modified: Sat, 02 Oct 2021 23:10:34 GMT  
		Size: 4.1 MB (4085877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb81f09de324d7eafb7dc79196a2d1a0aaaaeff8cf5ac7d677a48cca9b9c11`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348110f0ae217262ab74d39bdb78bc24d293b05a66c566e992e393aa8636729f`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cea75c843f202719e12d6c0b65b06a1a2743414d67560aa090dfab89f781a`  
		Last Modified: Sat, 02 Oct 2021 23:13:03 GMT  
		Size: 238.9 MB (238932373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4a908a0a89a54ec468746bc176e64be9430edab2bf39917df6e1f5bebad7d8`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ef458d73013d5c9b799742848a41a1f9cbd78cbde326a39b803252e573e99d`  
		Last Modified: Sat, 02 Oct 2021 23:13:45 GMT  
		Size: 54.7 MB (54696354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bca198f4909aba3f932611e3d650c626d3d048ef94761ee6c32858e7e4b54e`  
		Last Modified: Sat, 02 Oct 2021 23:13:15 GMT  
		Size: 273.0 KB (273025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61086c7dd1564bcc465f85db1b7f2909f76c12955724943f3cc231f86fb8d123`  
		Last Modified: Sat, 02 Oct 2021 23:13:59 GMT  
		Size: 64.7 MB (64746332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16465df1d782cdcb744de354dd6c511ba96fc0c32309b7bccba13b42675d8113`  
		Last Modified: Sat, 02 Oct 2021 23:17:16 GMT  
		Size: 259.9 MB (259862654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4e7c19827d274fcb40f7234442642adba0a7d674ab2bf364510621db269a74c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **702.7 MB (702726122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4f3038799045cd962e13d2c148417bfa5a89a26f0e24df050b26401831afbb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:13:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:14:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:14:19 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:14:20 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:14:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 Oct 2021 02:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:15:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:15:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:15:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:16:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:16:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b375d18c489948026f16ab6561023b9683664146a16727ea0d507f3212d10c88`  
		Last Modified: Sat, 16 Oct 2021 02:41:41 GMT  
		Size: 841.5 KB (841522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ee8d4939a8e2553ea047e48055e411b82560a018db242d498108e70b60627`  
		Last Modified: Sat, 16 Oct 2021 02:41:40 GMT  
		Size: 4.3 MB (4264000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862199e119a42d1ded50dd77acbe2078a38f8e1e7d178aa1132f95d77fc039d`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14963566c87e352863745e6c6c88f5e7dce6d77061d5c8585ba2f302da70ab7e`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4813509a2fdd51eb3e888f1b92d34fbeef04e05d071344ffb92fb8d5317a1a13`  
		Last Modified: Sat, 16 Oct 2021 02:42:15 GMT  
		Size: 252.4 MB (252356358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9e7629c2e32c08e9d73766f92d20e6568336a56f47e9a3452bef255c562a66`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cabbc72c38b3bd93fa364c1bf2771868db54d3addb7c6b38e4001f8bfe14a87`  
		Last Modified: Sat, 16 Oct 2021 02:42:35 GMT  
		Size: 63.1 MB (63067322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbeab3a7555411aa1fc5cc2196f41ba0abcd0974b1ddd8243eb0f81c05ac175`  
		Last Modified: Sat, 16 Oct 2021 02:42:27 GMT  
		Size: 273.4 KB (273368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feff670c1aa58b1e11ed8b369126064e9ced4f8439ff7696e3ce2bdfaca85df7`  
		Last Modified: Sat, 16 Oct 2021 02:42:38 GMT  
		Size: 67.0 MB (67002048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5858acbdb2942a888f3985d26856d672b08a0762489ac0e103f6fbfaf63e5f0`  
		Last Modified: Sat, 16 Oct 2021 02:43:49 GMT  
		Size: 291.2 MB (291191656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:e605e7f2b3c7d9bf763a549bdf04074d476cd65ccb750d062c1cf01772087a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:073274ee3ed4b8853373529777dc094d60f8a7690085cd8789f67e16608e3762
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742504012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eb9859ebf79cd993bb8f61e0a64932761983cf954bb32eb0dfb1220002a0958`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:01:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d2455ea11a3f51289e515125af2fd29538c49291c3d9de5bf605c367fd146c`  
		Last Modified: Fri, 01 Oct 2021 06:24:17 GMT  
		Size: 305.1 MB (305129149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:18983de90a8231f4772cbb4bd48f42d91307993c015347f3fd066acf16977f38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.7 MB (645744934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a57a275ef59016aa164b8013b4711ca65473bd2a171b44db6e165f690075900a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:47:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Oct 2021 22:48:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Oct 2021 22:48:19 GMT
ENV ROS_DISTRO=melodic
# Sat, 02 Oct 2021 22:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:51:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 02 Oct 2021 22:51:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Oct 2021 22:51:34 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:52:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:52:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Oct 2021 22:53:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c4e1c45e7370c0a89001ce3f27b8cb29dda1a3045cd21b5feb45b86814cc7`  
		Last Modified: Sat, 02 Oct 2021 23:10:35 GMT  
		Size: 841.6 KB (841600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761ddc01c5cd4707b222831b5c898c4b7c72dedbdf08c7c034c52e27d8fb48df`  
		Last Modified: Sat, 02 Oct 2021 23:10:34 GMT  
		Size: 4.1 MB (4085877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb81f09de324d7eafb7dc79196a2d1a0aaaaeff8cf5ac7d677a48cca9b9c11`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348110f0ae217262ab74d39bdb78bc24d293b05a66c566e992e393aa8636729f`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cea75c843f202719e12d6c0b65b06a1a2743414d67560aa090dfab89f781a`  
		Last Modified: Sat, 02 Oct 2021 23:13:03 GMT  
		Size: 238.9 MB (238932373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4a908a0a89a54ec468746bc176e64be9430edab2bf39917df6e1f5bebad7d8`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ef458d73013d5c9b799742848a41a1f9cbd78cbde326a39b803252e573e99d`  
		Last Modified: Sat, 02 Oct 2021 23:13:45 GMT  
		Size: 54.7 MB (54696354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bca198f4909aba3f932611e3d650c626d3d048ef94761ee6c32858e7e4b54e`  
		Last Modified: Sat, 02 Oct 2021 23:13:15 GMT  
		Size: 273.0 KB (273025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61086c7dd1564bcc465f85db1b7f2909f76c12955724943f3cc231f86fb8d123`  
		Last Modified: Sat, 02 Oct 2021 23:13:59 GMT  
		Size: 64.7 MB (64746332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16465df1d782cdcb744de354dd6c511ba96fc0c32309b7bccba13b42675d8113`  
		Last Modified: Sat, 02 Oct 2021 23:17:16 GMT  
		Size: 259.9 MB (259862654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4e7c19827d274fcb40f7234442642adba0a7d674ab2bf364510621db269a74c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **702.7 MB (702726122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4f3038799045cd962e13d2c148417bfa5a89a26f0e24df050b26401831afbb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:13:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:14:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:14:19 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:14:20 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:14:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 Oct 2021 02:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:15:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:15:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:15:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:16:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:16:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b375d18c489948026f16ab6561023b9683664146a16727ea0d507f3212d10c88`  
		Last Modified: Sat, 16 Oct 2021 02:41:41 GMT  
		Size: 841.5 KB (841522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ee8d4939a8e2553ea047e48055e411b82560a018db242d498108e70b60627`  
		Last Modified: Sat, 16 Oct 2021 02:41:40 GMT  
		Size: 4.3 MB (4264000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862199e119a42d1ded50dd77acbe2078a38f8e1e7d178aa1132f95d77fc039d`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14963566c87e352863745e6c6c88f5e7dce6d77061d5c8585ba2f302da70ab7e`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4813509a2fdd51eb3e888f1b92d34fbeef04e05d071344ffb92fb8d5317a1a13`  
		Last Modified: Sat, 16 Oct 2021 02:42:15 GMT  
		Size: 252.4 MB (252356358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9e7629c2e32c08e9d73766f92d20e6568336a56f47e9a3452bef255c562a66`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cabbc72c38b3bd93fa364c1bf2771868db54d3addb7c6b38e4001f8bfe14a87`  
		Last Modified: Sat, 16 Oct 2021 02:42:35 GMT  
		Size: 63.1 MB (63067322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbeab3a7555411aa1fc5cc2196f41ba0abcd0974b1ddd8243eb0f81c05ac175`  
		Last Modified: Sat, 16 Oct 2021 02:42:27 GMT  
		Size: 273.4 KB (273368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feff670c1aa58b1e11ed8b369126064e9ced4f8439ff7696e3ce2bdfaca85df7`  
		Last Modified: Sat, 16 Oct 2021 02:42:38 GMT  
		Size: 67.0 MB (67002048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5858acbdb2942a888f3985d26856d672b08a0762489ac0e103f6fbfaf63e5f0`  
		Last Modified: Sat, 16 Oct 2021 02:43:49 GMT  
		Size: 291.2 MB (291191656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:e70d3464abf83af48fdef1c60044628bf2ef3cfcd79d45ded06f593003e4213f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:2068a86fbf546af4d2cd04b0e08afa70e29d1381be8b26aa46a966da11982009
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448453243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b178cafe1ea49750b6b35cef8398a435e36e0fecde1734d6c237952eb817cc7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:55:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03991905598cbe2e1c4ae3b3c38af7910c05944eaaac7548daec1a84855a5bd4`  
		Last Modified: Fri, 01 Oct 2021 06:23:21 GMT  
		Size: 11.1 MB (11078380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:c5a8352da1891710826f59f1449c268663e049f964388d43ce7304dc4a01e158
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396003438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c14ee4a12e3290174f0e8cdbd172eedfea35785d16d298d14a22e5ea2c183018`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:47:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Oct 2021 22:48:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Oct 2021 22:48:19 GMT
ENV ROS_DISTRO=melodic
# Sat, 02 Oct 2021 22:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:51:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 02 Oct 2021 22:51:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Oct 2021 22:51:34 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:52:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:52:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Oct 2021 22:53:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:54:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c4e1c45e7370c0a89001ce3f27b8cb29dda1a3045cd21b5feb45b86814cc7`  
		Last Modified: Sat, 02 Oct 2021 23:10:35 GMT  
		Size: 841.6 KB (841600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761ddc01c5cd4707b222831b5c898c4b7c72dedbdf08c7c034c52e27d8fb48df`  
		Last Modified: Sat, 02 Oct 2021 23:10:34 GMT  
		Size: 4.1 MB (4085877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb81f09de324d7eafb7dc79196a2d1a0aaaaeff8cf5ac7d677a48cca9b9c11`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348110f0ae217262ab74d39bdb78bc24d293b05a66c566e992e393aa8636729f`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cea75c843f202719e12d6c0b65b06a1a2743414d67560aa090dfab89f781a`  
		Last Modified: Sat, 02 Oct 2021 23:13:03 GMT  
		Size: 238.9 MB (238932373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4a908a0a89a54ec468746bc176e64be9430edab2bf39917df6e1f5bebad7d8`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ef458d73013d5c9b799742848a41a1f9cbd78cbde326a39b803252e573e99d`  
		Last Modified: Sat, 02 Oct 2021 23:13:45 GMT  
		Size: 54.7 MB (54696354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bca198f4909aba3f932611e3d650c626d3d048ef94761ee6c32858e7e4b54e`  
		Last Modified: Sat, 02 Oct 2021 23:13:15 GMT  
		Size: 273.0 KB (273025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61086c7dd1564bcc465f85db1b7f2909f76c12955724943f3cc231f86fb8d123`  
		Last Modified: Sat, 02 Oct 2021 23:13:59 GMT  
		Size: 64.7 MB (64746332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f065e02bc77045d335e7e916e032acac076408cc0601a0541e5880438c6173`  
		Last Modified: Sat, 02 Oct 2021 23:14:23 GMT  
		Size: 10.1 MB (10121158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:55adcec7df0fe472d169a29eb71a1a1a980016075c544146ff6db0932dec7b49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.3 MB (422262375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb22982445c9975ae941f18159a931abd4ad545cfcf0b2c2782f6bf73225e73`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:13:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:14:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:14:19 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:14:20 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:14:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 Oct 2021 02:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:15:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:15:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:15:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:16:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:16:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b375d18c489948026f16ab6561023b9683664146a16727ea0d507f3212d10c88`  
		Last Modified: Sat, 16 Oct 2021 02:41:41 GMT  
		Size: 841.5 KB (841522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ee8d4939a8e2553ea047e48055e411b82560a018db242d498108e70b60627`  
		Last Modified: Sat, 16 Oct 2021 02:41:40 GMT  
		Size: 4.3 MB (4264000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862199e119a42d1ded50dd77acbe2078a38f8e1e7d178aa1132f95d77fc039d`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14963566c87e352863745e6c6c88f5e7dce6d77061d5c8585ba2f302da70ab7e`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4813509a2fdd51eb3e888f1b92d34fbeef04e05d071344ffb92fb8d5317a1a13`  
		Last Modified: Sat, 16 Oct 2021 02:42:15 GMT  
		Size: 252.4 MB (252356358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9e7629c2e32c08e9d73766f92d20e6568336a56f47e9a3452bef255c562a66`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cabbc72c38b3bd93fa364c1bf2771868db54d3addb7c6b38e4001f8bfe14a87`  
		Last Modified: Sat, 16 Oct 2021 02:42:35 GMT  
		Size: 63.1 MB (63067322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbeab3a7555411aa1fc5cc2196f41ba0abcd0974b1ddd8243eb0f81c05ac175`  
		Last Modified: Sat, 16 Oct 2021 02:42:27 GMT  
		Size: 273.4 KB (273368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feff670c1aa58b1e11ed8b369126064e9ced4f8439ff7696e3ce2bdfaca85df7`  
		Last Modified: Sat, 16 Oct 2021 02:42:38 GMT  
		Size: 67.0 MB (67002048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7a003f55f36db1da1751d86c408d72cb2a04485f660ec1362b4af0ca71fe90`  
		Last Modified: Sat, 16 Oct 2021 02:42:53 GMT  
		Size: 10.7 MB (10727909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:e70d3464abf83af48fdef1c60044628bf2ef3cfcd79d45ded06f593003e4213f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:2068a86fbf546af4d2cd04b0e08afa70e29d1381be8b26aa46a966da11982009
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448453243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b178cafe1ea49750b6b35cef8398a435e36e0fecde1734d6c237952eb817cc7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:55:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03991905598cbe2e1c4ae3b3c38af7910c05944eaaac7548daec1a84855a5bd4`  
		Last Modified: Fri, 01 Oct 2021 06:23:21 GMT  
		Size: 11.1 MB (11078380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:c5a8352da1891710826f59f1449c268663e049f964388d43ce7304dc4a01e158
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396003438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c14ee4a12e3290174f0e8cdbd172eedfea35785d16d298d14a22e5ea2c183018`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:47:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Oct 2021 22:48:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Oct 2021 22:48:19 GMT
ENV ROS_DISTRO=melodic
# Sat, 02 Oct 2021 22:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:51:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 02 Oct 2021 22:51:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Oct 2021 22:51:34 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:52:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:52:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Oct 2021 22:53:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:54:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c4e1c45e7370c0a89001ce3f27b8cb29dda1a3045cd21b5feb45b86814cc7`  
		Last Modified: Sat, 02 Oct 2021 23:10:35 GMT  
		Size: 841.6 KB (841600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761ddc01c5cd4707b222831b5c898c4b7c72dedbdf08c7c034c52e27d8fb48df`  
		Last Modified: Sat, 02 Oct 2021 23:10:34 GMT  
		Size: 4.1 MB (4085877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb81f09de324d7eafb7dc79196a2d1a0aaaaeff8cf5ac7d677a48cca9b9c11`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348110f0ae217262ab74d39bdb78bc24d293b05a66c566e992e393aa8636729f`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cea75c843f202719e12d6c0b65b06a1a2743414d67560aa090dfab89f781a`  
		Last Modified: Sat, 02 Oct 2021 23:13:03 GMT  
		Size: 238.9 MB (238932373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4a908a0a89a54ec468746bc176e64be9430edab2bf39917df6e1f5bebad7d8`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ef458d73013d5c9b799742848a41a1f9cbd78cbde326a39b803252e573e99d`  
		Last Modified: Sat, 02 Oct 2021 23:13:45 GMT  
		Size: 54.7 MB (54696354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bca198f4909aba3f932611e3d650c626d3d048ef94761ee6c32858e7e4b54e`  
		Last Modified: Sat, 02 Oct 2021 23:13:15 GMT  
		Size: 273.0 KB (273025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61086c7dd1564bcc465f85db1b7f2909f76c12955724943f3cc231f86fb8d123`  
		Last Modified: Sat, 02 Oct 2021 23:13:59 GMT  
		Size: 64.7 MB (64746332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f065e02bc77045d335e7e916e032acac076408cc0601a0541e5880438c6173`  
		Last Modified: Sat, 02 Oct 2021 23:14:23 GMT  
		Size: 10.1 MB (10121158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:55adcec7df0fe472d169a29eb71a1a1a980016075c544146ff6db0932dec7b49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.3 MB (422262375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb22982445c9975ae941f18159a931abd4ad545cfcf0b2c2782f6bf73225e73`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:13:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:14:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:14:19 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:14:20 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:14:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 Oct 2021 02:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:15:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:15:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:15:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:16:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:16:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b375d18c489948026f16ab6561023b9683664146a16727ea0d507f3212d10c88`  
		Last Modified: Sat, 16 Oct 2021 02:41:41 GMT  
		Size: 841.5 KB (841522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ee8d4939a8e2553ea047e48055e411b82560a018db242d498108e70b60627`  
		Last Modified: Sat, 16 Oct 2021 02:41:40 GMT  
		Size: 4.3 MB (4264000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862199e119a42d1ded50dd77acbe2078a38f8e1e7d178aa1132f95d77fc039d`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14963566c87e352863745e6c6c88f5e7dce6d77061d5c8585ba2f302da70ab7e`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4813509a2fdd51eb3e888f1b92d34fbeef04e05d071344ffb92fb8d5317a1a13`  
		Last Modified: Sat, 16 Oct 2021 02:42:15 GMT  
		Size: 252.4 MB (252356358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9e7629c2e32c08e9d73766f92d20e6568336a56f47e9a3452bef255c562a66`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cabbc72c38b3bd93fa364c1bf2771868db54d3addb7c6b38e4001f8bfe14a87`  
		Last Modified: Sat, 16 Oct 2021 02:42:35 GMT  
		Size: 63.1 MB (63067322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbeab3a7555411aa1fc5cc2196f41ba0abcd0974b1ddd8243eb0f81c05ac175`  
		Last Modified: Sat, 16 Oct 2021 02:42:27 GMT  
		Size: 273.4 KB (273368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feff670c1aa58b1e11ed8b369126064e9ced4f8439ff7696e3ce2bdfaca85df7`  
		Last Modified: Sat, 16 Oct 2021 02:42:38 GMT  
		Size: 67.0 MB (67002048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7a003f55f36db1da1751d86c408d72cb2a04485f660ec1362b4af0ca71fe90`  
		Last Modified: Sat, 16 Oct 2021 02:42:53 GMT  
		Size: 10.7 MB (10727909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:be382da2ecd6a236e02fe06da683760bf54c8e4363affb24f6abf0c8bfb1b557
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:6c99c80a97d9a6af8b830bd34c028e9a80d42138ab0d4ab9bfa78998c70c0954
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437374863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38caaa68c7ca79c4d362762f7247e2c807a9fd5f853a02aaae4e98b234c997e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:04acecfb9b8911a037727ca2a78502c80b888e42d6da628a42c2de4e56822718
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385882280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85fa2e457ee8085812f72b9b8e69931c8ea51bcd49d758276bc6f71b07d2bf8e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:47:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Oct 2021 22:48:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Oct 2021 22:48:19 GMT
ENV ROS_DISTRO=melodic
# Sat, 02 Oct 2021 22:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:51:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 02 Oct 2021 22:51:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Oct 2021 22:51:34 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:52:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:52:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Oct 2021 22:53:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c4e1c45e7370c0a89001ce3f27b8cb29dda1a3045cd21b5feb45b86814cc7`  
		Last Modified: Sat, 02 Oct 2021 23:10:35 GMT  
		Size: 841.6 KB (841600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761ddc01c5cd4707b222831b5c898c4b7c72dedbdf08c7c034c52e27d8fb48df`  
		Last Modified: Sat, 02 Oct 2021 23:10:34 GMT  
		Size: 4.1 MB (4085877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb81f09de324d7eafb7dc79196a2d1a0aaaaeff8cf5ac7d677a48cca9b9c11`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348110f0ae217262ab74d39bdb78bc24d293b05a66c566e992e393aa8636729f`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cea75c843f202719e12d6c0b65b06a1a2743414d67560aa090dfab89f781a`  
		Last Modified: Sat, 02 Oct 2021 23:13:03 GMT  
		Size: 238.9 MB (238932373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4a908a0a89a54ec468746bc176e64be9430edab2bf39917df6e1f5bebad7d8`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ef458d73013d5c9b799742848a41a1f9cbd78cbde326a39b803252e573e99d`  
		Last Modified: Sat, 02 Oct 2021 23:13:45 GMT  
		Size: 54.7 MB (54696354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bca198f4909aba3f932611e3d650c626d3d048ef94761ee6c32858e7e4b54e`  
		Last Modified: Sat, 02 Oct 2021 23:13:15 GMT  
		Size: 273.0 KB (273025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61086c7dd1564bcc465f85db1b7f2909f76c12955724943f3cc231f86fb8d123`  
		Last Modified: Sat, 02 Oct 2021 23:13:59 GMT  
		Size: 64.7 MB (64746332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e5239162ec4996a68f747d8b752f963e54c05186a59dc6a76dda4f6f8e0b23c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.5 MB (411534466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f31317abc163751ef8ad62ce84b944d92c3a1fa33a19bf4b00d33e99b244ec4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:13:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:14:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:14:19 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:14:20 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:14:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 Oct 2021 02:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:15:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:15:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:15:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:16:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:16:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b375d18c489948026f16ab6561023b9683664146a16727ea0d507f3212d10c88`  
		Last Modified: Sat, 16 Oct 2021 02:41:41 GMT  
		Size: 841.5 KB (841522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ee8d4939a8e2553ea047e48055e411b82560a018db242d498108e70b60627`  
		Last Modified: Sat, 16 Oct 2021 02:41:40 GMT  
		Size: 4.3 MB (4264000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862199e119a42d1ded50dd77acbe2078a38f8e1e7d178aa1132f95d77fc039d`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14963566c87e352863745e6c6c88f5e7dce6d77061d5c8585ba2f302da70ab7e`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4813509a2fdd51eb3e888f1b92d34fbeef04e05d071344ffb92fb8d5317a1a13`  
		Last Modified: Sat, 16 Oct 2021 02:42:15 GMT  
		Size: 252.4 MB (252356358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9e7629c2e32c08e9d73766f92d20e6568336a56f47e9a3452bef255c562a66`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cabbc72c38b3bd93fa364c1bf2771868db54d3addb7c6b38e4001f8bfe14a87`  
		Last Modified: Sat, 16 Oct 2021 02:42:35 GMT  
		Size: 63.1 MB (63067322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbeab3a7555411aa1fc5cc2196f41ba0abcd0974b1ddd8243eb0f81c05ac175`  
		Last Modified: Sat, 16 Oct 2021 02:42:27 GMT  
		Size: 273.4 KB (273368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feff670c1aa58b1e11ed8b369126064e9ced4f8439ff7696e3ce2bdfaca85df7`  
		Last Modified: Sat, 16 Oct 2021 02:42:38 GMT  
		Size: 67.0 MB (67002048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:be382da2ecd6a236e02fe06da683760bf54c8e4363affb24f6abf0c8bfb1b557
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:6c99c80a97d9a6af8b830bd34c028e9a80d42138ab0d4ab9bfa78998c70c0954
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437374863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38caaa68c7ca79c4d362762f7247e2c807a9fd5f853a02aaae4e98b234c997e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:04acecfb9b8911a037727ca2a78502c80b888e42d6da628a42c2de4e56822718
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385882280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85fa2e457ee8085812f72b9b8e69931c8ea51bcd49d758276bc6f71b07d2bf8e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:47:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Oct 2021 22:48:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Oct 2021 22:48:19 GMT
ENV ROS_DISTRO=melodic
# Sat, 02 Oct 2021 22:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:51:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 02 Oct 2021 22:51:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Oct 2021 22:51:34 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:52:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:52:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Oct 2021 22:53:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c4e1c45e7370c0a89001ce3f27b8cb29dda1a3045cd21b5feb45b86814cc7`  
		Last Modified: Sat, 02 Oct 2021 23:10:35 GMT  
		Size: 841.6 KB (841600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761ddc01c5cd4707b222831b5c898c4b7c72dedbdf08c7c034c52e27d8fb48df`  
		Last Modified: Sat, 02 Oct 2021 23:10:34 GMT  
		Size: 4.1 MB (4085877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb81f09de324d7eafb7dc79196a2d1a0aaaaeff8cf5ac7d677a48cca9b9c11`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348110f0ae217262ab74d39bdb78bc24d293b05a66c566e992e393aa8636729f`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cea75c843f202719e12d6c0b65b06a1a2743414d67560aa090dfab89f781a`  
		Last Modified: Sat, 02 Oct 2021 23:13:03 GMT  
		Size: 238.9 MB (238932373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4a908a0a89a54ec468746bc176e64be9430edab2bf39917df6e1f5bebad7d8`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ef458d73013d5c9b799742848a41a1f9cbd78cbde326a39b803252e573e99d`  
		Last Modified: Sat, 02 Oct 2021 23:13:45 GMT  
		Size: 54.7 MB (54696354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bca198f4909aba3f932611e3d650c626d3d048ef94761ee6c32858e7e4b54e`  
		Last Modified: Sat, 02 Oct 2021 23:13:15 GMT  
		Size: 273.0 KB (273025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61086c7dd1564bcc465f85db1b7f2909f76c12955724943f3cc231f86fb8d123`  
		Last Modified: Sat, 02 Oct 2021 23:13:59 GMT  
		Size: 64.7 MB (64746332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e5239162ec4996a68f747d8b752f963e54c05186a59dc6a76dda4f6f8e0b23c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.5 MB (411534466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f31317abc163751ef8ad62ce84b944d92c3a1fa33a19bf4b00d33e99b244ec4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:13:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:14:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:14:19 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:14:20 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:14:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 Oct 2021 02:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:15:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:15:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:15:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:16:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:16:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b375d18c489948026f16ab6561023b9683664146a16727ea0d507f3212d10c88`  
		Last Modified: Sat, 16 Oct 2021 02:41:41 GMT  
		Size: 841.5 KB (841522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ee8d4939a8e2553ea047e48055e411b82560a018db242d498108e70b60627`  
		Last Modified: Sat, 16 Oct 2021 02:41:40 GMT  
		Size: 4.3 MB (4264000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862199e119a42d1ded50dd77acbe2078a38f8e1e7d178aa1132f95d77fc039d`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14963566c87e352863745e6c6c88f5e7dce6d77061d5c8585ba2f302da70ab7e`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4813509a2fdd51eb3e888f1b92d34fbeef04e05d071344ffb92fb8d5317a1a13`  
		Last Modified: Sat, 16 Oct 2021 02:42:15 GMT  
		Size: 252.4 MB (252356358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9e7629c2e32c08e9d73766f92d20e6568336a56f47e9a3452bef255c562a66`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cabbc72c38b3bd93fa364c1bf2771868db54d3addb7c6b38e4001f8bfe14a87`  
		Last Modified: Sat, 16 Oct 2021 02:42:35 GMT  
		Size: 63.1 MB (63067322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbeab3a7555411aa1fc5cc2196f41ba0abcd0974b1ddd8243eb0f81c05ac175`  
		Last Modified: Sat, 16 Oct 2021 02:42:27 GMT  
		Size: 273.4 KB (273368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feff670c1aa58b1e11ed8b369126064e9ced4f8439ff7696e3ce2bdfaca85df7`  
		Last Modified: Sat, 16 Oct 2021 02:42:38 GMT  
		Size: 67.0 MB (67002048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:6c992c952fe41085e2ec1482bb5e1cf482a27ea6e3f362bf26b779e9a2b9851b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:5da99077487fb6a23334589c87442544965eff9960b0aef3bb5b385f60d6264a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291875817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ddab15692c93b05ddb281246caa09b9c5d97794a953a331cf7a991ee9f7e8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:ff7b3cf8acc651cc8db8e00e23bde7c1a1dad1b782efafa4100b30074b5e0671
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266166569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e9387a219849b2f096f1f2a9bc96cc52652f998913fbe0c93f32dec6197720b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:47:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Oct 2021 22:48:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Oct 2021 22:48:19 GMT
ENV ROS_DISTRO=melodic
# Sat, 02 Oct 2021 22:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:51:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 02 Oct 2021 22:51:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Oct 2021 22:51:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c4e1c45e7370c0a89001ce3f27b8cb29dda1a3045cd21b5feb45b86814cc7`  
		Last Modified: Sat, 02 Oct 2021 23:10:35 GMT  
		Size: 841.6 KB (841600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761ddc01c5cd4707b222831b5c898c4b7c72dedbdf08c7c034c52e27d8fb48df`  
		Last Modified: Sat, 02 Oct 2021 23:10:34 GMT  
		Size: 4.1 MB (4085877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb81f09de324d7eafb7dc79196a2d1a0aaaaeff8cf5ac7d677a48cca9b9c11`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348110f0ae217262ab74d39bdb78bc24d293b05a66c566e992e393aa8636729f`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cea75c843f202719e12d6c0b65b06a1a2743414d67560aa090dfab89f781a`  
		Last Modified: Sat, 02 Oct 2021 23:13:03 GMT  
		Size: 238.9 MB (238932373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4a908a0a89a54ec468746bc176e64be9430edab2bf39917df6e1f5bebad7d8`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3467b62a7088be32b61d81003a6de699e1e5ab978d5b06eb36fb656ce5e973d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281191728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd76c961d2c696ec7389d7e89b43c024d85a7845a975dda843a5b67f106c4d8c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:13:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:14:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:14:19 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:14:20 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:14:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 Oct 2021 02:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:15:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:15:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:15:39 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b375d18c489948026f16ab6561023b9683664146a16727ea0d507f3212d10c88`  
		Last Modified: Sat, 16 Oct 2021 02:41:41 GMT  
		Size: 841.5 KB (841522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ee8d4939a8e2553ea047e48055e411b82560a018db242d498108e70b60627`  
		Last Modified: Sat, 16 Oct 2021 02:41:40 GMT  
		Size: 4.3 MB (4264000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862199e119a42d1ded50dd77acbe2078a38f8e1e7d178aa1132f95d77fc039d`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14963566c87e352863745e6c6c88f5e7dce6d77061d5c8585ba2f302da70ab7e`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4813509a2fdd51eb3e888f1b92d34fbeef04e05d071344ffb92fb8d5317a1a13`  
		Last Modified: Sat, 16 Oct 2021 02:42:15 GMT  
		Size: 252.4 MB (252356358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9e7629c2e32c08e9d73766f92d20e6568336a56f47e9a3452bef255c562a66`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:6c992c952fe41085e2ec1482bb5e1cf482a27ea6e3f362bf26b779e9a2b9851b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:5da99077487fb6a23334589c87442544965eff9960b0aef3bb5b385f60d6264a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291875817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ddab15692c93b05ddb281246caa09b9c5d97794a953a331cf7a991ee9f7e8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:ff7b3cf8acc651cc8db8e00e23bde7c1a1dad1b782efafa4100b30074b5e0671
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266166569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e9387a219849b2f096f1f2a9bc96cc52652f998913fbe0c93f32dec6197720b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:47:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Oct 2021 22:48:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Oct 2021 22:48:19 GMT
ENV ROS_DISTRO=melodic
# Sat, 02 Oct 2021 22:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:51:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 02 Oct 2021 22:51:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Oct 2021 22:51:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c4e1c45e7370c0a89001ce3f27b8cb29dda1a3045cd21b5feb45b86814cc7`  
		Last Modified: Sat, 02 Oct 2021 23:10:35 GMT  
		Size: 841.6 KB (841600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761ddc01c5cd4707b222831b5c898c4b7c72dedbdf08c7c034c52e27d8fb48df`  
		Last Modified: Sat, 02 Oct 2021 23:10:34 GMT  
		Size: 4.1 MB (4085877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb81f09de324d7eafb7dc79196a2d1a0aaaaeff8cf5ac7d677a48cca9b9c11`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348110f0ae217262ab74d39bdb78bc24d293b05a66c566e992e393aa8636729f`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cea75c843f202719e12d6c0b65b06a1a2743414d67560aa090dfab89f781a`  
		Last Modified: Sat, 02 Oct 2021 23:13:03 GMT  
		Size: 238.9 MB (238932373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4a908a0a89a54ec468746bc176e64be9430edab2bf39917df6e1f5bebad7d8`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3467b62a7088be32b61d81003a6de699e1e5ab978d5b06eb36fb656ce5e973d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281191728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd76c961d2c696ec7389d7e89b43c024d85a7845a975dda843a5b67f106c4d8c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:38 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Sat, 16 Oct 2021 01:47:38 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:13:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:14:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:14:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:14:19 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:14:20 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:14:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 Oct 2021 02:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:15:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:15:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:15:39 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b375d18c489948026f16ab6561023b9683664146a16727ea0d507f3212d10c88`  
		Last Modified: Sat, 16 Oct 2021 02:41:41 GMT  
		Size: 841.5 KB (841522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ee8d4939a8e2553ea047e48055e411b82560a018db242d498108e70b60627`  
		Last Modified: Sat, 16 Oct 2021 02:41:40 GMT  
		Size: 4.3 MB (4264000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862199e119a42d1ded50dd77acbe2078a38f8e1e7d178aa1132f95d77fc039d`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14963566c87e352863745e6c6c88f5e7dce6d77061d5c8585ba2f302da70ab7e`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4813509a2fdd51eb3e888f1b92d34fbeef04e05d071344ffb92fb8d5317a1a13`  
		Last Modified: Sat, 16 Oct 2021 02:42:15 GMT  
		Size: 252.4 MB (252356358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9e7629c2e32c08e9d73766f92d20e6568336a56f47e9a3452bef255c562a66`  
		Last Modified: Sat, 16 Oct 2021 02:41:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic`

```console
$ docker pull ros@sha256:ef2030579a6637986cc03e6418adb14f3b684b991a295b367852c1d7dd09aafc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:2d75db570a0b16a6dc075c45c8263252fbeee945b9333eed33ff98af49c58895
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339197678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ead05d68f2187667ad2a43b6fcf6349e150e77bc13f7917591f87f7fdb4836`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:26:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 03:28:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 03:28:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:28:05 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:28:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef1669a6b741da8d10348ca5478bc92ed459dd5ae9dc872bc2901aa4a4885a`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7bc8cdeda44965808907e244e5edd3ed9d6efd6c0105fc84123b986946a806`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b82bc5a2b4db46195d4cb9bb39816b83ede6c31f565651abb9b15e6d4335ee8`  
		Last Modified: Sat, 16 Oct 2021 03:47:14 GMT  
		Size: 176.7 MB (176707219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389d5741667b5453a3f2fd8e79c5521bf1f17e95d6042d56595b80623e04aba`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d0df0db2441b7744370d28a551a1152f79b7249050aa09e18996bbd0428ebf`  
		Last Modified: Sat, 16 Oct 2021 03:47:32 GMT  
		Size: 47.3 MB (47259872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80707a4f3d4ddd0562cb757ab166458ffe0a134b59935f1619d10653486a8049`  
		Last Modified: Sat, 16 Oct 2021 03:47:24 GMT  
		Size: 322.9 KB (322897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626c61368773f58359917c9e5cd1e8c6555b27f66d55fda64ca5306f6748046b`  
		Last Modified: Sat, 16 Oct 2021 03:47:37 GMT  
		Size: 79.6 MB (79604503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:0a3716d6cb18a81fec1cfc5432a842d427d986e07b8d7665dba5fb18bb1b6687
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c32c2fedb278f6c38d9255abb83eedd072db50ee75a9e3462dac4cb7832785`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:17:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:17:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:17:55 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:17 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:22:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764ddf81fcf398a2a4cf14036409b82f4f4a06bd8f23171e840ff36accba4d4f`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 1.2 MB (1186846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02b4dedc9080b63cee4513e2787d54376223246780de27866414412fce505a7`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 4.7 MB (4676770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb049eda64c876c1ee585dd51f3f8b9a9807c82541e8243ea725bcf5ee59fb2c`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7037e3e565c8acccf66678f470f9ceae8503c90974e2dd927764191193ffdbb`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69724b9a0973ce0c31fba9293b5ca2cc8e252ee13673b3053258594c1fa8b815`  
		Last Modified: Sat, 16 Oct 2021 02:31:48 GMT  
		Size: 157.2 MB (157179504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df68017d0a78706560ec19c60581120f31997ecd5e9223e1eec432c47ae86e8`  
		Last Modified: Sat, 16 Oct 2021 02:29:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb98f2a916633a1fb1a69dd5aebc5416fb396d43233943523788ff874a76fde`  
		Last Modified: Sat, 16 Oct 2021 02:32:19 GMT  
		Size: 36.7 MB (36691673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242c94fc3e260adf5325a33e1e99237f52197a87e7ea5b471bdd8bd9eb4b0b0`  
		Last Modified: Sat, 16 Oct 2021 02:32:00 GMT  
		Size: 322.9 KB (322903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5bbb4e057a5f879119a31a98e9617ab535d39046bf80b55735ded907115af3`  
		Last Modified: Sat, 16 Oct 2021 02:32:38 GMT  
		Size: 60.5 MB (60484275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ec02baf086f3161863a635d2b2df2454d0295eebf71581502327d6660c166562
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318192403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2de807f1bc97c1d09c087e0a9f287128a9b048361c5f049ce3ea7bfdae5ae3be`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:19:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:19:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:19:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:19:43 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:21:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c260b335cf07f336d1a4e8a82a9d7c692b2bd9787a59304939f8efa4f0101336`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c22181ff3d3903d9cd1bf4e764959b25637ae8513f97bce318dd8a7bd39e5ac`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4102e4fa66f5f968fd33f8eba29fb388cbe15692b65aa6ee4b73ee49911cc03c`  
		Last Modified: Sat, 16 Oct 2021 02:44:31 GMT  
		Size: 171.1 MB (171127704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd3223aef57941776d9e8c82021b54601bc6c98c9c4e37c09088868f34689ad`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67dce296a497287c39667aecbda14a56772cabb7fce0bf6814c5b0fc71fe902`  
		Last Modified: Sat, 16 Oct 2021 02:44:48 GMT  
		Size: 41.3 MB (41305313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b380c08d48bfaa5743c1d9aa123728e4bfe4d4de65c3042c42b18d2316d777`  
		Last Modified: Sat, 16 Oct 2021 02:44:42 GMT  
		Size: 322.8 KB (322832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1c8b80456c31f0be34412d39189749a6937d731e58136ac9d81186b6dbc6b`  
		Last Modified: Sat, 16 Oct 2021 02:44:52 GMT  
		Size: 71.8 MB (71754103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception`

```console
$ docker pull ros@sha256:c36c0be0f3d08698536bc3e1c1f2bd928ea497008f94f3ccc3d2da1481188e86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:fbd67a89dfd9604f46220e0ff52df6fb97eff79d52c9c23e6afb33759e03532d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.7 MB (840673772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dc9f05a7391983a0db62f22423a49770ced093b6d496acc35718383846ece27`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:26:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 03:28:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 03:28:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:28:05 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:28:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef1669a6b741da8d10348ca5478bc92ed459dd5ae9dc872bc2901aa4a4885a`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7bc8cdeda44965808907e244e5edd3ed9d6efd6c0105fc84123b986946a806`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b82bc5a2b4db46195d4cb9bb39816b83ede6c31f565651abb9b15e6d4335ee8`  
		Last Modified: Sat, 16 Oct 2021 03:47:14 GMT  
		Size: 176.7 MB (176707219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389d5741667b5453a3f2fd8e79c5521bf1f17e95d6042d56595b80623e04aba`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d0df0db2441b7744370d28a551a1152f79b7249050aa09e18996bbd0428ebf`  
		Last Modified: Sat, 16 Oct 2021 03:47:32 GMT  
		Size: 47.3 MB (47259872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80707a4f3d4ddd0562cb757ab166458ffe0a134b59935f1619d10653486a8049`  
		Last Modified: Sat, 16 Oct 2021 03:47:24 GMT  
		Size: 322.9 KB (322897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626c61368773f58359917c9e5cd1e8c6555b27f66d55fda64ca5306f6748046b`  
		Last Modified: Sat, 16 Oct 2021 03:47:37 GMT  
		Size: 79.6 MB (79604503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873295b83c834b53855fb3ee53b9f7e4f8d7cda9106ad9604caa6571771e892a`  
		Last Modified: Sat, 16 Oct 2021 03:49:16 GMT  
		Size: 501.5 MB (501476094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:aa669918818c839ad440818ea7731b8d1c1f20e1746c9f4cf270e88d21e05923
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **730.2 MB (730212759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05cb62f5e4efda20a5c96427dae3666b8eb03a6225fc9055c3882574df32dced`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:17:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:17:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:17:55 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:17 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:22:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:27:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764ddf81fcf398a2a4cf14036409b82f4f4a06bd8f23171e840ff36accba4d4f`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 1.2 MB (1186846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02b4dedc9080b63cee4513e2787d54376223246780de27866414412fce505a7`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 4.7 MB (4676770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb049eda64c876c1ee585dd51f3f8b9a9807c82541e8243ea725bcf5ee59fb2c`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7037e3e565c8acccf66678f470f9ceae8503c90974e2dd927764191193ffdbb`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69724b9a0973ce0c31fba9293b5ca2cc8e252ee13673b3053258594c1fa8b815`  
		Last Modified: Sat, 16 Oct 2021 02:31:48 GMT  
		Size: 157.2 MB (157179504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df68017d0a78706560ec19c60581120f31997ecd5e9223e1eec432c47ae86e8`  
		Last Modified: Sat, 16 Oct 2021 02:29:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb98f2a916633a1fb1a69dd5aebc5416fb396d43233943523788ff874a76fde`  
		Last Modified: Sat, 16 Oct 2021 02:32:19 GMT  
		Size: 36.7 MB (36691673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242c94fc3e260adf5325a33e1e99237f52197a87e7ea5b471bdd8bd9eb4b0b0`  
		Last Modified: Sat, 16 Oct 2021 02:32:00 GMT  
		Size: 322.9 KB (322903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5bbb4e057a5f879119a31a98e9617ab535d39046bf80b55735ded907115af3`  
		Last Modified: Sat, 16 Oct 2021 02:32:38 GMT  
		Size: 60.5 MB (60484275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e5eb8963b50319044bc13007fdc627b1d47ca37089b51bdd7b779be78d79a7`  
		Last Modified: Sat, 16 Oct 2021 02:37:52 GMT  
		Size: 445.6 MB (445603920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3c1141727711ac978073d166f5eef74ee08532010d450a66b2e1cc2d702b17e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **790.3 MB (790280874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc902c8a6890acc480fe9e9036723decff79e227ab2da60422b3df6e457f7ba`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:19:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:19:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:19:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:19:43 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:21:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:24:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c260b335cf07f336d1a4e8a82a9d7c692b2bd9787a59304939f8efa4f0101336`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c22181ff3d3903d9cd1bf4e764959b25637ae8513f97bce318dd8a7bd39e5ac`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4102e4fa66f5f968fd33f8eba29fb388cbe15692b65aa6ee4b73ee49911cc03c`  
		Last Modified: Sat, 16 Oct 2021 02:44:31 GMT  
		Size: 171.1 MB (171127704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd3223aef57941776d9e8c82021b54601bc6c98c9c4e37c09088868f34689ad`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67dce296a497287c39667aecbda14a56772cabb7fce0bf6814c5b0fc71fe902`  
		Last Modified: Sat, 16 Oct 2021 02:44:48 GMT  
		Size: 41.3 MB (41305313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b380c08d48bfaa5743c1d9aa123728e4bfe4d4de65c3042c42b18d2316d777`  
		Last Modified: Sat, 16 Oct 2021 02:44:42 GMT  
		Size: 322.8 KB (322832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1c8b80456c31f0be34412d39189749a6937d731e58136ac9d81186b6dbc6b`  
		Last Modified: Sat, 16 Oct 2021 02:44:52 GMT  
		Size: 71.8 MB (71754103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ea47d5f61b04a7e2aa1cbe6894978cedb3e14bb45ccdb7bc0195ae78825468`  
		Last Modified: Sat, 16 Oct 2021 02:46:29 GMT  
		Size: 472.1 MB (472088471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:085e0c483b309294e6a340e41478f9d8a1967d13e990fbdb077bf99dfaa0afea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:afd77bd93f4a35888d711b08907cfa2a3ae1dd0ffda4674f229f089c6316d0f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **968.1 MB (968054133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4e11f4a8b63c326ec6a2258bb2a394a7e3c6b5e2d72db6bcda977e84e7c5ef0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:22:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:22:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Oct 2021 04:22:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Oct 2021 04:22:45 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:22:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Oct 2021 04:22:46 GMT
ENV ROS_DISTRO=noetic
# Tue, 12 Oct 2021 04:24:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:24:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 12 Oct 2021 04:24:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Oct 2021 04:24:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:25:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:25:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 12 Oct 2021 04:25:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1879fc7dd1b539861f67f1a1f2560ac72901b2ec692bcd502d7dbd78747aec`  
		Last Modified: Tue, 12 Oct 2021 04:30:11 GMT  
		Size: 10.9 MB (10891815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6513f455c2f9ae29007328538218f9e3fb1ad2f676464032ac997367c06bd20f`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acccdf05e200940e857fda740a50ca8637c81a0035ec822e0bd50a4a0f869adf`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4f3f2e3176a668407560bf65a733da19af24e22a7017e0b28b27cc775aecdc`  
		Last Modified: Tue, 12 Oct 2021 04:30:46 GMT  
		Size: 239.1 MB (239086052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7276317c1b25ab860c01a572280c0f14572628e108816c4971ff0e711979e2`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cd7ef11df9f4c2994b6c766b52d97136fd40ddf75f985c0256383ff4c20c09`  
		Last Modified: Tue, 12 Oct 2021 04:31:10 GMT  
		Size: 86.6 MB (86566451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76df43754e281f9238cf8d03034b1548ed88b4b2fc4010c703439cdeeec0ff8`  
		Last Modified: Tue, 12 Oct 2021 04:30:54 GMT  
		Size: 317.2 KB (317177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899a51b12df1bc48c66b5be9054bdaea88bbde4fbf2eb0be77273b2aa54eb5b3`  
		Last Modified: Tue, 12 Oct 2021 04:31:05 GMT  
		Size: 76.0 MB (75975282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f736f433f571e3ce92a96bef321135e51899045a0925a5fe7f00a6eff5d64589`  
		Last Modified: Tue, 12 Oct 2021 04:32:46 GMT  
		Size: 504.8 MB (504778250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:df1440787394e70492a1bed0255bed5627ca71b0a4ed41f59ca0e1a397a4f31f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **884.3 MB (884335973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be8fb36bf89a3a95ec7638196e6ea89a3dc4d24b4587db1316e2d6e5342dde6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:24:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:24:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:24:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:24:31 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:24:32 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:24:33 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:25:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:25:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:25:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:25:40 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:26:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:26:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:26:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98b0896d14723a47f07ff594a967f0814c0da1df689f3d040057105fded61dd`  
		Last Modified: Sat, 16 Oct 2021 02:46:41 GMT  
		Size: 10.7 MB (10688087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b48989cd59e4ee347354a79194b7c1eba7afb598beb801e96a74d107a7d5a0`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9f5ab07bbddbafdfffd7f0ffa550462ceec189b0115c34df2d09d7bd1494b9`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a12ee73202cbe490b5ab854a5d822c301c942147652309f4fb95def7dada00`  
		Last Modified: Sat, 16 Oct 2021 02:47:11 GMT  
		Size: 184.3 MB (184301395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1eab669b7e7dc130e74420c37f0e029bcf02f638a0c578f7d44b74eaa394a5`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c9b95993ca257da5139529fd479ebc2185f0b4e6d477fbff1c2f8832ff8554`  
		Last Modified: Sat, 16 Oct 2021 02:47:31 GMT  
		Size: 84.3 MB (84349569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e334956eeaa640b444c8af3d1ad174a5ace287add09dbd72522ddb8abc4fd1`  
		Last Modified: Sat, 16 Oct 2021 02:47:19 GMT  
		Size: 317.2 KB (317202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643ca74f42e35eeb9d1ae7db84b7877cbd31af2bf303518e69eb902563cb0b1f`  
		Last Modified: Sat, 16 Oct 2021 02:47:29 GMT  
		Size: 73.9 MB (73864504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9c718e1b6b5dc9eec547f1d59929a819ce757a5dc849db3b8b0aff25335191`  
		Last Modified: Sat, 16 Oct 2021 02:49:00 GMT  
		Size: 481.6 MB (481590091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:c36c0be0f3d08698536bc3e1c1f2bd928ea497008f94f3ccc3d2da1481188e86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:fbd67a89dfd9604f46220e0ff52df6fb97eff79d52c9c23e6afb33759e03532d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.7 MB (840673772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dc9f05a7391983a0db62f22423a49770ced093b6d496acc35718383846ece27`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:26:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 03:28:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 03:28:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:28:05 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:28:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef1669a6b741da8d10348ca5478bc92ed459dd5ae9dc872bc2901aa4a4885a`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7bc8cdeda44965808907e244e5edd3ed9d6efd6c0105fc84123b986946a806`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b82bc5a2b4db46195d4cb9bb39816b83ede6c31f565651abb9b15e6d4335ee8`  
		Last Modified: Sat, 16 Oct 2021 03:47:14 GMT  
		Size: 176.7 MB (176707219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389d5741667b5453a3f2fd8e79c5521bf1f17e95d6042d56595b80623e04aba`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d0df0db2441b7744370d28a551a1152f79b7249050aa09e18996bbd0428ebf`  
		Last Modified: Sat, 16 Oct 2021 03:47:32 GMT  
		Size: 47.3 MB (47259872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80707a4f3d4ddd0562cb757ab166458ffe0a134b59935f1619d10653486a8049`  
		Last Modified: Sat, 16 Oct 2021 03:47:24 GMT  
		Size: 322.9 KB (322897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626c61368773f58359917c9e5cd1e8c6555b27f66d55fda64ca5306f6748046b`  
		Last Modified: Sat, 16 Oct 2021 03:47:37 GMT  
		Size: 79.6 MB (79604503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873295b83c834b53855fb3ee53b9f7e4f8d7cda9106ad9604caa6571771e892a`  
		Last Modified: Sat, 16 Oct 2021 03:49:16 GMT  
		Size: 501.5 MB (501476094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:aa669918818c839ad440818ea7731b8d1c1f20e1746c9f4cf270e88d21e05923
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **730.2 MB (730212759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05cb62f5e4efda20a5c96427dae3666b8eb03a6225fc9055c3882574df32dced`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:17:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:17:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:17:55 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:17 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:22:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:27:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764ddf81fcf398a2a4cf14036409b82f4f4a06bd8f23171e840ff36accba4d4f`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 1.2 MB (1186846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02b4dedc9080b63cee4513e2787d54376223246780de27866414412fce505a7`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 4.7 MB (4676770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb049eda64c876c1ee585dd51f3f8b9a9807c82541e8243ea725bcf5ee59fb2c`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7037e3e565c8acccf66678f470f9ceae8503c90974e2dd927764191193ffdbb`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69724b9a0973ce0c31fba9293b5ca2cc8e252ee13673b3053258594c1fa8b815`  
		Last Modified: Sat, 16 Oct 2021 02:31:48 GMT  
		Size: 157.2 MB (157179504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df68017d0a78706560ec19c60581120f31997ecd5e9223e1eec432c47ae86e8`  
		Last Modified: Sat, 16 Oct 2021 02:29:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb98f2a916633a1fb1a69dd5aebc5416fb396d43233943523788ff874a76fde`  
		Last Modified: Sat, 16 Oct 2021 02:32:19 GMT  
		Size: 36.7 MB (36691673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242c94fc3e260adf5325a33e1e99237f52197a87e7ea5b471bdd8bd9eb4b0b0`  
		Last Modified: Sat, 16 Oct 2021 02:32:00 GMT  
		Size: 322.9 KB (322903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5bbb4e057a5f879119a31a98e9617ab535d39046bf80b55735ded907115af3`  
		Last Modified: Sat, 16 Oct 2021 02:32:38 GMT  
		Size: 60.5 MB (60484275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e5eb8963b50319044bc13007fdc627b1d47ca37089b51bdd7b779be78d79a7`  
		Last Modified: Sat, 16 Oct 2021 02:37:52 GMT  
		Size: 445.6 MB (445603920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3c1141727711ac978073d166f5eef74ee08532010d450a66b2e1cc2d702b17e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **790.3 MB (790280874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc902c8a6890acc480fe9e9036723decff79e227ab2da60422b3df6e457f7ba`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:19:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:19:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:19:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:19:43 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:21:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:24:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c260b335cf07f336d1a4e8a82a9d7c692b2bd9787a59304939f8efa4f0101336`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c22181ff3d3903d9cd1bf4e764959b25637ae8513f97bce318dd8a7bd39e5ac`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4102e4fa66f5f968fd33f8eba29fb388cbe15692b65aa6ee4b73ee49911cc03c`  
		Last Modified: Sat, 16 Oct 2021 02:44:31 GMT  
		Size: 171.1 MB (171127704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd3223aef57941776d9e8c82021b54601bc6c98c9c4e37c09088868f34689ad`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67dce296a497287c39667aecbda14a56772cabb7fce0bf6814c5b0fc71fe902`  
		Last Modified: Sat, 16 Oct 2021 02:44:48 GMT  
		Size: 41.3 MB (41305313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b380c08d48bfaa5743c1d9aa123728e4bfe4d4de65c3042c42b18d2316d777`  
		Last Modified: Sat, 16 Oct 2021 02:44:42 GMT  
		Size: 322.8 KB (322832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1c8b80456c31f0be34412d39189749a6937d731e58136ac9d81186b6dbc6b`  
		Last Modified: Sat, 16 Oct 2021 02:44:52 GMT  
		Size: 71.8 MB (71754103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ea47d5f61b04a7e2aa1cbe6894978cedb3e14bb45ccdb7bc0195ae78825468`  
		Last Modified: Sat, 16 Oct 2021 02:46:29 GMT  
		Size: 472.1 MB (472088471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot`

```console
$ docker pull ros@sha256:5cc5578f038e0536340a965355dc7871db0095460e947c71c0c00201f7bb7214
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:f7140a67da24853af70f42b8d78d682bcf9cc45907ad74f9886cedb3c4939f83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.9 MB (354946140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b211266230d77466432d034f5d374384bdf95b61211922e43c03a0c77af7cb4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:26:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 03:28:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 03:28:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:28:05 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:28:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:30:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef1669a6b741da8d10348ca5478bc92ed459dd5ae9dc872bc2901aa4a4885a`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7bc8cdeda44965808907e244e5edd3ed9d6efd6c0105fc84123b986946a806`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b82bc5a2b4db46195d4cb9bb39816b83ede6c31f565651abb9b15e6d4335ee8`  
		Last Modified: Sat, 16 Oct 2021 03:47:14 GMT  
		Size: 176.7 MB (176707219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389d5741667b5453a3f2fd8e79c5521bf1f17e95d6042d56595b80623e04aba`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d0df0db2441b7744370d28a551a1152f79b7249050aa09e18996bbd0428ebf`  
		Last Modified: Sat, 16 Oct 2021 03:47:32 GMT  
		Size: 47.3 MB (47259872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80707a4f3d4ddd0562cb757ab166458ffe0a134b59935f1619d10653486a8049`  
		Last Modified: Sat, 16 Oct 2021 03:47:24 GMT  
		Size: 322.9 KB (322897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626c61368773f58359917c9e5cd1e8c6555b27f66d55fda64ca5306f6748046b`  
		Last Modified: Sat, 16 Oct 2021 03:47:37 GMT  
		Size: 79.6 MB (79604503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943befb25f2aa4af6ba036d4dab1cede9f6b46fa36708c220fc86920c38bbfcf`  
		Last Modified: Sat, 16 Oct 2021 03:47:52 GMT  
		Size: 15.7 MB (15748462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:9a7de897dae99a7589a7d920c3fc323a2b1b2ab317f8d997a0958605ec26188b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298573997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4021fb42a3360ba288aadda7e5e6d7d9f5b59bfcf5ecb74b9ca689f5d238c6f7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:17:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:17:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:17:55 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:17 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:22:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:22:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764ddf81fcf398a2a4cf14036409b82f4f4a06bd8f23171e840ff36accba4d4f`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 1.2 MB (1186846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02b4dedc9080b63cee4513e2787d54376223246780de27866414412fce505a7`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 4.7 MB (4676770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb049eda64c876c1ee585dd51f3f8b9a9807c82541e8243ea725bcf5ee59fb2c`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7037e3e565c8acccf66678f470f9ceae8503c90974e2dd927764191193ffdbb`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69724b9a0973ce0c31fba9293b5ca2cc8e252ee13673b3053258594c1fa8b815`  
		Last Modified: Sat, 16 Oct 2021 02:31:48 GMT  
		Size: 157.2 MB (157179504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df68017d0a78706560ec19c60581120f31997ecd5e9223e1eec432c47ae86e8`  
		Last Modified: Sat, 16 Oct 2021 02:29:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb98f2a916633a1fb1a69dd5aebc5416fb396d43233943523788ff874a76fde`  
		Last Modified: Sat, 16 Oct 2021 02:32:19 GMT  
		Size: 36.7 MB (36691673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242c94fc3e260adf5325a33e1e99237f52197a87e7ea5b471bdd8bd9eb4b0b0`  
		Last Modified: Sat, 16 Oct 2021 02:32:00 GMT  
		Size: 322.9 KB (322903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5bbb4e057a5f879119a31a98e9617ab535d39046bf80b55735ded907115af3`  
		Last Modified: Sat, 16 Oct 2021 02:32:38 GMT  
		Size: 60.5 MB (60484275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a73ef1a5ea79bedbff1bb66d2f1ca1debb4e3e7765cdeeb3e358f8ce0414b5`  
		Last Modified: Sat, 16 Oct 2021 02:33:03 GMT  
		Size: 14.0 MB (13965158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2f3aeaf51a9ac77b48225d1409b34c215f795f9a712512976654c5aca682694b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.5 MB (333540491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43134256327b8117993acef98a723b33f18ce79eeb96bc4afdc4664950dcbe35`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:19:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:19:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:19:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:19:43 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:21:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c260b335cf07f336d1a4e8a82a9d7c692b2bd9787a59304939f8efa4f0101336`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c22181ff3d3903d9cd1bf4e764959b25637ae8513f97bce318dd8a7bd39e5ac`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4102e4fa66f5f968fd33f8eba29fb388cbe15692b65aa6ee4b73ee49911cc03c`  
		Last Modified: Sat, 16 Oct 2021 02:44:31 GMT  
		Size: 171.1 MB (171127704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd3223aef57941776d9e8c82021b54601bc6c98c9c4e37c09088868f34689ad`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67dce296a497287c39667aecbda14a56772cabb7fce0bf6814c5b0fc71fe902`  
		Last Modified: Sat, 16 Oct 2021 02:44:48 GMT  
		Size: 41.3 MB (41305313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b380c08d48bfaa5743c1d9aa123728e4bfe4d4de65c3042c42b18d2316d777`  
		Last Modified: Sat, 16 Oct 2021 02:44:42 GMT  
		Size: 322.8 KB (322832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1c8b80456c31f0be34412d39189749a6937d731e58136ac9d81186b6dbc6b`  
		Last Modified: Sat, 16 Oct 2021 02:44:52 GMT  
		Size: 71.8 MB (71754103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9588c58320e3d7dc3f7913b1c3e314b42ff8f4161ab305728a1932470117d2b`  
		Last Modified: Sat, 16 Oct 2021 02:45:09 GMT  
		Size: 15.3 MB (15348088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:7cb2df22883855b59991df6cd80f81efba89e94c32d22316fc509d6216e17b31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:22efe71de7d84a34179a737915c1925b176069eaf4d8b795bf0dcf7393074707
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.5 MB (484494381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7aff3bf5c44dd947334f976f3bf7032515484d74ffd611c1edb141534823352`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:22:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:22:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Oct 2021 04:22:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Oct 2021 04:22:45 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:22:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Oct 2021 04:22:46 GMT
ENV ROS_DISTRO=noetic
# Tue, 12 Oct 2021 04:24:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:24:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 12 Oct 2021 04:24:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Oct 2021 04:24:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:25:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:25:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 12 Oct 2021 04:25:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:26:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1879fc7dd1b539861f67f1a1f2560ac72901b2ec692bcd502d7dbd78747aec`  
		Last Modified: Tue, 12 Oct 2021 04:30:11 GMT  
		Size: 10.9 MB (10891815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6513f455c2f9ae29007328538218f9e3fb1ad2f676464032ac997367c06bd20f`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acccdf05e200940e857fda740a50ca8637c81a0035ec822e0bd50a4a0f869adf`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4f3f2e3176a668407560bf65a733da19af24e22a7017e0b28b27cc775aecdc`  
		Last Modified: Tue, 12 Oct 2021 04:30:46 GMT  
		Size: 239.1 MB (239086052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7276317c1b25ab860c01a572280c0f14572628e108816c4971ff0e711979e2`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cd7ef11df9f4c2994b6c766b52d97136fd40ddf75f985c0256383ff4c20c09`  
		Last Modified: Tue, 12 Oct 2021 04:31:10 GMT  
		Size: 86.6 MB (86566451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76df43754e281f9238cf8d03034b1548ed88b4b2fc4010c703439cdeeec0ff8`  
		Last Modified: Tue, 12 Oct 2021 04:30:54 GMT  
		Size: 317.2 KB (317177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899a51b12df1bc48c66b5be9054bdaea88bbde4fbf2eb0be77273b2aa54eb5b3`  
		Last Modified: Tue, 12 Oct 2021 04:31:05 GMT  
		Size: 76.0 MB (75975282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc55481530e10c8596c3f649cbac594031eb2183b9af2d6c1fc15e6dd2755461`  
		Last Modified: Tue, 12 Oct 2021 04:31:20 GMT  
		Size: 21.2 MB (21218498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8a57c5bf894fef67bf1f223b1b5d91fa24fd078eff5af6517f83fb2fa8e37f3a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.6 MB (423640231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a6dbc268770631989335a0e92d3531a74bc782f85dda62c2eed402342251144`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:24:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:24:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:24:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:24:31 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:24:32 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:24:33 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:25:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:25:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:25:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:25:40 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:26:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:26:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:26:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:27:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98b0896d14723a47f07ff594a967f0814c0da1df689f3d040057105fded61dd`  
		Last Modified: Sat, 16 Oct 2021 02:46:41 GMT  
		Size: 10.7 MB (10688087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b48989cd59e4ee347354a79194b7c1eba7afb598beb801e96a74d107a7d5a0`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9f5ab07bbddbafdfffd7f0ffa550462ceec189b0115c34df2d09d7bd1494b9`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a12ee73202cbe490b5ab854a5d822c301c942147652309f4fb95def7dada00`  
		Last Modified: Sat, 16 Oct 2021 02:47:11 GMT  
		Size: 184.3 MB (184301395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1eab669b7e7dc130e74420c37f0e029bcf02f638a0c578f7d44b74eaa394a5`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c9b95993ca257da5139529fd479ebc2185f0b4e6d477fbff1c2f8832ff8554`  
		Last Modified: Sat, 16 Oct 2021 02:47:31 GMT  
		Size: 84.3 MB (84349569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e334956eeaa640b444c8af3d1ad174a5ace287add09dbd72522ddb8abc4fd1`  
		Last Modified: Sat, 16 Oct 2021 02:47:19 GMT  
		Size: 317.2 KB (317202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643ca74f42e35eeb9d1ae7db84b7877cbd31af2bf303518e69eb902563cb0b1f`  
		Last Modified: Sat, 16 Oct 2021 02:47:29 GMT  
		Size: 73.9 MB (73864504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c47609157e379743bab7f1deafe317c8976b4a1a6b1b961646eb62c78c31e2c`  
		Last Modified: Sat, 16 Oct 2021 02:47:42 GMT  
		Size: 20.9 MB (20894349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:5cc5578f038e0536340a965355dc7871db0095460e947c71c0c00201f7bb7214
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:f7140a67da24853af70f42b8d78d682bcf9cc45907ad74f9886cedb3c4939f83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.9 MB (354946140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b211266230d77466432d034f5d374384bdf95b61211922e43c03a0c77af7cb4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:26:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 03:28:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 03:28:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:28:05 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:28:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:30:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef1669a6b741da8d10348ca5478bc92ed459dd5ae9dc872bc2901aa4a4885a`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7bc8cdeda44965808907e244e5edd3ed9d6efd6c0105fc84123b986946a806`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b82bc5a2b4db46195d4cb9bb39816b83ede6c31f565651abb9b15e6d4335ee8`  
		Last Modified: Sat, 16 Oct 2021 03:47:14 GMT  
		Size: 176.7 MB (176707219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389d5741667b5453a3f2fd8e79c5521bf1f17e95d6042d56595b80623e04aba`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d0df0db2441b7744370d28a551a1152f79b7249050aa09e18996bbd0428ebf`  
		Last Modified: Sat, 16 Oct 2021 03:47:32 GMT  
		Size: 47.3 MB (47259872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80707a4f3d4ddd0562cb757ab166458ffe0a134b59935f1619d10653486a8049`  
		Last Modified: Sat, 16 Oct 2021 03:47:24 GMT  
		Size: 322.9 KB (322897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626c61368773f58359917c9e5cd1e8c6555b27f66d55fda64ca5306f6748046b`  
		Last Modified: Sat, 16 Oct 2021 03:47:37 GMT  
		Size: 79.6 MB (79604503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943befb25f2aa4af6ba036d4dab1cede9f6b46fa36708c220fc86920c38bbfcf`  
		Last Modified: Sat, 16 Oct 2021 03:47:52 GMT  
		Size: 15.7 MB (15748462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:9a7de897dae99a7589a7d920c3fc323a2b1b2ab317f8d997a0958605ec26188b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298573997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4021fb42a3360ba288aadda7e5e6d7d9f5b59bfcf5ecb74b9ca689f5d238c6f7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:17:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:17:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:17:55 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:17 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:22:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:22:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764ddf81fcf398a2a4cf14036409b82f4f4a06bd8f23171e840ff36accba4d4f`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 1.2 MB (1186846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02b4dedc9080b63cee4513e2787d54376223246780de27866414412fce505a7`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 4.7 MB (4676770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb049eda64c876c1ee585dd51f3f8b9a9807c82541e8243ea725bcf5ee59fb2c`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7037e3e565c8acccf66678f470f9ceae8503c90974e2dd927764191193ffdbb`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69724b9a0973ce0c31fba9293b5ca2cc8e252ee13673b3053258594c1fa8b815`  
		Last Modified: Sat, 16 Oct 2021 02:31:48 GMT  
		Size: 157.2 MB (157179504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df68017d0a78706560ec19c60581120f31997ecd5e9223e1eec432c47ae86e8`  
		Last Modified: Sat, 16 Oct 2021 02:29:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb98f2a916633a1fb1a69dd5aebc5416fb396d43233943523788ff874a76fde`  
		Last Modified: Sat, 16 Oct 2021 02:32:19 GMT  
		Size: 36.7 MB (36691673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242c94fc3e260adf5325a33e1e99237f52197a87e7ea5b471bdd8bd9eb4b0b0`  
		Last Modified: Sat, 16 Oct 2021 02:32:00 GMT  
		Size: 322.9 KB (322903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5bbb4e057a5f879119a31a98e9617ab535d39046bf80b55735ded907115af3`  
		Last Modified: Sat, 16 Oct 2021 02:32:38 GMT  
		Size: 60.5 MB (60484275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a73ef1a5ea79bedbff1bb66d2f1ca1debb4e3e7765cdeeb3e358f8ce0414b5`  
		Last Modified: Sat, 16 Oct 2021 02:33:03 GMT  
		Size: 14.0 MB (13965158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2f3aeaf51a9ac77b48225d1409b34c215f795f9a712512976654c5aca682694b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.5 MB (333540491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43134256327b8117993acef98a723b33f18ce79eeb96bc4afdc4664950dcbe35`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:19:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:19:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:19:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:19:43 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:21:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c260b335cf07f336d1a4e8a82a9d7c692b2bd9787a59304939f8efa4f0101336`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c22181ff3d3903d9cd1bf4e764959b25637ae8513f97bce318dd8a7bd39e5ac`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4102e4fa66f5f968fd33f8eba29fb388cbe15692b65aa6ee4b73ee49911cc03c`  
		Last Modified: Sat, 16 Oct 2021 02:44:31 GMT  
		Size: 171.1 MB (171127704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd3223aef57941776d9e8c82021b54601bc6c98c9c4e37c09088868f34689ad`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67dce296a497287c39667aecbda14a56772cabb7fce0bf6814c5b0fc71fe902`  
		Last Modified: Sat, 16 Oct 2021 02:44:48 GMT  
		Size: 41.3 MB (41305313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b380c08d48bfaa5743c1d9aa123728e4bfe4d4de65c3042c42b18d2316d777`  
		Last Modified: Sat, 16 Oct 2021 02:44:42 GMT  
		Size: 322.8 KB (322832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1c8b80456c31f0be34412d39189749a6937d731e58136ac9d81186b6dbc6b`  
		Last Modified: Sat, 16 Oct 2021 02:44:52 GMT  
		Size: 71.8 MB (71754103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9588c58320e3d7dc3f7913b1c3e314b42ff8f4161ab305728a1932470117d2b`  
		Last Modified: Sat, 16 Oct 2021 02:45:09 GMT  
		Size: 15.3 MB (15348088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base`

```console
$ docker pull ros@sha256:ef2030579a6637986cc03e6418adb14f3b684b991a295b367852c1d7dd09aafc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:2d75db570a0b16a6dc075c45c8263252fbeee945b9333eed33ff98af49c58895
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339197678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ead05d68f2187667ad2a43b6fcf6349e150e77bc13f7917591f87f7fdb4836`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:26:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 03:28:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 03:28:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:28:05 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:28:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef1669a6b741da8d10348ca5478bc92ed459dd5ae9dc872bc2901aa4a4885a`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7bc8cdeda44965808907e244e5edd3ed9d6efd6c0105fc84123b986946a806`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b82bc5a2b4db46195d4cb9bb39816b83ede6c31f565651abb9b15e6d4335ee8`  
		Last Modified: Sat, 16 Oct 2021 03:47:14 GMT  
		Size: 176.7 MB (176707219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389d5741667b5453a3f2fd8e79c5521bf1f17e95d6042d56595b80623e04aba`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d0df0db2441b7744370d28a551a1152f79b7249050aa09e18996bbd0428ebf`  
		Last Modified: Sat, 16 Oct 2021 03:47:32 GMT  
		Size: 47.3 MB (47259872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80707a4f3d4ddd0562cb757ab166458ffe0a134b59935f1619d10653486a8049`  
		Last Modified: Sat, 16 Oct 2021 03:47:24 GMT  
		Size: 322.9 KB (322897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626c61368773f58359917c9e5cd1e8c6555b27f66d55fda64ca5306f6748046b`  
		Last Modified: Sat, 16 Oct 2021 03:47:37 GMT  
		Size: 79.6 MB (79604503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:0a3716d6cb18a81fec1cfc5432a842d427d986e07b8d7665dba5fb18bb1b6687
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c32c2fedb278f6c38d9255abb83eedd072db50ee75a9e3462dac4cb7832785`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:17:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:17:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:17:55 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:17 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:22:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764ddf81fcf398a2a4cf14036409b82f4f4a06bd8f23171e840ff36accba4d4f`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 1.2 MB (1186846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02b4dedc9080b63cee4513e2787d54376223246780de27866414412fce505a7`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 4.7 MB (4676770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb049eda64c876c1ee585dd51f3f8b9a9807c82541e8243ea725bcf5ee59fb2c`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7037e3e565c8acccf66678f470f9ceae8503c90974e2dd927764191193ffdbb`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69724b9a0973ce0c31fba9293b5ca2cc8e252ee13673b3053258594c1fa8b815`  
		Last Modified: Sat, 16 Oct 2021 02:31:48 GMT  
		Size: 157.2 MB (157179504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df68017d0a78706560ec19c60581120f31997ecd5e9223e1eec432c47ae86e8`  
		Last Modified: Sat, 16 Oct 2021 02:29:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb98f2a916633a1fb1a69dd5aebc5416fb396d43233943523788ff874a76fde`  
		Last Modified: Sat, 16 Oct 2021 02:32:19 GMT  
		Size: 36.7 MB (36691673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242c94fc3e260adf5325a33e1e99237f52197a87e7ea5b471bdd8bd9eb4b0b0`  
		Last Modified: Sat, 16 Oct 2021 02:32:00 GMT  
		Size: 322.9 KB (322903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5bbb4e057a5f879119a31a98e9617ab535d39046bf80b55735ded907115af3`  
		Last Modified: Sat, 16 Oct 2021 02:32:38 GMT  
		Size: 60.5 MB (60484275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ec02baf086f3161863a635d2b2df2454d0295eebf71581502327d6660c166562
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318192403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2de807f1bc97c1d09c087e0a9f287128a9b048361c5f049ce3ea7bfdae5ae3be`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:19:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:19:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:19:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:19:43 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:21:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c260b335cf07f336d1a4e8a82a9d7c692b2bd9787a59304939f8efa4f0101336`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c22181ff3d3903d9cd1bf4e764959b25637ae8513f97bce318dd8a7bd39e5ac`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4102e4fa66f5f968fd33f8eba29fb388cbe15692b65aa6ee4b73ee49911cc03c`  
		Last Modified: Sat, 16 Oct 2021 02:44:31 GMT  
		Size: 171.1 MB (171127704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd3223aef57941776d9e8c82021b54601bc6c98c9c4e37c09088868f34689ad`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67dce296a497287c39667aecbda14a56772cabb7fce0bf6814c5b0fc71fe902`  
		Last Modified: Sat, 16 Oct 2021 02:44:48 GMT  
		Size: 41.3 MB (41305313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b380c08d48bfaa5743c1d9aa123728e4bfe4d4de65c3042c42b18d2316d777`  
		Last Modified: Sat, 16 Oct 2021 02:44:42 GMT  
		Size: 322.8 KB (322832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1c8b80456c31f0be34412d39189749a6937d731e58136ac9d81186b6dbc6b`  
		Last Modified: Sat, 16 Oct 2021 02:44:52 GMT  
		Size: 71.8 MB (71754103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:65556bbde19b8995ef126b0866190de68ebf91a259bd7e79c00696a6937e439f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:0562cc97b056eb1e665438bf2c68a5686fbedd7990ff6788f2da5c30d45665f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.3 MB (463275883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e294c766aaf32edb1a2885f0482b1848b8c496b16a4e2d0c469e4eea1d4157f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:22:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:22:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Oct 2021 04:22:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Oct 2021 04:22:45 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:22:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Oct 2021 04:22:46 GMT
ENV ROS_DISTRO=noetic
# Tue, 12 Oct 2021 04:24:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:24:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 12 Oct 2021 04:24:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Oct 2021 04:24:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:25:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:25:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 12 Oct 2021 04:25:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1879fc7dd1b539861f67f1a1f2560ac72901b2ec692bcd502d7dbd78747aec`  
		Last Modified: Tue, 12 Oct 2021 04:30:11 GMT  
		Size: 10.9 MB (10891815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6513f455c2f9ae29007328538218f9e3fb1ad2f676464032ac997367c06bd20f`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acccdf05e200940e857fda740a50ca8637c81a0035ec822e0bd50a4a0f869adf`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4f3f2e3176a668407560bf65a733da19af24e22a7017e0b28b27cc775aecdc`  
		Last Modified: Tue, 12 Oct 2021 04:30:46 GMT  
		Size: 239.1 MB (239086052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7276317c1b25ab860c01a572280c0f14572628e108816c4971ff0e711979e2`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cd7ef11df9f4c2994b6c766b52d97136fd40ddf75f985c0256383ff4c20c09`  
		Last Modified: Tue, 12 Oct 2021 04:31:10 GMT  
		Size: 86.6 MB (86566451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76df43754e281f9238cf8d03034b1548ed88b4b2fc4010c703439cdeeec0ff8`  
		Last Modified: Tue, 12 Oct 2021 04:30:54 GMT  
		Size: 317.2 KB (317177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899a51b12df1bc48c66b5be9054bdaea88bbde4fbf2eb0be77273b2aa54eb5b3`  
		Last Modified: Tue, 12 Oct 2021 04:31:05 GMT  
		Size: 76.0 MB (75975282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:73f1a97d81b47b81f7f147d7b273d50db287cbb2211052cfebac95281a224c00
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.7 MB (402745882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a9cee320818edd12e14a6ccd74b405ea618b7f60606afbbd0888e72da00230`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:24:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:24:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:24:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:24:31 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:24:32 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:24:33 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:25:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:25:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:25:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:25:40 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:26:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:26:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:26:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98b0896d14723a47f07ff594a967f0814c0da1df689f3d040057105fded61dd`  
		Last Modified: Sat, 16 Oct 2021 02:46:41 GMT  
		Size: 10.7 MB (10688087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b48989cd59e4ee347354a79194b7c1eba7afb598beb801e96a74d107a7d5a0`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9f5ab07bbddbafdfffd7f0ffa550462ceec189b0115c34df2d09d7bd1494b9`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a12ee73202cbe490b5ab854a5d822c301c942147652309f4fb95def7dada00`  
		Last Modified: Sat, 16 Oct 2021 02:47:11 GMT  
		Size: 184.3 MB (184301395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1eab669b7e7dc130e74420c37f0e029bcf02f638a0c578f7d44b74eaa394a5`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c9b95993ca257da5139529fd479ebc2185f0b4e6d477fbff1c2f8832ff8554`  
		Last Modified: Sat, 16 Oct 2021 02:47:31 GMT  
		Size: 84.3 MB (84349569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e334956eeaa640b444c8af3d1ad174a5ace287add09dbd72522ddb8abc4fd1`  
		Last Modified: Sat, 16 Oct 2021 02:47:19 GMT  
		Size: 317.2 KB (317202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643ca74f42e35eeb9d1ae7db84b7877cbd31af2bf303518e69eb902563cb0b1f`  
		Last Modified: Sat, 16 Oct 2021 02:47:29 GMT  
		Size: 73.9 MB (73864504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:ef2030579a6637986cc03e6418adb14f3b684b991a295b367852c1d7dd09aafc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:2d75db570a0b16a6dc075c45c8263252fbeee945b9333eed33ff98af49c58895
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.2 MB (339197678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ead05d68f2187667ad2a43b6fcf6349e150e77bc13f7917591f87f7fdb4836`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:26:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 03:28:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 03:28:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:28:05 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:28:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:30:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef1669a6b741da8d10348ca5478bc92ed459dd5ae9dc872bc2901aa4a4885a`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7bc8cdeda44965808907e244e5edd3ed9d6efd6c0105fc84123b986946a806`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b82bc5a2b4db46195d4cb9bb39816b83ede6c31f565651abb9b15e6d4335ee8`  
		Last Modified: Sat, 16 Oct 2021 03:47:14 GMT  
		Size: 176.7 MB (176707219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389d5741667b5453a3f2fd8e79c5521bf1f17e95d6042d56595b80623e04aba`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d0df0db2441b7744370d28a551a1152f79b7249050aa09e18996bbd0428ebf`  
		Last Modified: Sat, 16 Oct 2021 03:47:32 GMT  
		Size: 47.3 MB (47259872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80707a4f3d4ddd0562cb757ab166458ffe0a134b59935f1619d10653486a8049`  
		Last Modified: Sat, 16 Oct 2021 03:47:24 GMT  
		Size: 322.9 KB (322897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626c61368773f58359917c9e5cd1e8c6555b27f66d55fda64ca5306f6748046b`  
		Last Modified: Sat, 16 Oct 2021 03:47:37 GMT  
		Size: 79.6 MB (79604503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:0a3716d6cb18a81fec1cfc5432a842d427d986e07b8d7665dba5fb18bb1b6687
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.6 MB (284608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c32c2fedb278f6c38d9255abb83eedd072db50ee75a9e3462dac4cb7832785`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:17:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:17:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:17:55 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:17 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:22:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764ddf81fcf398a2a4cf14036409b82f4f4a06bd8f23171e840ff36accba4d4f`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 1.2 MB (1186846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02b4dedc9080b63cee4513e2787d54376223246780de27866414412fce505a7`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 4.7 MB (4676770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb049eda64c876c1ee585dd51f3f8b9a9807c82541e8243ea725bcf5ee59fb2c`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7037e3e565c8acccf66678f470f9ceae8503c90974e2dd927764191193ffdbb`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69724b9a0973ce0c31fba9293b5ca2cc8e252ee13673b3053258594c1fa8b815`  
		Last Modified: Sat, 16 Oct 2021 02:31:48 GMT  
		Size: 157.2 MB (157179504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df68017d0a78706560ec19c60581120f31997ecd5e9223e1eec432c47ae86e8`  
		Last Modified: Sat, 16 Oct 2021 02:29:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb98f2a916633a1fb1a69dd5aebc5416fb396d43233943523788ff874a76fde`  
		Last Modified: Sat, 16 Oct 2021 02:32:19 GMT  
		Size: 36.7 MB (36691673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242c94fc3e260adf5325a33e1e99237f52197a87e7ea5b471bdd8bd9eb4b0b0`  
		Last Modified: Sat, 16 Oct 2021 02:32:00 GMT  
		Size: 322.9 KB (322903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5bbb4e057a5f879119a31a98e9617ab535d39046bf80b55735ded907115af3`  
		Last Modified: Sat, 16 Oct 2021 02:32:38 GMT  
		Size: 60.5 MB (60484275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ec02baf086f3161863a635d2b2df2454d0295eebf71581502327d6660c166562
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318192403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2de807f1bc97c1d09c087e0a9f287128a9b048361c5f049ce3ea7bfdae5ae3be`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:19:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:19:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:19:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:19:43 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:39 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:21:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:21:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:21:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c260b335cf07f336d1a4e8a82a9d7c692b2bd9787a59304939f8efa4f0101336`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c22181ff3d3903d9cd1bf4e764959b25637ae8513f97bce318dd8a7bd39e5ac`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4102e4fa66f5f968fd33f8eba29fb388cbe15692b65aa6ee4b73ee49911cc03c`  
		Last Modified: Sat, 16 Oct 2021 02:44:31 GMT  
		Size: 171.1 MB (171127704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd3223aef57941776d9e8c82021b54601bc6c98c9c4e37c09088868f34689ad`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67dce296a497287c39667aecbda14a56772cabb7fce0bf6814c5b0fc71fe902`  
		Last Modified: Sat, 16 Oct 2021 02:44:48 GMT  
		Size: 41.3 MB (41305313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b380c08d48bfaa5743c1d9aa123728e4bfe4d4de65c3042c42b18d2316d777`  
		Last Modified: Sat, 16 Oct 2021 02:44:42 GMT  
		Size: 322.8 KB (322832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1c8b80456c31f0be34412d39189749a6937d731e58136ac9d81186b6dbc6b`  
		Last Modified: Sat, 16 Oct 2021 02:44:52 GMT  
		Size: 71.8 MB (71754103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:5cff44ffbbb0588137b4e084a3de8df921d1a0bab3fd8944a038cffa70e0b70f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:3e09b34491850d2ba1876c2a342ef40ee07a92534c28058212df0bed7a33c76e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (212010406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee3903de61af282162eb3c75363e5f7991a8cb6802c352c58c1414b4313aba7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:26:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 03:28:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 03:28:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:28:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef1669a6b741da8d10348ca5478bc92ed459dd5ae9dc872bc2901aa4a4885a`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7bc8cdeda44965808907e244e5edd3ed9d6efd6c0105fc84123b986946a806`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b82bc5a2b4db46195d4cb9bb39816b83ede6c31f565651abb9b15e6d4335ee8`  
		Last Modified: Sat, 16 Oct 2021 03:47:14 GMT  
		Size: 176.7 MB (176707219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389d5741667b5453a3f2fd8e79c5521bf1f17e95d6042d56595b80623e04aba`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:7f2df9319c18ffcadb15468ca75d9a6702b9123a1f121a8e4b48f9d6e55e6e58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187109988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184036e2cc45b4b9baf77d53d7ea4dd148781bd49bb50bbe839ebcc338eb2df8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:17:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:17:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:17:55 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764ddf81fcf398a2a4cf14036409b82f4f4a06bd8f23171e840ff36accba4d4f`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 1.2 MB (1186846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02b4dedc9080b63cee4513e2787d54376223246780de27866414412fce505a7`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 4.7 MB (4676770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb049eda64c876c1ee585dd51f3f8b9a9807c82541e8243ea725bcf5ee59fb2c`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7037e3e565c8acccf66678f470f9ceae8503c90974e2dd927764191193ffdbb`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69724b9a0973ce0c31fba9293b5ca2cc8e252ee13673b3053258594c1fa8b815`  
		Last Modified: Sat, 16 Oct 2021 02:31:48 GMT  
		Size: 157.2 MB (157179504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df68017d0a78706560ec19c60581120f31997ecd5e9223e1eec432c47ae86e8`  
		Last Modified: Sat, 16 Oct 2021 02:29:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:17c0d23c023a333484d3477f95efa41dac9a55b88483df83822e6ac70aada487
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.8 MB (204810155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed66f435b1c51203c84577df97a8656a554855156272ec0d0ad12e762feb1c7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:19:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:19:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:19:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:19:43 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:39 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c260b335cf07f336d1a4e8a82a9d7c692b2bd9787a59304939f8efa4f0101336`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c22181ff3d3903d9cd1bf4e764959b25637ae8513f97bce318dd8a7bd39e5ac`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4102e4fa66f5f968fd33f8eba29fb388cbe15692b65aa6ee4b73ee49911cc03c`  
		Last Modified: Sat, 16 Oct 2021 02:44:31 GMT  
		Size: 171.1 MB (171127704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd3223aef57941776d9e8c82021b54601bc6c98c9c4e37c09088868f34689ad`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:2cf887060e96627fdfc53d29244ca16c47fa4532d5b4842ad4fc64769c922a7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:5e3947dafaece2bec30dcf3f592f401311c6046917cca0f58c76518e5f60d4d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300416973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e5ac7916996347de74cc39c400cdc5dc620b549a3587aee8f5306d8289b0af2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:22:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:22:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Oct 2021 04:22:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Oct 2021 04:22:45 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:22:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Oct 2021 04:22:46 GMT
ENV ROS_DISTRO=noetic
# Tue, 12 Oct 2021 04:24:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:24:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 12 Oct 2021 04:24:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Oct 2021 04:24:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1879fc7dd1b539861f67f1a1f2560ac72901b2ec692bcd502d7dbd78747aec`  
		Last Modified: Tue, 12 Oct 2021 04:30:11 GMT  
		Size: 10.9 MB (10891815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6513f455c2f9ae29007328538218f9e3fb1ad2f676464032ac997367c06bd20f`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acccdf05e200940e857fda740a50ca8637c81a0035ec822e0bd50a4a0f869adf`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4f3f2e3176a668407560bf65a733da19af24e22a7017e0b28b27cc775aecdc`  
		Last Modified: Tue, 12 Oct 2021 04:30:46 GMT  
		Size: 239.1 MB (239086052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7276317c1b25ab860c01a572280c0f14572628e108816c4971ff0e711979e2`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f3f9e998344e0623721f433692a9e98ffc022385ba0b30a2d08f5852a98ff412
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244214607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9caac251e259cd57583d5e91d2eb4d58aa5d9e872125e2f58d940b8c4c16d893`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:24:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:24:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:24:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:24:31 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:24:32 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:24:33 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:25:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:25:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:25:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:25:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98b0896d14723a47f07ff594a967f0814c0da1df689f3d040057105fded61dd`  
		Last Modified: Sat, 16 Oct 2021 02:46:41 GMT  
		Size: 10.7 MB (10688087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b48989cd59e4ee347354a79194b7c1eba7afb598beb801e96a74d107a7d5a0`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9f5ab07bbddbafdfffd7f0ffa550462ceec189b0115c34df2d09d7bd1494b9`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a12ee73202cbe490b5ab854a5d822c301c942147652309f4fb95def7dada00`  
		Last Modified: Sat, 16 Oct 2021 02:47:11 GMT  
		Size: 184.3 MB (184301395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1eab669b7e7dc130e74420c37f0e029bcf02f638a0c578f7d44b74eaa394a5`  
		Last Modified: Sat, 16 Oct 2021 02:46:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:5cff44ffbbb0588137b4e084a3de8df921d1a0bab3fd8944a038cffa70e0b70f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:3e09b34491850d2ba1876c2a342ef40ee07a92534c28058212df0bed7a33c76e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (212010406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee3903de61af282162eb3c75363e5f7991a8cb6802c352c58c1414b4313aba7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:26:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:26:10 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 03:28:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:28:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 03:28:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:28:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef1669a6b741da8d10348ca5478bc92ed459dd5ae9dc872bc2901aa4a4885a`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7bc8cdeda44965808907e244e5edd3ed9d6efd6c0105fc84123b986946a806`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b82bc5a2b4db46195d4cb9bb39816b83ede6c31f565651abb9b15e6d4335ee8`  
		Last Modified: Sat, 16 Oct 2021 03:47:14 GMT  
		Size: 176.7 MB (176707219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389d5741667b5453a3f2fd8e79c5521bf1f17e95d6042d56595b80623e04aba`  
		Last Modified: Sat, 16 Oct 2021 03:46:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:7f2df9319c18ffcadb15468ca75d9a6702b9123a1f121a8e4b48f9d6e55e6e58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187109988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184036e2cc45b4b9baf77d53d7ea4dd148781bd49bb50bbe839ebcc338eb2df8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:17:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:17:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:17:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:17:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:17:55 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764ddf81fcf398a2a4cf14036409b82f4f4a06bd8f23171e840ff36accba4d4f`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 1.2 MB (1186846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02b4dedc9080b63cee4513e2787d54376223246780de27866414412fce505a7`  
		Last Modified: Sat, 16 Oct 2021 02:29:43 GMT  
		Size: 4.7 MB (4676770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb049eda64c876c1ee585dd51f3f8b9a9807c82541e8243ea725bcf5ee59fb2c`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7037e3e565c8acccf66678f470f9ceae8503c90974e2dd927764191193ffdbb`  
		Last Modified: Sat, 16 Oct 2021 02:29:40 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69724b9a0973ce0c31fba9293b5ca2cc8e252ee13673b3053258594c1fa8b815`  
		Last Modified: Sat, 16 Oct 2021 02:31:48 GMT  
		Size: 157.2 MB (157179504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df68017d0a78706560ec19c60581120f31997ecd5e9223e1eec432c47ae86e8`  
		Last Modified: Sat, 16 Oct 2021 02:29:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:17c0d23c023a333484d3477f95efa41dac9a55b88483df83822e6ac70aada487
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.8 MB (204810155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed66f435b1c51203c84577df97a8656a554855156272ec0d0ad12e762feb1c7f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:19:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:19:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:19:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:19:43 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Oct 2021 02:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:20:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 Oct 2021 02:20:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:20:39 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c260b335cf07f336d1a4e8a82a9d7c692b2bd9787a59304939f8efa4f0101336`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c22181ff3d3903d9cd1bf4e764959b25637ae8513f97bce318dd8a7bd39e5ac`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4102e4fa66f5f968fd33f8eba29fb388cbe15692b65aa6ee4b73ee49911cc03c`  
		Last Modified: Sat, 16 Oct 2021 02:44:31 GMT  
		Size: 171.1 MB (171127704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd3223aef57941776d9e8c82021b54601bc6c98c9c4e37c09088868f34689ad`  
		Last Modified: Sat, 16 Oct 2021 02:44:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling`

```console
$ docker pull ros@sha256:4b2c3cea9a24377ef17849b0b956198edd73351b5ba287196c3a0a6365fc3f33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:660697b6ebaafa37ae39e5c462f5f789aeb2a3cfccd3b3d86f9c241c9c1991d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.7 MB (232747962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d87d298b0c2d4fd632c61dca8f405782cfb08dbb078b359644b99ceb09b94ecb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:43:25 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 03:44:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:44:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:44:10 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:44:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:44:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:44:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8bee2b5a1507bb0b409e973d369b0bee5c61d9429220e7511f7d34e11c4e6d`  
		Last Modified: Sat, 16 Oct 2021 03:52:23 GMT  
		Size: 104.2 MB (104214475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfab2596705bca5df8835dcd748c852003ebe630614e4c71569980fd0962003`  
		Last Modified: Sat, 16 Oct 2021 03:52:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29283b46cfd735b60062e5f91075c6f2ea843931acc59c14f37eb39221dd2b8`  
		Last Modified: Sat, 16 Oct 2021 03:52:44 GMT  
		Size: 70.8 MB (70796841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e9ed06c574509d9c0bb9d4a2c44f6ff114c1077e353cba7362c84cc4e6928`  
		Last Modified: Sat, 16 Oct 2021 03:52:34 GMT  
		Size: 246.5 KB (246456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9610fdb8a0efd75ac022b32e5bd0ab2e949a04010b31b2a1f1955479553203b4`  
		Last Modified: Sat, 16 Oct 2021 03:52:33 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf5624b902d835e1730c98d69e69b0b0b7426d0fa45bb0bfc22612403589e0b`  
		Last Modified: Sat, 16 Oct 2021 03:52:37 GMT  
		Size: 22.2 MB (22184954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:82a80df0e03fc37a4baf73d1c03b9fc968dea740ee502742fe2ce4526767cdc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.9 MB (220944962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3422c6512a41b27c8dc446dafaaefa7bf1d51a251ca3043d622285eb8ccc17fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:37:00 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 02:37:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:37:57 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:37:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:37:59 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:38:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:38:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:39:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cad6ffb3dc60f95d5943b3d5acda12c57965d2d65f7f2872b8c1606c16ee237`  
		Last Modified: Sat, 16 Oct 2021 02:52:06 GMT  
		Size: 100.6 MB (100573282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2ebcd20493ee87f05a7a06631f0e49a219d4e69224ecd485721c5533349280`  
		Last Modified: Sat, 16 Oct 2021 02:51:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0d3c7da3194f2ecfb190e30268c8d48f6234b20e8aec520afaabc90cb86057`  
		Last Modified: Sat, 16 Oct 2021 02:52:27 GMT  
		Size: 64.9 MB (64922124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605cd44436c348c295974385f97270bbfe47c80a3004ac7e1470ecd75955075f`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 246.4 KB (246396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef09852bd281240a5a11ad01942f7d7b2d78bc9910b588bc5b648036202ba2aa`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64fed610107408e1af96e0fc9d2c3da4e93ff305321078387b8a569e0e297c8`  
		Last Modified: Sat, 16 Oct 2021 02:52:21 GMT  
		Size: 21.5 MB (21518723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:4b2c3cea9a24377ef17849b0b956198edd73351b5ba287196c3a0a6365fc3f33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:660697b6ebaafa37ae39e5c462f5f789aeb2a3cfccd3b3d86f9c241c9c1991d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.7 MB (232747962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d87d298b0c2d4fd632c61dca8f405782cfb08dbb078b359644b99ceb09b94ecb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:43:25 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 03:44:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:44:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:44:10 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:44:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:44:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:44:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8bee2b5a1507bb0b409e973d369b0bee5c61d9429220e7511f7d34e11c4e6d`  
		Last Modified: Sat, 16 Oct 2021 03:52:23 GMT  
		Size: 104.2 MB (104214475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfab2596705bca5df8835dcd748c852003ebe630614e4c71569980fd0962003`  
		Last Modified: Sat, 16 Oct 2021 03:52:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29283b46cfd735b60062e5f91075c6f2ea843931acc59c14f37eb39221dd2b8`  
		Last Modified: Sat, 16 Oct 2021 03:52:44 GMT  
		Size: 70.8 MB (70796841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e9ed06c574509d9c0bb9d4a2c44f6ff114c1077e353cba7362c84cc4e6928`  
		Last Modified: Sat, 16 Oct 2021 03:52:34 GMT  
		Size: 246.5 KB (246456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9610fdb8a0efd75ac022b32e5bd0ab2e949a04010b31b2a1f1955479553203b4`  
		Last Modified: Sat, 16 Oct 2021 03:52:33 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf5624b902d835e1730c98d69e69b0b0b7426d0fa45bb0bfc22612403589e0b`  
		Last Modified: Sat, 16 Oct 2021 03:52:37 GMT  
		Size: 22.2 MB (22184954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:82a80df0e03fc37a4baf73d1c03b9fc968dea740ee502742fe2ce4526767cdc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.9 MB (220944962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3422c6512a41b27c8dc446dafaaefa7bf1d51a251ca3043d622285eb8ccc17fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:37:00 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 02:37:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:37:57 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:37:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:37:59 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:38:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:38:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:39:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cad6ffb3dc60f95d5943b3d5acda12c57965d2d65f7f2872b8c1606c16ee237`  
		Last Modified: Sat, 16 Oct 2021 02:52:06 GMT  
		Size: 100.6 MB (100573282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2ebcd20493ee87f05a7a06631f0e49a219d4e69224ecd485721c5533349280`  
		Last Modified: Sat, 16 Oct 2021 02:51:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0d3c7da3194f2ecfb190e30268c8d48f6234b20e8aec520afaabc90cb86057`  
		Last Modified: Sat, 16 Oct 2021 02:52:27 GMT  
		Size: 64.9 MB (64922124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605cd44436c348c295974385f97270bbfe47c80a3004ac7e1470ecd75955075f`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 246.4 KB (246396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef09852bd281240a5a11ad01942f7d7b2d78bc9910b588bc5b648036202ba2aa`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64fed610107408e1af96e0fc9d2c3da4e93ff305321078387b8a569e0e297c8`  
		Last Modified: Sat, 16 Oct 2021 02:52:21 GMT  
		Size: 21.5 MB (21518723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-base-focal`

```console
$ docker pull ros@sha256:4b2c3cea9a24377ef17849b0b956198edd73351b5ba287196c3a0a6365fc3f33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:660697b6ebaafa37ae39e5c462f5f789aeb2a3cfccd3b3d86f9c241c9c1991d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.7 MB (232747962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d87d298b0c2d4fd632c61dca8f405782cfb08dbb078b359644b99ceb09b94ecb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:43:25 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 03:44:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:44:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:44:10 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:44:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:44:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:44:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8bee2b5a1507bb0b409e973d369b0bee5c61d9429220e7511f7d34e11c4e6d`  
		Last Modified: Sat, 16 Oct 2021 03:52:23 GMT  
		Size: 104.2 MB (104214475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfab2596705bca5df8835dcd748c852003ebe630614e4c71569980fd0962003`  
		Last Modified: Sat, 16 Oct 2021 03:52:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29283b46cfd735b60062e5f91075c6f2ea843931acc59c14f37eb39221dd2b8`  
		Last Modified: Sat, 16 Oct 2021 03:52:44 GMT  
		Size: 70.8 MB (70796841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e9ed06c574509d9c0bb9d4a2c44f6ff114c1077e353cba7362c84cc4e6928`  
		Last Modified: Sat, 16 Oct 2021 03:52:34 GMT  
		Size: 246.5 KB (246456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9610fdb8a0efd75ac022b32e5bd0ab2e949a04010b31b2a1f1955479553203b4`  
		Last Modified: Sat, 16 Oct 2021 03:52:33 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf5624b902d835e1730c98d69e69b0b0b7426d0fa45bb0bfc22612403589e0b`  
		Last Modified: Sat, 16 Oct 2021 03:52:37 GMT  
		Size: 22.2 MB (22184954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:82a80df0e03fc37a4baf73d1c03b9fc968dea740ee502742fe2ce4526767cdc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.9 MB (220944962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3422c6512a41b27c8dc446dafaaefa7bf1d51a251ca3043d622285eb8ccc17fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:37:00 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 02:37:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:37:57 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:37:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:37:59 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:38:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:38:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:39:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cad6ffb3dc60f95d5943b3d5acda12c57965d2d65f7f2872b8c1606c16ee237`  
		Last Modified: Sat, 16 Oct 2021 02:52:06 GMT  
		Size: 100.6 MB (100573282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2ebcd20493ee87f05a7a06631f0e49a219d4e69224ecd485721c5533349280`  
		Last Modified: Sat, 16 Oct 2021 02:51:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0d3c7da3194f2ecfb190e30268c8d48f6234b20e8aec520afaabc90cb86057`  
		Last Modified: Sat, 16 Oct 2021 02:52:27 GMT  
		Size: 64.9 MB (64922124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605cd44436c348c295974385f97270bbfe47c80a3004ac7e1470ecd75955075f`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 246.4 KB (246396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef09852bd281240a5a11ad01942f7d7b2d78bc9910b588bc5b648036202ba2aa`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64fed610107408e1af96e0fc9d2c3da4e93ff305321078387b8a569e0e297c8`  
		Last Modified: Sat, 16 Oct 2021 02:52:21 GMT  
		Size: 21.5 MB (21518723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:e62ceb1739225eb592e9fff35c96f5179c46f0abd8bd2f6ddd1c9e8be3af9299
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:caae8f56e59f2e82e8383fa494ffacad1298d97d445350908794b2e5633a5594
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139517662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34b72bba109cd79a2c78a4c4eccb365eab453ee63fba435baf53e7f683ff8c8e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:43:25 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 03:44:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:44:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:44:10 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8bee2b5a1507bb0b409e973d369b0bee5c61d9429220e7511f7d34e11c4e6d`  
		Last Modified: Sat, 16 Oct 2021 03:52:23 GMT  
		Size: 104.2 MB (104214475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfab2596705bca5df8835dcd748c852003ebe630614e4c71569980fd0962003`  
		Last Modified: Sat, 16 Oct 2021 03:52:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:73bcdef8a189458795348b153fd586f83f471c9aec6be0e790f79840d3167491
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134255736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70933e0dd5cec3b3f1951e2202493fa577a008a45cce982eae9d0c219ab46b3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:37:00 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 02:37:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:37:57 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:37:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:37:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cad6ffb3dc60f95d5943b3d5acda12c57965d2d65f7f2872b8c1606c16ee237`  
		Last Modified: Sat, 16 Oct 2021 02:52:06 GMT  
		Size: 100.6 MB (100573282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2ebcd20493ee87f05a7a06631f0e49a219d4e69224ecd485721c5533349280`  
		Last Modified: Sat, 16 Oct 2021 02:51:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros-core-focal`

```console
$ docker pull ros@sha256:e62ceb1739225eb592e9fff35c96f5179c46f0abd8bd2f6ddd1c9e8be3af9299
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:caae8f56e59f2e82e8383fa494ffacad1298d97d445350908794b2e5633a5594
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139517662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34b72bba109cd79a2c78a4c4eccb365eab453ee63fba435baf53e7f683ff8c8e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:43:25 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 03:44:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:44:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:44:10 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8bee2b5a1507bb0b409e973d369b0bee5c61d9429220e7511f7d34e11c4e6d`  
		Last Modified: Sat, 16 Oct 2021 03:52:23 GMT  
		Size: 104.2 MB (104214475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfab2596705bca5df8835dcd748c852003ebe630614e4c71569980fd0962003`  
		Last Modified: Sat, 16 Oct 2021 03:52:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:73bcdef8a189458795348b153fd586f83f471c9aec6be0e790f79840d3167491
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134255736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70933e0dd5cec3b3f1951e2202493fa577a008a45cce982eae9d0c219ab46b3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:37:00 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 02:37:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:37:57 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:37:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:37:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cad6ffb3dc60f95d5943b3d5acda12c57965d2d65f7f2872b8c1606c16ee237`  
		Last Modified: Sat, 16 Oct 2021 02:52:06 GMT  
		Size: 100.6 MB (100573282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2ebcd20493ee87f05a7a06631f0e49a219d4e69224ecd485721c5533349280`  
		Last Modified: Sat, 16 Oct 2021 02:51:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge`

```console
$ docker pull ros@sha256:41ed09bfe510d8f1917a2c19fff4def4e5530b3b5584955a3ff4f97066b42f7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:38f52106bd035bf0f6b11f3a4a7cb5df16ba7f907b8d4929c6e77ad855be9a43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.9 MB (328878897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f8ebeb07a93dcd1df45cf05457b81dcc130e9b3a2f7be9c5fca06e9880ca2a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:43:25 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 03:44:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:44:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:44:10 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:44:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:44:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:44:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:45:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:45:19 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 03:45:19 GMT
ENV ROS2_DISTRO=rolling
# Sat, 16 Oct 2021 03:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:41:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.17.0-1*     ros-rolling-demo-nodes-py=0.17.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:41:34 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8bee2b5a1507bb0b409e973d369b0bee5c61d9429220e7511f7d34e11c4e6d`  
		Last Modified: Sat, 16 Oct 2021 03:52:23 GMT  
		Size: 104.2 MB (104214475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfab2596705bca5df8835dcd748c852003ebe630614e4c71569980fd0962003`  
		Last Modified: Sat, 16 Oct 2021 03:52:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29283b46cfd735b60062e5f91075c6f2ea843931acc59c14f37eb39221dd2b8`  
		Last Modified: Sat, 16 Oct 2021 03:52:44 GMT  
		Size: 70.8 MB (70796841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e9ed06c574509d9c0bb9d4a2c44f6ff114c1077e353cba7362c84cc4e6928`  
		Last Modified: Sat, 16 Oct 2021 03:52:34 GMT  
		Size: 246.5 KB (246456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9610fdb8a0efd75ac022b32e5bd0ab2e949a04010b31b2a1f1955479553203b4`  
		Last Modified: Sat, 16 Oct 2021 03:52:33 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf5624b902d835e1730c98d69e69b0b0b7426d0fa45bb0bfc22612403589e0b`  
		Last Modified: Sat, 16 Oct 2021 03:52:37 GMT  
		Size: 22.2 MB (22184954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33db4091cb9bc6536ddafd99784ef2739f5ab1f90d5ffa63bb125186ec7dfe6`  
		Last Modified: Sat, 16 Oct 2021 03:52:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b8ed699742f417db6e46477f6cbbbd143b369a666b9504d8fd3ef42c6b4827`  
		Last Modified: Sat, 16 Oct 2021 03:52:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac122dc08231f6b44fa9d50c299b4f9721a1351adba204bb58863fbf0fba1b14`  
		Last Modified: Sat, 16 Oct 2021 03:53:13 GMT  
		Size: 78.4 MB (78428391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd9582a655c0588ddd7b3cdbe066a85156e3cace0a3c7d2cdb8de6543b4a6b4`  
		Last Modified: Fri, 12 Nov 2021 01:42:41 GMT  
		Size: 17.7 MB (17701920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65cb722cddccca5b5b84c3c341e411432269ca99d7fb35dfb562c3c99f78e23`  
		Last Modified: Fri, 12 Nov 2021 01:42:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:69fd36b6bc76e9a69e1dbe9fd7baba4175c11591de07f6cc6dec6469aa41104e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.1 MB (316060914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a943606e0177bd34cc3f1cad5cbc775f7c190ab64f981346b25b13dda8f229f1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:37:00 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 02:37:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:37:57 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:37:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:37:59 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:38:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:38:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:39:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:39:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:39:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:39:13 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 02:39:14 GMT
ENV ROS2_DISTRO=rolling
# Sat, 16 Oct 2021 02:39:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:21:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.17.0-1*     ros-rolling-demo-nodes-py=0.17.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:21:21 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cad6ffb3dc60f95d5943b3d5acda12c57965d2d65f7f2872b8c1606c16ee237`  
		Last Modified: Sat, 16 Oct 2021 02:52:06 GMT  
		Size: 100.6 MB (100573282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2ebcd20493ee87f05a7a06631f0e49a219d4e69224ecd485721c5533349280`  
		Last Modified: Sat, 16 Oct 2021 02:51:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0d3c7da3194f2ecfb190e30268c8d48f6234b20e8aec520afaabc90cb86057`  
		Last Modified: Sat, 16 Oct 2021 02:52:27 GMT  
		Size: 64.9 MB (64922124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605cd44436c348c295974385f97270bbfe47c80a3004ac7e1470ecd75955075f`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 246.4 KB (246396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef09852bd281240a5a11ad01942f7d7b2d78bc9910b588bc5b648036202ba2aa`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64fed610107408e1af96e0fc9d2c3da4e93ff305321078387b8a569e0e297c8`  
		Last Modified: Sat, 16 Oct 2021 02:52:21 GMT  
		Size: 21.5 MB (21518723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b23a5fc866c0d86236bcc6617a57feeec98579b0653da4ec56e140a78395fc`  
		Last Modified: Sat, 16 Oct 2021 02:52:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cd393f58617c01a967f7b190061a1be8d33528cce968c447c4c5f437fa1378`  
		Last Modified: Sat, 16 Oct 2021 02:52:56 GMT  
		Size: 78.2 MB (78154328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d2314c5b843696dca1afa6c872380d59c40733a274735e8d0716614632bf53`  
		Last Modified: Fri, 12 Nov 2021 01:23:23 GMT  
		Size: 17.0 MB (16961150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34424424413d3f4a7b9136c2085242a96bcfc3cb8ccf15117fa3328694e674d5`  
		Last Modified: Fri, 12 Nov 2021 01:23:19 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:41ed09bfe510d8f1917a2c19fff4def4e5530b3b5584955a3ff4f97066b42f7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:38f52106bd035bf0f6b11f3a4a7cb5df16ba7f907b8d4929c6e77ad855be9a43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.9 MB (328878897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f8ebeb07a93dcd1df45cf05457b81dcc130e9b3a2f7be9c5fca06e9880ca2a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:26:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:37:43 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 03:37:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 03:37:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 03:43:25 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 03:44:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:09 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 03:44:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 03:44:10 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:44:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:44:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 03:44:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 03:44:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:45:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 03:45:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 03:45:19 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 03:45:19 GMT
ENV ROS2_DISTRO=rolling
# Sat, 16 Oct 2021 03:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:41:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.17.0-1*     ros-rolling-demo-nodes-py=0.17.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:41:34 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9dfa7092d8b77085dc1f7f400d3a0618187cefd4af7037e9dec2f88eadec7`  
		Last Modified: Sat, 16 Oct 2021 03:46:47 GMT  
		Size: 5.5 MB (5547495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc9a74c1dba9c88845d88e89e5987b2c38fa8df2fceefed614e3f8cf7d835b5`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8299091b3ca45435fb28fad59303294248fb9b00ddcdf278f067eb472a8c86ef`  
		Last Modified: Sat, 16 Oct 2021 03:49:29 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8bee2b5a1507bb0b409e973d369b0bee5c61d9429220e7511f7d34e11c4e6d`  
		Last Modified: Sat, 16 Oct 2021 03:52:23 GMT  
		Size: 104.2 MB (104214475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfab2596705bca5df8835dcd748c852003ebe630614e4c71569980fd0962003`  
		Last Modified: Sat, 16 Oct 2021 03:52:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29283b46cfd735b60062e5f91075c6f2ea843931acc59c14f37eb39221dd2b8`  
		Last Modified: Sat, 16 Oct 2021 03:52:44 GMT  
		Size: 70.8 MB (70796841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e9ed06c574509d9c0bb9d4a2c44f6ff114c1077e353cba7362c84cc4e6928`  
		Last Modified: Sat, 16 Oct 2021 03:52:34 GMT  
		Size: 246.5 KB (246456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9610fdb8a0efd75ac022b32e5bd0ab2e949a04010b31b2a1f1955479553203b4`  
		Last Modified: Sat, 16 Oct 2021 03:52:33 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf5624b902d835e1730c98d69e69b0b0b7426d0fa45bb0bfc22612403589e0b`  
		Last Modified: Sat, 16 Oct 2021 03:52:37 GMT  
		Size: 22.2 MB (22184954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33db4091cb9bc6536ddafd99784ef2739f5ab1f90d5ffa63bb125186ec7dfe6`  
		Last Modified: Sat, 16 Oct 2021 03:52:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b8ed699742f417db6e46477f6cbbbd143b369a666b9504d8fd3ef42c6b4827`  
		Last Modified: Sat, 16 Oct 2021 03:52:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac122dc08231f6b44fa9d50c299b4f9721a1351adba204bb58863fbf0fba1b14`  
		Last Modified: Sat, 16 Oct 2021 03:53:13 GMT  
		Size: 78.4 MB (78428391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd9582a655c0588ddd7b3cdbe066a85156e3cace0a3c7d2cdb8de6543b4a6b4`  
		Last Modified: Fri, 12 Nov 2021 01:42:41 GMT  
		Size: 17.7 MB (17701920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65cb722cddccca5b5b84c3c341e411432269ca99d7fb35dfb562c3c99f78e23`  
		Last Modified: Fri, 12 Nov 2021 01:42:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:69fd36b6bc76e9a69e1dbe9fd7baba4175c11591de07f6cc6dec6469aa41104e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.1 MB (316060914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a943606e0177bd34cc3f1cad5cbc775f7c190ab64f981346b25b13dda8f229f1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:19:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:19:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:30:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 16 Oct 2021 02:30:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:30:41 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 02:30:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Oct 2021 02:37:00 GMT
ENV ROS_DISTRO=rolling
# Sat, 16 Oct 2021 02:37:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:37:57 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 16 Oct 2021 02:37:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Oct 2021 02:37:59 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:38:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Oct 2021 02:38:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 16 Oct 2021 02:39:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:39:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Oct 2021 02:39:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Oct 2021 02:39:13 GMT
ENV ROS1_DISTRO=noetic
# Sat, 16 Oct 2021 02:39:14 GMT
ENV ROS2_DISTRO=rolling
# Sat, 16 Oct 2021 02:39:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.13-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:21:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.2-1*     ros-rolling-demo-nodes-cpp=0.17.0-1*     ros-rolling-demo-nodes-py=0.17.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Nov 2021 01:21:21 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426e3a0ed188569ceb995612f61d01b012f19e6849dacdcdef24f70e9e820b`  
		Last Modified: Sat, 16 Oct 2021 02:44:04 GMT  
		Size: 1.2 MB (1186725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74557b92a76c488a6e2f31c091f03671baadbd5b593c4af9dbde2baea1616333`  
		Last Modified: Sat, 16 Oct 2021 02:44:02 GMT  
		Size: 5.3 MB (5322455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799e8bd4d8f9479b13bd0d148a873ef866dc81e123396022ca5230b690127bc`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac91bb16ec2aa9ad80cd7ef5c44472bd9691216081f8f16049fb6a2b377b9cf`  
		Last Modified: Sat, 16 Oct 2021 02:49:08 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cad6ffb3dc60f95d5943b3d5acda12c57965d2d65f7f2872b8c1606c16ee237`  
		Last Modified: Sat, 16 Oct 2021 02:52:06 GMT  
		Size: 100.6 MB (100573282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2ebcd20493ee87f05a7a06631f0e49a219d4e69224ecd485721c5533349280`  
		Last Modified: Sat, 16 Oct 2021 02:51:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0d3c7da3194f2ecfb190e30268c8d48f6234b20e8aec520afaabc90cb86057`  
		Last Modified: Sat, 16 Oct 2021 02:52:27 GMT  
		Size: 64.9 MB (64922124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605cd44436c348c295974385f97270bbfe47c80a3004ac7e1470ecd75955075f`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 246.4 KB (246396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef09852bd281240a5a11ad01942f7d7b2d78bc9910b588bc5b648036202ba2aa`  
		Last Modified: Sat, 16 Oct 2021 02:52:17 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64fed610107408e1af96e0fc9d2c3da4e93ff305321078387b8a569e0e297c8`  
		Last Modified: Sat, 16 Oct 2021 02:52:21 GMT  
		Size: 21.5 MB (21518723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b23a5fc866c0d86236bcc6617a57feeec98579b0653da4ec56e140a78395fc`  
		Last Modified: Sat, 16 Oct 2021 02:52:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cd393f58617c01a967f7b190061a1be8d33528cce968c447c4c5f437fa1378`  
		Last Modified: Sat, 16 Oct 2021 02:52:56 GMT  
		Size: 78.2 MB (78154328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d2314c5b843696dca1afa6c872380d59c40733a274735e8d0716614632bf53`  
		Last Modified: Fri, 12 Nov 2021 01:23:23 GMT  
		Size: 17.0 MB (16961150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34424424413d3f4a7b9136c2085242a96bcfc3cb8ccf15117fa3328694e674d5`  
		Last Modified: Fri, 12 Nov 2021 01:23:19 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
